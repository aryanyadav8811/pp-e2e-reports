# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: settings/account-lifecycle.spec.ts >> Settings - Account Lifecycle >> Delete account freezes the user, ends the session and refuses the next login
- Location: tests/settings/account-lifecycle.spec.ts:83:3

# Error details

```
Error: [e2e] userFactory: /api/v1/signup/check_phone/ returned non-JSON HTTP 403
```

# Test source

```ts
  1   | // Throwaway accounts for specs that leave a user in a state no shared account
  2   | // may end up in (frozen by "delete account", stale terms). Registers through
  3   | // the same endpoints the signup wizard calls, with the backend's fixed OTP, so
  4   | // it works wherever @mock-otp does; cleanup hard-deletes via cleanupSignupUser.
  5   | 
  6   | import { request as pwRequest, type APIRequestContext } from '@playwright/test';
  7   | import { E2E_REQUEST_UA } from './ua';
  8   | import { assertNotProd } from './env';
  9   | import { generateTestData } from './testData';
  10  | import { cleanupSignupUser } from './cleanupSignupUser';
  11  | import { maskUser } from './secrets';
  12  | import { log } from './logger';
  13  | 
  14  | export type ThrowawayUser = {
  15  |   username: string;
  16  |   password: string;
  17  |   email: string;
  18  |   /** E.164, as the signup wizard submits it. */
  19  |   phoneNumber: string;
  20  | };
  21  | 
  22  | type HttpCredentials = { username: string; password: string };
  23  | 
  24  | const API_HEADERS = {
  25  |   'X-Requested-With': 'XMLHttpRequest',
  26  |   'X-Parlay-Request': '1',
  27  | };
  28  | const FIXED_OTP = '123456';
  29  | // dj-rest-auth throttles registration and login together (10/min per IP);
  30  | // three device projects each signing up and logging in can trip it.
  31  | const REGISTER_ATTEMPTS = 3;
  32  | 
  33  | async function postJson<T>(
  34  |   rc: APIRequestContext,
  35  |   path: string,
  36  |   data: Record<string, unknown>,
  37  | ): Promise<{ status: number; body: T }> {
  38  |   const resp = await rc.post(path, { headers: API_HEADERS, data, timeout: 30_000 });
  39  |   const text = await resp.text();
  40  |   let body: T;
  41  |   try {
  42  |     body = JSON.parse(text) as T;
  43  |   } catch {
> 44  |     throw new Error(`[e2e] userFactory: ${path} returned non-JSON HTTP ${resp.status()}`);
      |           ^ Error: [e2e] userFactory: /api/v1/signup/check_phone/ returned non-JSON HTTP 403
  45  |   }
  46  |   return { status: resp.status(), body };
  47  | }
  48  | 
  49  | /**
  50  |  * Registers a fresh account (phone check → fixed OTP → registration) and
  51  |  * returns its credentials. Callers own cleanup: `deleteThrowawayUser` in a
  52  |  * `finally`, even after the account was frozen in-test.
  53  |  */
  54  | export async function createThrowawayUser(opts: {
  55  |   baseURL?: string;
  56  |   httpCredentials?: HttpCredentials;
  57  | }): Promise<ThrowawayUser> {
  58  |   assertNotProd('createThrowawayUser (registers accounts)');
  59  |   const data = generateTestData({ lettersOnlyUsername: true });
  60  |   const phoneNumber = `+1${data.phoneNumber}`;
  61  |   const rc = await pwRequest.newContext({
  62  |     baseURL: opts.baseURL,
  63  |     httpCredentials: opts.httpCredentials,
  64  |     userAgent: E2E_REQUEST_UA,
  65  |   });
  66  |   const t0 = Date.now();
  67  |   try {
  68  |     type StepResult = { value: boolean; message?: string };
  69  |     const sent = await postJson<StepResult>(rc, '/api/v1/signup/check_phone/', {
  70  |       phonenumber: phoneNumber,
  71  |     });
  72  |     if (!sent.body.value) {
  73  |       throw new Error(
  74  |         `[e2e] userFactory: phone step rejected (${sent.body.message ?? sent.status}). ` +
  75  |           'Throwaway users need FIXED_OTP_ENABLED on the backend (@mock-otp).',
  76  |       );
  77  |     }
  78  |     const code = await postJson<StepResult>(rc, '/api/v1/signup/check_phonecode/', {
  79  |       phonecode: FIXED_OTP,
  80  |       phonenumber: phoneNumber,
  81  |     });
  82  |     if (!code.body.value) {
  83  |       throw new Error(
  84  |         `[e2e] userFactory: fixed OTP rejected (${code.body.message ?? code.status})`,
  85  |       );
  86  |     }
  87  | 
  88  |     const payload = {
  89  |       username: data.username,
  90  |       password: data.password,
  91  |       confirmPassword: data.password,
  92  |       email: data.email,
  93  |       phonenumber: phoneNumber,
  94  |       phonecode: FIXED_OTP,
  95  |       firstname: data.firstName,
  96  |       lastname: data.lastName,
  97  |       dob: '1990-06-15',
  98  |       couponCode: '',
  99  |       // In ephemeral mode the run's btag lets `e2e_purge --run-key` sweep the
  100 |       // account if the in-test cleanup never ran.
  101 |       ...(data.btag ? { btag: data.btag } : {}),
  102 |       termsandconditions: true,
  103 |       packsterms: true,
  104 |     };
  105 |     for (let attempt = 1; ; attempt++) {
  106 |       const resp = await rc.post('/api/v1/dj-rest-auth/registration/', {
  107 |         headers: API_HEADERS,
  108 |         data: payload,
  109 |         timeout: 30_000,
  110 |       });
  111 |       if (resp.ok()) break;
  112 |       const body = await resp.text().catch(() => '');
  113 |       if (resp.status() === 429 && attempt < REGISTER_ATTEMPTS) {
  114 |         const retryAfter = Number(resp.headers()['retry-after']);
  115 |         const waitMs = (Number.isFinite(retryAfter) && retryAfter > 0 ? retryAfter : 30) * 1000;
  116 |         log.warn('userFactory: registration throttled (429) — backing off', { waitMs, attempt });
  117 |         await new Promise((r) => setTimeout(r, waitMs));
  118 |         continue;
  119 |       }
  120 |       throw new Error(
  121 |         `[e2e] userFactory: registration failed HTTP ${resp.status()}: ${body.slice(0, 300)}`,
  122 |       );
  123 |     }
  124 |     log.info('userFactory: throwaway user registered', {
  125 |       user: maskUser(data.username),
  126 |       durationMs: Date.now() - t0,
  127 |     });
  128 |     return { username: data.username, password: data.password, email: data.email, phoneNumber };
  129 |   } finally {
  130 |     await rc.dispose();
  131 |   }
  132 | }
  133 | 
  134 | /** Hard-deletes the account; safe to call for a user the test already froze. */
  135 | export async function deleteThrowawayUser(user: Pick<ThrowawayUser, 'username'>): Promise<void> {
  136 |   try {
  137 |     await cleanupSignupUser({ username: user.username });
  138 |     log.info('userFactory: throwaway user deleted', { user: maskUser(user.username) });
  139 |   } catch (err) {
  140 |     // Surface but never mask the test's own outcome; the purge sweep is the backstop.
  141 |     log.error('userFactory: cleanup failed — account left behind', {
  142 |       user: maskUser(user.username),
  143 |       error: (err as Error).message,
  144 |     });
```