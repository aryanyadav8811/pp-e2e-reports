# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: data-verification/player-detail-modal.spec.ts >> Data verification - player detail modal >> Expert-opinion modal renders the API's player data
- Location: tests/data-verification/player-detail-modal.spec.ts:23:5

# Error details

```
Error: expect(locator).toBeVisible() failed

Locator: locator('div[role="dialog"]').filter({ visible: true }).first().getByText('Matt Olson').first()
Expected: visible
Timeout: 15000ms
Error: element(s) not found

Call log:
  - Expect "toBeVisible" with timeout 15000ms
  - waiting for locator('div[role="dialog"]').filter({ visible: true }).first().getByText('Matt Olson').first()

```

# Page snapshot

```yaml
- generic [active] [ref=e1]:
  - generic [ref=e2]:
    - generic [ref=e3]:
      - banner [ref=e4]:
        - navigation [ref=e5]:
          - link "Parlay Play Logo" [ref=e6]:
            - /url: /
            - img "Parlay Play Logo" [ref=e8]
          - generic [ref=e10]:
            - generic [ref=e13]: $499.00
            - button "Toggle Menu" [ref=e14]:
              - img [ref=e15]
      - main [ref=e17]:
        - generic [ref=e20]:
          - img "warning icon" [ref=e21]
          - paragraph [ref=e22]: Something Went Wrong
          - paragraph [ref=e23]:
            - text: Sorry an unexpected error occurred!
            - text: Our team has been notified.
          - paragraph [ref=e24]:
            - text: If you require additional support please
            - button "contact us" [ref=e25] [cursor=pointer]
            - text: .
      - contentinfo [ref=e26]:
        - navigation [ref=e27]:
          - list [ref=e28]:
            - listitem [ref=e29]:
              - button "Home" [ref=e30] [cursor=pointer]:
                - generic [ref=e31]:
                  - img [ref=e32]
                  - generic [ref=e33]: Home
            - listitem [ref=e34]:
              - button "Entries 1" [ref=e35] [cursor=pointer]:
                - generic [ref=e36]:
                  - img [ref=e37]
                  - generic [ref=e38]: Entries
                - generic [ref=e39]: "1"
            - listitem [ref=e40]:
              - button "Feed" [ref=e41] [cursor=pointer]:
                - generic [ref=e42]:
                  - img [ref=e43]
                  - generic [ref=e44]: Feed
            - listitem [ref=e45]:
              - button "Rewards" [ref=e46] [cursor=pointer]:
                - generic [ref=e47]:
                  - img [ref=e48]
                  - generic [ref=e49]: Rewards
            - listitem [ref=e50]:
              - button "Packs" [ref=e51] [cursor=pointer]:
                - generic [ref=e52]:
                  - img [ref=e53]
                  - generic [ref=e54]: Packs
    - generic:
      - region "Notifications Alt+T"
  - alert [ref=e55]
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
  65  |         // challengeType must be one of the stats the offering gives this player.
  66  |         // The offering puts `challengeOption` directly on each stat (offering
  67  |         // `Stat.challenge_option`); the nested `challengeType.challengeOption`
  68  |         // lookups are kept only as a fallback for the legacy payload shape.
  69  |         const offeredOptions = apiPlayer!.stats
  70  |           .flatMap((s) => [
  71  |             s.challengeOption,
  72  |             s.challengeType?.challengeOption,
  73  |             ...(s.altLines?.values ?? []).map((v) => v.challengeType?.challengeOption),
  74  |           ])
  75  |           .filter(Boolean);
  76  |         expect(offeredOptions).toContain(requestUrl.searchParams.get('challengeType'));
  77  |       });
  78  | 
  79  |       // Oddin-widget and error responses render an iframe / fallback instead
  80  |       // of the opinion layout — nothing of ours to verify there.
  81  |       test.skip(
  82  |         body.type === 'oddin' || Boolean(body.error),
  83  |         `expert-opinion returned ${body.type ?? body.error}; no opinion layout to verify`,
  84  |       );
  85  | 
  86  |       const dialog = page.locator('div[role="dialog"]').filter({ visible: true }).first();
  87  |       await expect(dialog).toBeVisible();
  88  | 
  89  |       await test.step('Modal shows the API player name', async () => {
  90  |         const { firstName, lastName } = body.player ?? {};
  91  |         expect(firstName, 'expert-opinion response has no player.firstName').toBeTruthy();
  92  |         // The name appears in both the modal title and the narrative copy —
  93  |         // any visible occurrence proves the API name rendered.
> 94  |         await expect(dialog.getByText(`${firstName} ${lastName}`).first()).toBeVisible();
      |                                                                            ^ Error: expect(locator).toBeVisible() failed
  95  |       });
  96  | 
  97  |       await test.step("Modal stat tabs are the player's offered stats", async () => {
  98  |         // Mobile renders the stat switcher as a <select> (options are not
  99  |         // "visible"), desktop as tab buttons — check text content of both.
  100 |         const optionTexts = (await dialog.locator('select option').allInnerTexts()).map((t) =>
  101 |           t.trim(),
  102 |         );
  103 |         const dialogText = (await dialog.innerText()).replace(/\s+/g, ' ');
  104 |         const missing = apiPlayer!.stats
  105 |           .filter((stat) => mainLine(stat))
  106 |           .map((stat) => stat.challengeName)
  107 |           .filter((name) => !optionTexts.includes(name) && !dialogText.includes(name));
  108 |         expect(
  109 |           missing,
  110 |           `stats offered by the API but absent from the modal switcher: ${missing.join(', ')}`,
  111 |         ).toEqual([]);
  112 |       });
  113 |     });
  114 |   },
  115 | );
  116 | 
```