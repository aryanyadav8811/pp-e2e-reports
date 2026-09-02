# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: slip_sharing/slip_sharing_and_tailing.spec.ts >> Slip sharing & tailing >> Logged-out tailer signs in via the tail link, then auto-tails and submits
- Location: tests/slip_sharing/slip_sharing_and_tailing.spec.ts:173:5

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
  204 |             let shareUrlPath = '';
  205 |             await test.step(
  206 |                 `Sharer selects ${PICK_COUNT} picks and places the entry (rotate stat on limit)`,
  207 |                 async () => {
  208 |                     const result = await placeContestWithRetry({
  209 |                         homePage: sHome,
  210 |                         contestPage: sContest,
  211 |                         pickCount: PICK_COUNT,
  212 |                         entryAmount: ENTRY_AMOUNT,
  213 |                         submit: async () => {
  214 |                             const sharePromise = sPage.waitForResponse(
  215 |                                 (resp) =>
  216 |                                     SHARE_API_PATH.test(new URL(resp.url()).pathname) &&
  217 |                                     resp.request().method() === 'POST' &&
  218 |                                     resp.status() === 200,
  219 |                                 { timeout: 60_000 },
  220 |                             );
  221 |                             sharePromise.catch(() => undefined);
  222 | 
  223 |                             const submitResult = await sContest.submitAndAwaitResult();
  224 |                             if (submitResult.success) {
  225 |                                 const shareResp = await sharePromise;
  226 |                                 const body = await shareResp.json();
  227 |                                 expect(body?.shareUrl, 'share API should return shareUrl').toBeTruthy();
  228 |                                 shareUrlPath = new URL(body.shareUrl).pathname;
  229 |                                 expect(shareUrlPath).toMatch(TAIL_PATH);
  230 |                             }
  231 |                             return submitResult;
  232 |                         },
  233 |                     });
  234 |                     pickIds = result.pickIds;
  235 |                     expect(pickIds).toHaveLength(PICK_COUNT);
  236 |                 },
  237 |             );
  238 | 
  239 |             // ---------------- TAILER (starts unauthenticated) ----------------
  240 |             const tailerSetup = await newContextWithDefaults(browser, contextOptions, baseURL);
  241 |             tailerCtx = tailerSetup.context;
  242 |             const tPage = tailerSetup.page;
  243 | 
  244 |             const tLogin = new AuthPage(tPage);
  245 |             const tTail = new TailPage(tPage);
  246 |             const tContest = new ContestPage(tPage);
  247 |             const tSuccess = new ContestSuccessPage(tPage);
  248 | 
  249 |             await test.step('Unauthenticated tailer opens the shared tail link and is routed to the lobby', async () => {
  250 |                 // New-user share flow (ui/pages/tail/[uuid].tsx): a logged-out
  251 |                 // visitor to /tail/<uuid> no longer sees a "Log In to Tail"
  252 |                 // CTA — the page stores the tail intent in a cookie
  253 |                 // (utils/tailIntent.ts) and redirects to the lobby so they
  254 |                 // authenticate via the header. Only ?auto_tail deep links
  255 |                 // still route straight to the login page.
  256 |                 await tTail.openByPath(shareUrlPath);
  257 |                 await tPage.waitForURL((url) => HOME_PATH.test(url.pathname), { timeout: 30_000 });
  258 |             });
  259 | 
  260 |             await test.step('Tailer logs in; the lobby consumes the tail intent and routes back to the tail page', async () => {
  261 |                 await tLogin.logIn(tailer.username, tailer.password);
  262 |                 // pages/index.tsx reads the pending-tail cookie once the user
  263 |                 // is authenticated and pushes back to /tail/<uuid>.
  264 |                 await tPage.waitForURL((url) => TAIL_PATH.test(url.pathname), { timeout: 60_000 });
  265 |                 await tTail.assertReadyToTail();
  266 |             });
  267 | 
  268 |             await test.step('Tailer taps "Tail this entry" — submission overlay auto-opens', async () => {
  269 |                 await tTail.clickTailThisEntry();
  270 |                 await tTail.confirmOverrideIfPresent();
  271 |                 await tPage.waitForURL((url) => HOME_PATH.test(url.pathname), { timeout: 60_000 });
  272 |                 await expect(tContest.submissionReady).toBeVisible({ timeout: 30_000 });
  273 |             });
  274 | 
  275 |             await test.step("Tailer's persistent slip matches the sharer's picks", async () => {
  276 |                 // pickPlayers returns DOM ids like "player-1314", but pp_persistent_slip:v1's
  277 |                 // selectedPicks is keyed by the bare player id ("1314") — strip the prefix.
  278 |                 const expected = pickIds.map((id) => id.replace(/^player-/, '')).sort();
  279 |                 await expect
  280 |                     .poll(
  281 |                         async () =>
  282 |                             tPage.evaluate((key) => {
  283 |                                 const raw = localStorage.getItem(key);
  284 |                                 if (!raw) return [];
  285 |                                 try {
  286 |                                     return Object.keys(JSON.parse(raw).selectedPicks ?? {}).sort();
  287 |                                 } catch {
  288 |                                     return [];
  289 |                                 }
  290 |                             }, SLIP_STORAGE_KEY),
  291 |                         {
  292 |                             timeout: 15_000,
  293 |                             message: "Tailer's persistent slip should match Sharer's pick IDs",
  294 |                         },
  295 |                     )
  296 |                     .toEqual(expected);
  297 |             });
  298 | 
  299 |             await test.step('Tailer places the tailed entry and the success page is shareable', async () => {
  300 |                 await tContest.setEntryAmountIfEditable(ENTRY_AMOUNT);
  301 |                 await tContest.placePick();
  302 |                 await expect(
  303 |                     tPage.getByRole('button', { name: 'Continue' }).filter({ visible: true }).first(),
> 304 |                 ).toBeVisible();
      |                   ^ Error: expect(locator).toBeVisible() failed
  305 |                 await tSuccess.assertContestShareable();
  306 |             });
  307 |         } finally {
  308 |             await sharerCtx?.close();
  309 |             await tailerCtx?.close();
  310 |         }
  311 |     });
  312 | });
  313 | 
```