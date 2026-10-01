# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: signup/signup.spec.ts >> Signup - Field Validation >> Username must be 3–30 letters or digits that nobody owns yet
- Location: tests/signup/signup.spec.ts:204:3

# Error details

```
Error: GET /api/v1/user/ failed: HTTP 403
```

# Page snapshot

```yaml
- generic [active] [ref=e1]:
  - generic [ref=e2]:
    - generic [ref=e3]:
      - banner [ref=e4]:
        - navigation [ref=e5]:
          - link "Parlay Play Logo" [ref=e6] [cursor=pointer]:
            - /url: /
            - img "Parlay Play Logo" [ref=e8]
          - link "Login" [ref=e10] [cursor=pointer]:
            - /url: /account/login
            - generic [ref=e12]: Login
      - main [ref=e13]:
        - generic [ref=e19]:
          - text: Account Creation
          - button "Back" [ref=e20] [cursor=pointer]:
            - img [ref=e21]
            - generic [ref=e23]: Back
          - generic [ref=e25]:
            - generic [ref=e26]: Choose your Username
            - textbox "Choose your Username" [ref=e29]:
              - /placeholder: Username
            - generic [ref=e30]: Choose your Password
            - generic [ref=e33]:
              - textbox "Choose your Password" [ref=e34]:
                - /placeholder: Password
              - separator [ref=e35]
              - button "Show or Hide Password" [ref=e36]:
                - img [ref=e37]
            - generic [ref=e41]:
              - textbox "Confirm Password" [ref=e42]
              - separator [ref=e43]
              - button "Show or Hide Password" [ref=e44]:
                - img [ref=e45]
            - paragraph [ref=e48]: Enter your name and date of birth exactly as shown on your ID or passport.
            - generic [ref=e49]: First Name
            - textbox "First Name" [ref=e52]
            - generic [ref=e53]: Last Name
            - textbox "Last Name" [ref=e56]
            - generic [ref=e57]: Date of Birth
            - textbox "Date of birth" [ref=e59]
            - generic [ref=e60]: Referral Code (optional)
            - textbox "Referral Code" [ref=e63]
            - generic [ref=e64]: E-mail Address
            - textbox "E-mail Address" [ref=e67]
            - generic [ref=e68]: Phone number
            - generic [ref=e70]:
              - generic [ref=e71]:
                - combobox "Phone number country" [ref=e72] [cursor=pointer]:
                  - option "Canada"
                  - option "United States" [selected]
                - img [ref=e74]
              - textbox "Phone number" [ref=e80]
            - button "Text me a Code" [disabled] [ref=e82]
    - generic:
      - region "Notifications Alt+T"
  - alert [ref=e83]
  - iframe [ref=e84]:
    
```

# Test source

```ts
  1  | // Profile of an already-registered account, read through its saved
  2  | // storageState. The signup validation specs use it as the "taken" username /
  3  | // email / phone, so the duplicate checks hit the real backend on every env
  4  | // without creating a user first.
  5  | 
  6  | import { request as pwRequest } from '@playwright/test';
  7  | import { E2E_REQUEST_UA } from './ua';
  8  | 
  9  | export type UserProfile = {
  10 |   username: string;
  11 |   email: string;
  12 |   /** E.164 as stored by the backend, e.g. "+16175551234"; null when unset. */
  13 |   phoneNumber: string | null;
  14 |   /** The account's own referral code (a valid coupon), if it has one. */
  15 |   referralCode: string | null;
  16 | };
  17 | 
  18 | const API_HEADERS = {
  19 |   'X-Requested-With': 'XMLHttpRequest',
  20 |   'X-Parlay-Request': '1',
  21 | };
  22 | 
  23 | export async function fetchUserProfile(
  24 |   storageStatePath: string,
  25 |   baseURL?: string,
  26 |   httpCredentials?: { username: string; password: string },
  27 | ): Promise<UserProfile> {
  28 |   const rc = await pwRequest.newContext({
  29 |     baseURL,
  30 |     httpCredentials,
  31 |     userAgent: E2E_REQUEST_UA,
  32 |     storageState: storageStatePath,
  33 |   });
  34 |   try {
  35 |     const resp = await rc.get('/api/v1/user/', { headers: API_HEADERS, timeout: 15_000 });
> 36 |     if (!resp.ok()) throw new Error(`GET /api/v1/user/ failed: HTTP ${resp.status()}`);
     |                           ^ Error: GET /api/v1/user/ failed: HTTP 403
  37 |     const body = (await resp.json()) as {
  38 |       username?: string;
  39 |       email?: string;
  40 |       phoneNumber?: string | null;
  41 |       userCouponCode?: { couponId?: string } | null;
  42 |     };
  43 |     if (!body.username) throw new Error('GET /api/v1/user/ returned no username — session dead?');
  44 |     return {
  45 |       username: body.username,
  46 |       email: body.email ?? '',
  47 |       phoneNumber: body.phoneNumber || null,
  48 |       referralCode: body.userCouponCode?.couponId ?? null,
  49 |     };
  50 |   } finally {
  51 |     await rc.dispose();
  52 |   }
  53 | }
  54 | 
  55 | /** Digits of a US E.164 number without the +1, as the phone input expects them. */
  56 | export function nationalDigits(e164: string): string | null {
  57 |   const m = e164.replace(/\D/g, '').match(/^1?(\d{10})$/);
  58 |   return m ? m[1] : null;
  59 | }
  60 | 
```