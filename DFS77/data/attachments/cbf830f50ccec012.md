# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: auth/login.spec.ts >> Login - Invalid Credentials >> cannot login with invalid password
- Location: tests/auth/login.spec.ts:134:3

# Error details

```
Error: expect(locator).toBeVisible() failed

Locator: getByRole('alert').filter({ hasText: /unable to log in/i }).filter({ visible: true }).first()
Expected: visible
Timeout: 15000ms
Error: element(s) not found

Call log:
  - Expect "toBeVisible" with timeout 15000ms
  - waiting for getByRole('alert').filter({ hasText: /unable to log in/i }).filter({ visible: true }).first()

```

# Page snapshot

```yaml
- generic [ref=e1]:
  - generic [ref=e2]:
    - generic [ref=e3]:
      - banner [ref=e4]:
        - navigation [ref=e5]:
          - link "Parlay Play LogoParlay Play text" [ref=e6] [cursor=pointer]:
            - /url: /
            - generic [ref=e7]:
              - img "Parlay Play Logo" [ref=e8]
              - img "Parlay Play text" [ref=e9]
          - link "Join Now" [ref=e11] [cursor=pointer]:
            - /url: /account/signup
            - generic [ref=e13]: Join Now
      - main [ref=e14]:
        - generic [ref=e19]:
          - generic [ref=e20]: Login
          - generic [ref=e21]:
            - textbox "Username/E-mail" [ref=e24]: ***
            - generic [ref=e27]:
              - textbox "Password" [ref=e28]: WrongPassword123
              - separator [ref=e29]
              - button "Show or Hide Password" [ref=e30]:
                - img [ref=e31]
            - generic [ref=e33] [cursor=pointer]:
              - generic [ref=e34]:
                - img "face id icon" [ref=e35]
                - generic [ref=e36]: Login with your Touch ID
              - checkbox "face id icon Login with your Touch ID" [ref=e37]
          - button "Login" [active] [ref=e40] [cursor=pointer]
          - generic [ref=e41]: Forgot your password?
    - region "Notifications Alt+T"
  - alert [ref=e42]
  - iframe [ref=e43]:
    
```

# Test source

```ts
  3   | 
  4   | // staging sits behind Cloudflare, whose rate-limit rule answers login POSTs
  5   | // with a 429 ("Error 1015") long before Django sees them. The volume of logins
  6   | // in the auth suite trips it, so every submit retries on a 429, honoring the
  7   | // backoff Cloudflare hands back.
  8   | const LOGIN_PATH = /\/api\/v1\/dj-rest-auth\/login\/?$/;
  9   | const LOGIN_MAX_ATTEMPTS = 4;
  10  | 
  11  | export class AuthPage extends BasePage {
  12  |     readonly usernameField = this.locator('#username');
  13  |     readonly passwordField = this.locator('#password');
  14  |     readonly submitBtn = this.locator('button[type="submit"]', { hasText: 'Login' });
  15  | 
  16  |     readonly joinNowBtn = this.byRole('link', { name: 'Join Now' });
  17  |     readonly forgotPasswordLink = this.byText('Forgot your password?');
  18  |     readonly signUpLink = this.byRole('button', { name: 'Sign Up' });
  19  | 
  20  |     constructor(page: Page) {
  21  |         super(page);
  22  |     }
  23  | 
  24  |     async logIn(username: string, password: string): Promise<void> {
  25  |         await this.open('/account/login');
  26  |         await this.usernameField.fill(username);
  27  |         await this.passwordField.fill(password);
  28  |         await this.submit();
  29  |     };
  30  | 
  31  |     //Submit credentials on the login page that's already loaded
  32  |     async submitLoginForm(username: string, password: string): Promise<void> {
  33  |         await this.usernameField.fill(username);
  34  |         await this.passwordField.fill(password);
  35  |         await this.submit();
  36  |     };
  37  | 
  38  |     /**
  39  |      * Clicks Login and, if Cloudflare rate-limits the POST (429 / Error 1015),
  40  |      * waits out the backoff and re-submits. On any non-429 outcome (200, a 400
  41  |      * validation error, or no observable POST) it returns immediately so the
  42  |      * negative-path assertions run as before. The form keeps its filled values
  43  |      * across a 429, so a bare re-click re-POSTs the same credentials.
  44  |      */
  45  |     async submit(maxAttempts = LOGIN_MAX_ATTEMPTS): Promise<void> {
  46  |         for (let attempt = 1; ; attempt++) {
  47  |             const responsePromise = this.page
  48  |                 .waitForResponse(
  49  |                     (resp) =>
  50  |                         LOGIN_PATH.test(new URL(resp.url()).pathname) &&
  51  |                         resp.request().method() === 'POST',
  52  |                     { timeout: 30_000 },
  53  |                 )
  54  |                 .catch(() => null);
  55  | 
  56  |             await this.submitBtn.click();
  57  |             const resp = await responsePromise;
  58  | 
  59  |             if (!resp || resp.status() !== 429 || attempt >= maxAttempts) return;
  60  | 
  61  |             const waitMs = await AuthPage.rateLimitBackoffMs(resp);
  62  |             console.warn(
  63  |                 `[auth] login rate-limited (429); waiting ${waitMs}ms before retry ${attempt + 1}/${maxAttempts}`,
  64  |             );
  65  |             await this.page.waitForTimeout(waitMs);
  66  |         }
  67  |     };
  68  | 
  69  |     // Cloudflare's 1015 body carries `retry_after` (seconds); fall back to the
  70  |     // Retry-After header, then a floor matching its ~30s window. Buffered a few
  71  |     // seconds and capped so a stuck limit can't hang the whole suite.
  72  |     private static async rateLimitBackoffMs(resp: Response): Promise<number> {
  73  |         let seconds = 0;
  74  |         try {
  75  |             const body = await resp.json();
  76  |             if (typeof body?.retry_after === 'number') seconds = body.retry_after;
  77  |         } catch {
  78  |             /* non-JSON body — fall through to the header */
  79  |         }
  80  |         if (!seconds) {
  81  |             const header = resp.headers()['retry-after'];
  82  |             const parsed = header ? parseInt(header, 10) : NaN;
  83  |             if (Number.isFinite(parsed)) seconds = parsed;
  84  |         }
  85  |         const buffered = Math.max(seconds, 30) + 3;
  86  |         return Math.min(buffered, 90) * 1000;
  87  |     };
  88  | 
  89  |     async assertSuccess(): Promise<void> {
  90  |         // Cold-start dev compile of `/` can take 20–30s on first hit after
  91  |         // the container reboots; the default 15s expect timeout times out
  92  |         // while the home shell still shows "Loading...". 60s is a safer
  93  |         // ceiling for cold runs without slowing the happy path.
  94  |         await expect(this.joinNowBtn).toHaveCount(0, { timeout: 60_000 });
  95  |     };
  96  | 
  97  |     async assertFailure(messagePattern: RegExp): Promise<void> {
  98  |         const alert = this.page
  99  |             .getByRole('alert')
  100 |             .filter({ hasText: messagePattern })
  101 |             .filter({ visible: true })
  102 |             .first();
> 103 |         await expect(alert).toBeVisible();
      |                             ^ Error: expect(locator).toBeVisible() failed
  104 |     };
  105 | 
  106 |     async openLogIn(): Promise<void> {
  107 |         await this.open('/account/login');
  108 |     };
  109 | 
  110 |     async joinBtnAssertion(): Promise<void> {
  111 |         await expect(this.joinNowBtn).toBeVisible();
  112 |     };
  113 | 
  114 |     async assertOnLoginPage(): Promise<void> {
  115 |         await expect(this.page).toHaveURL(/\/account\/login/);
  116 |         await expect(this.usernameField).toBeVisible();
  117 |         await expect(this.passwordField).toBeVisible();
  118 |         await expect(this.submitBtn).toBeVisible();
  119 |     };
  120 | };
  121 | 
```