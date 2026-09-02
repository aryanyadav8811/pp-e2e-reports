# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: auth/login.spec.ts >> Login - Navigation >> unauthenticated user sees Join Now button on home
- Location: tests/auth/login.spec.ts:211:3

# Error details

```
Error: expect(locator).toBeVisible() failed

Locator: getByRole('link', { name: 'Join Now' }).filter({ visible: true }).first()
Expected: visible
Timeout: 15000ms
Error: element(s) not found

Call log:
  - Expect "toBeVisible" with timeout 15000ms
  - waiting for getByRole('link', { name: 'Join Now' }).filter({ visible: true }).first()

```

```yaml
- banner:
  - navigation:
    - link "Parlay Play Logo":
      - /url: /
      - img "Parlay Play Logo"
    - list:
      - listitem:
        - link "Home":
          - /url: /
      - listitem:
        - button "Free2Play"
      - listitem:
        - button "Feed"
      - listitem:
        - button "Rewards"
      - listitem:
        - button "Track Picks"
    - button "Join Now"
    - button "Login"
- main:
  - button "previous slide"
  - img "white lightning bol"
  - text: Join Now! $5 Free Entry
  - img "treasureBox"
  - text: Join Now and receive a $5 Free Entry. No deposit required!
  - button "Join Now!"
  - text: $100
  - img "black lightning bol"
  - text: = $200
  - img "black lightning bol"
  - text: We match your 1st deposit We match your first deposit up to $100.
  - button "Deposit Now"
  - button "next slide"
  - textbox "Search player or team"
  - button "All"
  - button "MLB"
  - button "SerieA"
  - button "EPL"
  - button "WNBA"
  - button "WNBA-Combos"
  - button "WNBA Q1"
  - button "WNBA H1"
  - button "MLS"
  - button "LaLiga"
  - button "UFC"
  - button "Bundes"
  - button "right chevron sign Filter":
    - img "right chevron sign"
    - text: Filter
  - img "Ian Seymour"
  - text: Ian Seymour SP - TB TB @ DET 6:40 PM
  - button "Open expert opinion for Ian Seymour"
  - text: Less Strikeouts (K) More
  - button "Select over 5.5 Strikeouts (K) for 1.78 times": 1.78x
  - text: 5.5 Strikeouts (K)
  - button "Select over 5.5 Strikeouts (K) for 1.78 times": 1.78x
  - text: Less Hits Allowed More
  - button "Select over 4.5 Hits Allowed for 1.78 times": 1.78x
  - text: 4.5 Hits Allowed
  - button "Select over 4.5 Hits Allowed for 1.78 times": 1.78x
  - button "Show More Stats"
  - img "Junior Caminero"
  - text: J. Caminero 3B - TB TB @ DET 6:40 PM
  - button "Open expert opinion for Junior Caminero"
  - text: Less Hits More
  - button "Select over 0.5 Hits for 2.61 times": 2.61x
  - text: 0.5 Hits
  - button "Select over 0.5 Hits for 1.28 times": 1.28x
  - button "Select over 1.5 Hits for 0 times" [disabled]
  - text: 1.5 Hits
  - button "Select over 1.5 Hits for 2.84 times": 2.84x
  - button "Select over 2.5 Hits for 0 times" [disabled]
  - text: 2.5 Hits
  - button "Select over 2.5 Hits for 7.79 times": 7.79x
  - button "Select over 3.5 Hits for 0 times" [disabled]
  - text: 3.5 Hits
  - button "Select over 3.5 Hits for 27.4 times": 27.4x
  - text: Less Hits + Runs + RBIs More
  - button "Select over 0.5 Hits + Runs + RBIs for 0 times" [disabled]
  - text: 0.5 H+R+R
  - button "Select over 0.5 Hits + Runs + RBIs for 1.21 times": 1.21x
  - button "Select over 1.5 Hits + Runs + RBIs for 1.89 times": 1.89x
  - text: 1.5 H+R+R
  - button "Select over 1.5 Hits + Runs + RBIs for 1.68 times": 1.68x
  - button "Select over 2.5 Hits + Runs + RBIs for 0 times" [disabled]
  - text: 2.5 H+R+R
  - button "Select over 2.5 Hits + Runs + RBIs for 2.34 times": 2.34x
  - button "Select over 3.5 Hits + Runs + RBIs for 0 times" [disabled]
  - text: 3.5 H+R+R
  - button "Select over 3.5 Hits + Runs + RBIs for 3.18 times": 3.18x
  - button "Select over 4.5 Hits + Runs + RBIs for 0 times" [disabled]
  - text: 4.5 H+R+R
  - button "Select over 4.5 Hits + Runs + RBIs for 4.51 times": 4.51x
  - text: Less Singles More
  - button "Select over 0.5 Singles for 1.72 times": 1.72x
  - text: 0.5 Singles
  - button "Select over 0.5 Singles for 1.78 times": 1.78x
  - button "Select over 1.5 Singles for 0 times" [disabled]
  - text: 1.5 Singles
  - button "Select over 1.5 Singles for 5.31 times": 5.31x
  - text: Less Doubles More
  - button "Select over 0.5 Doubles for 1.07 times": 1.07x
  - text: 0.5 Doubles
  - button "Select over 0.5 Doubles for 4.18 times": 4.18x
  - text: Less Triples More
  - button "Select over 0.5 Triples for 0 times" [disabled]
  - text: 0.5 Triples
  - button "Select over 0.5 Triples for 34 times": 34x
  - text: Less Runs More
  - button "Select over 0.5 Runs for 1.65 times": 1.65x
  - text: 0.5 Runs
  - button "Select over 0.5 Runs for 1.88 times": 1.88x
  - button "Select over 1.5 Runs for 0 times" [disabled]
  - text: 1.5 Runs
  - button "Select over 1.5 Runs for 5.66 times": 5.66x
  - text: Less RBIs More
  - button "Select over 0.5 RBIs for 1.35 times": 1.35x
  - text: 0.5 RBIs
  - button "Select over 0.5 RBIs for 2.27 times": 2.27x
  - button "Select over 1.5 RBIs for 0 times" [disabled]
  - text: 1.5 RBIs
  - button "Select over 1.5 RBIs for 4.2 times": 4.2x
  - button "Select over 2.5 RBIs for 0 times" [disabled]
  - text: 2.5 RBIs
  - button "Select over 2.5 RBIs for 7.79 times": 7.79x
  - text: Less Homeruns More
  - button "Select over 0.5 Homeruns for 0 times" [disabled]
  - text: 0.5 Homeruns
  - button "Select over 0.5 Homeruns for 4 times": 4x
  - button "Select over 1.5 Homeruns for 0 times" [disabled]
  - text: 1.5 Homeruns
  - button "Select over 1.5 Homeruns for 21.99 times": 21.99x
  - text: Less Total Bases More
  - button "Select over 1.5 Total Bases for 1.59 times": 1.59x
  - text: 1.5 Total Bases
  - button "Select over 1.5 Total Bases for 1.95 times": 1.95x
  - button "Select over 2.5 Total Bases for 0 times" [disabled]
  - text: 2.5 Total Bases
  - button "Select over 2.5 Total Bases for 2.74 times": 2.74x
  - button "Select over 3.5 Total Bases for 0 times" [disabled]
  - text: 3.5 Total Bases
  - button "Select over 3.5 Total Bases for 3.3 times": 3.3x
  - button "Select over 4.5 Total Bases for 0 times" [disabled]
  - text: 4.5 Total Bases
  - button "Select over 4.5 Total Bases for 5.24 times": 5.24x
  - button "Select over 5.5 Total Bases for 0 times" [disabled]
  - text: 5.5 Total Bases
  - button "Select over 5.5 Total Bases for 7.48 times": 7.48x
  - text: Less Strikeouts More
  - button "Select over 0.5 Strikeouts for 0 times" [disabled]
  - text: 0.5 Strikeouts
  - button "Select over 0.5 Strikeouts for 1.29 times": 1.29x
  - button "Select over 1.5 Strikeouts for 0 times" [disabled]
  - text: 1.5 Strikeouts
  - button "Select over 1.5 Strikeouts for 2.94 times": 2.94x
  - button "Select over 2.5 Strikeouts for 0 times" [disabled]
  - text: 2.5 Strikeouts
  - button "Select over 2.5 Strikeouts for 8.08 times": 8.08x
  - text: Less Fantasy Points More
  - button "Select over 6.5 Fantasy Points for 1.78 times": 1.78x
  - text: 6.5 Fantasy Points
  - button "Select over 6.5 Fantasy Points for 1.78 times": 1.78x
  - button "Show More Stats"
  - text: Please select your 1st pick
  - img "arrow"
  - heading "Let's Start!" [level=2]
  - text: Pick at least two players from different teams to play
  - link "Parlay Play Logo":
    - /url: /
    - img "Parlay Play Logo"
  - text: Improve your experience. Download our app.
  - link "Apple Store":
    - /url: https://parlayplay.onelink.me/oLJk/gnqpwjha
    - img "Apple Store"
  - link "Google Play Store":
    - /url: https://parlayplay.onelink.me/oLJk/fh7u6juo
    - img "Google Play Store"
  - link "Privacy":
    - /url: /privacy-policy
  - link "Fantasy Terms":
    - /url: /terms
  - link "Packs Terms":
    - /url: /terms/packs
  - link "Responsible Gaming":
    - /url: /responsible-gaming
  - link "Gaming Rules":
    - /url: /rules
  - link "FAQ":
    - /url: https://intercom.help/parlayplay/en/
  - link "Contact Us":
    - /url: /
  - paragraph: © ParlayPlay 2026 - All Rights Reserved
  - list:
    - listitem:
      - log
      - text: 🇺🇸English
      - combobox "Select language"
    - listitem:
      - img "18+-icon"
    - listitem:
      - link "ParlayPlay on Twitter":
        - /url: https://twitter.com/parlay_play?lang=en
    - listitem:
      - link "ParlayPlay on Facebook":
        - /url: https://www.facebook.com/ParlayPlay.io/
    - listitem:
      - link "ParlayPlay on Instagram":
        - /url: https://www.instagram.com/parlayplay_?igsh=bHBldWQyMmV2b3Y4
    - listitem:
      - link "ParlayPlay on Discord":
        - /url: https://discord.com/invite/parlayplay
  - link "Powered by SportsDataIO":
    - /url: https://sportsdata.io/
    - img "Powered by SportsDataIO"
- region "Notifications Alt+T"
- alert
```

# Test source

```ts
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
  103 |         await expect(alert).toBeVisible();
  104 |     };
  105 | 
  106 |     async openLogIn(): Promise<void> {
  107 |         await this.open('/account/login');
  108 |     };
  109 | 
  110 |     async joinBtnAssertion(): Promise<void> {
> 111 |         await expect(this.joinNowBtn).toBeVisible();
      |                                       ^ Error: expect(locator).toBeVisible() failed
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