# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: slip-sharing/share-and-tail.spec.ts >> Slip sharing - share and tail >> Logged-in tailer clicks "Tail this entry" and submits the same picks
- Location: tests/slip-sharing/share-and-tail.spec.ts:38:5

# Error details

```
Error: expect(locator).toBeVisible() failed

Locator: getByRole('button', { name: 'Continue' }).filter({ visible: true }).first()
Expected: visible
Timeout: 15000ms
Error: element(s) not found

Call log:
  - Expect "toBeVisible" with timeout 15000ms
  - waiting for getByRole('button', { name: 'Continue' }).filter({ visible: true }).first()

```

# Test source

```ts
  63  | 
  64  |         await test.step('Sharer opens home (already authenticated)', async () => {
  65  |           await sPage.goto('/');
  66  |           await sHome.waitForFeedReady();
  67  |         });
  68  | 
  69  |         let pickIds: string[] = [];
  70  |         let shareUrlPath = '';
  71  |         await test.step(`Sharer selects ${PICK_COUNT} picks and places a $${ENTRY_AMOUNT} entry`, async () => {
  72  |           const result = await placeContestWithRetry({
  73  |             homePage: sHome,
  74  |             contestPage: sContest,
  75  |             pickCount: PICK_COUNT,
  76  |             entryAmount: ENTRY_AMOUNT,
  77  |             submit: async () => {
  78  |               // Start listening before placePick so the share response
  79  |               // can't slip past us between click and await.
  80  |               const sharePromise = sPage.waitForResponse(
  81  |                 (resp) =>
  82  |                   SHARE_API_PATH.test(new URL(resp.url()).pathname) &&
  83  |                   resp.request().method() === 'POST' &&
  84  |                   resp.status() === 200,
  85  |                 { timeout: 60_000 },
  86  |               );
  87  |               // Swallow rejection on retried attempts where the share
  88  |               // call never resolves with 200.
  89  |               sharePromise.catch(() => undefined);
  90  | 
  91  |               const submitResult = await sContest.submitAndAwaitResult();
  92  |               if (submitResult.success) {
  93  |                 const shareResp = await sharePromise;
  94  |                 const body = await shareResp.json();
  95  |                 expect(body?.shareUrl, 'share API should return shareUrl').toBeTruthy();
  96  |                 shareUrlPath = new URL(body.shareUrl).pathname;
  97  |                 expect(shareUrlPath).toMatch(TAIL_PATH);
  98  |               }
  99  |               return submitResult;
  100 |             },
  101 |           });
  102 |           pickIds = result.pickIds;
  103 |           expect(pickIds).toHaveLength(PICK_COUNT);
  104 |         });
  105 | 
  106 |         const tailerStatePath = await storageStateFor(tailer.username, tailer.password);
  107 |         const tailerSetup = await newContextWithDefaults(
  108 |           browser,
  109 |           { ...contextOptions, storageState: tailerStatePath },
  110 |           baseURL,
  111 |           diag,
  112 |         );
  113 |         tailerCtx = tailerSetup.context;
  114 |         const tPage = tailerSetup.page;
  115 | 
  116 |         const tTail = new TailPage(tPage);
  117 |         const tContest = new ContestPage(tPage);
  118 |         const tSuccess = new ContestSuccessPage(tPage);
  119 | 
  120 |         await test.step('Tailer opens home (already authenticated)', async () => {
  121 |           await tPage.goto('/');
  122 |         });
  123 | 
  124 |         await test.step(`Tailer opens the shared tail link ${shareUrlPath}`, async () => {
  125 |           await tTail.openByPath(shareUrlPath);
  126 |           await tTail.assertReadyToTail();
  127 |         });
  128 | 
  129 |         await test.step('Tailer taps "Tail this entry" — submission overlay auto-opens', async () => {
  130 |           await tTail.clickTailThisEntry();
  131 |           await tTail.confirmOverrideIfPresent();
  132 |           await tPage.waitForURL((url) => HOME_PATH.test(url.pathname), { timeout: 60_000 });
  133 |           await expect(tContest.submissionReady).toBeVisible({ timeout: 30_000 });
  134 |         });
  135 | 
  136 |         await test.step(`Tailer's persistent slip holds the sharer's ${PICK_COUNT} pick ids`, async () => {
  137 |           const expected = pickIds.map((id) => id.replace(/^player-/, '')).sort();
  138 |           await expect
  139 |             .poll(
  140 |               async () =>
  141 |                 tPage.evaluate((key) => {
  142 |                   const raw = localStorage.getItem(key);
  143 |                   if (!raw) return [];
  144 |                   try {
  145 |                     return Object.keys(JSON.parse(raw).selectedPicks ?? {}).sort();
  146 |                   } catch {
  147 |                     return [];
  148 |                   }
  149 |                 }, SLIP_STORAGE_KEY),
  150 |               {
  151 |                 timeout: 15_000,
  152 |                 message: "Tailer's persistent slip should match Sharer's pick IDs",
  153 |               },
  154 |             )
  155 |             .toEqual(expected);
  156 |         });
  157 | 
  158 |         await test.step(`Tailer places the tailed $${ENTRY_AMOUNT} entry — success page is shareable`, async () => {
  159 |           await tContest.setEntryAmountIfEditable(ENTRY_AMOUNT);
  160 |           await tContest.placePick();
  161 |           await expect(
  162 |             tPage.getByRole('button', { name: 'Continue' }).filter({ visible: true }).first(),
> 163 |           ).toBeVisible();
      |             ^ Error: expect(locator).toBeVisible() failed
  164 |           await tSuccess.assertContestShareable();
  165 |         });
  166 |       } finally {
  167 |         await sharerCtx?.close();
  168 |         await tailerCtx?.close();
  169 |       }
  170 |     });
  171 | 
  172 |     test('Logged-out tailer signs in via the tail link, then auto-tails and submits', async ({
  173 |       browser,
  174 |       contextOptions,
  175 |       baseURL,
  176 |       storageStateFor,
  177 |       diag,
  178 |     }) => {
  179 |       test.setTimeout(480_000);
  180 | 
  181 |       let sharerCtx: BrowserContext | undefined;
  182 |       let tailerCtx: BrowserContext | undefined;
  183 | 
  184 |       try {
  185 |         const sharerStatePath = await storageStateFor(sharer.username, sharer.password);
  186 |         const sharerSetup = await newContextWithDefaults(
  187 |           browser,
  188 |           { ...contextOptions, storageState: sharerStatePath },
  189 |           baseURL,
  190 |           diag,
  191 |         );
  192 |         sharerCtx = sharerSetup.context;
  193 |         const sPage = sharerSetup.page;
  194 | 
  195 |         const sHome = new HomePage(sPage);
  196 |         const sContest = new ContestPage(sPage);
  197 | 
  198 |         await test.step('Sharer opens home (already authenticated)', async () => {
  199 |           await sPage.goto('/');
  200 |           await sHome.waitForFeedReady();
  201 |         });
  202 | 
  203 |         let pickIds: string[] = [];
  204 |         let shareUrlPath = '';
  205 |         await test.step(`Sharer selects ${PICK_COUNT} picks and places a $${ENTRY_AMOUNT} entry`, async () => {
  206 |           const result = await placeContestWithRetry({
  207 |             homePage: sHome,
  208 |             contestPage: sContest,
  209 |             pickCount: PICK_COUNT,
  210 |             entryAmount: ENTRY_AMOUNT,
  211 |             submit: async () => {
  212 |               const sharePromise = sPage.waitForResponse(
  213 |                 (resp) =>
  214 |                   SHARE_API_PATH.test(new URL(resp.url()).pathname) &&
  215 |                   resp.request().method() === 'POST' &&
  216 |                   resp.status() === 200,
  217 |                 { timeout: 60_000 },
  218 |               );
  219 |               sharePromise.catch(() => undefined);
  220 | 
  221 |               const submitResult = await sContest.submitAndAwaitResult();
  222 |               if (submitResult.success) {
  223 |                 const shareResp = await sharePromise;
  224 |                 const body = await shareResp.json();
  225 |                 expect(body?.shareUrl, 'share API should return shareUrl').toBeTruthy();
  226 |                 shareUrlPath = new URL(body.shareUrl).pathname;
  227 |                 expect(shareUrlPath).toMatch(TAIL_PATH);
  228 |               }
  229 |               return submitResult;
  230 |             },
  231 |           });
  232 |           pickIds = result.pickIds;
  233 |           expect(pickIds).toHaveLength(PICK_COUNT);
  234 |         });
  235 | 
  236 |         const tailerSetup = await newContextWithDefaults(browser, contextOptions, baseURL, diag);
  237 |         tailerCtx = tailerSetup.context;
  238 |         const tPage = tailerSetup.page;
  239 | 
  240 |         const tLogin = new AuthPage(tPage);
  241 |         const tTail = new TailPage(tPage);
  242 |         const tContest = new ContestPage(tPage);
  243 |         const tSuccess = new ContestSuccessPage(tPage);
  244 | 
  245 |         await test.step(`Logged-out tailer opens ${shareUrlPath} and is routed to the lobby`, async () => {
  246 |           // A logged-out visitor to /tail/<uuid> sees no "Log In to Tail" CTA:
  247 |           // the page stores the tail intent in a cookie (utils/tailIntent.ts) and
  248 |           // redirects to the lobby. Only ?auto_tail deep links go straight to login.
  249 |           await tTail.openByPath(shareUrlPath);
  250 |           await tPage.waitForURL((url) => HOME_PATH.test(url.pathname), { timeout: 30_000 });
  251 |         });
  252 | 
  253 |         await test.step('Tailer logs in — lobby consumes the tail intent and returns to the tail page', async () => {
  254 |           await tLogin.logIn(tailer.username, tailer.password);
  255 |           // pages/index.tsx reads the pending-tail cookie once authenticated
  256 |           // and pushes back to /tail/<uuid>.
  257 |           await tPage.waitForURL((url) => TAIL_PATH.test(url.pathname), { timeout: 60_000 });
  258 |           await tTail.assertReadyToTail();
  259 |         });
  260 | 
  261 |         await test.step('Tailer taps "Tail this entry" — submission overlay auto-opens', async () => {
  262 |           await tTail.clickTailThisEntry();
  263 |           await tTail.confirmOverrideIfPresent();
```