# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: modals/userlimits.spec.ts >> User Limits - Limit Exceeded Modal >> Exceeding the daily entry limit shows the Limit Exceeded modal and Reset Limits clears it
- Location: tests/modals/userlimits.spec.ts:46:3

# Error details

```
Error: submission must be rejected by the user limit

expect(received).toBe(expected) // Object.is equality

Expected: false
Received: true
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
          - generic [ref=e9]:
            - list [ref=e10]:
              - listitem [ref=e11]:
                - link "Home" [ref=e12] [cursor=pointer]:
                  - /url: /
                  - generic [ref=e14]: Home
              - listitem [ref=e15]:
                - link "Packs" [ref=e16] [cursor=pointer]:
                  - /url: /packs
                  - generic [ref=e18]: Packs
              - listitem [ref=e19]:
                - link "Feed" [ref=e20] [cursor=pointer]:
                  - /url: /challenges/feed
                  - generic [ref=e22]: Feed
              - listitem [ref=e23]:
                - link "Rewards" [ref=e24] [cursor=pointer]:
                  - /url: /rewards
                  - generic [ref=e26]: Rewards
              - listitem [ref=e27]:
                - link "Track Picks 1" [ref=e28] [cursor=pointer]:
                  - /url: /challenges/pending
                  - generic [ref=e29]:
                    - generic [ref=e30]: Track Picks
                    - generic [ref=e31]: "1"
            - button "Claim your $100 Deposit Match" [ref=e32] [cursor=pointer]
            - generic [ref=e33]:
              - generic [ref=e35]: $494.00
              - button "Add" [ref=e36]:
                - img [ref=e38]
                - img [ref=e40]
              - button "Toggle Menu" [ref=e42]:
                - img [ref=e43]
      - main [ref=e45]:
        - generic [ref=e47]:
          - generic [ref=e51]:
            - button "previous slide" [ref=e52] [cursor=pointer]:
              - img [ref=e53]
            - generic [ref=e56]:
              - generic [ref=e58]:
                - generic [ref=e59]:
                  - generic [ref=e60]: Receive a referral Bonus!
                  - generic [ref=e61]: $20
                - generic [ref=e62]:
                  - text: Refer a Friend
                  - text: when they make their first deposit
                  - button "Invite Now" [ref=e64] [cursor=pointer]
              - generic [ref=e66]:
                - generic [ref=e67]:
                  - text: $100
                  - img "black lightning bol" [ref=e68]
                - generic [ref=e70]: =
                - generic [ref=e71]:
                  - text: $200
                  - img "black lightning bol" [ref=e72]
                - generic [ref=e73]:
                  - text: We match your 1st deposit
                  - text: We match your first deposit up to $100.
                  - button "Deposit Now" [ref=e75] [cursor=pointer]
            - button "next slide" [ref=e76] [cursor=pointer]:
              - img [ref=e77]
          - generic [ref=e85]:
            - button [ref=e86]
            - dialog [ref=e88]:
              - generic [ref=e89]:
                - button [ref=e90]:
                  - img [ref=e91]
                - generic [ref=e95]:
                  - generic [ref=e97]: Picks Submitted
                  - generic [ref=e98]:
                    - generic [ref=e99]:
                      - generic [ref=e100]: All-in Play
                      - generic [ref=e101]: 10/13/2026
                    - generic [ref=e102]:
                      - generic [ref=e103]:
                        - generic [ref=e104]: Multiplier
                        - generic [ref=e105]: 3.91x
                      - generic [ref=e106]:
                        - generic [ref=e107]: $6.00 To Win
                        - generic [ref=e108]: $23.46
                    - generic [ref=e109]:
                      - generic [ref=e110]:
                        - generic [ref=e111]: "1."
                        - generic [ref=e113]: Jan Oblak
                        - generic [ref=e114]:
                          - generic [ref=e115]: More
                          - img [ref=e116]
                          - generic [ref=e118]: "1.50"
                          - generic [ref=e119]: Saves
                      - generic [ref=e120]:
                        - generic [ref=e121]: "2."
                        - generic [ref=e123]: Jurrien Timber
                        - generic [ref=e124]:
                          - generic [ref=e125]: More
                          - img [ref=e126]
                          - generic [ref=e128]: "0.50"
                          - generic [ref=e129]: Shots
                      - generic [ref=e130]:
                        - generic [ref=e131]: "3."
                        - generic [ref=e133]: Pablo Barrios Rivas
                        - generic [ref=e134]:
                          - generic [ref=e135]: More
                          - img [ref=e136]
                          - generic [ref=e138]: "0.50"
                          - generic [ref=e139]: Shots
                      - generic [ref=e140]:
                        - generic [ref=e141]: "4."
                        - generic [ref=e143]: Riccardo Calafiori
                        - generic [ref=e144]:
                          - generic [ref=e145]: More
                          - img [ref=e146]
                          - generic [ref=e148]: "0.50"
                          - generic [ref=e149]: Shots
                      - generic [ref=e150]:
                        - generic [ref=e151]: "5."
                        - generic [ref=e153]: Junior Caminero
                        - generic [ref=e154]:
                          - generic [ref=e155]: Less
                          - img [ref=e156]
                          - generic [ref=e158]: "0.50"
                          - generic [ref=e159]: Hits
                  - generic [ref=e160]: Track your lineup on the Leaderboard against other participants.
                  - generic [ref=e161]:
                    - button "share" [ref=e162] [cursor=pointer]:
                      - img "share" [ref=e163]
                    - button "Add Description" [ref=e164] [cursor=pointer]:
                      - img "Add Description" [ref=e165]
                    - button "Continue" [ref=e166] [cursor=pointer]
    - generic:
      - region "Notifications Alt+T"
  - alert [ref=e167]: ParlayPlay | Fun Fantasy Sports - Contest Submitted
  - iframe [ref=e168]:
    
```

# Test source

```ts
  7   | 
  8   | /**
  9   |  * Restore the account's limits to the platform defaults via the endpoint the
  10  |  * modal's "Reset Limits" button posts to. Runs in-page (not page.request) so
  11  |  * the call carries session cookies and dodges Cloudflare's bot challenge. A run
  12  |  * that dies between setting the $5 limit and resetting would otherwise poison
  13  |  * the shared account, and every later submission in the suite would 400.
  14  |  */
  15  | async function resetLimitsViaAPI(page: Page): Promise<void> {
  16  |   const status = await page.evaluate(async () => {
  17  |     const csrf = document.cookie
  18  |       .split('; ')
  19  |       .find((c) => c.startsWith('csrftoken='))
  20  |       ?.split('=')[1];
  21  |     const resp = await fetch('/api/v1/account/information/reset-limits/', {
  22  |       method: 'POST',
  23  |       headers: {
  24  |         'X-Requested-With': 'XMLHttpRequest',
  25  |         'X-Parlay-Request': '1',
  26  |         'X-CSRFToken': csrf ?? '',
  27  |         'Content-Type': 'application/json',
  28  |       },
  29  |       credentials: 'include',
  30  |     });
  31  |     return resp.status;
  32  |   });
  33  |   expect(status, 'reset-limits API should restore the default limits').toBe(200);
  34  | }
  35  | 
  36  | test.describe('User Limits - Limit Exceeded Modal', { tag: '@staging' }, () => {
  37  |   // loggedInPage opens about:blank — the home shell (Toggle Menu, etc.) only
  38  |   // mounts after navigation, so without this beforeEach enterMenu() hangs
  39  |   // until the test timeout.
  40  |   test.beforeEach(async ({ loggedInPage }) => {
  41  |     const home = new HomePage(loggedInPage);
  42  |     await loggedInPage.goto('/');
  43  |     await home.waitForFeedReady();
  44  |   });
  45  | 
  46  |   test('Exceeding the daily entry limit shows the Limit Exceeded modal and Reset Limits clears it', async ({
  47  |     loggedInPage: page,
  48  |   }) => {
  49  |     const homePage = new HomePage(page);
  50  |     const menuPage = new MenuPage(page);
  51  |     const responsiblePlayPage = new ResponsiblePlayPage(page);
  52  |     const contestPage = new ContestPage(page);
  53  | 
  54  |     // Demo-flagged accounts bypass every limit validator server-side, so the
  55  |     // modal can never appear for them — skip instead of failing. In-page
  56  |     // fetch, not page.request: Cloudflare bot-challenges Playwright's
  57  |     // out-of-browser HTTP client with a 403 interstitial.
  58  |     const userInfo = await page.evaluate(async () => {
  59  |       const resp = await fetch('/api/v1/user/', {
  60  |         headers: { 'X-Requested-With': 'XMLHttpRequest', 'X-Parlay-Request': '1' },
  61  |       });
  62  |       return resp.ok ? resp.json() : null;
  63  |     });
  64  |     test.skip(
  65  |       userInfo?.isDemoAccount === true,
  66  |       `${userInfo?.username} is demo-flagged — limit validators are bypassed by design. ` +
  67  |         'Unflag the account in admin or run with a non-demo user (TEST_USER=<suffix>).',
  68  |     );
  69  | 
  70  |     // Everything below mutates the account's limits; the finally-reset keeps a
  71  |     // mid-test failure from leaving a $5 daily cap on the shared user.
  72  |     try {
  73  |       await test.step('Open Responsible Play from the menu', async () => {
  74  |         await homePage.enterMenu();
  75  |         await menuPage.goToResponsiblePlay();
  76  |         await page.waitForURL('**/account/responsible-play');
  77  |         await responsiblePlayPage.verifyPage();
  78  |       });
  79  | 
  80  |       await test.step('Set the daily entry limit to $5', async () => {
  81  |         await responsiblePlayPage.updateAndVerifyDailyEntryLimit('5');
  82  |       });
  83  | 
  84  |       await test.step('Return to the home feed', async () => {
  85  |         await homePage.clickHomeLink();
  86  |       });
  87  | 
  88  |       await test.step('Pick five players and open the contest page', async () => {
  89  |         await homePage.waitForPlayersGrid();
  90  |         await homePage.pickFivePlayers();
  91  |         await homePage.enterFinalContestPage();
  92  |       });
  93  | 
  94  |       await test.step('Submit a $6 entry — rejected by the daily contest limit', async () => {
  95  |         await contestPage.verifyPage();
  96  |         await contestPage.setEntryAmountIfEditable(6);
  97  | 
  98  |         // Several workers submit as the same user, so the 1-per-5s throttle
  99  |         // can answer with a 429 before the limit validator runs (toast, no
  100 |         // modal). Retry through throttles until the server evaluates the entry.
  101 |         let result: { success: boolean; error: string | null } | null = null;
  102 |         for (let attempt = 1; attempt <= 5; attempt++) {
  103 |           result = await contestPage.submitAndAwaitResult();
  104 |           if (!/\b429\b|throttled|too many requests/i.test(result.error ?? '')) break;
  105 |           await page.waitForTimeout(8_000 + Math.floor(Math.random() * 7_000));
  106 |         }
> 107 |         expect(result?.success, 'submission must be rejected by the user limit').toBe(false);
      |                                                                                  ^ Error: submission must be rejected by the user limit
  108 |         expect(result?.error ?? '').toMatch(/exceed your (daily|weekly|monthly) contest limit/i);
  109 |       });
  110 | 
  111 |       await test.step('Limit Exceeded modal is shown', async () => {
  112 |         await contestPage.verifyLimitModalVisible();
  113 |       });
  114 | 
  115 |       await test.step('Reset Limits from the modal restores the defaults', async () => {
  116 |         await contestPage.clickResetLimit();
  117 |       });
  118 |     } finally {
  119 |       // Even if the modal flow already reset the limits (or never got that
  120 |       // far), leave the account on the defaults.
  121 |       await resetLimitsViaAPI(page);
  122 |     }
  123 |   });
  124 | });
  125 | 
```