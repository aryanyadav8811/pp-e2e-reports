# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: navigation/footer-nav.spec.ts >> Bottom nav — tab routing & active indicator (DFS-1998) >> Rewards tab routes into /rewards and takes the indicator
- Location: tests/navigation/footer-nav.spec.ts:58:5

# Error details

```
Error: page.waitForURL: Target page, context or browser has been closed
=========================== logs ===========================
waiting for navigation until "load"
  navigated to "https://dev.parlayplay.io/account/login?showFreeSignup=true"
============================================================
```

# Test source

```ts
  1   | /**
  2   |  * Bottom-nav tab routing + active indicator — footer restructure
  3   |  * (DFS-1998 / DFS-2088).
  4   |  *
  5   |  * The mobile bottom nav (components/Footer/index.tsx) has five tabs, each
  6   |  * routing to its own destination and lighting up an active underline while
  7   |  * that route is showing:
  8   |  *
  9   |  *   Home       → /
  10  |  *   Entries    → /challenges/pending   (also active on /challenges/history)
  11  |  *   Feed       → /challenges/feed
  12  |  *   Rewards    → /rewards/...           (pathname.startsWith("/rewards"))
  13  |  *   Free2Play  → /challenges/mp         (only when packs_visibility hides Packs)
  14  |  *   Packs      → /packs                 (DFS-2115/DFS-2146 kill switch; replaces
  15  |  *                                        the Free2Play slot when visible)
  16  |  *
  17  |  * The Entries indicator's cross-sub-tab behaviour is locked in separately by
  18  |  * entries-nav-indicator.spec.ts (DFS-1816); this spec covers the *other* tabs'
  19  |  * routing and the mutual-exclusivity of the indicator. In the markup each tab
  20  |  * label <span> always carries `border-playYellow`; the active underline is the
  21  |  * extra `border-b-2` class toggled on only for the current route — so that
  22  |  * class is what these tests assert on (via HomePage.navIndicator, which scopes
  23  |  * to the bottom-nav <nav> so a tab label can't collide with same-named page
  24  |  * content).
  25  |  *
  26  |  * All routes are internal and need no payment / KYC / feed data to reach, so
  27  |  * this suite is safe to fan out across workers.
  28  |  */
  29  | import { test, expect } from '../../fixtures/test.extend';
  30  | import { HomePage } from '@pages/home.page';
  31  | 
  32  | test.describe('Bottom nav — tab routing & active indicator (DFS-1998)', { tag: ['@navigation', '@dfs1998', '@prod'] }, () => {
  33  |     // Read-only navigation, isolated context per test — safe in parallel.
  34  |     test.describe.configure({ mode: 'parallel' });
  35  | 
  36  |     test.beforeEach(async ({ loggedInPage }) => {
  37  |         const homePage = new HomePage(loggedInPage);
  38  |         await loggedInPage.goto('/');
  39  |         await homePage.waitForFeedReady();
  40  |     });
  41  | 
  42  |     test('Feed tab routes to /challenges/feed and takes the indicator', async ({ loggedInPage: page }) => {
  43  |         const homePage = new HomePage(page);
  44  | 
  45  |         await test.step('Home is active on landing', async () => {
  46  |             await expect(homePage.navIndicator('Home')).toHaveClass(/border-b-2/);
  47  |             await expect(homePage.navIndicator('Feed')).not.toHaveClass(/border-b-2/);
  48  |         });
  49  | 
  50  |         await test.step('Open Feed — indicator moves to Feed, off Home', async () => {
  51  |             await homePage.enterFeedPage();
  52  |             await page.waitForURL('**/challenges/feed');
  53  |             await expect(homePage.navIndicator('Feed')).toHaveClass(/border-b-2/);
  54  |             await expect(homePage.navIndicator('Home')).not.toHaveClass(/border-b-2/);
  55  |         });
  56  |     });
  57  | 
  58  |     test('Rewards tab routes into /rewards and takes the indicator', async ({ loggedInPage: page }) => {
  59  |         const homePage = new HomePage(page);
  60  | 
  61  |         await test.step('Open Rewards — lands on a /rewards route', async () => {
  62  |             await homePage.enterRewarsdsPage();
  63  |             // The tab resolves to /rewards or /rewards/promotions depending on
  64  |             // the partner-reward count, so match the /rewards prefix.
> 65  |             await page.waitForURL(/\/rewards(\/|$)/);
      |                        ^ Error: page.waitForURL: Target page, context or browser has been closed
  66  |             await expect(homePage.navIndicator('Rewards')).toHaveClass(/border-b-2/);
  67  |         });
  68  |     });
  69  | 
  70  |     test('Fifth tab (Free2Play or Packs) routes and takes the indicator', async ({ loggedInPage: page }) => {
  71  |         const homePage = new HomePage(page);
  72  | 
  73  |         // DFS-2115 / DFS-2146: the fifth footer slot renders Packs when the
  74  |         // user's packs_visibility allows it and Free2Play otherwise, so detect
  75  |         // which one this environment mounted and assert that tab's routing.
  76  |         const packsVisible = await homePage.packsTab
  77  |             .isVisible()
  78  |             .catch(() => false);
  79  | 
  80  |         if (packsVisible) {
  81  |             await test.step('Open Packs — indicator moves to Packs', async () => {
  82  |                 await homePage.packsTab.click();
  83  |                 await page.waitForURL('**/packs**');
  84  |                 await expect(homePage.navIndicator('Packs')).toHaveClass(/border-b-2/);
  85  |                 await expect(homePage.navIndicator('Home')).not.toHaveClass(/border-b-2/);
  86  |             });
  87  | 
  88  |             // DFS-2115: with Packs in the footer, Free2Play relocates to the
  89  |             // burger menu (Account Center → Rewards) — it must still route.
  90  |             // No indicator assertion here: there's no footer tab to underline.
  91  |             await test.step('Free2Play still routes from the burger menu', async () => {
  92  |                 await homePage.enterFree2PlayPage();
  93  |                 await page.waitForURL('**/challenges/mp');
  94  |             });
  95  |         } else {
  96  |             await test.step('Open Free2Play — indicator moves to Free2Play', async () => {
  97  |                 await homePage.enterFree2PlayPage();
  98  |                 await page.waitForURL('**/challenges/mp');
  99  |                 await expect(homePage.navIndicator('Free2Play')).toHaveClass(/border-b-2/);
  100 |                 await expect(homePage.navIndicator('Home')).not.toHaveClass(/border-b-2/);
  101 |             });
  102 |         }
  103 |     });
  104 | 
  105 |     test('Only one tab is active at a time and Home restores', { tag: ['@smoke', '@critical'] }, async ({ loggedInPage: page }) => {
  106 |         const homePage = new HomePage(page);
  107 | 
  108 |         await test.step('Navigate to Feed', async () => {
  109 |             await homePage.enterFeedPage();
  110 |             await page.waitForURL('**/challenges/feed');
  111 |             await expect(homePage.navIndicator('Feed')).toHaveClass(/border-b-2/);
  112 |             await expect(homePage.navIndicator('Home')).not.toHaveClass(/border-b-2/);
  113 |         });
  114 | 
  115 |         await test.step('Back to Home — indicator returns to Home, off Feed', async () => {
  116 |             await homePage.enterHomePage();
  117 |             await page.waitForURL(/\/$/);
  118 |             await expect(homePage.navIndicator('Home')).toHaveClass(/border-b-2/);
  119 |             await expect(homePage.navIndicator('Feed')).not.toHaveClass(/border-b-2/);
  120 |         });
  121 |     });
  122 | });
  123 | 
```