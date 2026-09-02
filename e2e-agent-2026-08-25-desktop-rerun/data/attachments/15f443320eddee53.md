# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: home/home-search.spec.ts >> Home feed search >> Gibberish query shows the empty state, clearing restores the grid
- Location: tests/home/home-search.spec.ts:29:5

# Error details

```
Error: expect(locator).toBeVisible() failed

Locator: locator('div.relative.grow').filter({ has: locator('#search') }).locator('button[type="button"]').filter({ visible: true }).first()
Expected: visible
Timeout: 15000ms
Error: element(s) not found

Call log:
  - Expect "toBeVisible" with timeout 15000ms
  - waiting for locator('div.relative.grow').filter({ has: locator('#search') }).locator('button[type="button"]').filter({ visible: true }).first()

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
        - link "Packs":
          - /url: /packs
      - listitem:
        - link "Feed":
          - /url: /challenges/feed
      - listitem:
        - link "Rewards 6":
          - /url: /rewards
      - listitem:
        - link "Track Picks 55":
          - /url: /challenges/pending
    - button "Claim your $100 Deposit Match"
    - text: $208.92
    - img "gift-icon"
    - text: "5.00"
    - button "Toggle Menu"
- main:
  - button "previous slide"
  - text: Receive a referral Bonus! $20 Refer a Friend when they make their first deposit
  - button "Invite Now"
  - text: $100
  - img "black lightning bol"
  - text: = $200
  - img "black lightning bol"
  - text: We match your 1st deposit We match your first deposit up to $100.
  - button "Deposit Now"
  - button "next slide"
  - textbox "Search player or team": zzzqqqxyz
  - button
  - button "All"
  - button "MLB"
  - button "SerieA"
  - button "EPL"
  - button "WNBA"
  - button "WNBA-Combos"
  - button "WNBA Q1"
  - button "WNBA H1"
  - button "MLS"
  - button "NFLSZN"
  - button "LaLiga"
  - button "UFC"
  - button "Bundes"
  - button "right chevron sign Filter":
    - img "right chevron sign"
    - text: Filter
  - text: No Players Found Please select your 1st pick
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
  1  | /**
  2  |  * Home feed — player/team search filtering.
  3  |  *
  4  |  * The mobile feed header (components/Crossgame/Mobile/Header/SearchBar) filters
  5  |  * the player grid as you type and shows a clear (×) affordance while a term is
  6  |  * present; clearing restores the full grid. When nothing matches, the feed
  7  |  * renders the NoPlayerFound empty state (data-testid="no-player-found").
  8  |  *
  9  |  * This exercises the search surface end-to-end without depending on any
  10 |  * specific player being in the feed: the "no results" case uses a gibberish
  11 |  * term (deterministically matches nothing), and the "results" cases only
  12 |  * assert that the grid is non-empty before and after — so it stays green
  13 |  * regardless of which players the local/staging feed happens to carry. No
  14 |  * payment / KYC / third-party data is involved.
  15 |  */
  16 | import { test, expect } from '../../fixtures/test.extend';
  17 | import { HomePage } from '@pages/home.page';
  18 | 
  19 | test.describe('Home feed search', { tag: ['@home', '@search'] }, () => {
  20 |     // Read-only — no state mutation, isolated context per test. Fan out.
  21 |     test.describe.configure({ mode: 'parallel' });
  22 | 
  23 |     test.beforeEach(async ({ loggedInPage }) => {
  24 |         const homePage = new HomePage(loggedInPage);
  25 |         await loggedInPage.goto('/');
  26 |         await homePage.waitForFeedReady();
  27 |     });
  28 | 
  29 |     test('Gibberish query shows the empty state, clearing restores the grid', { tag: '@smoke' }, async ({ loggedInPage: page }) => {
  30 |         const homePage = new HomePage(page);
  31 | 
  32 |         await test.step('Feed starts with players and no empty state', async () => {
  33 |             await expect(homePage.playerCardsVisible.first()).toBeVisible();
  34 |             await expect(homePage.noPlayerFoundVisible).toBeHidden();
  35 |         });
  36 | 
  37 |         await test.step('Searching gibberish empties the grid', async () => {
  38 |             await homePage.searchPlayers('zzzqqqxyz');
  39 |             // The × clear affordance only renders once a term is present.
> 40 |             await expect(homePage.searchClearBtn).toBeVisible();
     |                                                   ^ Error: expect(locator).toBeVisible() failed
  41 |             await expect(homePage.noPlayerFoundVisible).toBeVisible();
  42 |             await expect(homePage.playerCardsVisible).toHaveCount(0);
  43 |         });
  44 | 
  45 |         await test.step('Clearing the search restores the players', async () => {
  46 |             await homePage.clearSearch();
  47 |             await expect(homePage.searchInput).toHaveValue('');
  48 |             await expect(homePage.noPlayerFoundVisible).toBeHidden();
  49 |             await expect(homePage.playerCardsVisible.first()).toBeVisible();
  50 |         });
  51 |     });
  52 | 
  53 |     test('Typing a term narrows the grid without dropping below the results', async ({ loggedInPage: page }) => {
  54 |         const homePage = new HomePage(page);
  55 | 
  56 |         await test.step('Grid is populated before searching', async () => {
  57 |             await expect(homePage.playerCardsVisible.first()).toBeVisible();
  58 |         });
  59 | 
  60 |         await test.step('A common letter keeps a non-empty, no-larger result set', async () => {
  61 |             const before = await homePage.playerCardsVisible.count();
  62 |             await homePage.searchPlayers('a');
  63 |             // A single-letter query is a filter, so the visible set can only
  64 |             // shrink or stay the same — never grow — and the empty state must
  65 |             // not appear for such a common letter.
  66 |             await expect(homePage.noPlayerFoundVisible).toBeHidden();
  67 |             await expect
  68 |                 .poll(async () => homePage.playerCardsVisible.count())
  69 |                 .toBeLessThanOrEqual(before);
  70 |             expect(await homePage.playerCardsVisible.count()).toBeGreaterThan(0);
  71 |         });
  72 |     });
  73 | });
  74 | 
```