# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: slip-sharing/share-and-tail.spec.ts >> Slip sharing - share and tail >> Logged-in tailer clicks "Tail this entry" and submits the same picks
- Location: tests/slip-sharing/share-and-tail.spec.ts:31:3

# Error details

```
Error: Tailer's persistent slip should match Sharer's pick IDs

expect(received).toEqual(expected) // deep equality

- Expected  - 1
+ Received  + 0

  Array [
-   "1514638",
    "849956",
    "851041",
  ]

Call Log:
- Timeout 15000ms exceeded while waiting on the predicate
```

# Test source

```ts
  31  |   test('Logged-in tailer clicks "Tail this entry" and submits the same picks', async ({
  32  |     browser,
  33  |     contextOptions,
  34  |     baseURL,
  35  |     storageStateFor,
  36  |     diag,
  37  |   }) => {
  38  |     test.setTimeout(480_000);
  39  | 
  40  |     let sharerCtx: BrowserContext | undefined;
  41  |     let tailerCtx: BrowserContext | undefined;
  42  | 
  43  |     try {
  44  |       const sharerStatePath = await storageStateFor(sharer.username, sharer.password);
  45  |       const sharerSetup = await newContextWithDefaults(
  46  |         browser,
  47  |         { ...contextOptions, storageState: sharerStatePath },
  48  |         baseURL,
  49  |         diag,
  50  |       );
  51  |       sharerCtx = sharerSetup.context;
  52  |       const sPage = sharerSetup.page;
  53  | 
  54  |       const sHome = new HomePage(sPage);
  55  |       const sContest = new ContestPage(sPage);
  56  | 
  57  |       await test.step('Sharer opens home (already authenticated)', async () => {
  58  |         await sPage.goto('/');
  59  |         await sHome.waitForFeedReady();
  60  |       });
  61  | 
  62  |       let pickIds: string[] = [];
  63  |       let shareUrlPath = '';
  64  |       await test.step(`Sharer selects ${PICK_COUNT} picks and places a $${ENTRY_AMOUNT} entry`, async () => {
  65  |         const result = await placeContestWithRetry({
  66  |           homePage: sHome,
  67  |           contestPage: sContest,
  68  |           pickCount: PICK_COUNT,
  69  |           entryAmount: ENTRY_AMOUNT,
  70  |           submit: async () => {
  71  |             // Start listening before placePick so the share response
  72  |             // can't slip past us between click and await.
  73  |             const sharePromise = sPage.waitForResponse(
  74  |               (resp) =>
  75  |                 SHARE_API_PATH.test(new URL(resp.url()).pathname) &&
  76  |                 resp.request().method() === 'POST' &&
  77  |                 resp.status() === 200,
  78  |               { timeout: 60_000 },
  79  |             );
  80  |             // Swallow rejection on retried attempts where the share
  81  |             // call never resolves with 200.
  82  |             sharePromise.catch(() => undefined);
  83  | 
  84  |             const submitResult = await sContest.submitAndAwaitResult();
  85  |             if (submitResult.success) {
  86  |               const shareResp = await sharePromise;
  87  |               const body = await shareResp.json();
  88  |               expect(body?.shareUrl, 'share API should return shareUrl').toBeTruthy();
  89  |               shareUrlPath = new URL(body.shareUrl).pathname;
  90  |               expect(shareUrlPath).toMatch(TAIL_PATH);
  91  |             }
  92  |             return submitResult;
  93  |           },
  94  |         });
  95  |         pickIds = result.pickIds;
  96  |         expect(pickIds).toHaveLength(PICK_COUNT);
  97  |       });
  98  | 
  99  |       const tailerStatePath = await storageStateFor(tailer.username, tailer.password);
  100 |       const tailerSetup = await newContextWithDefaults(
  101 |         browser,
  102 |         { ...contextOptions, storageState: tailerStatePath },
  103 |         baseURL,
  104 |         diag,
  105 |       );
  106 |       tailerCtx = tailerSetup.context;
  107 |       const tPage = tailerSetup.page;
  108 | 
  109 |       const tTail = new TailPage(tPage);
  110 |       const tContest = new ContestPage(tPage);
  111 |       const tSuccess = new ContestSuccessPage(tPage);
  112 | 
  113 |       await test.step('Tailer opens home (already authenticated)', async () => {
  114 |         await tPage.goto('/');
  115 |       });
  116 | 
  117 |       await test.step(`Tailer opens the shared tail link ${shareUrlPath}`, async () => {
  118 |         await tTail.openByPath(shareUrlPath);
  119 |         await tTail.assertReadyToTail();
  120 |       });
  121 | 
  122 |       await test.step('Tailer taps "Tail this entry" — submission overlay auto-opens', async () => {
  123 |         await tTail.clickTailThisEntry();
  124 |         await tTail.confirmOverrideIfPresent();
  125 |         await tPage.waitForURL((url) => HOME_PATH.test(url.pathname), { timeout: 60_000 });
  126 |         await expect(tContest.submissionReady).toBeVisible({ timeout: 30_000 });
  127 |       });
  128 | 
  129 |       await test.step(`Tailer's persistent slip holds the sharer's ${PICK_COUNT} pick ids`, async () => {
  130 |         const expected = pickIds.map((id) => id.replace(/^player-/, '')).sort();
> 131 |         await expect
      |         ^ Error: Tailer's persistent slip should match Sharer's pick IDs
  132 |           .poll(
  133 |             async () =>
  134 |               tPage.evaluate((key) => {
  135 |                 const raw = localStorage.getItem(key);
  136 |                 if (!raw) return [];
  137 |                 try {
  138 |                   return Object.keys(JSON.parse(raw).selectedPicks ?? {}).sort();
  139 |                 } catch {
  140 |                   return [];
  141 |                 }
  142 |               }, SLIP_STORAGE_KEY),
  143 |             {
  144 |               timeout: 15_000,
  145 |               message: "Tailer's persistent slip should match Sharer's pick IDs",
  146 |             },
  147 |           )
  148 |           .toEqual(expected);
  149 |       });
  150 | 
  151 |       await test.step(`Tailer places the tailed $${ENTRY_AMOUNT} entry — success page is shareable`, async () => {
  152 |         await tContest.setEntryAmountIfEditable(ENTRY_AMOUNT);
  153 |         await tContest.placePick();
  154 |         await expect(
  155 |           tPage.getByRole('button', { name: 'Continue' }).filter({ visible: true }).first(),
  156 |         ).toBeVisible();
  157 |         await tSuccess.assertContestShareable();
  158 |       });
  159 |     } finally {
  160 |       await sharerCtx?.close();
  161 |       await tailerCtx?.close();
  162 |     }
  163 |   });
  164 | 
  165 |   test('Logged-out tailer signs in via the tail link, then auto-tails and submits', async ({
  166 |     browser,
  167 |     contextOptions,
  168 |     baseURL,
  169 |     storageStateFor,
  170 |     diag,
  171 |   }) => {
  172 |     test.setTimeout(480_000);
  173 | 
  174 |     let sharerCtx: BrowserContext | undefined;
  175 |     let tailerCtx: BrowserContext | undefined;
  176 | 
  177 |     try {
  178 |       const sharerStatePath = await storageStateFor(sharer.username, sharer.password);
  179 |       const sharerSetup = await newContextWithDefaults(
  180 |         browser,
  181 |         { ...contextOptions, storageState: sharerStatePath },
  182 |         baseURL,
  183 |         diag,
  184 |       );
  185 |       sharerCtx = sharerSetup.context;
  186 |       const sPage = sharerSetup.page;
  187 | 
  188 |       const sHome = new HomePage(sPage);
  189 |       const sContest = new ContestPage(sPage);
  190 | 
  191 |       await test.step('Sharer opens home (already authenticated)', async () => {
  192 |         await sPage.goto('/');
  193 |         await sHome.waitForFeedReady();
  194 |       });
  195 | 
  196 |       let pickIds: string[] = [];
  197 |       let shareUrlPath = '';
  198 |       await test.step(`Sharer selects ${PICK_COUNT} picks and places a $${ENTRY_AMOUNT} entry`, async () => {
  199 |         const result = await placeContestWithRetry({
  200 |           homePage: sHome,
  201 |           contestPage: sContest,
  202 |           pickCount: PICK_COUNT,
  203 |           entryAmount: ENTRY_AMOUNT,
  204 |           submit: async () => {
  205 |             const sharePromise = sPage.waitForResponse(
  206 |               (resp) =>
  207 |                 SHARE_API_PATH.test(new URL(resp.url()).pathname) &&
  208 |                 resp.request().method() === 'POST' &&
  209 |                 resp.status() === 200,
  210 |               { timeout: 60_000 },
  211 |             );
  212 |             sharePromise.catch(() => undefined);
  213 | 
  214 |             const submitResult = await sContest.submitAndAwaitResult();
  215 |             if (submitResult.success) {
  216 |               const shareResp = await sharePromise;
  217 |               const body = await shareResp.json();
  218 |               expect(body?.shareUrl, 'share API should return shareUrl').toBeTruthy();
  219 |               shareUrlPath = new URL(body.shareUrl).pathname;
  220 |               expect(shareUrlPath).toMatch(TAIL_PATH);
  221 |             }
  222 |             return submitResult;
  223 |           },
  224 |         });
  225 |         pickIds = result.pickIds;
  226 |         expect(pickIds).toHaveLength(PICK_COUNT);
  227 |       });
  228 | 
  229 |       const tailerSetup = await newContextWithDefaults(browser, contextOptions, baseURL, diag);
  230 |       tailerCtx = tailerSetup.context;
  231 |       const tPage = tailerSetup.page;
```