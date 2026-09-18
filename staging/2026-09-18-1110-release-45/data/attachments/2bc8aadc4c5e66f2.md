# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: contests/user-enter-contest.spec.ts >> Contests - Enter Contest >> Placed contest appears in the My Entries list
- Location: tests/contests/user-enter-contest.spec.ts:88:3

# Error details

```
Error: Timeout 30000ms exceeded while waiting on the predicate
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
              - generic [ref=e13]: $879.00
              - generic [ref=e14]:
                - img "gift-icon" [ref=e15]
                - text: "3.00"
            - button "Toggle Menu" [ref=e16]:
              - img [ref=e17]
      - main [ref=e19]:
        - generic [ref=e22]:
          - navigation [ref=e23]:
            - list [ref=e24]:
              - listitem [ref=e25]:
                - button "Active" [ref=e26]
              - listitem [ref=e27]:
                - button "History" [ref=e28]
          - generic [ref=e29]:
            - generic [ref=e31]:
              - generic [ref=e32]:
                - generic [ref=e33]: $396
                - generic [ref=e34]: Entry Amount
              - img "chest-icon" [ref=e35]
              - generic [ref=e36]:
                - generic [ref=e37]: $7450.05
                - generic [ref=e38]: Max Payout
            - generic [ref=e39]:
              - region [ref=e40]:
                - button "Expand entry details" [ref=e41]:
                  - generic [ref=e43]:
                    - generic [ref=e45]:
                      - text: $3
                      - generic [ref=e46]: for $16.59
                    - generic [ref=e47]: All In 5.53x
                  - generic [ref=e48]:
                    - generic [ref=e50]: "1"
                    - generic [ref=e52]: "2"
                    - generic [ref=e54]: "3"
                    - generic [ref=e56]: "4"
                - button "Expand entry details" [ref=e59]:
                  - img "Expand" [ref=e60]
              - region [ref=e61]:
                - button "Expand entry details" [ref=e62]:
                  - generic [ref=e64]:
                    - generic [ref=e66]:
                      - text: $3
                      - generic [ref=e67]: for $30.45
                    - generic [ref=e68]: All In 10.15x
                  - generic [ref=e69]:
                    - generic [ref=e71]: "1"
                    - generic [ref=e73]: "2"
                    - generic [ref=e75]: "3"
                    - generic [ref=e77]: "4"
                    - generic [ref=e79]: "5"
                - button "Expand entry details" [ref=e82]:
                  - img "Expand" [ref=e83]
              - region [ref=e84]:
                - button "Expand entry details" [ref=e85]:
                  - generic [ref=e87]:
                    - generic [ref=e89]:
                      - text: $3
                      - generic [ref=e90]: for $5.97
                    - generic [ref=e91]: All In 1.99x
                  - generic [ref=e92]:
                    - generic [ref=e94]: "1"
                    - generic [ref=e96]: "2"
                - button "Expand entry details" [ref=e99]:
                  - img "Expand" [ref=e100]
              - region [ref=e101]:
                - button "Expand entry details" [ref=e102]:
                  - generic [ref=e104]:
                    - generic [ref=e106]:
                      - text: $3
                      - generic [ref=e107]: for $30.45
                    - generic [ref=e108]: All In 10.15x
                  - generic [ref=e109]:
                    - generic [ref=e111]: "1"
                    - generic [ref=e113]: "2"
                    - generic [ref=e115]: "3"
                    - generic [ref=e117]: "4"
                    - generic [ref=e119]: "5"
                - button "Expand entry details" [ref=e122]:
                  - img "Expand" [ref=e123]
              - region [ref=e124]:
                - button "Expand entry details" [ref=e125]:
                  - generic [ref=e127]:
                    - generic [ref=e129]:
                      - text: $3
                      - generic [ref=e130]: for $31.29
                    - generic [ref=e131]: All In 10.43x
                  - generic [ref=e132]:
                    - img [ref=e134]
                    - generic [ref=e137]: "2"
                    - generic [ref=e139]: "3"
                    - generic [ref=e141]: "4"
                - button "Expand entry details" [ref=e144]:
                  - img "Expand" [ref=e145]
              - region [ref=e146]:
                - button "Expand entry details" [ref=e147]:
                  - generic [ref=e149]:
                    - generic [ref=e151]:
                      - text: $3
                      - generic [ref=e152]: for $37.29
                    - generic [ref=e153]: All In 12.43x
                  - generic [ref=e154]:
                    - img [ref=e156]
                    - generic [ref=e159]: "2"
                    - generic [ref=e161]: "3"
                    - generic [ref=e163]: "4"
                - button "Expand entry details" [ref=e166]:
                  - img "Expand" [ref=e167]
              - region [ref=e168]:
                - button "Expand entry details" [ref=e169]:
                  - generic [ref=e170]:
                    - generic [ref=e171]:
                      - generic [ref=e173]:
                        - text: $3
                        - generic [ref=e174]: for $40.35
                      - generic [ref=e175]: All In 13.45x
                    - generic [ref=e178]: Live
                  - generic [ref=e179]:
                    - generic [ref=e181]: "1"
                    - generic [ref=e183]: "2"
                    - generic [ref=e185]: "3"
                    - img [ref=e187]
                - button "Expand entry details" [ref=e193]:
                  - img "Expand" [ref=e194]
              - region [ref=e195]:
                - button "Expand entry details" [ref=e196]:
                  - generic [ref=e198]:
                    - generic [ref=e200]:
                      - text: $3
                      - generic [ref=e201]: for $59.43
                    - generic [ref=e202]: All In 19.81x
                  - generic [ref=e203]:
                    - img [ref=e205]
                    - img [ref=e208]
                    - generic [ref=e211]: "3"
                    - generic [ref=e213]: "4"
                    - generic [ref=e215]: "5"
                - button "Expand entry details" [ref=e218]:
                  - img "Expand" [ref=e219]
              - region [ref=e220]:
                - button "Expand entry details" [ref=e221]:
                  - generic [ref=e223]:
                    - generic [ref=e225]:
                      - text: $3
                      - generic [ref=e226]: for $58.38
                    - generic [ref=e227]: All In 19.46x
                  - generic [ref=e228]:
                    - img [ref=e230]
                    - img [ref=e233]
                    - generic [ref=e236]: "3"
                    - generic [ref=e238]: "4"
                    - generic [ref=e240]: "5"
                - button "Expand entry details" [ref=e243]:
                  - img "Expand" [ref=e244]
              - region [ref=e245]:
                - button "Expand entry details" [ref=e246]:
                  - generic [ref=e248]:
                    - generic [ref=e250]:
                      - text: $3
                      - generic [ref=e251]: for $59.43
                    - generic [ref=e252]: All In 19.81x
                  - generic [ref=e253]:
                    - img [ref=e255]
                    - img [ref=e258]
                    - generic [ref=e261]: "3"
                    - generic [ref=e263]: "4"
                    - generic [ref=e265]: "5"
                - button "Expand entry details" [ref=e268]:
                  - img "Expand" [ref=e269]
              - region [ref=e270]:
                - button "Expand entry details" [ref=e271]:
                  - generic [ref=e273]:
                    - generic [ref=e275]:
                      - text: $3
                      - generic [ref=e276]: for $58.38
                    - generic [ref=e277]: All In 19.46x
                  - generic [ref=e278]:
                    - img [ref=e280]
                    - img [ref=e283]
                    - generic [ref=e286]: "3"
                    - generic [ref=e288]: "4"
                    - generic [ref=e290]: "5"
                - button "Expand entry details" [ref=e293]:
                  - img "Expand" [ref=e294]
              - region [ref=e295]:
                - button "Expand entry details" [ref=e296]:
                  - generic [ref=e298]:
                    - generic [ref=e300]:
                      - text: $3
                      - generic [ref=e301]: for $60.57
                    - generic [ref=e302]: All In 20.19x
                  - generic [ref=e303]:
                    - img [ref=e305]
                    - img [ref=e308]
                    - generic [ref=e311]: "3"
                    - generic [ref=e313]: "4"
                    - generic [ref=e315]: "5"
                - button "Expand entry details" [ref=e318]:
                  - img "Expand" [ref=e319]
              - region [ref=e320]:
                - button "Expand entry details" [ref=e321]:
                  - generic [ref=e323]:
                    - generic [ref=e325]:
                      - text: $3
                      - generic [ref=e326]: for $58.38
                    - generic [ref=e327]: All In 19.46x
                  - generic [ref=e328]:
                    - img [ref=e330]
                    - img [ref=e333]
                    - generic [ref=e336]: "3"
                    - generic [ref=e338]: "4"
                    - generic [ref=e340]: "5"
                - button "Expand entry details" [ref=e343]:
                  - img "Expand" [ref=e344]
              - region [ref=e345]:
                - button "Expand entry details" [ref=e346]:
                  - generic [ref=e348]:
                    - generic [ref=e350]:
                      - text: $3
                      - generic [ref=e351]: for $25.86
                    - generic [ref=e352]: All In 8.62x
                  - generic [ref=e353]:
                    - img [ref=e355]
                    - generic [ref=e358]: "2"
                    - generic [ref=e360]: "3"
                    - generic [ref=e362]: "4"
                    - generic [ref=e364]: "5"
                - button "Expand entry details" [ref=e367]:
                  - img "Expand" [ref=e368]
              - region [ref=e369]:
                - button "Expand entry details" [ref=e370]:
                  - generic [ref=e372]:
                    - generic [ref=e374]:
                      - text: $3
                      - generic [ref=e375]: for $22.38
                    - generic [ref=e376]: All In 7.46x
                  - generic [ref=e377]:
                    - img [ref=e379]
                    - generic [ref=e382]: "2"
                    - generic [ref=e384]: "3"
                    - generic [ref=e386]: "4"
                - button "Expand entry details" [ref=e389]:
                  - img "Expand" [ref=e390]
              - region [ref=e391]:
                - button "Expand entry details" [ref=e392]:
                  - generic [ref=e394]:
                    - generic [ref=e396]:
                      - text: $3
                      - generic [ref=e397]: for $25.86
                    - generic [ref=e398]: All In 8.62x
                  - generic [ref=e399]:
                    - img [ref=e401]
                    - generic [ref=e404]: "2"
                    - generic [ref=e406]: "3"
                    - generic [ref=e408]: "4"
                    - generic [ref=e410]: "5"
                - button "Expand entry details" [ref=e413]:
                  - img "Expand" [ref=e414]
          - generic [ref=e416]:
            - button [active] [ref=e417]:
              - img [ref=e418]
            - button "2" [ref=e420]:
              - generic [ref=e421]: "2"
            - button "3" [ref=e422]:
              - generic [ref=e423]: "3"
            - button "4" [ref=e424]:
              - generic [ref=e425]: "4"
            - button "5" [ref=e426]:
              - generic [ref=e427]: "5"
            - button "6" [ref=e428]:
              - generic [ref=e429]: "6"
            - button [ref=e430]:
              - img [ref=e431]
      - contentinfo [ref=e433]:
        - navigation [ref=e434]:
          - list [ref=e435]:
            - listitem [ref=e436]:
              - button "Home" [ref=e437] [cursor=pointer]:
                - generic [ref=e438]:
                  - img [ref=e439]
                  - generic [ref=e440]: Home
            - listitem [ref=e441]:
              - button "Entries 131" [ref=e442] [cursor=pointer]:
                - generic [ref=e443]:
                  - img [ref=e444]
                  - generic [ref=e445]: Entries
                - generic [ref=e446]: "131"
            - listitem [ref=e447]:
              - button "Feed" [ref=e448] [cursor=pointer]:
                - generic [ref=e449]:
                  - img [ref=e450]
                  - generic [ref=e451]: Feed
            - listitem [ref=e452]:
              - button "Rewards 4" [ref=e453] [cursor=pointer]:
                - generic [ref=e454]:
                  - img [ref=e455]
                  - generic [ref=e456]: Rewards
                - generic [ref=e457]: "4"
            - listitem [ref=e458]:
              - button "Packs" [ref=e459] [cursor=pointer]:
                - generic [ref=e460]:
                  - img [ref=e461]
                  - generic [ref=e462]: Packs
    - generic:
      - region "Notifications Alt+T"
  - alert [ref=e463]: ParlayPlay | Fun Fantasy Sports - My Entries
```

# Test source

```ts
  22  |     await loggedInPage.goto('/');
  23  |     await home.waitForFeedReady();
  24  |   });
  25  | 
  26  |   test(
  27  |     'Five-pick contest is submitted successfully',
  28  |     { tag: ['@smoke', '@prod', '@critical', '@money'] },
  29  |     async ({ loggedInPage: page }) => {
  30  |       test.setTimeout(120000);
  31  | 
  32  |       test.skip(
  33  |         isProdEnv() && test.info().project.name !== 'Mobile Chrome',
  34  |         'prod money test runs on Mobile Chrome only — one real entry per deploy',
  35  |       );
  36  | 
  37  |       const homePage = new HomePage(page);
  38  |       const contestPage = new ContestPage(page);
  39  |       const contestSuccessPage = new ContestSuccessPage(page);
  40  | 
  41  |       await test.step('Place 5-pick contest for $3 — rotating stat on limit', async () => {
  42  |         await placeContestWithRetry({
  43  |           homePage,
  44  |           contestPage,
  45  |           pickCount: 5,
  46  |           entryAmount: 3,
  47  |         });
  48  |       });
  49  | 
  50  |       await test.step('Success screen is shown — continue to home', async () => {
  51  |         await contestSuccessPage.continueToHomePage();
  52  |       });
  53  | 
  54  |       await test.step('Home feed is ready after continuing', async () => {
  55  |         await new HomePage(page).assertReady();
  56  |       });
  57  |     },
  58  |   );
  59  | 
  60  |   test('Picks Submitted screen exposes the description CTA and opens the editor', async ({
  61  |     loggedInPage: page,
  62  |   }) => {
  63  |     test.setTimeout(120000);
  64  | 
  65  |     const homePage = new HomePage(page);
  66  |     const contestPage = new ContestPage(page);
  67  |     const contestSuccessPage = new ContestSuccessPage(page);
  68  | 
  69  |     await test.step('Place 2-pick contest for $3', async () => {
  70  |       await placeContestWithRetry({
  71  |         homePage,
  72  |         contestPage,
  73  |         pickCount: 2,
  74  |         entryAmount: 3,
  75  |       });
  76  |     });
  77  | 
  78  |     await test.step('Description CTA is present and opens the inline editor', async () => {
  79  |       // The CTA only renders for feed-eligible contests; skip rather than
  80  |       // assert on data we can't control.
  81  |       const ctaVisible = await contestSuccessPage.descriptionCta.isVisible().catch(() => false);
  82  |       test.skip(!ctaVisible, 'Placed contest is not feed-eligible — no description CTA.');
  83  | 
  84  |       await contestSuccessPage.openDescriptionEditor();
  85  |     });
  86  |   });
  87  | 
  88  |   test('Placed contest appears in the My Entries list', async ({ loggedInPage: page }) => {
  89  |     test.setTimeout(300000);
  90  | 
  91  |     const homePage = new HomePage(page);
  92  |     const contestPage = new ContestPage(page);
  93  |     const contestSuccessPage = new ContestSuccessPage(page);
  94  |     const entriesPage = new EntriesPage(page);
  95  | 
  96  |     let entriesBeforeSubmission!: number;
  97  | 
  98  |     await test.step('Record the entries count before submission', async () => {
  99  |       await homePage.enterEntriesPage();
  100 |       await entriesPage.assertEntriesPageLoaded();
  101 |       entriesBeforeSubmission = await entriesPage.getEntriesCount();
  102 |       await homePage.clickHomeLink();
  103 |     });
  104 | 
  105 |     await test.step('Place 5-pick contest for $3 — rotating stat on limit', async () => {
  106 |       await placeContestWithRetry({
  107 |         homePage,
  108 |         contestPage,
  109 |         pickCount: 5,
  110 |         entryAmount: 3,
  111 |       });
  112 |     });
  113 | 
  114 |     await test.step('Success screen is shown — continue to home', async () => {
  115 |       await contestSuccessPage.continueToHomePage();
  116 |     });
  117 | 
  118 |     await test.step(`Entries count grows from ${entriesBeforeSubmission} to at least ${entriesBeforeSubmission + 1}`, async () => {
  119 |       await homePage.enterEntriesPage();
  120 |       await entriesPage.assertEntriesPageLoaded();
  121 |       // Other workers submit as the same user, so only a lower bound holds.
> 122 |       await expect
      |       ^ Error: Timeout 30000ms exceeded while waiting on the predicate
  123 |         .poll(async () => entriesPage.getEntriesCount(), {
  124 |           timeout: 30_000,
  125 |           intervals: [1_000, 2_000, 4_000],
  126 |         })
  127 |         .toBeGreaterThanOrEqual(entriesBeforeSubmission + 1);
  128 |     });
  129 |   });
  130 | 
  131 |   test('Submitting a contest raises the entry amount and max payout totals', async ({
  132 |     loggedInPage: page,
  133 |   }) => {
  134 |     test.setTimeout(180000);
  135 | 
  136 |     const homePage = new HomePage(page);
  137 |     const contestPage = new ContestPage(page);
  138 |     const contestSuccessPage = new ContestSuccessPage(page);
  139 |     const entriesPage = new EntriesPage(page);
  140 | 
  141 |     const entryAmount = 3;
  142 |     let statsBefore!: { entryAmount: number; maxPayout: number };
  143 |     let contestMaxPayout = 0;
  144 | 
  145 |     await test.step('Record entry amount and max payout before submission', async () => {
  146 |       await homePage.enterEntriesPage();
  147 |       await entriesPage.assertEntriesPageLoaded();
  148 |       statsBefore = await entriesPage.getStats();
  149 |       await homePage.clickHomeLink();
  150 |     });
  151 | 
  152 |     await test.step(`Place 4-pick contest for $${entryAmount} — rotating stat on limit`, async () => {
  153 |       await placeContestWithRetry({
  154 |         homePage,
  155 |         contestPage,
  156 |         pickCount: 4,
  157 |         entryAmount,
  158 |         submit: async () => {
  159 |           contestMaxPayout = await contestPage.getMaxPayout();
  160 |           return contestPage.submitAndAwaitResult();
  161 |         },
  162 |       });
  163 |     });
  164 | 
  165 |     await test.step('Success screen is shown — continue to home', async () => {
  166 |       await contestSuccessPage.continueToHomePage();
  167 |     });
  168 | 
  169 |     await test.step(`Entry amount grows by $${entryAmount} and max payout by $${contestMaxPayout}`, async () => {
  170 |       await homePage.enterEntriesPage();
  171 |       // The Entries tab click navigates client-side; reloading before the URL
  172 |       // has changed reloads the lobby instead and the History tab never shows.
  173 |       await page.waitForURL(/\/challenges\/pending/, { timeout: 15_000 });
  174 |       // /entries-summary/ is served from an 18s axios-hooks LRU cache and only
  175 |       // fetched on mount, so a quick revisit would read pre-submission stats
  176 |       // for the whole poll. A full reload forces a fresh fetch.
  177 |       await page.reload();
  178 |       await entriesPage.assertEntriesPageLoaded();
  179 |       // SWR + replica lag + parallel workers: 30s has proven too tight under
  180 |       // load, 90s lets the aggregate catch up without hiding a regression.
  181 |       await expect
  182 |         .poll(async () => (await entriesPage.getStats()).entryAmount, {
  183 |           timeout: 90_000,
  184 |           intervals: [1_000, 2_000, 4_000, 8_000],
  185 |         })
  186 |         .toBeGreaterThanOrEqual(statsBefore.entryAmount + entryAmount);
  187 |       await expect
  188 |         .poll(async () => (await entriesPage.getStats()).maxPayout, {
  189 |           timeout: 90_000,
  190 |           intervals: [1_000, 2_000, 4_000, 8_000],
  191 |         })
  192 |         .toBeGreaterThanOrEqual(statsBefore.maxPayout + contestMaxPayout);
  193 |     });
  194 |   });
  195 | 
  196 |   // 4 min of wall time (two full contest flows) — the single slowest test in
  197 |   // the suite. Excluded from CI runs (IGNORE_TAGS=@slow) to hold the 30-min
  198 |   // budget; run it locally / append it when contest coverage matters.
  199 |   test(
  200 |     'Two contests submitted back to back both appear in My Entries',
  201 |     { tag: '@slow' },
  202 |     async ({ loggedInPage: page }) => {
  203 |       test.setTimeout(240000);
  204 | 
  205 |       const homePage = new HomePage(page);
  206 |       const contestPage = new ContestPage(page);
  207 |       const contestSuccessPage = new ContestSuccessPage(page);
  208 |       const entriesPage = new EntriesPage(page);
  209 | 
  210 |       await test.step('Place first contest — 3 picks for $3', async () => {
  211 |         await placeContestWithRetry({
  212 |           homePage,
  213 |           contestPage,
  214 |           pickCount: 3,
  215 |           entryAmount: 3,
  216 |         });
  217 |         await contestSuccessPage.continueToHomePage();
  218 |       });
  219 | 
  220 |       await test.step('Place second contest — 5 picks for $3', async () => {
  221 |         await placeContestWithRetry({
  222 |           homePage,
```