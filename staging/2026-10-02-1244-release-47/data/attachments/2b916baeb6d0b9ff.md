# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: slip-sharing/share-and-tail.spec.ts >> Slip sharing - share and tail >> Logged-in tailer clicks "Tail this entry" and submits the same picks
- Location: tests/slip-sharing/share-and-tail.spec.ts:34:5

# Error details

```
Error: Tailer's persistent slip should match Sharer's pick IDs

expect(received).toEqual(expected) // deep equality

- Expected  - 1
+ Received  + 0

  Array [
    "1362339",
-   "2206733",
    "22230",
  ]

Call Log:
- Timeout 15000ms exceeded while waiting on the predicate
```

# Test source

```ts
  34  |     test('Logged-in tailer clicks "Tail this entry" and submits the same picks', async ({
  35  |       browser,
  36  |       contextOptions,
  37  |       baseURL,
  38  |       storageStateFor,
  39  |       diag,
  40  |     }) => {
  41  |       test.setTimeout(480_000);
  42  | 
  43  |       let sharerCtx: BrowserContext | undefined;
  44  |       let tailerCtx: BrowserContext | undefined;
  45  | 
  46  |       try {
  47  |         const sharerStatePath = await storageStateFor(sharer.username, sharer.password);
  48  |         const sharerSetup = await newContextWithDefaults(
  49  |           browser,
  50  |           { ...contextOptions, storageState: sharerStatePath },
  51  |           baseURL,
  52  |           diag,
  53  |         );
  54  |         sharerCtx = sharerSetup.context;
  55  |         const sPage = sharerSetup.page;
  56  | 
  57  |         const sHome = new HomePage(sPage);
  58  |         const sContest = new ContestPage(sPage);
  59  | 
  60  |         await test.step('Sharer opens home (already authenticated)', async () => {
  61  |           await sPage.goto('/');
  62  |           await sHome.waitForFeedReady();
  63  |         });
  64  | 
  65  |         let pickIds: string[] = [];
  66  |         let shareUrlPath = '';
  67  |         await test.step(`Sharer selects ${PICK_COUNT} picks and places a $${ENTRY_AMOUNT} entry`, async () => {
  68  |           const result = await placeContestWithRetry({
  69  |             homePage: sHome,
  70  |             contestPage: sContest,
  71  |             pickCount: PICK_COUNT,
  72  |             entryAmount: ENTRY_AMOUNT,
  73  |             submit: async () => {
  74  |               // Start listening before placePick so the share response
  75  |               // can't slip past us between click and await.
  76  |               const sharePromise = sPage.waitForResponse(
  77  |                 (resp) =>
  78  |                   SHARE_API_PATH.test(new URL(resp.url()).pathname) &&
  79  |                   resp.request().method() === 'POST' &&
  80  |                   resp.status() === 200,
  81  |                 { timeout: 60_000 },
  82  |               );
  83  |               // Swallow rejection on retried attempts where the share
  84  |               // call never resolves with 200.
  85  |               sharePromise.catch(() => undefined);
  86  | 
  87  |               const submitResult = await sContest.submitAndAwaitResult();
  88  |               if (submitResult.success) {
  89  |                 const shareResp = await sharePromise;
  90  |                 const body = await shareResp.json();
  91  |                 expect(body?.shareUrl, 'share API should return shareUrl').toBeTruthy();
  92  |                 shareUrlPath = new URL(body.shareUrl).pathname;
  93  |                 expect(shareUrlPath).toMatch(TAIL_PATH);
  94  |               }
  95  |               return submitResult;
  96  |             },
  97  |           });
  98  |           pickIds = result.pickIds;
  99  |           expect(pickIds).toHaveLength(PICK_COUNT);
  100 |         });
  101 | 
  102 |         const tailerStatePath = await storageStateFor(tailer.username, tailer.password);
  103 |         const tailerSetup = await newContextWithDefaults(
  104 |           browser,
  105 |           { ...contextOptions, storageState: tailerStatePath },
  106 |           baseURL,
  107 |           diag,
  108 |         );
  109 |         tailerCtx = tailerSetup.context;
  110 |         const tPage = tailerSetup.page;
  111 | 
  112 |         const tTail = new TailPage(tPage);
  113 |         const tContest = new ContestPage(tPage);
  114 |         const tSuccess = new ContestSuccessPage(tPage);
  115 | 
  116 |         await test.step('Tailer opens home (already authenticated)', async () => {
  117 |           await tPage.goto('/');
  118 |         });
  119 | 
  120 |         await test.step(`Tailer opens the shared tail link ${shareUrlPath}`, async () => {
  121 |           await tTail.openByPath(shareUrlPath);
  122 |           await tTail.assertReadyToTail();
  123 |         });
  124 | 
  125 |         await test.step('Tailer taps "Tail this entry" — submission overlay auto-opens', async () => {
  126 |           await tTail.clickTailThisEntry();
  127 |           await tTail.confirmOverrideIfPresent();
  128 |           await tPage.waitForURL((url) => HOME_PATH.test(url.pathname), { timeout: 60_000 });
  129 |           await expect(tContest.submissionReady).toBeVisible({ timeout: 30_000 });
  130 |         });
  131 | 
  132 |         await test.step(`Tailer's persistent slip holds the sharer's ${PICK_COUNT} pick ids`, async () => {
  133 |           const expected = pickIds.map((id) => id.replace(/^player-/, '')).sort();
> 134 |           await expect
      |           ^ Error: Tailer's persistent slip should match Sharer's pick IDs
  135 |             .poll(
  136 |               async () =>
  137 |                 tPage.evaluate((key) => {
  138 |                   const raw = localStorage.getItem(key);
  139 |                   if (!raw) return [];
  140 |                   try {
  141 |                     return Object.keys(JSON.parse(raw).selectedPicks ?? {}).sort();
  142 |                   } catch {
  143 |                     return [];
  144 |                   }
  145 |                 }, SLIP_STORAGE_KEY),
  146 |               {
  147 |                 timeout: 15_000,
  148 |                 message: "Tailer's persistent slip should match Sharer's pick IDs",
  149 |               },
  150 |             )
  151 |             .toEqual(expected);
  152 |         });
  153 | 
  154 |         await test.step(`Tailer places the tailed $${ENTRY_AMOUNT} entry — success page is shareable`, async () => {
  155 |           await tContest.setEntryAmountIfEditable(ENTRY_AMOUNT);
  156 |           await tContest.placePick();
  157 |           await expect(
  158 |             tPage.getByRole('button', { name: 'Continue' }).filter({ visible: true }).first(),
  159 |           ).toBeVisible();
  160 |           await tSuccess.assertContestShareable();
  161 |         });
  162 |       } finally {
  163 |         await sharerCtx?.close();
  164 |         await tailerCtx?.close();
  165 |       }
  166 |     });
  167 | 
  168 |     test('Logged-out tailer signs in via the tail link, then auto-tails and submits', async ({
  169 |       browser,
  170 |       contextOptions,
  171 |       baseURL,
  172 |       storageStateFor,
  173 |       diag,
  174 |     }) => {
  175 |       test.setTimeout(480_000);
  176 | 
  177 |       let sharerCtx: BrowserContext | undefined;
  178 |       let tailerCtx: BrowserContext | undefined;
  179 | 
  180 |       try {
  181 |         const sharerStatePath = await storageStateFor(sharer.username, sharer.password);
  182 |         const sharerSetup = await newContextWithDefaults(
  183 |           browser,
  184 |           { ...contextOptions, storageState: sharerStatePath },
  185 |           baseURL,
  186 |           diag,
  187 |         );
  188 |         sharerCtx = sharerSetup.context;
  189 |         const sPage = sharerSetup.page;
  190 | 
  191 |         const sHome = new HomePage(sPage);
  192 |         const sContest = new ContestPage(sPage);
  193 | 
  194 |         await test.step('Sharer opens home (already authenticated)', async () => {
  195 |           await sPage.goto('/');
  196 |           await sHome.waitForFeedReady();
  197 |         });
  198 | 
  199 |         let pickIds: string[] = [];
  200 |         let shareUrlPath = '';
  201 |         await test.step(`Sharer selects ${PICK_COUNT} picks and places a $${ENTRY_AMOUNT} entry`, async () => {
  202 |           const result = await placeContestWithRetry({
  203 |             homePage: sHome,
  204 |             contestPage: sContest,
  205 |             pickCount: PICK_COUNT,
  206 |             entryAmount: ENTRY_AMOUNT,
  207 |             submit: async () => {
  208 |               const sharePromise = sPage.waitForResponse(
  209 |                 (resp) =>
  210 |                   SHARE_API_PATH.test(new URL(resp.url()).pathname) &&
  211 |                   resp.request().method() === 'POST' &&
  212 |                   resp.status() === 200,
  213 |                 { timeout: 60_000 },
  214 |               );
  215 |               sharePromise.catch(() => undefined);
  216 | 
  217 |               const submitResult = await sContest.submitAndAwaitResult();
  218 |               if (submitResult.success) {
  219 |                 const shareResp = await sharePromise;
  220 |                 const body = await shareResp.json();
  221 |                 expect(body?.shareUrl, 'share API should return shareUrl').toBeTruthy();
  222 |                 shareUrlPath = new URL(body.shareUrl).pathname;
  223 |                 expect(shareUrlPath).toMatch(TAIL_PATH);
  224 |               }
  225 |               return submitResult;
  226 |             },
  227 |           });
  228 |           pickIds = result.pickIds;
  229 |           expect(pickIds).toHaveLength(PICK_COUNT);
  230 |         });
  231 | 
  232 |         const tailerSetup = await newContextWithDefaults(browser, contextOptions, baseURL, diag);
  233 |         tailerCtx = tailerSetup.context;
  234 |         const tPage = tailerSetup.page;
```