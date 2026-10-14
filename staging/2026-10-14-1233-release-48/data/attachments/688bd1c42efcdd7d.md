# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: contests/user-enter-contest.spec.ts >> Contests - Enter Contest >> Submitting a contest raises the entry amount and max payout totals
- Location: tests/contests/user-enter-contest.spec.ts:132:3

# Error details

```
Error: expect(received).toBeGreaterThanOrEqual(expected)

Expected: >= 103.74000000000001
Received:    103.74

Call Log:
- Timeout 90000ms exceeded while waiting on the predicate
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
            - generic [ref=e12]: $488.00
            - button "Add" [ref=e13]:
              - img [ref=e15]
              - img [ref=e17]
            - button "Toggle Menu" [ref=e19]:
              - img [ref=e20]
      - main [ref=e22]:
        - generic [ref=e25]:
          - navigation [ref=e26]:
            - list [ref=e27]:
              - listitem [ref=e28]:
                - button "Active" [ref=e29]
              - listitem [ref=e30]:
                - button "History" [ref=e31]
          - generic [ref=e32]:
            - generic [ref=e34]:
              - generic [ref=e35]:
                - generic [ref=e36]: $12
                - generic [ref=e37]: Entry Amount
              - img "chest-icon" [ref=e38]
              - generic [ref=e39]:
                - generic [ref=e40]: $103.74
                - generic [ref=e41]: Max Payout
            - generic [ref=e42]:
              - region [ref=e43]:
                - button "Expand entry details" [ref=e44]:
                  - generic [ref=e46]:
                    - generic [ref=e48]:
                      - text: $3
                      - generic [ref=e49]: for $35.28
                    - generic [ref=e50]: All In 11.76x
                - generic [ref=e58]:
                  - button "Share entry" [ref=e59]:
                    - img "share" [ref=e60]
                  - button "Expand entry details" [ref=e61]:
                    - img "Expand" [ref=e62]
              - region [ref=e63]:
                - button "Expand entry details" [ref=e64]:
                  - generic [ref=e66]:
                    - generic [ref=e68]:
                      - text: $3
                      - generic [ref=e69]: for $10.5
                    - generic [ref=e70]: All In 3.5x
                - generic [ref=e75]:
                  - button "Share entry" [ref=e76]:
                    - img "share" [ref=e77]
                  - button "Expand entry details" [ref=e78]:
                    - img "Expand" [ref=e79]
              - region [ref=e80]:
                - button "Expand entry details" [ref=e81]:
                  - generic [ref=e83]:
                    - generic [ref=e85]:
                      - text: $3
                      - generic [ref=e86]: for $35.28
                    - generic [ref=e87]: All In 11.76x
                - generic [ref=e95]:
                  - button "Share entry" [ref=e96]:
                    - img "share" [ref=e97]
                  - button "Expand entry details" [ref=e98]:
                    - img "Expand" [ref=e99]
              - region [ref=e100]:
                - button "Expand entry details" [ref=e101]:
                  - generic [ref=e103]:
                    - generic [ref=e105]:
                      - text: $3
                      - generic [ref=e106]: for $22.68
                    - generic [ref=e107]: All In 7.56x
                - generic [ref=e114]:
                  - button "Share entry" [ref=e115]:
                    - img "share" [ref=e116]
                  - button "Expand entry details" [ref=e117]:
                    - img "Expand" [ref=e118]
      - contentinfo [ref=e119]:
        - navigation [ref=e120]:
          - list [ref=e121]:
            - listitem [ref=e122]:
              - button "Home" [ref=e123] [cursor=pointer]:
                - generic [ref=e124]:
                  - img [ref=e125]
                  - generic [ref=e126]: Home
            - listitem [ref=e127]:
              - button "Entries 4" [ref=e128] [cursor=pointer]:
                - generic [ref=e129]:
                  - img [ref=e130]
                  - generic [ref=e131]: Entries
                - generic [ref=e132]: "4"
            - listitem [ref=e133]:
              - button "Feed" [ref=e134] [cursor=pointer]:
                - generic [ref=e135]:
                  - img [ref=e136]
                  - generic [ref=e137]: Feed
            - listitem [ref=e138]:
              - button "Rewards" [ref=e139] [cursor=pointer]:
                - generic [ref=e140]:
                  - img [ref=e141]
                  - generic [ref=e142]: Rewards
            - listitem [ref=e143]:
              - button "Packs" [ref=e144] [cursor=pointer]:
                - generic [ref=e145]:
                  - img [ref=e146]
                  - generic [ref=e147]: Packs
    - generic:
      - region "Notifications Alt+T"
  - alert [ref=e148]
```

# Test source

```ts
  88  | 
  89  |   test('Placed contest appears in the My Entries list', async ({ loggedInPage: page }) => {
  90  |     test.setTimeout(300000);
  91  | 
  92  |     const homePage = new HomePage(page);
  93  |     const contestPage = new ContestPage(page);
  94  |     const contestSuccessPage = new ContestSuccessPage(page);
  95  |     const entriesPage = new EntriesPage(page);
  96  | 
  97  |     let entriesBeforeSubmission!: number;
  98  | 
  99  |     await test.step('Record the entries count before submission', async () => {
  100 |       await homePage.enterEntriesPage();
  101 |       await entriesPage.assertEntriesPageLoaded();
  102 |       entriesBeforeSubmission = await entriesPage.getEntriesCount();
  103 |       await homePage.clickHomeLink();
  104 |     });
  105 | 
  106 |     await test.step('Place 5-pick contest for $3 — rotating stat on limit', async () => {
  107 |       await placeContestWithRetry({
  108 |         homePage,
  109 |         contestPage,
  110 |         pickCount: 5,
  111 |         entryAmount: 3,
  112 |       });
  113 |     });
  114 | 
  115 |     await test.step('Success screen is shown — continue to home', async () => {
  116 |       await contestSuccessPage.continueToHomePage();
  117 |     });
  118 | 
  119 |     await test.step(`Entries count grows from ${entriesBeforeSubmission} to at least ${entriesBeforeSubmission + 1}`, async () => {
  120 |       await homePage.enterEntriesPage();
  121 |       await entriesPage.assertEntriesPageLoaded();
  122 |       // Other workers submit as the same user, so only a lower bound holds.
  123 |       await expect
  124 |         .poll(async () => entriesPage.getEntriesCount(), {
  125 |           timeout: 30_000,
  126 |           intervals: [1_000, 2_000, 4_000],
  127 |         })
  128 |         .toBeGreaterThanOrEqual(entriesBeforeSubmission + 1);
  129 |     });
  130 |   });
  131 | 
  132 |   test('Submitting a contest raises the entry amount and max payout totals', async ({
  133 |     loggedInPage: page,
  134 |   }) => {
  135 |     test.setTimeout(180000);
  136 | 
  137 |     const homePage = new HomePage(page);
  138 |     const contestPage = new ContestPage(page);
  139 |     const contestSuccessPage = new ContestSuccessPage(page);
  140 |     const entriesPage = new EntriesPage(page);
  141 | 
  142 |     const entryAmount = 3;
  143 |     let statsBefore!: { entryAmount: number; maxPayout: number };
  144 |     let contestMaxPayout = 0;
  145 | 
  146 |     await test.step('Record entry amount and max payout before submission', async () => {
  147 |       await homePage.enterEntriesPage();
  148 |       await entriesPage.assertEntriesPageLoaded();
  149 |       statsBefore = await entriesPage.getStats();
  150 |       await homePage.clickHomeLink();
  151 |     });
  152 | 
  153 |     await test.step(`Place 4-pick contest for $${entryAmount} — rotating stat on limit`, async () => {
  154 |       await placeContestWithRetry({
  155 |         homePage,
  156 |         contestPage,
  157 |         pickCount: 4,
  158 |         entryAmount,
  159 |         submit: async () => {
  160 |           contestMaxPayout = await contestPage.getMaxPayout();
  161 |           return contestPage.submitAndAwaitResult();
  162 |         },
  163 |       });
  164 |     });
  165 | 
  166 |     await test.step('Success screen is shown — continue to home', async () => {
  167 |       await contestSuccessPage.continueToHomePage();
  168 |     });
  169 | 
  170 |     await test.step(`Entry amount grows by $${entryAmount} and max payout by $${contestMaxPayout}`, async () => {
  171 |       await homePage.enterEntriesPage();
  172 |       // The Entries tab click navigates client-side; reloading before the URL
  173 |       // has changed reloads the lobby instead and the History tab never shows.
  174 |       await page.waitForURL(/\/challenges\/pending/, { timeout: 15_000 });
  175 |       // /entries-summary/ is served from an 18s axios-hooks LRU cache and only
  176 |       // fetched on mount, so a quick revisit would read pre-submission stats
  177 |       // for the whole poll. A full reload forces a fresh fetch.
  178 |       await page.reload();
  179 |       await entriesPage.assertEntriesPageLoaded();
  180 |       // SWR + replica lag + parallel workers: 30s has proven too tight under
  181 |       // load, 90s lets the aggregate catch up without hiding a regression.
  182 |       await expect
  183 |         .poll(async () => (await entriesPage.getStats()).entryAmount, {
  184 |           timeout: 90_000,
  185 |           intervals: [1_000, 2_000, 4_000, 8_000],
  186 |         })
  187 |         .toBeGreaterThanOrEqual(statsBefore.entryAmount + entryAmount);
> 188 |       await expect
      |       ^ Error: expect(received).toBeGreaterThanOrEqual(expected)
  189 |         .poll(async () => (await entriesPage.getStats()).maxPayout, {
  190 |           timeout: 90_000,
  191 |           intervals: [1_000, 2_000, 4_000, 8_000],
  192 |         })
  193 |         .toBeGreaterThanOrEqual(statsBefore.maxPayout + contestMaxPayout);
  194 |     });
  195 |   });
  196 | 
  197 |   test('Placing an entry debits the wallet by the entry amount and cancelling refunds it', async ({
  198 |     loggedInPage: page,
  199 |   }) => {
  200 |     test.setTimeout(300000);
  201 | 
  202 |     const homePage = new HomePage(page);
  203 |     const contestPage = new ContestPage(page);
  204 |     const contestSuccessPage = new ContestSuccessPage(page);
  205 |     const entriesPage = new EntriesPage(page);
  206 | 
  207 |     const entryAmount = 3;
  208 |     let balanceBefore = 0;
  209 |     let contestUuid = '';
  210 | 
  211 |     await test.step(`Place 3-pick contest for $${entryAmount}`, async () => {
  212 |       await placeContestWithRetry({
  213 |         homePage,
  214 |         contestPage,
  215 |         pickCount: 3,
  216 |         entryAmount,
  217 |         submit: async () => {
  218 |           // Read right before the click: picking takes a while, and in env
  219 |           // mode a sibling worker on the same account can move money meanwhile.
  220 |           balanceBefore = await fetchCashBalance(page);
  221 |           const placed = page
  222 |             .waitForResponse((resp) => isSubmissionPost(resp) && resp.ok(), { timeout: 20_000 })
  223 |             .catch(() => null);
  224 |           const result = await contestPage.submitAndAwaitResult();
  225 |           if (result.success) {
  226 |             // redirectUrl is /challenges/contest/<uuid> — the only handle on
  227 |             // the new entry, since cards expose just their numeric id.
  228 |             const body = await (await placed)?.json();
  229 |             contestUuid =
  230 |               String(body?.redirectUrl ?? '')
  231 |                 .split('/')
  232 |                 .pop() ?? '';
  233 |           }
  234 |           return result;
  235 |         },
  236 |       });
  237 |       await contestSuccessPage.continueToHomePage();
  238 |     });
  239 | 
  240 |     await test.step(`Header wallet drops by exactly $${entryAmount}`, async () => {
  241 |       // The header refreshes from a fire-and-forget getUser(); reload so the
  242 |       // pill is read from a fresh fetch rather than the pre-submit context.
  243 |       await page.reload();
  244 |       await homePage.waitForFeedReady();
  245 |       await expect
  246 |         .poll(() => homePage.getWalletBalance(), { timeout: 30_000 })
  247 |         .toBeCloseTo(balanceBefore - entryAmount, 2);
  248 |     });
  249 | 
  250 |     const card = await test.step('Find the placed entry on the Active tab', async () => {
  251 |       expect(contestUuid, 'submission response carried no contest uuid').not.toBe('');
  252 |       await homePage.enterEntriesPage();
  253 |       await entriesPage.assertEntriesPageLoaded();
  254 |       return entriesPage.findCardByUuid(contestUuid);
  255 |     });
  256 |     expect(card, 'placed entry is not listed on the Active tab').not.toBeNull();
  257 | 
  258 |     // Other fresh entries on the account are cancellable too, so the button
  259 |     // must belong to this card, not just any card.
  260 |     const cancelButton = card!.getByRole('button', { name: /Cancel Entry/ });
  261 |     if (!(await cancelButton.isVisible().catch(() => false))) {
  262 |       // Cancel needs every match >= 15 min from kickoff; the debit above still holds.
  263 |       test.info().annotations.push({
  264 |         type: 'note',
  265 |         description: 'Placed entry was not cancellable — refund not asserted',
  266 |       });
  267 |       return;
  268 |     }
  269 | 
  270 |     await test.step(`Cancelling the entry refunds $${entryAmount} to the wallet`, async () => {
  271 |       const beforeCancel = await fetchCashBalance(page);
  272 |       await cancelButton.click();
  273 |       const confirmDialog = page
  274 |         .getByRole('dialog')
  275 |         .filter({ hasText: 'Are you sure you want to cancel your entry?' });
  276 |       await expect(confirmDialog).toBeVisible();
  277 |       await confirmDialog.getByRole('button', { name: 'Confirm' }).click();
  278 |       await expect(confirmDialog).toHaveCount(0);
  279 | 
  280 |       await expect
  281 |         .poll(() => entriesPage.getWalletBalance(), { timeout: 30_000 })
  282 |         .toBeCloseTo(beforeCancel + entryAmount, 2);
  283 |     });
  284 |   });
  285 | 
  286 |   // 4 min of wall time (two full contest flows) — the single slowest test in
  287 |   // the suite. Skipped in CI to hold the 30-min budget; run it locally /
  288 |   // append it when contest coverage matters.
```