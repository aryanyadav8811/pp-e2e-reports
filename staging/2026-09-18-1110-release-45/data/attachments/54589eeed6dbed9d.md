# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: home/home-search.spec.ts >> Home - Feed Search >> A common letter narrows the grid without emptying it
- Location: tests/home/home-search.spec.ts:48:3

# Error details

```
Error: expect(received).toBeLessThanOrEqual(expected)

Expected: <= 1
Received:    4

Call Log:
- Timeout 15000ms exceeded while waiting on the predicate
```

# Page snapshot

```yaml
- generic [ref=e1]:
  - generic [ref=e2]:
    - generic [ref=e3]:
      - banner [ref=e4]:
        - navigation [ref=e5]:
          - link "Parlay Play Logo" [ref=e6]:
            - /url: /
            - img "Parlay Play Logo" [ref=e8]
          - generic [ref=e10]:
            - generic [ref=e12]:
              - generic [ref=e13]: $873.00
              - generic [ref=e14]:
                - img "gift-icon" [ref=e15]
                - text: "3.00"
            - button "Toggle Menu" [ref=e16]:
              - img [ref=e17]
      - main [ref=e19]:
        - generic [ref=e24]:
          - generic [ref=e25]:
            - generic [ref=e26]:
              - list [ref=e28]:
                - button "MLB" [ref=e29] [cursor=pointer]
                - button "NHL" [ref=e30] [cursor=pointer]
                - button "SerieA" [ref=e31] [cursor=pointer]
                - button "EPL" [ref=e32] [cursor=pointer]
                - button "CSGO" [ref=e33] [cursor=pointer]
                - button "WNBA" [ref=e34] [cursor=pointer]
                - button "WNBA-Combos" [ref=e35] [cursor=pointer]
                - button "WNBA Q1" [ref=e36] [cursor=pointer]
                - button "WNBA H1" [ref=e37] [cursor=pointer]
                - button "MLS" [ref=e38] [cursor=pointer]
                - button "LaLiga" [ref=e39] [cursor=pointer]
                - button "UFC" [ref=e40] [cursor=pointer]
                - button "Bundes" [ref=e41] [cursor=pointer]
                - button "Rugby League" [ref=e42] [cursor=pointer]
              - list [ref=e44]:
                - listitem [ref=e45]:
                  - button "ALL" [ref=e46] [cursor=pointer]:
                    - generic [ref=e47]: ALL
                - listitem [ref=e48]:
                  - button "CHC@CIN 6:40PM" [ref=e49] [cursor=pointer]:
                    - text: CHC@CIN
                    - generic [ref=e50]: 6:40PM
                - listitem [ref=e51]:
                  - button "KC@PIT 6:40PM" [ref=e52] [cursor=pointer]:
                    - text: KC@PIT
                    - generic [ref=e53]: 6:40PM
                - listitem [ref=e54]:
                  - button "MIL@BAL 7:05PM" [ref=e55] [cursor=pointer]:
                    - text: MIL@BAL
                    - generic [ref=e56]: 7:05PM
                - listitem [ref=e57]:
                  - button "OAK@CLE 7:10PM" [ref=e58] [cursor=pointer]:
                    - text: OAK@CLE
                    - generic [ref=e59]: 7:10PM
                - listitem [ref=e60]:
                  - button "BOS@TB 7:10PM" [ref=e61] [cursor=pointer]:
                    - text: BOS@TB
                    - generic [ref=e62]: 7:10PM
                - listitem [ref=e63]:
                  - button "PHI@NYM 7:15PM" [ref=e64] [cursor=pointer]:
                    - text: PHI@NYM
                    - generic [ref=e65]: 7:15PM
                - listitem [ref=e66]:
                  - button "DET@CWS 7:40PM" [ref=e67] [cursor=pointer]:
                    - text: DET@CWS
                    - generic [ref=e68]: 7:40PM
                - listitem [ref=e69]:
                  - button "TOR@TEX 8:05PM" [ref=e70] [cursor=pointer]:
                    - text: TOR@TEX
                    - generic [ref=e71]: 8:05PM
                - listitem [ref=e72]:
                  - button "SEA@COL 8:10PM" [ref=e73] [cursor=pointer]:
                    - text: SEA@COL
                    - generic [ref=e74]: 8:10PM
                - listitem [ref=e75]:
                  - button "ATL@HOU 8:10PM" [ref=e76] [cursor=pointer]:
                    - text: ATL@HOU
                    - generic [ref=e77]: 8:10PM
                - listitem [ref=e78]:
                  - button "WSH@STL 8:15PM" [ref=e79] [cursor=pointer]:
                    - text: WSH@STL
                    - generic [ref=e80]: 8:15PM
                - listitem [ref=e81]:
                  - button "MIN@LAA 9:38PM" [ref=e82] [cursor=pointer]:
                    - text: MIN@LAA
                    - generic [ref=e83]: 9:38PM
                - listitem [ref=e84]:
                  - button "NYY@ARI 9:40PM" [ref=e85] [cursor=pointer]:
                    - text: NYY@ARI
                    - generic [ref=e86]: 9:40PM
                - listitem [ref=e87]:
                  - button "MIA@SD 9:40PM" [ref=e88] [cursor=pointer]:
                    - text: MIA@SD
                    - generic [ref=e89]: 9:40PM
                - listitem [ref=e90]:
                  - button "SF@LAD 10:15PM" [ref=e91] [cursor=pointer]:
                    - text: SF@LAD
                    - generic [ref=e92]: 10:15PM
              - generic [ref=e93]:
                - generic [ref=e94]:
                  - generic [ref=e95]:
                    - generic [ref=e97]:
                      - generic:
                        - img
                      - textbox "Search player or team" [active] [ref=e98]: a
                    - button [ref=e99]:
                      - img [ref=e100]
                  - button "Change card style from grid" [ref=e103]
                - list [ref=e105]:
                  - listitem [ref=e106]:
                    - button "Strikeouts (K)" [ref=e107]
                  - listitem [ref=e108]:
                    - button "Hits" [ref=e109]
                  - listitem [ref=e110]:
                    - button "Hits + Runs + RBIs" [ref=e111]
                  - listitem [ref=e112]:
                    - button "Singles" [ref=e113]
                  - listitem [ref=e114]:
                    - button "Doubles" [ref=e115]
                  - listitem [ref=e116]:
                    - button "Triples" [ref=e117]
                  - listitem [ref=e118]:
                    - button "Runs" [ref=e119]
                  - listitem [ref=e120]:
                    - button "RBIs" [ref=e121]
                  - listitem [ref=e122]:
                    - button "Hits Allowed" [ref=e123]
                  - listitem [ref=e124]:
                    - button "Pitching Outs" [ref=e125]
                  - listitem [ref=e126]:
                    - button "Earned Runs" [ref=e127]
                  - listitem [ref=e128]:
                    - button "Homeruns" [ref=e129]
                  - listitem [ref=e130]:
                    - button "Total Bases" [ref=e131]
                  - listitem [ref=e132]:
                    - button "Strikeouts" [ref=e133]
                  - listitem [ref=e134]:
                    - button "Fantasy Points" [ref=e135]
            - generic [ref=e136]:
              - generic [ref=e141]:
                - generic [ref=e144] [cursor=pointer]:
                  - generic [ref=e145]:
                    - generic [ref=e146]:
                      - generic [ref=e147]: 100%
                      - generic [ref=e148]: Deposit Match
                    - generic [ref=e149]: New User Promotion
                  - button "Deposit" [ref=e151]
                - generic [ref=e155] [cursor=pointer]:
                  - generic [ref=e156]: Pull real graded cards worth up to $10,000
                  - generic [ref=e157]: Sell or ship instantly
                  - button "Rip a pack" [ref=e158]:
                    - generic [ref=e159]:
                      - img [ref=e160]
                      - text: Rip a pack
                - generic [ref=e165] [cursor=pointer]:
                  - generic [ref=e166]:
                    - generic [ref=e167]: Refer a friend, get a $20 Free Entry
                    - generic [ref=e168]: Referral bonus
                  - button "Refer" [ref=e169]
                - generic [ref=e172] [cursor=pointer]:
                  - generic [ref=e173]:
                    - generic [ref=e174]:
                      - img [ref=e175]
                      - generic [ref=e179]: Boosted Picks
                    - generic [ref=e180]: "Every Pick Pays: Up to a 35% Boost!"
                  - button "Details" [ref=e182]
              - generic [ref=e186]:
                - generic [ref=e189]:
                  - generic [ref=e192]:
                    - button "Open expert opinion for Paul Skenes" [ref=e193]:
                      - img [ref=e194]
                    - img "Paul Skenes" [ref=e197]
                  - generic [ref=e198]:
                    - generic [ref=e199]: Paul Skenes
                    - button "5.5 SO (K)" [ref=e200]:
                      - generic [ref=e201]:
                        - img [ref=e202]
                        - img [ref=e204]
                      - generic [ref=e206]: "5.5"
                      - generic [ref=e207]: SO (K)
                    - generic [ref=e208]:
                      - generic [ref=e209]: KC@PIT
                      - generic [ref=e210]: 6:40PM
                    - generic [ref=e211]:
                      - button "Select over 5.5 Strikeouts (K) for 1.93 times" [ref=e212]:
                        - img [ref=e213]
                        - generic [ref=e215]: 1.93x
                      - button "Select over 5.5 Strikeouts (K) for 1.72 times" [ref=e216]:
                        - generic [ref=e217]: 1.72x
                        - img [ref=e218]
                - generic [ref=e222]:
                  - generic [ref=e225]:
                    - button "Open expert opinion for Ian Seymour" [ref=e226]:
                      - img [ref=e227]
                    - img "Ian Seymour" [ref=e230]
                  - generic [ref=e231]:
                    - generic [ref=e232]: Ian Seymour
                    - button "5.5 SO (K)" [ref=e233]:
                      - generic [ref=e234]:
                        - img [ref=e235]
                        - img [ref=e237]
                      - generic [ref=e239]: "5.5"
                      - generic [ref=e240]: SO (K)
                    - generic [ref=e241]:
                      - generic [ref=e242]: BOS@TB
                      - generic [ref=e243]: 7:10PM
                    - generic [ref=e244]:
                      - button "Select over 5.5 Strikeouts (K) for 1.91 times" [ref=e245]:
                        - img [ref=e246]
                        - generic [ref=e248]: 1.91x
                      - button "Select over 5.5 Strikeouts (K) for 1.74 times" [ref=e249]:
                        - generic [ref=e250]: 1.74x
                        - img [ref=e251]
                - generic [ref=e255]:
                  - generic [ref=e258]:
                    - button "Open expert opinion for Dylan Cease" [ref=e259]:
                      - img [ref=e260]
                    - img "Dylan Cease" [ref=e263]
                  - generic [ref=e264]:
                    - generic [ref=e265]: Dylan Cease
                    - button "7.5 SO (K)" [ref=e266]:
                      - generic [ref=e267]:
                        - img [ref=e268]
                        - img [ref=e270]
                      - generic [ref=e272]: "7.5"
                      - generic [ref=e273]: SO (K)
                    - generic [ref=e274]:
                      - generic [ref=e275]: TOR@TEX
                      - generic [ref=e276]: 8:05PM
                    - generic [ref=e277]:
                      - button "Select over 7.5 Strikeouts (K) for 1.56 times" [ref=e278]:
                        - img [ref=e279]
                        - generic [ref=e281]: 1.56x
                      - button "Select over 7.5 Strikeouts (K) for 2.09 times" [ref=e282]:
                        - generic [ref=e283]: 2.09x
                        - img [ref=e284]
                - generic [ref=e288]:
                  - generic [ref=e291]:
                    - button "Open expert opinion for Nick Pivetta" [ref=e292]:
                      - img [ref=e293]
                    - img "Nick Pivetta" [ref=e296]
                  - generic [ref=e297]:
                    - generic [ref=e298]: Nick Pivetta
                    - button "4.5 SO (K)" [ref=e299]:
                      - generic [ref=e300]:
                        - img [ref=e301]
                        - img [ref=e303]
                      - generic [ref=e305]: "4.5"
                      - generic [ref=e306]: SO (K)
                    - generic [ref=e307]:
                      - generic [ref=e308]: MIA@SD
                      - generic [ref=e309]: 9:40PM
                    - generic [ref=e310]:
                      - button "Select over 4.5 Strikeouts (K) for 2.18 times" [ref=e311]:
                        - img [ref=e312]
                        - generic [ref=e314]: 2.18x
                      - button "Select over 4.5 Strikeouts (K) for 1.52 times" [ref=e315]:
                        - generic [ref=e316]: 1.52x
                        - img [ref=e317]
          - generic [ref=e320]:
            - generic [ref=e322]:
              - link "Download ParlayPlay On The App Store" [ref=e323]:
                - /url: https://parlayplay.onelink.me/oLJk/gnqpwjha
                - img "Download ParlayPlay On The App Store" [ref=e324]
              - paragraph [ref=e325]:
                - text: Get the app.
                - text: Better. Faster. Convenient
            - navigation [ref=e326]:
              - link "Privacy" [ref=e327]:
                - /url: /privacy-policy
              - link "Fantasy Terms" [ref=e328]:
                - /url: /terms
              - link "Packs Terms" [ref=e329]:
                - /url: /terms/packs
              - link "Responsible Gaming" [ref=e330]:
                - /url: /responsible-gaming
              - link "Gaming Rules" [ref=e331]:
                - /url: /rules
              - link "FAQ" [ref=e332]:
                - /url: https://intercom.help/parlayplay/en/
            - navigation [ref=e333]:
              - generic [ref=e334]:
                - paragraph [ref=e335]: © ParlayPlay 2026
                - generic [ref=e336]:
                  - link "ParlayPlay on Facebook" [ref=e337]:
                    - /url: https://www.facebook.com/parlayplay.io
                    - img [ref=e338]
                  - link "ParlayPlay on Instagram" [ref=e340]:
                    - /url: https://www.instagram.com/parlayplay_?igsh=bHBldWQyMmV2b3Y4
                    - img [ref=e341]
                  - link "ParlayPlay on Twitter" [ref=e343]:
                    - /url: https://www.twitter.com/parlay_play
                    - img [ref=e344]
                  - link "ParlayPlay on Discord" [ref=e346]:
                    - /url: https://discord.com/invite/parlayplay
                    - img [ref=e347]
                - img "18+ icon" [ref=e349]
            - paragraph [ref=e351]
      - contentinfo [ref=e352]:
        - navigation [ref=e353]:
          - list [ref=e354]:
            - listitem [ref=e355]:
              - button "Home" [ref=e356] [cursor=pointer]:
                - generic [ref=e357]:
                  - img [ref=e358]
                  - generic [ref=e359]: Home
            - listitem [ref=e360]:
              - button "Entries 133" [ref=e361] [cursor=pointer]:
                - generic [ref=e362]:
                  - img [ref=e363]
                  - generic [ref=e364]: Entries
                - generic [ref=e365]: "133"
            - listitem [ref=e366]:
              - button "Feed" [ref=e367] [cursor=pointer]:
                - generic [ref=e368]:
                  - img [ref=e369]
                  - generic [ref=e370]: Feed
            - listitem [ref=e371]:
              - button "Rewards 4" [ref=e372] [cursor=pointer]:
                - generic [ref=e373]:
                  - img [ref=e374]
                  - generic [ref=e375]: Rewards
                - generic [ref=e376]: "4"
            - listitem [ref=e377]:
              - button "Packs" [ref=e378] [cursor=pointer]:
                - generic [ref=e379]:
                  - img [ref=e380]
                  - generic [ref=e381]: Packs
    - generic:
      - region "Notifications Alt+T"
  - alert [ref=e382]
```

# Test source

```ts
  1  | /**
  2  |  * Home feed search: the mobile feed header filters the player grid as you
  3  |  * type, shows a clear (×) affordance while a term is present, and renders the
  4  |  * NoPlayerFound empty state when nothing matches. Independent of feed
  5  |  * contents — the "no results" case uses a gibberish term.
  6  |  */
  7  | import { test, expect } from '../../fixtures/test.extend';
  8  | import { HomePage } from '@pages/home.page';
  9  | 
  10 | test.describe('Home - Feed Search', { tag: ['@home', '@search', '@prod'] }, () => {
  11 |   // Read-only — no state mutation, isolated context per test. Fan out.
  12 |   test.describe.configure({ mode: 'parallel' });
  13 | 
  14 |   test.beforeEach(async ({ loggedInPage }) => {
  15 |     const homePage = new HomePage(loggedInPage);
  16 |     await loggedInPage.goto('/');
  17 |     await homePage.waitForFeedReady();
  18 |   });
  19 | 
  20 |   test(
  21 |     'Gibberish query shows the empty state, clearing restores the grid',
  22 |     { tag: ['@smoke', '@critical'] },
  23 |     async ({ loggedInPage: page }) => {
  24 |       const homePage = new HomePage(page);
  25 | 
  26 |       await test.step('Feed starts with players and no empty state', async () => {
  27 |         await expect(homePage.playerCardsVisible.first()).toBeVisible();
  28 |         await expect(homePage.noPlayerFoundVisible).toBeHidden();
  29 |       });
  30 | 
  31 |       await test.step('Searching "zzzqqqxyz" empties the grid and shows the empty state', async () => {
  32 |         await homePage.searchPlayers('zzzqqqxyz');
  33 |         // The × clear affordance only renders once a term is present.
  34 |         await expect(homePage.searchClearBtn).toBeVisible();
  35 |         await expect(homePage.noPlayerFoundVisible).toBeVisible();
  36 |         await expect(homePage.playerCardsVisible).toHaveCount(0);
  37 |       });
  38 | 
  39 |       await test.step('Clearing the search restores the players', async () => {
  40 |         await homePage.clearSearch();
  41 |         await expect(homePage.searchInput).toHaveValue('');
  42 |         await expect(homePage.noPlayerFoundVisible).toBeHidden();
  43 |         await expect(homePage.playerCardsVisible.first()).toBeVisible();
  44 |       });
  45 |     },
  46 |   );
  47 | 
  48 |   test('A common letter narrows the grid without emptying it', async ({ loggedInPage: page }) => {
  49 |     const homePage = new HomePage(page);
  50 | 
  51 |     await test.step('Grid is populated before searching', async () => {
  52 |       await expect(homePage.playerCardsVisible.first()).toBeVisible();
  53 |     });
  54 | 
  55 |     await test.step('Searching "a" keeps a non-empty result set no larger than before', async () => {
  56 |       const before = await homePage.playerCardsVisible.count();
  57 |       await homePage.searchPlayers('a');
  58 |       // A query is a filter: the visible set can shrink or stay the same,
  59 |       // never grow, and such a common letter must not hit the empty state.
  60 |       await expect(homePage.noPlayerFoundVisible).toBeHidden();
> 61 |       await expect
     |       ^ Error: expect(received).toBeLessThanOrEqual(expected)
  62 |         .poll(async () => homePage.playerCardsVisible.count())
  63 |         .toBeLessThanOrEqual(before);
  64 |       expect(await homePage.playerCardsVisible.count()).toBeGreaterThan(0);
  65 |     });
  66 |   });
  67 | });
  68 | 
```