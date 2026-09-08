# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: entries/entry-card.spec.ts >> My Entries - cancel entry >> Fresh entry shows a live cancel countdown and confirming Cancel Entry removes it everywhere
- Location: tests/entries/entry-card.spec.ts:261:5

# Error details

```
Test timeout of 300000ms exceeded.
```

```
Error: locator.textContent: Target page, context or browser has been closed
Call log:
  - waiting for locator('section div[role="region"][aria-controls^="entry-"]').filter({ visible: true }).first().getByRole('button', { name: /Cancel Entry/ })

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
              - generic [ref=e13]: $570.24
              - generic [ref=e14]:
                - img "gift-icon" [ref=e15]
                - text: "43.00"
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
                - generic [ref=e33]: $246
                - generic [ref=e34]: Entry Amount
              - img "chest-icon" [ref=e35]
              - generic [ref=e36]:
                - generic [ref=e37]: $6585.81
                - generic [ref=e38]: Max Payout
            - generic [ref=e39]:
              - region [ref=e40]:
                - button "Collapse entry details" [active] [ref=e41]:
                  - generic [ref=e43]:
                    - generic [ref=e45]:
                      - text: $3
                      - generic [ref=e46]: for $7.17
                    - generic [ref=e47]: All In 2.39x
                - generic [ref=e48]:
                  - generic [ref=e49]:
                    - generic [ref=e56]:
                      - generic [ref=e57]: T. Bibee - Guardians
                      - generic [ref=e59]: Guardians vs. Orioles - 8 Sep 6:35 PM
                      - generic [ref=e62]:
                        - text: Less
                        - generic [ref=e63]: 5.5 Strikeouts (K)
                    - generic [ref=e70]:
                      - generic [ref=e71]: S. Manaea - Mets
                      - generic [ref=e73]: Mets vs. Marlins - 8 Sep 6:40 PM
                      - generic [ref=e76]:
                        - text: Less
                        - generic [ref=e77]: 5.5 Strikeouts (K)
                  - button "View Leaderboard" [ref=e81] [cursor=pointer]
                - generic [ref=e83]:
                  - button "Share entry" [ref=e84]:
                    - img "share" [ref=e85]
                  - button "Collapse entry details" [ref=e86]:
                    - img "Collapse" [ref=e87]
              - region [ref=e88]:
                - button "Expand entry details" [ref=e89]:
                  - generic [ref=e91]:
                    - generic [ref=e93]:
                      - text: $3
                      - generic [ref=e94]: for $32.73
                    - generic [ref=e95]: All In 10.91x
                - generic [ref=e102]:
                  - button "Share entry" [ref=e103]:
                    - img "share" [ref=e104]
                  - button "Expand entry details" [ref=e105]:
                    - img "Expand" [ref=e106]
          - generic [ref=e108]:
            - button [ref=e109]:
              - img [ref=e110]
            - button "2" [ref=e112]:
              - generic [ref=e113]: "2"
            - button "3" [ref=e114]:
              - generic [ref=e115]: "3"
            - button "4" [ref=e116]:
              - generic [ref=e117]: "4"
            - button "5" [ref=e118]:
              - generic [ref=e119]: "5"
            - button "6" [ref=e120]:
              - generic [ref=e121]: "6"
            - button [disabled] [ref=e122]:
              - img [ref=e123]
      - contentinfo [ref=e125]:
        - navigation [ref=e126]:
          - list [ref=e127]:
            - listitem [ref=e128]:
              - button "Home" [ref=e129] [cursor=pointer]:
                - generic [ref=e130]:
                  - img [ref=e131]
                  - generic [ref=e132]: Home
            - listitem [ref=e133]:
              - button "Entries 82" [ref=e134] [cursor=pointer]:
                - generic [ref=e135]:
                  - img [ref=e136]
                  - generic [ref=e137]: Entries
                - generic [ref=e138]: "82"
            - listitem [ref=e139]:
              - button "Feed" [ref=e140] [cursor=pointer]:
                - generic [ref=e141]:
                  - img [ref=e142]
                  - generic [ref=e143]: Feed
            - listitem [ref=e144]:
              - button "Rewards 44" [ref=e145] [cursor=pointer]:
                - generic [ref=e146]:
                  - img [ref=e147]
                  - generic [ref=e148]: Rewards
                - generic [ref=e149]: "44"
            - listitem [ref=e150]:
              - button "Packs" [ref=e151] [cursor=pointer]:
                - generic [ref=e152]:
                  - img [ref=e153]
                  - generic [ref=e154]: Packs
    - generic:
      - region "Notifications Alt+T"
  - alert [ref=e155]: ParlayPlay | Fun Fantasy Sports - My Entries
```

# Test source

```ts
  216 |     await entriesPage.assertEntriesPageLoaded();
  217 |     await entriesPage.waitForEntriesReady();
  218 | 
  219 |     test.skip(await entriesPage.isNoDataVisible(), 'No active entries for the test user.');
  220 | 
  221 |     // "View Leaderboard" only renders for in-group P2P entries, inside the
  222 |     // expanded card. Probe the first few cards before giving up.
  223 |     const cardsToProbe = Math.min(await entriesPage.cardDivs.count(), 4);
  224 |     let leaderboardButton = null;
  225 | 
  226 |     for (let i = 0; i < cardsToProbe; i++) {
  227 |       const card = entriesPage.cardDivs.nth(i);
  228 |       await entriesPage.expandCard(card);
  229 |       const candidate = card.getByRole('button', { name: 'View Leaderboard' });
  230 |       if (await candidate.isVisible().catch(() => false)) {
  231 |         leaderboardButton = candidate;
  232 |         break;
  233 |       }
  234 |     }
  235 | 
  236 |     test.skip(leaderboardButton === null, 'No in-group P2P entries with a leaderboard available.');
  237 | 
  238 |     await leaderboardButton!.click();
  239 | 
  240 |     const dialog = page.getByRole('dialog').filter({ visible: true }).first();
  241 |     await expect(dialog).toBeVisible();
  242 |     await dialog.locator('button').first().click();
  243 |     await expect(dialog).toHaveCount(0);
  244 |   });
  245 | });
  246 | 
  247 | test.describe(
  248 |   'My Entries - cancel entry',
  249 |   { tag: ['@entries', '@contests', '@mutates', '@money'] },
  250 |   () => {
  251 |     // Places a real contest, so keep it serial to avoid racing other submissions.
  252 |     test.describe.configure({ mode: 'serial' });
  253 | 
  254 |     test.beforeEach(async ({ loggedInPage }) => {
  255 |       const homePage = new HomePage(loggedInPage);
  256 | 
  257 |       await loggedInPage.goto('/');
  258 |       await homePage.waitForFeedReady();
  259 |     });
  260 | 
  261 |     test('Fresh entry shows a live cancel countdown and confirming Cancel Entry removes it everywhere', async ({
  262 |       loggedInPage: page,
  263 |     }) => {
  264 |       test.setTimeout(300000);
  265 | 
  266 |       const homePage = new HomePage(page);
  267 |       const contestPage = new ContestPage(page);
  268 |       const contestSuccessPage = new ContestSuccessPage(page);
  269 |       const entriesPage = new EntriesPage(page);
  270 | 
  271 |       await test.step('Place a 3-pick contest for $3 to own a cancellable entry', async () => {
  272 |         await placeContestWithRetry({ homePage, contestPage, pickCount: 3, entryAmount: 3 });
  273 |         await contestSuccessPage.continueToHomePage();
  274 |       });
  275 | 
  276 |       let cancellableCard: Awaited<ReturnType<EntriesPage['findCancellableCard']>> = null;
  277 | 
  278 |       await test.step('Find the cancellable entry on the Active tab', async () => {
  279 |         await homePage.enterEntriesPage();
  280 |         await entriesPage.assertEntriesPageLoaded();
  281 |         await entriesPage.waitForEntriesReady();
  282 |         cancellableCard = await entriesPage.findCancellableCard();
  283 |       });
  284 | 
  285 |       // An entry is only cancellable when its earliest match is >=15 min from
  286 |       // kickoff. On a feed where every available match starts sooner, no entry
  287 |       // is cancellable — skip rather than fail on data we don't control.
  288 |       test.skip(
  289 |         cancellableCard === null,
  290 |         'Placed entry was not cancellable (selected matches start within 15 minutes).',
  291 |       );
  292 | 
  293 |       const cancelButton = cancellableCard!.getByRole('button', { name: /Cancel Entry/ });
  294 | 
  295 |       // The card's aria-controls (`entry-<id>-content`) is stable across the
  296 |       // Active and History tabs, so it tracks this exact entry through
  297 |       // cancellation and onto History.
  298 |       await expect(cancellableCard!, 'card exposes its content region id').toHaveAttribute(
  299 |         'aria-controls',
  300 |         /.+/,
  301 |       );
  302 |       const entryId = await cancellableCard!.getAttribute('aria-controls');
  303 |       const entryCard = page.locator(`[role="region"][aria-controls="${entryId}"]`);
  304 | 
  305 |       await test.step('Cancel Entry countdown is shown in M:SS and ticks down over 3s', async () => {
  306 |         await expect(cancelButton).toBeVisible();
  307 |         await expect(cancelButton).toContainText(/\d+:\d{2}/);
  308 | 
  309 |         const startSeconds = parseCountdownSeconds(await cancelButton.textContent());
  310 |         expect(startSeconds).toBeGreaterThan(0);
  311 | 
  312 |         // Observe real wall-clock ticks — the component decrements every 1s,
  313 |         // so a 3s pause must drop the displayed value by at least 1s.
  314 |         await page.waitForTimeout(3000);
  315 | 
> 316 |         const laterSeconds = parseCountdownSeconds(await cancelButton.textContent());
      |                                                                       ^ Error: locator.textContent: Target page, context or browser has been closed
  317 |         expect(laterSeconds).toBeLessThan(startSeconds);
  318 |       });
  319 | 
  320 |       await test.step('Cancel Entry opens the confirmation modal, dismissible without cancelling', async () => {
  321 |         await cancelButton.click();
  322 | 
  323 |         const confirmDialog = page
  324 |           .getByRole('dialog')
  325 |           .filter({ hasText: 'Are you sure you want to cancel your entry?' });
  326 |         await expect(confirmDialog).toBeVisible();
  327 |         await expect(confirmDialog.getByRole('button', { name: 'Confirm' })).toBeVisible();
  328 | 
  329 |         await page.keyboard.press('Escape');
  330 |         await expect(confirmDialog).toHaveCount(0);
  331 |         await expect(cancelButton).toBeVisible();
  332 |       });
  333 | 
  334 |       await test.step('Confirming the cancellation removes the entry from the Active tab', async () => {
  335 |         await cancelButton.click();
  336 | 
  337 |         const confirmDialog = page
  338 |           .getByRole('dialog')
  339 |           .filter({ hasText: 'Are you sure you want to cancel your entry?' });
  340 |         await expect(confirmDialog).toBeVisible();
  341 |         await confirmDialog.getByRole('button', { name: 'Confirm' }).click();
  342 | 
  343 |         // The page re-fetches the active list after cancelling, and the
  344 |         // cancelled entry is no longer pending, so it drops off Active.
  345 |         await expect(confirmDialog).toHaveCount(0);
  346 |         await expect(entryCard).toHaveCount(0);
  347 |       });
  348 | 
  349 |       await test.step('Cancelled entry is gone for good — History never lists it', async () => {
  350 |         // A user-cancelled entry is refunded and then hard-deleted by the
  351 |         // backend, so no "Cancelled" record survives. The "Cancelled" pill in
  352 |         // History belongs to system-voided entries (postponed matches etc.).
  353 |         await entriesPage.enterHistorytab();
  354 |         await entriesPage.selectTimeRangeValue('7 Days');
  355 |         await entriesPage.waitForEntriesReady();
  356 | 
  357 |         await expect(entryCard).toHaveCount(0);
  358 |       });
  359 |     });
  360 | 
  361 |     // Two rapid Confirm clicks must fire POST /entries/<uuid>/cancel/ only once
  362 |     // — the `cancelInFlight` ref in pages/challenges/pending.tsx short-circuits
  363 |     // the second call. We place and consume our own entry, so nothing shared breaks.
  364 |     test('Confirming cancel twice fires the cancel request only once (double-submit guard)', async ({
  365 |       loggedInPage: page,
  366 |     }) => {
  367 |       test.setTimeout(300000);
  368 | 
  369 |       const homePage = new HomePage(page);
  370 |       const contestPage = new ContestPage(page);
  371 |       const contestSuccessPage = new ContestSuccessPage(page);
  372 |       const entriesPage = new EntriesPage(page);
  373 | 
  374 |       await test.step('Place a 3-pick contest for $3 to own a cancellable entry', async () => {
  375 |         await placeContestWithRetry({ homePage, contestPage, pickCount: 3, entryAmount: 3 });
  376 |         await contestSuccessPage.continueToHomePage();
  377 |       });
  378 | 
  379 |       let cancellableCard: Awaited<ReturnType<EntriesPage['findCancellableCard']>> = null;
  380 | 
  381 |       await test.step('Find the cancellable entry on the Active tab', async () => {
  382 |         await homePage.enterEntriesPage();
  383 |         await entriesPage.assertEntriesPageLoaded();
  384 |         await entriesPage.waitForEntriesReady();
  385 |         cancellableCard = await entriesPage.findCancellableCard();
  386 |       });
  387 | 
  388 |       test.skip(
  389 |         cancellableCard === null,
  390 |         'Placed entry was not cancellable (selected matches start within 15 minutes).',
  391 |       );
  392 | 
  393 |       // Stable across tabs — used to confirm this exact entry gets cancelled.
  394 |       await expect(cancellableCard!, 'card exposes its content region id').toHaveAttribute(
  395 |         'aria-controls',
  396 |         /.+/,
  397 |       );
  398 |       const entryId = await cancellableCard!.getAttribute('aria-controls');
  399 |       const entryCard = page.locator(`[role="region"][aria-controls="${entryId}"]`);
  400 |       const cancelButton = cancellableCard!.getByRole('button', { name: /Cancel Entry/ });
  401 | 
  402 |       // Count POSTs with a request listener — it sees every request the page
  403 |       // issues, whereas the route handler only sees what the interception layer
  404 |       // hands it (Mobile Safari has counted 0 there while the trace showed one).
  405 |       // The route's only job is to hold the first response briefly so a broken
  406 |       // guard's second request would race in and push the count to 2.
  407 |       const CANCEL_POST = /\/api\/v1\/entries\/[^/]+\/cancel\//;
  408 |       let cancelPostCount = 0;
  409 |       page.on('request', (request) => {
  410 |         if (request.method() === 'POST' && CANCEL_POST.test(request.url())) {
  411 |           cancelPostCount += 1;
  412 |         }
  413 |       });
  414 |       let firstHeld = false;
  415 |       await page.route(CANCEL_POST, async (route) => {
  416 |         if (route.request().method() !== 'POST') {
```