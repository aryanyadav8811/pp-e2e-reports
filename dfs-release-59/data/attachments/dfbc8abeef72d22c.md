# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: auth/login.spec.ts >> Login - Invalid Credentials >> error message clears on retry with valid credentials
- Location: tests/auth/login.spec.ts:171:3

# Error details

```
Error: expect(locator).toHaveCount(expected) failed

Locator:  getByRole('link', { name: 'Join Now' }).filter({ visible: true }).first()
Expected: 0
Received: 1
Timeout:  15000ms

Call log:
  - Expect "toHaveCount" with timeout 15000ms
  - waiting for getByRole('link', { name: 'Join Now' }).filter({ visible: true }).first()
    19 × locator resolved to 1 element
       - unexpected value "1"

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
              - textbox "Password" [ref=e28]: ***
              - separator [ref=e29]
              - button "Show or Hide Password" [ref=e30]:
                - img [ref=e31]
          - button "Login" [active] [ref=e34] [cursor=pointer]
          - generic [ref=e35]: Forgot your password?
    - region "Notifications Alt+T"
  - alert [ref=e36]
  - iframe [ref=e37]:
    
```

# Test source

```ts
  1  | import { BasePage } from "./base.page";
  2  | import { expect, type Page } from "@playwright/test";
  3  | 
  4  | export class AuthPage extends BasePage {
  5  |     readonly usernameField = this.locator('#username');
  6  |     readonly passwordField = this.locator('#password');
  7  |     readonly submitBtn = this.locator('button[type="submit"]', { hasText: 'Login' });
  8  | 
  9  |     readonly joinNowBtn = this.byRole('link', { name: 'Join Now' });
  10 |     readonly forgotPasswordLink = this.byText('Forgot your password?');
  11 |     readonly signUpLink = this.byRole('button', { name: 'Sign Up' });
  12 | 
  13 |     constructor(page: Page) {
  14 |         super(page);
  15 |     }
  16 | 
  17 |     async logIn(username: string, password: string): Promise<void> {
  18 |         await this.open('/account/login');
  19 |         await this.usernameField.fill(username);
  20 |         await this.passwordField.fill(password);
  21 |         await this.submitBtn.click();
  22 |     };
  23 | 
  24 |     //Submit credentials on the login page that's already loaded
  25 |     async submitLoginForm(username: string, password: string): Promise<void> {
  26 |         await this.usernameField.fill(username);
  27 |         await this.passwordField.fill(password);
  28 |         await this.submitBtn.click();
  29 |     };
  30 | 
  31 |     async assertSuccess(): Promise<void> {
> 32 |         await expect(this.joinNowBtn).toHaveCount(0);
     |                                       ^ Error: expect(locator).toHaveCount(expected) failed
  33 |     };
  34 | 
  35 |     async assertFailure(messagePattern: RegExp): Promise<void> {
  36 |         const alert = this.page
  37 |             .getByRole('alert')
  38 |             .filter({ hasText: messagePattern })
  39 |             .filter({ visible: true })
  40 |             .first();
  41 |         await expect(alert).toBeVisible();
  42 |     };
  43 | 
  44 |     async openLogIn(): Promise<void> {
  45 |         await this.open('/account/login');
  46 |     };
  47 | 
  48 |     async joinBtnAssertion(): Promise<void> {
  49 |         await expect(this.joinNowBtn).toBeVisible();
  50 |     };
  51 | 
  52 |     async assertOnLoginPage(): Promise<void> {
  53 |         await expect(this.page).toHaveURL(/\/account\/login/);
  54 |         await expect(this.usernameField).toBeVisible();
  55 |         await expect(this.passwordField).toBeVisible();
  56 |         await expect(this.submitBtn).toBeVisible();
  57 |     };
  58 | };
  59 | 
```