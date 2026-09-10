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
              - generic [ref=e13]: $480.15
              - generic [ref=e14]:
                - img "gift-icon" [ref=e15]
                - text: "56.00"
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
                - generic [ref=e33]: $261
                - generic [ref=e34]: Entry Amount
              - img "chest-icon" [ref=e35]
              - generic [ref=e36]:
                - generic [ref=e37]: $6854.55
                - generic [ref=e38]: Max Payout
            - generic [ref=e39]:
              - region [ref=e40]:
                - button "Expand entry details" [ref=e41]:
                  - generic [ref=e43]:
                    - generic [ref=e45]:
                      - text: $3
                      - generic [ref=e46]: for $10.38
                    - generic [ref=e47]: All In 3.46x
                  - generic [ref=e48]:
                    - generic [ref=e50]: "1"
                    - generic [ref=e52]: "2"
                    - generic [ref=e54]: "3"
                - button "Expand entry details" [ref=e57]:
                  - img "Expand" [ref=e58]
              - region [ref=e59]:
                - button "Expand entry details" [ref=e60]:
                  - generic [ref=e62]:
                    - generic [ref=e64]:
                      - text: $3
                      - generic [ref=e65]: for $10.38
                    - generic [ref=e66]: All In 3.46x
                  - generic [ref=e67]:
                    - generic [ref=e69]: "1"
                    - generic [ref=e71]: "2"
                    - generic [ref=e73]: "3"
                - button "Expand entry details" [ref=e76]:
                  - img "Expand" [ref=e77]
              - region [ref=e78]:
                - button "Expand entry details" [ref=e79]:
                  - generic [ref=e81]:
                    - generic [ref=e83]:
                      - text: $3
                      - generic [ref=e84]: for $10.38
                    - generic [ref=e85]: All In 3.46x
                  - generic [ref=e86]:
                    - generic [ref=e88]: "1"
                    - generic [ref=e90]: "2"
                    - generic [ref=e92]: "3"
                - button "Expand entry details" [ref=e95]:
                  - img "Expand" [ref=e96]
              - region [ref=e97]:
                - button "Expand entry details" [ref=e98]:
                  - generic [ref=e100]:
                    - generic [ref=e102]:
                      - text: $3
                      - generic [ref=e103]: for $10.38
                    - generic [ref=e104]: All In 3.46x
                  - generic [ref=e105]:
                    - generic [ref=e107]: "1"
                    - generic [ref=e109]: "2"
                    - generic [ref=e111]: "3"
                - button "Expand entry details" [ref=e114]:
                  - img "Expand" [ref=e115]
              - region [ref=e116]:
                - button "Expand entry details" [ref=e117]:
                  - generic [ref=e118]:
                    - generic [ref=e119]:
                      - generic [ref=e121]:
                        - text: $3
                        - generic [ref=e122]: for $23.04
                      - generic [ref=e123]: All In 7.68x
                    - generic [ref=e126]: Live
                  - generic [ref=e127]:
                    - generic [ref=e131]: "2"
                    - img [ref=e133]
                - button "Expand entry details" [ref=e137]:
                  - img "Expand" [ref=e138]
              - region [ref=e139]:
                - button "Expand entry details" [ref=e140]:
                  - generic [ref=e141]:
                    - generic [ref=e142]:
                      - generic [ref=e144]:
                        - text: $3
                        - generic [ref=e145]: for $23.04
                      - generic [ref=e146]: All In 7.68x
                    - generic [ref=e149]: Live
                  - generic [ref=e150]:
                    - generic [ref=e154]: "2"
                    - img [ref=e156]
                - button "Expand entry details" [ref=e160]:
                  - img "Expand" [ref=e161]
              - region [ref=e162]:
                - button "Expand entry details" [ref=e163]:
                  - generic [ref=e164]:
                    - generic [ref=e165]:
                      - generic [ref=e167]:
                        - text: $3
                        - generic [ref=e168]: for $23.04
                      - generic [ref=e169]: All In 7.68x
                    - generic [ref=e172]: Live
                  - generic [ref=e173]:
                    - generic [ref=e177]: "2"
                    - img [ref=e179]
                - button "Expand entry details" [ref=e183]:
                  - img "Expand" [ref=e184]
              - region [ref=e185]:
                - button "Expand entry details" [ref=e186]:
                  - generic [ref=e187]:
                    - generic [ref=e188]:
                      - generic [ref=e190]:
                        - text: $3
                        - generic [ref=e191]: for $23.04
                      - generic [ref=e192]: All In 7.68x
                    - generic [ref=e195]: Live
                  - generic [ref=e196]:
                    - generic [ref=e200]: "2"
                    - img [ref=e202]
                - button "Expand entry details" [ref=e206]:
                  - img "Expand" [ref=e207]
              - region [ref=e208]:
                - button "Expand entry details" [ref=e209]:
                  - generic [ref=e210]:
                    - generic [ref=e211]:
                      - generic [ref=e213]:
                        - text: $3
                        - generic [ref=e214]: for $93.75
                      - generic [ref=e215]: All In 31.25x
                    - generic [ref=e218]: Live
                  - generic [ref=e219]:
                    - generic [ref=e223]: "2"
                    - img [ref=e225]
                    - generic [ref=e228]: "4"
                    - generic [ref=e230]: "5"
                - button "Expand entry details" [ref=e233]:
                  - img "Expand" [ref=e234]
              - region [ref=e235]:
                - button "Expand entry details" [ref=e236]:
                  - generic [ref=e237]:
                    - generic [ref=e238]:
                      - generic [ref=e240]:
                        - text: $3
                        - generic [ref=e241]: for $10.68
                      - generic [ref=e242]: All In 3.56x
                    - generic [ref=e245]: Live
                  - generic [ref=e250]: "2"
                - button "Expand entry details" [ref=e253]:
                  - img "Expand" [ref=e254]
              - region [ref=e255]:
                - button "Expand entry details" [ref=e256]:
                  - generic [ref=e257]:
                    - generic [ref=e258]:
                      - generic [ref=e260]:
                        - text: $3
                        - generic [ref=e261]: for $93.75
                      - generic [ref=e262]: All In 31.25x
                    - generic [ref=e265]: Live
                  - generic [ref=e266]:
                    - generic [ref=e270]: "2"
                    - img [ref=e272]
                    - generic [ref=e275]: "4"
                    - generic [ref=e277]: "5"
                - button "Expand entry details" [ref=e280]:
                  - img "Expand" [ref=e281]
              - region [ref=e282]:
                - button "Expand entry details" [ref=e283]:
                  - generic [ref=e284]:
                    - generic [ref=e285]:
                      - generic [ref=e287]:
                        - text: $3
                        - generic [ref=e288]: for $14.76
                      - generic [ref=e289]: All In 4.92x
                    - generic [ref=e292]: Live
                  - generic [ref=e293]:
                    - generic [ref=e297]: "2"
                    - img [ref=e299]
                - button "Expand entry details" [ref=e303]:
                  - img "Expand" [ref=e304]
              - region [ref=e305]:
                - button "Expand entry details" [ref=e306]:
                  - generic [ref=e307]:
                    - generic [ref=e308]:
                      - generic [ref=e310]:
                        - text: $3
                        - generic [ref=e311]: for $14.76
                      - generic [ref=e312]: All In 4.92x
                    - generic [ref=e315]: Live
                  - generic [ref=e316]:
                    - generic [ref=e320]: "2"
                    - img [ref=e322]
                - button "Expand entry details" [ref=e326]:
                  - img "Expand" [ref=e327]
              - region [ref=e328]:
                - button "Expand entry details" [ref=e329]:
                  - generic [ref=e330]:
                    - generic [ref=e331]:
                      - generic [ref=e333]:
                        - text: $3
                        - generic [ref=e334]: for $8.16
                      - generic [ref=e335]: All In 2.72x
                    - generic [ref=e338]: Live
                  - generic [ref=e339]:
                    - generic [ref=e343]: "2"
                    - img [ref=e345]
                - button "Expand entry details" [ref=e349]:
                  - img "Expand" [ref=e350]
              - region [ref=e351]:
                - button "Expand entry details" [ref=e352]:
                  - generic [ref=e353]:
                    - generic [ref=e354]:
                      - generic [ref=e356]:
                        - text: $3
                        - generic [ref=e357]: for $8.16
                      - generic [ref=e358]: All In 2.72x
                    - generic [ref=e361]: Live
                  - generic [ref=e362]:
                    - generic [ref=e366]: "2"
                    - img [ref=e368]
                - button "Expand entry details" [ref=e372]:
                  - img "Expand" [ref=e373]
              - region [ref=e374]:
                - button "Expand entry details" [ref=e375]:
                  - generic [ref=e376]:
                    - generic [ref=e377]:
                      - generic [ref=e379]:
                        - text: $3
                        - generic [ref=e380]: for $23.04
                      - generic [ref=e381]: All In 7.68x
                    - generic [ref=e384]: Live
                  - generic [ref=e385]:
                    - generic [ref=e389]: "2"
                    - img [ref=e391]
                - button "Expand entry details" [ref=e395]:
                  - img "Expand" [ref=e396]
          - generic [ref=e398]:
            - button [active] [ref=e399]:
              - img [ref=e400]
            - button "2" [ref=e402]:
              - generic [ref=e403]: "2"
            - button "3" [ref=e404]:
              - generic [ref=e405]: "3"
            - button "4" [ref=e406]:
              - generic [ref=e407]: "4"
            - button "5" [ref=e408]:
              - generic [ref=e409]: "5"
            - button "6" [ref=e410]:
              - generic [ref=e411]: "6"
            - button [ref=e412]:
              - img [ref=e413]
      - contentinfo [ref=e415]:
        - navigation [ref=e416]:
          - list [ref=e417]:
            - listitem [ref=e418]:
              - button "Home" [ref=e419] [cursor=pointer]:
                - generic [ref=e420]:
                  - img [ref=e421]
                  - generic [ref=e422]: Home
            - listitem [ref=e423]:
              - button "Entries 86" [ref=e424] [cursor=pointer]:
                - generic [ref=e425]:
                  - img [ref=e426]
                  - generic [ref=e427]: Entries
                - generic [ref=e428]: "86"
            - listitem [ref=e429]:
              - button "Feed" [ref=e430] [cursor=pointer]:
                - generic [ref=e431]:
                  - img [ref=e432]
                  - generic [ref=e433]: Feed
            - listitem [ref=e434]:
              - button "Rewards 56" [ref=e435] [cursor=pointer]:
                - generic [ref=e436]:
                  - img [ref=e437]
                  - generic [ref=e438]: Rewards
                - generic [ref=e439]: "56"
            - listitem [ref=e440]:
              - button "Packs" [ref=e441] [cursor=pointer]:
                - generic [ref=e442]:
                  - img [ref=e443]
                  - generic [ref=e444]: Packs
    - generic:
      - region "Notifications Alt+T"
  - alert [ref=e445]: ParlayPlay | Fun Fantasy Sports - My Entries
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
  171 |       // /entries-summary/ is served from an 18s axios-hooks LRU cache and only
  172 |       // fetched on mount, so a quick revisit would read pre-submission stats
  173 |       // for the whole poll. A full reload forces a fresh fetch.
  174 |       await page.reload();
  175 |       await entriesPage.assertEntriesPageLoaded();
  176 |       // SWR + replica lag + parallel workers: 30s has proven too tight under
  177 |       // load, 90s lets the aggregate catch up without hiding a regression.
  178 |       await expect
  179 |         .poll(async () => (await entriesPage.getStats()).entryAmount, {
  180 |           timeout: 90_000,
  181 |           intervals: [1_000, 2_000, 4_000, 8_000],
  182 |         })
  183 |         .toBeGreaterThanOrEqual(statsBefore.entryAmount + entryAmount);
  184 |       await expect
  185 |         .poll(async () => (await entriesPage.getStats()).maxPayout, {
  186 |           timeout: 90_000,
  187 |           intervals: [1_000, 2_000, 4_000, 8_000],
  188 |         })
  189 |         .toBeGreaterThanOrEqual(statsBefore.maxPayout + contestMaxPayout);
  190 |     });
  191 |   });
  192 | 
  193 |   // 4 min of wall time (two full contest flows) — the single slowest test in
  194 |   // the suite. Excluded from CI runs (IGNORE_TAGS=@slow) to hold the 30-min
  195 |   // budget; run it locally / append it when contest coverage matters.
  196 |   test(
  197 |     'Two contests submitted back to back both appear in My Entries',
  198 |     { tag: '@slow' },
  199 |     async ({ loggedInPage: page }) => {
  200 |       test.setTimeout(240000);
  201 | 
  202 |       const homePage = new HomePage(page);
  203 |       const contestPage = new ContestPage(page);
  204 |       const contestSuccessPage = new ContestSuccessPage(page);
  205 |       const entriesPage = new EntriesPage(page);
  206 | 
  207 |       await test.step('Place first contest — 3 picks for $3', async () => {
  208 |         await placeContestWithRetry({
  209 |           homePage,
  210 |           contestPage,
  211 |           pickCount: 3,
  212 |           entryAmount: 3,
  213 |         });
  214 |         await contestSuccessPage.continueToHomePage();
  215 |       });
  216 | 
  217 |       await test.step('Place second contest — 5 picks for $3', async () => {
  218 |         await placeContestWithRetry({
  219 |           homePage,
  220 |           contestPage,
  221 |           pickCount: 5,
  222 |           entryAmount: 3,
```