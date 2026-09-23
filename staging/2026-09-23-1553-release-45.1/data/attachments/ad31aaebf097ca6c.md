# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: contests/user-enter-contest.spec.ts >> Contests - Enter Contest >> Placed contest appears in the My Entries list
- Location: tests/contests/user-enter-contest.spec.ts:88:3

# Error details

```
Error: expect(received).toBeGreaterThanOrEqual(expected)

Expected: >= 172
Received:    0

Call Log:
- Timeout 30000ms exceeded while waiting on the predicate
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
            - generic [ref=e13]: $666.48
            - button "Toggle Menu" [ref=e14]:
              - img [ref=e15]
      - main [ref=e17]:
        - generic [ref=e20]:
          - navigation [ref=e21]:
            - list [ref=e22]:
              - listitem [ref=e23]:
                - button "Active" [ref=e24]
              - listitem [ref=e25]:
                - button "History" [ref=e26]
          - generic [ref=e28]:
            - generic [ref=e29]: Looks like you don't have any pending entries.
            - button "Browse now" [ref=e31] [cursor=pointer]
      - contentinfo [ref=e32]:
        - navigation [ref=e33]:
          - list [ref=e34]:
            - listitem [ref=e35]:
              - button "Home" [ref=e36] [cursor=pointer]:
                - generic [ref=e37]:
                  - img [ref=e38]
                  - generic [ref=e39]: Home
            - listitem [ref=e40]:
              - button "Entries 172" [active] [ref=e41] [cursor=pointer]:
                - generic [ref=e42]:
                  - img [ref=e43]
                  - generic [ref=e44]: Entries
                - generic [ref=e45]: "172"
            - listitem [ref=e46]:
              - button "Feed" [ref=e47] [cursor=pointer]:
                - generic [ref=e48]:
                  - img [ref=e49]
                  - generic [ref=e50]: Feed
            - listitem [ref=e51]:
              - button "Rewards" [ref=e52] [cursor=pointer]:
                - generic [ref=e53]:
                  - img [ref=e54]
                  - generic [ref=e55]: Rewards
            - listitem [ref=e56]:
              - button "Packs" [ref=e57] [cursor=pointer]:
                - generic [ref=e58]:
                  - img [ref=e59]
                  - generic [ref=e60]: Packs
    - generic:
      - region "Notifications Alt+T"
  - alert [ref=e61]: ParlayPlay | Fun Fantasy Sports - My Entries
  - iframe [ref=e62]:
    
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
      |       ^ Error: expect(received).toBeGreaterThanOrEqual(expected)
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