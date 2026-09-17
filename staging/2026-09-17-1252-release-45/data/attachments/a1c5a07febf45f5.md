# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: data-verification/player-detail-modal.spec.ts >> Data verification - player detail modal >> Expert-opinion modal renders the API's player data
- Location: tests/data-verification/player-detail-modal.spec.ts:23:5

# Error details

```
Error: expect(received).toContain(expected) // indexOf

Expected value: "bab_pitchingStrikeouts"
Received array: []
```

# Page snapshot

```yaml
- generic [ref=e1]:
  - generic [ref=e2]:
    - generic [ref=e3]:
      - banner [ref=e4]:
        - navigation [ref=e5]:
          - link "Parlay Play Logo" [ref=e6] [cursor=pointer]:
            - /url: /
            - img "Parlay Play Logo" [ref=e8]
          - generic [ref=e10]:
            - generic [ref=e12]:
              - generic [ref=e13]: $591.00
              - generic [ref=e14]:
                - img "gift-icon" [ref=e15]
                - text: "17.00"
            - button "Toggle Menu" [ref=e16]:
              - img [ref=e17]
      - main [ref=e19]:
        - generic [ref=e20]:
          - generic [ref=e24]:
            - generic [ref=e25]:
              - generic [ref=e26]:
                - list [ref=e28]:
                  - button "MLB" [ref=e29] [cursor=pointer]
                  - button "NHL" [ref=e30] [cursor=pointer]
                  - button "SerieA" [ref=e31] [cursor=pointer]
                  - button "EPL" [ref=e32] [cursor=pointer]
                  - button "WNBA" [ref=e33] [cursor=pointer]
                  - button "WNBA-Combos" [ref=e34] [cursor=pointer]
                  - button "WNBA H1" [ref=e35] [cursor=pointer]
                  - button "WNBA Q1" [ref=e36] [cursor=pointer]
                  - button "CSGO" [ref=e37] [cursor=pointer]
                  - button "CSGO MAP1" [ref=e38] [cursor=pointer]
                  - button "MLS" [ref=e39] [cursor=pointer]
                  - button "LaLiga" [ref=e40] [cursor=pointer]
                  - button "UFC" [ref=e41] [cursor=pointer]
                  - button "Bundes" [ref=e42] [cursor=pointer]
                - list [ref=e44]:
                  - listitem [ref=e45]:
                    - button "ALL" [ref=e46] [cursor=pointer]:
                      - generic [ref=e47]: ALL
                  - listitem [ref=e48]:
                    - button "MIL@PIT 12:35PM" [ref=e49] [cursor=pointer]:
                      - text: MIL@PIT
                      - generic [ref=e50]: 12:35PM
                  - listitem [ref=e51]:
                    - button "LAD@CIN 12:40PM" [ref=e52] [cursor=pointer]:
                      - text: LAD@CIN
                      - generic [ref=e53]: 12:40PM
                  - listitem [ref=e54]:
                    - button "OAK@TB 1:10PM" [ref=e55] [cursor=pointer]:
                      - text: OAK@TB
                      - generic [ref=e56]: 1:10PM
                  - listitem [ref=e57]:
                    - button "SD@COL 3:10PM" [ref=e58] [cursor=pointer]:
                      - text: SD@COL
                      - generic [ref=e59]: 3:10PM
                  - listitem [ref=e60]:
                    - button "KC@HOU 7:15PM" [ref=e61] [cursor=pointer]:
                      - text: KC@HOU
                      - generic [ref=e62]: 7:15PM
                  - listitem [ref=e63]:
                    - button "PHI@NYM 7:15PM" [ref=e64] [cursor=pointer]:
                      - text: PHI@NYM
                      - generic [ref=e65]: 7:15PM
                  - listitem [ref=e66]:
                    - button "DET@CWS 7:40PM" [ref=e67] [cursor=pointer]:
                      - text: DET@CWS
                      - generic [ref=e68]: 7:40PM
                  - listitem [ref=e69]:
                    - button "BOS@TEX 8:05PM" [ref=e70] [cursor=pointer]:
                      - text: BOS@TEX
                      - generic [ref=e71]: 8:05PM
                  - listitem [ref=e72]:
                    - button "MIN@LAA 9:38PM" [ref=e73] [cursor=pointer]:
                      - text: MIN@LAA
                      - generic [ref=e74]: 9:38PM
                - generic [ref=e75]:
                  - generic [ref=e76]:
                    - generic [ref=e79]:
                      - generic:
                        - img
                      - textbox "Search player or team" [ref=e80]
                    - button "Change card style from grid" [ref=e82]
                  - list [ref=e84]:
                    - listitem [ref=e85]:
                      - button "Strikeouts (K)" [ref=e86]
                    - listitem [ref=e87]:
                      - button "Hits" [ref=e88]
                    - listitem [ref=e89]:
                      - button "Hits + Runs + RBIs" [ref=e90]
                    - listitem [ref=e91]:
                      - button "Singles" [ref=e92]
                    - listitem [ref=e93]:
                      - button "Doubles" [ref=e94]
                    - listitem [ref=e95]:
                      - button "Triples" [ref=e96]
                    - listitem [ref=e97]:
                      - button "Runs" [ref=e98]
                    - listitem [ref=e99]:
                      - button "RBIs" [ref=e100]
                    - listitem [ref=e101]:
                      - button "Hits Allowed" [ref=e102]
                    - listitem [ref=e103]:
                      - button "Pitching Outs" [ref=e104]
                    - listitem [ref=e105]:
                      - button "Pitches Thrown" [ref=e106]
                    - listitem [ref=e107]:
                      - button "Earned Runs" [ref=e108]
                    - listitem [ref=e109]:
                      - button "Homeruns" [ref=e110]
                    - listitem [ref=e111]:
                      - button "Total Bases" [ref=e112]
                    - listitem [ref=e113]:
                      - button "Strikeouts" [ref=e114]
                    - listitem [ref=e115]:
                      - button "Fantasy Points" [ref=e116]
              - generic [ref=e117]:
                - generic [ref=e122]:
                  - generic [ref=e125] [cursor=pointer]:
                    - generic [ref=e126]:
                      - generic [ref=e127]:
                        - generic [ref=e128]: 100%
                        - generic [ref=e129]: Deposit Match
                      - generic [ref=e130]: New User Promotion
                    - button "Deposit" [ref=e132]
                  - generic [ref=e136] [cursor=pointer]:
                    - generic [ref=e137]: Pull real graded cards worth up to $10,000
                    - generic [ref=e138]: Sell or ship instantly
                    - button "Rip a pack" [ref=e139]:
                      - generic [ref=e140]:
                        - img [ref=e141]
                        - text: Rip a pack
                  - generic [ref=e146] [cursor=pointer]:
                    - generic [ref=e147]:
                      - generic [ref=e148]: Refer a friend, get a $20 Free Entry
                      - generic [ref=e149]: Referral bonus
                    - button "Refer" [ref=e150]
                  - generic [ref=e153] [cursor=pointer]:
                    - generic [ref=e154]:
                      - generic [ref=e155]:
                        - img [ref=e156]
                        - generic [ref=e160]: Boosted Picks
                      - generic [ref=e161]: "Every Pick Pays: Up to a 35% Boost!"
                    - button "Details" [ref=e163]
                - generic [ref=e170]:
                  - generic [ref=e173]:
                    - button "Open expert opinion for Nolan McLean" [ref=e174]:
                      - img [ref=e175]
                    - img "Nolan McLean" [ref=e178]
                  - generic [ref=e179]:
                    - generic [ref=e180]: Nolan McLean
                    - button "5.5 SO (K)" [ref=e181]:
                      - generic [ref=e182]:
                        - img [ref=e183]
                        - img [ref=e185]
                      - generic [ref=e187]: "5.5"
                      - generic [ref=e188]: SO (K)
                    - generic [ref=e189]:
                      - generic [ref=e190]: PHI@NYM
                      - generic [ref=e191]: 7:15PM
                    - generic [ref=e192]:
                      - button "Select over 5.5 Strikeouts (K) for 1.71 times" [ref=e193]:
                        - img [ref=e194]
                        - generic [ref=e196]: 1.71x
                      - button "Select over 5.5 Strikeouts (K) for 1.94 times" [ref=e197]:
                        - generic [ref=e198]: 1.94x
                        - img [ref=e199]
            - generic [ref=e202]:
              - generic [ref=e204]:
                - link "Download ParlayPlay On The Play Store" [ref=e205] [cursor=pointer]:
                  - /url: https://parlayplay.onelink.me/oLJk/fh7u6juo
                  - img "Download ParlayPlay On The Play Store" [ref=e206]
                - paragraph [ref=e207]:
                  - text: Get the app.
                  - text: Better. Faster. Convenient
              - navigation [ref=e208]:
                - link "Privacy" [ref=e209] [cursor=pointer]:
                  - /url: /privacy-policy
                - link "Fantasy Terms" [ref=e210] [cursor=pointer]:
                  - /url: /terms
                - link "Packs Terms" [ref=e211] [cursor=pointer]:
                  - /url: /terms/packs
                - link "Responsible Gaming" [ref=e212] [cursor=pointer]:
                  - /url: /responsible-gaming
                - link "Gaming Rules" [ref=e213] [cursor=pointer]:
                  - /url: /rules
                - link "FAQ" [ref=e214] [cursor=pointer]:
                  - /url: https://intercom.help/parlayplay/en/
              - navigation [ref=e215]:
                - generic [ref=e216]:
                  - paragraph [ref=e217]: © ParlayPlay 2026
                  - generic [ref=e218]:
                    - link "ParlayPlay on Facebook" [ref=e219] [cursor=pointer]:
                      - /url: https://www.facebook.com/parlayplay.io
                      - img [ref=e220]
                    - link "ParlayPlay on Instagram" [ref=e222] [cursor=pointer]:
                      - /url: https://www.instagram.com/parlayplay_?igsh=bHBldWQyMmV2b3Y4
                      - img [ref=e223]
                    - link "ParlayPlay on Twitter" [ref=e225] [cursor=pointer]:
                      - /url: https://www.twitter.com/parlay_play
                      - img [ref=e226]
                    - link "ParlayPlay on Discord" [ref=e228] [cursor=pointer]:
                      - /url: https://discord.com/invite/parlayplay
                      - img [ref=e229]
                  - img "18+ icon" [ref=e231]
              - paragraph [ref=e233]
          - generic [ref=e235]:
            - button [ref=e236]
            - dialog [ref=e238]:
              - generic [ref=e239]:
                - button [active] [ref=e240]:
                  - img [ref=e241]
                - generic [ref=e244]:
                  - generic [ref=e246] [cursor=pointer]:
                    - combobox "Strikeouts (K)" [ref=e247]:
                      - option "Strikeouts (K)" [selected]
                      - option "Hits Allowed"
                      - option "Pitching Outs"
                      - option "Pitches Thrown"
                      - option "Earned Runs"
                      - option "Fantasy Points"
                    - generic: Strikeouts (K)
                    - generic:
                      - img
                  - generic [ref=e248]: Nolan McLean (SP)
                  - generic [ref=e249]:
                    - generic [ref=e250]: What others picked
                    - generic [ref=e253]:
                      - generic [ref=e254]: 55.0%
                      - generic [ref=e255]: NYM Win
                    - generic [ref=e258]:
                      - generic [ref=e259]: 50.0%
                      - generic [ref=e260]: More
                  - generic [ref=e261]:
                    - generic [ref=e262]: Season average
                    - generic [ref=e263]:
                      - generic [ref=e264]: "5.7"
                      - generic [ref=e265]: IP
                    - generic [ref=e266]:
                      - generic [ref=e267]: "6.3"
                      - generic [ref=e268]: K
                    - generic [ref=e269]:
                      - generic [ref=e270]: "2"
                      - generic [ref=e271]: ERA
                    - generic [ref=e272]:
                      - generic [ref=e273]: 12 - 8
                      - generic [ref=e274]: W-L
                  - generic [ref=e276]: Strikeouts (K) Last 5 Games
                  - generic [ref=e278]: This really can go either way for Nolan McLean...
      - contentinfo [ref=e279]:
        - navigation [ref=e280]:
          - list [ref=e281]:
            - listitem [ref=e282]:
              - button "Home" [ref=e283] [cursor=pointer]:
                - generic [ref=e284]:
                  - img [ref=e285]
                  - generic [ref=e286]: Home
            - listitem [ref=e287]:
              - button "Entries 138" [ref=e288] [cursor=pointer]:
                - generic [ref=e289]:
                  - img [ref=e290]
                  - generic [ref=e291]: Entries
                - generic [ref=e292]: "138"
            - listitem [ref=e293]:
              - button "Feed" [ref=e294] [cursor=pointer]:
                - generic [ref=e295]:
                  - img [ref=e296]
                  - generic [ref=e297]: Feed
            - listitem [ref=e298]:
              - button "Rewards 17" [ref=e299] [cursor=pointer]:
                - generic [ref=e300]:
                  - img [ref=e301]
                  - generic [ref=e302]: Rewards
                - generic [ref=e303]: "17"
            - listitem [ref=e304]:
              - button "Packs" [ref=e305] [cursor=pointer]:
                - generic [ref=e306]:
                  - img [ref=e307]
                  - generic [ref=e308]: Packs
    - generic:
      - region "Notifications Alt+T"
  - alert [ref=e309]
  - iframe [ref=e310]:
    
```

# Test source

```ts
  1   | /*
  2   |  The expert-opinion (player detail) modal must render the data from
  3   |  GET /api/v1/challenges-sp/expert-opinion/0/: the request carries the card's
  4   |  own player and matchId, the modal shows the API player name, and its stat
  5   |  tabs are the stats the offering actually gives that player.
  6   | */
  7   | 
  8   | import { test, expect } from '../../fixtures/test.extend';
  9   | import { HomePage } from '../../pages/home.page';
  10  | import {
  11  |   waitForOffering,
  12  |   indexPlayersById,
  13  |   mainLine,
  14  |   type OfferingResponse,
  15  | } from '../../utils/offeringData';
  16  | 
  17  | const EXPERT_OPINION_PATH = /\/api\/v1\/challenges-sp\/expert-opinion\//;
  18  | 
  19  | test.describe(
  20  |   'Data verification - player detail modal',
  21  |   { tag: ['@data-verification', '@prod'] },
  22  |   () => {
  23  |     test("Expert-opinion modal renders the API's player data", async ({ loggedInPage: page }) => {
  24  |       test.setTimeout(120_000);
  25  |       const home = new HomePage(page);
  26  | 
  27  |       let offering!: OfferingResponse;
  28  |       await test.step('Load home feed and capture /crossgame/offering/', async () => {
  29  |         const offeringPromise = waitForOffering(page);
  30  |         await page.goto('/');
  31  |         offering = await offeringPromise;
  32  |         await home.waitForFeedReady();
  33  |       });
  34  | 
  35  |       const playerIds = await home.listVisiblePlayerIds();
  36  |       expect(playerIds.length, 'no player cards mounted').toBeGreaterThan(0);
  37  |       const cardId = playerIds[0];
  38  |       const apiPlayer = indexPlayersById(offering).get(cardId.replace('player-', ''));
  39  |       expect(apiPlayer, `card ${cardId} missing from offering`).toBeTruthy();
  40  | 
  41  |       let body!: {
  42  |         player?: { firstName?: string; lastName?: string };
  43  |         error?: string;
  44  |         type?: string;
  45  |       };
  46  |       let requestUrl!: URL;
  47  |       await test.step(`Open the modal for ${cardId} and capture the expert-opinion response`, async () => {
  48  |         const card = home.playerCardById(cardId);
  49  |         const respPromise = page.waitForResponse(
  50  |           (r) =>
  51  |             EXPERT_OPINION_PATH.test(r.url()) &&
  52  |             r.request().method() === 'GET' &&
  53  |             r.status() === 200,
  54  |           { timeout: 30_000 },
  55  |         );
  56  |         await card.getByRole('button', { name: /open expert opinion for/i }).click();
  57  |         const resp = await respPromise;
  58  |         requestUrl = new URL(resp.url());
  59  |         body = await resp.json();
  60  |       });
  61  | 
  62  |       await test.step(`Request carries player=${apiPlayer!.player.id} and matchId=${apiPlayer!.match.id}`, async () => {
  63  |         expect(requestUrl.searchParams.get('player')).toBe(String(apiPlayer!.player.id));
  64  |         expect(requestUrl.searchParams.get('matchId')).toBe(String(apiPlayer!.match.id));
  65  |         // challengeType must be one of the stats the offering gives this player
  66  |         // (challengeOption lives on each alt-line value's challengeType).
  67  |         const offeredOptions = apiPlayer!.stats
  68  |           .flatMap((s) => [
  69  |             s.challengeType?.challengeOption,
  70  |             ...(s.altLines?.values ?? []).map((v) => v.challengeType?.challengeOption),
  71  |           ])
  72  |           .filter(Boolean);
> 73  |         expect(offeredOptions).toContain(requestUrl.searchParams.get('challengeType'));
      |                                ^ Error: expect(received).toContain(expected) // indexOf
  74  |       });
  75  | 
  76  |       // Oddin-widget and error responses render an iframe / fallback instead
  77  |       // of the opinion layout — nothing of ours to verify there.
  78  |       test.skip(
  79  |         body.type === 'oddin' || Boolean(body.error),
  80  |         `expert-opinion returned ${body.type ?? body.error}; no opinion layout to verify`,
  81  |       );
  82  | 
  83  |       const dialog = page.locator('div[role="dialog"]').filter({ visible: true }).first();
  84  |       await expect(dialog).toBeVisible();
  85  | 
  86  |       await test.step('Modal shows the API player name', async () => {
  87  |         const { firstName, lastName } = body.player ?? {};
  88  |         expect(firstName, 'expert-opinion response has no player.firstName').toBeTruthy();
  89  |         // The name appears in both the modal title and the narrative copy —
  90  |         // any visible occurrence proves the API name rendered.
  91  |         await expect(dialog.getByText(`${firstName} ${lastName}`).first()).toBeVisible();
  92  |       });
  93  | 
  94  |       await test.step("Modal stat tabs are the player's offered stats", async () => {
  95  |         // Mobile renders the stat switcher as a <select> (options are not
  96  |         // "visible"), desktop as tab buttons — check text content of both.
  97  |         const optionTexts = (await dialog.locator('select option').allInnerTexts()).map((t) =>
  98  |           t.trim(),
  99  |         );
  100 |         const dialogText = (await dialog.innerText()).replace(/\s+/g, ' ');
  101 |         const missing = apiPlayer!.stats
  102 |           .filter((stat) => mainLine(stat))
  103 |           .map((stat) => stat.challengeName)
  104 |           .filter((name) => !optionTexts.includes(name) && !dialogText.includes(name));
  105 |         expect(
  106 |           missing,
  107 |           `stats offered by the API but absent from the modal switcher: ${missing.join(', ')}`,
  108 |         ).toEqual([]);
  109 |       });
  110 |     });
  111 |   },
  112 | );
  113 | 
```