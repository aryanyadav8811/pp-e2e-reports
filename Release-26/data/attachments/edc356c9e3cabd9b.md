# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: slipPersistent/slip_persistent.spec.ts >> Slip persistence >> slip persists through hard page reload
- Location: tests/slipPersistent/slip_persistent.spec.ts:74:5

# Error details

```
Test timeout of 240000ms exceeded.
```

```
Error: locator.count: Target page, context or browser has been closed
```

# Page snapshot

```yaml
- generic [active] [ref=e1]:
  - generic [ref=e2]:
    - generic [ref=e3]:
      - banner [ref=e4]:
        - navigation [ref=e5]:
          - link "Parlay Play LogoParlay Play text" [ref=e6]:
            - /url: /
            - generic [ref=e7]:
              - img "Parlay Play Logo" [ref=e8]
              - img "Parlay Play text" [ref=e9]
          - generic [ref=e10]:
            - button "Switch to dark mode" [ref=e11]:
              - img [ref=e12]
            - generic [ref=e14]:
              - generic [ref=e16]:
                - generic [ref=e17]: $250.45
                - generic [ref=e18]:
                  - img "gift-icon" [ref=e19]
                  - text: "114.00"
              - button "Toggle Menu" [ref=e20]:
                - img [ref=e21]
      - main [ref=e23]:
        - generic [ref=e26]:
          - generic [ref=e27]:
            - generic [ref=e28]:
              - list [ref=e30]:
                - button "Promo" [ref=e31] [cursor=pointer]
                - button "NBA" [ref=e32] [cursor=pointer]
                - button "NBA-Combos" [ref=e33] [cursor=pointer]
                - button "NBA Q1" [ref=e34] [cursor=pointer]
                - button "NBA H1" [ref=e35] [cursor=pointer]
                - button "MLB" [ref=e36] [cursor=pointer]
                - button "MLB-Combos" [ref=e37] [cursor=pointer]
                - button "NHL" [ref=e38] [cursor=pointer]
                - button "NHL-Combos" [ref=e39] [cursor=pointer]
                - button "SerieA" [ref=e40] [cursor=pointer]
                - button "EPL" [ref=e41] [cursor=pointer]
                - button "MLS" [ref=e42] [cursor=pointer]
                - button "CSGO" [ref=e43] [cursor=pointer]
                - button "LoL" [ref=e44] [cursor=pointer]
                - button "Valorant" [ref=e45] [cursor=pointer]
                - button "Cricket" [ref=e46] [cursor=pointer]
                - button "LaLiga" [ref=e47] [cursor=pointer]
              - list [ref=e49]:
                - listitem [ref=e50]:
                  - button "ALL" [ref=e51] [cursor=pointer]:
                    - generic [ref=e52]: ALL
                - listitem [ref=e53]:
                  - button "CLE@NYK 8:10PM" [ref=e54] [cursor=pointer]:
                    - text: CLE@NYK
                    - generic [ref=e55]: 8:10PM
                - listitem [ref=e56]:
                  - button "OKC@SAS Fri 8PM" [ref=e57] [cursor=pointer]:
                    - text: OKC@SAS
                    - generic [ref=e58]: Fri 8PM
              - generic [ref=e59]:
                - generic [ref=e60]:
                  - generic [ref=e63]:
                    - img [ref=e65]
                    - textbox "Search player or team" [ref=e67]
                  - button "Change card style from grid" [ref=e69]
                - list [ref=e71]:
                  - listitem [ref=e72]:
                    - button "Points" [ref=e73]
                  - listitem [ref=e74]:
                    - button "Rebounds" [ref=e75]
                  - listitem [ref=e76]:
                    - button "Assists" [ref=e77]
                  - listitem [ref=e78]:
                    - button "Triple Double" [ref=e79]
                  - listitem [ref=e80]:
                    - button "3PT Made" [ref=e81]
                  - listitem [ref=e82]:
                    - button "Pts + Reb + Ast" [ref=e83]
                  - listitem [ref=e84]:
                    - button "Double Double" [ref=e85]
                  - listitem [ref=e86]:
                    - button "Pts + Reb" [ref=e87]
                  - listitem [ref=e88]:
                    - button "Pts + Ast" [ref=e89]
                  - listitem [ref=e90]:
                    - button "Reb + Ast" [ref=e91]
                  - listitem [ref=e92]:
                    - button "Stl + Blk" [ref=e93]
                  - listitem [ref=e94]:
                    - button "3PT Attempted" [ref=e95]
                  - listitem [ref=e96]:
                    - button "FT Made" [ref=e97]
                  - listitem [ref=e98]:
                    - button "FG Made" [ref=e99]
                  - listitem [ref=e100]:
                    - button "FG Attempted" [ref=e101]
                  - listitem [ref=e102]:
                    - button "Steals" [ref=e103]
                  - listitem [ref=e104]:
                    - button "Blocks" [ref=e105]
                  - listitem [ref=e106]:
                    - button "Turnovers" [ref=e107]
            - generic [ref=e108]:
              - generic [ref=e112]:
                - button "previous slide / item" [ref=e113] [cursor=pointer]:
                  - img [ref=e114]
                - list [ref=e117]:
                  - listitem [ref=e118]:
                    - generic [ref=e120] [cursor=pointer]:
                      - img "huddle-bg-small"
                      - generic [ref=e121]:
                        - generic [ref=e122]:
                          - generic [ref=e123]: Pistons
                          - generic [ref=e126]: VS
                          - generic [ref=e127]: Magic
                        - generic [ref=e128]: Huddle
                        - generic [ref=e129]:
                          - generic [ref=e130]:
                            - generic [ref=e131]:
                              - text: Win
                              - generic [ref=e132]: $1000
                            - generic [ref=e133]: + many more prizes
                          - button "Enter" [ref=e135]
                  - listitem [ref=e136]:
                    - 'button "Boosted Picks 🚀 Every Pick Pays: Up to a 35% Boost! lightning-bolt-yellow" [ref=e137] [cursor=pointer]':
                      - generic [ref=e138]:
                        - generic [ref=e140]: Boosted Picks 🚀
                        - generic [ref=e141]: "Every Pick Pays: Up to a 35% Boost!"
                      - img "lightning-bolt-yellow"
                  - listitem [ref=e142]:
                    - button "Get $20 By referring a friend making a first $10 deposit. lightning-bolt-yellow" [ref=e143] [cursor=pointer]:
                      - generic [ref=e144]:
                        - generic [ref=e146]: Get $20
                        - generic [ref=e147]: By referring a friend making a first $10 deposit.
                      - img "lightning-bolt-yellow"
                  - listitem [ref=e148]:
                    - generic [ref=e150] [cursor=pointer]:
                      - img "huddle-bg-small"
                      - generic [ref=e151]:
                        - generic [ref=e152]:
                          - generic [ref=e153]: Pistons
                          - generic [ref=e156]: VS
                          - generic [ref=e157]: Magic
                        - generic [ref=e158]: Huddle
                        - generic [ref=e159]:
                          - generic [ref=e160]:
                            - generic [ref=e161]:
                              - text: Win
                              - generic [ref=e162]: $1000
                            - generic [ref=e163]: + many more prizes
                          - button "Enter" [ref=e165]
                  - listitem [ref=e166]:
                    - 'button "Boosted Picks 🚀 Every Pick Pays: Up to a 35% Boost! lightning-bolt-yellow" [ref=e167] [cursor=pointer]':
                      - generic [ref=e168]:
                        - generic [ref=e170]: Boosted Picks 🚀
                        - generic [ref=e171]: "Every Pick Pays: Up to a 35% Boost!"
                      - img "lightning-bolt-yellow"
                - button "next slide / item" [ref=e172] [cursor=pointer]:
                  - img [ref=e173]
              - generic [ref=e175]:
                - generic [ref=e178]:
                  - generic [ref=e181]:
                    - button "Open expert opinion for Jarrett Allen" [ref=e182]:
                      - img [ref=e183]
                    - img "Jarrett Allen" [ref=e186]
                    - generic [ref=e188]: Boost Special
                  - generic [ref=e189]:
                    - generic [ref=e190]: Jarrett Allen
                    - button "6.5 Rebounds" [ref=e191]:
                      - generic [ref=e192]:
                        - img [ref=e193]
                        - img [ref=e195]
                      - generic [ref=e197]: "6.5"
                      - generic [ref=e198]: Rebounds
                    - generic [ref=e199]:
                      - generic [ref=e200]: CLE@NYK
                      - generic [ref=e201]: 08:51:16
                    - generic [ref=e202]:
                      - button "Select over 6.5 Rebounds for 2.29 times" [ref=e203]:
                        - img [ref=e204]
                        - img [ref=e208]
                        - generic [ref=e210]: 2.29x
                      - button "Select over 6.5 Rebounds for 1.52 times" [ref=e211]:
                        - generic [ref=e212]: 1.52x
                        - img "Promo Boost Arrow" [ref=e214]
                - generic [ref=e217]:
                  - generic [ref=e220]:
                    - button "Open expert opinion for Sam Merrill" [ref=e221]:
                      - img [ref=e222]
                    - img "Sam Merrill" [ref=e225]
                  - generic [ref=e226]:
                    - generic [ref=e227]: Sam Merrill
                    - button "1.5 Rebounds" [ref=e228]:
                      - generic [ref=e229]:
                        - img [ref=e230]
                        - img [ref=e232]
                      - generic [ref=e234]: "1.5"
                      - generic [ref=e235]: Rebounds
                    - generic [ref=e236]:
                      - generic [ref=e237]: CLE@NYK
                      - generic [ref=e238]: 8:10PM
                    - generic [ref=e239]:
                      - button "Select over 1.5 Rebounds for 1.68 times" [ref=e240]:
                        - img [ref=e241]
                        - generic [ref=e243]: 1.68x
                      - button "Select over 1.5 Rebounds for 1.68 times" [ref=e244]:
                        - generic [ref=e245]: 1.68x
                        - img [ref=e246]
                - generic [ref=e250]:
                  - generic [ref=e253]:
                    - button "Open expert opinion for James Harden" [ref=e254]:
                      - img [ref=e255]
                    - img "James Harden" [ref=e258]
                  - generic [ref=e259]:
                    - generic [ref=e260]: James Harden
                    - button "4.5 Rebounds" [ref=e261]:
                      - generic [ref=e262]:
                        - img [ref=e263]
                        - img [ref=e265]
                      - generic [ref=e267]: "4.5"
                      - generic [ref=e268]: Rebounds
                    - generic [ref=e269]:
                      - generic [ref=e270]: CLE@NYK
                      - generic [ref=e271]: 8:10PM
                    - generic [ref=e272]:
                      - button "Select over 4.5 Rebounds for 1.74 times" [ref=e273]:
                        - img [ref=e274]
                        - generic [ref=e276]: 1.74x
                      - button "Select over 4.5 Rebounds for 1.88 times" [ref=e277]:
                        - generic [ref=e278]: 1.88x
                        - img [ref=e279]
                - generic [ref=e283]:
                  - generic [ref=e286]:
                    - button "Open expert opinion for Donovan Mitchell" [ref=e287]:
                      - img [ref=e288]
                    - img "Donovan Mitchell" [ref=e291]
                  - generic [ref=e292]:
                    - generic [ref=e293]: D. Mitchell
                    - button "4.5 Rebounds" [ref=e294]:
                      - generic [ref=e295]:
                        - img [ref=e296]
                        - img [ref=e298]
                      - generic [ref=e300]: "4.5"
                      - generic [ref=e301]: Rebounds
                    - generic [ref=e302]:
                      - generic [ref=e303]: CLE@NYK
                      - generic [ref=e304]: 8:10PM
                    - generic [ref=e305]:
                      - button "Select over 4.5 Rebounds for 1.68 times" [ref=e306]:
                        - img [ref=e307]
                        - generic [ref=e309]: 1.68x
                      - button "Select over 4.5 Rebounds for 1.93 times" [ref=e310]:
                        - generic [ref=e311]: 1.93x
                        - img [ref=e312]
            - generic [ref=e513]:
              - img [ref=e515]
              - generic [ref=e517]:
                - generic [ref=e519]:
                  - generic [ref=e520]: 7x
                  - generic [ref=e521]: 7.35x
                - generic [ref=e522]:
                  - button "+ 10% Boost 🚀" [ref=e528]:
                    - generic [ref=e529]: + 10% Boost 🚀
                  - generic [ref=e539]: "Add 4th Pick: 10% Boost"
              - button "Continue" [ref=e540] [cursor=pointer]
          - generic [ref=e542]:
            - generic [ref=e544]:
              - link "Download ParlayPlay On The App Store" [ref=e545]:
                - /url: https://parlayplay.onelink.me/oLJk/gnqpwjha
                - img "Download ParlayPlay On The App Store" [ref=e546]
              - paragraph [ref=e547]:
                - text: Get the app.
                - text: Better. Faster. Convenient
            - navigation [ref=e548]:
              - link "Privacy" [ref=e549]:
                - /url: /privacy-policy
              - link "Terms" [ref=e550]:
                - /url: /terms
              - link "Responsible Gaming" [ref=e551]:
                - /url: /responsible-gaming
              - link "Gaming Rules" [ref=e552]:
                - /url: /rules
              - link "FAQ" [ref=e553]:
                - /url: https://intercom.help/parlayplay/en/
            - navigation [ref=e554]:
              - generic [ref=e555]:
                - paragraph [ref=e556]: © ParlayPlay 2026
                - generic [ref=e557]:
                  - link [ref=e558]:
                    - /url: https://www.facebook.com/parlayplay.io
                    - img [ref=e559]
                  - link [ref=e561]:
                    - /url: https://www.instagram.com/parlayplay_?igsh=bHBldWQyMmV2b3Y4
                    - img [ref=e562]
                  - link [ref=e564]:
                    - /url: https://www.twitter.com/parlay_play
                    - img [ref=e565]
                  - link [ref=e567]:
                    - /url: https://discord.com/invite/parlayplay
                    - img [ref=e568]
                - img "21+-icon" [ref=e570]
              - paragraph [ref=e572]: Gambling can be addictive. Please play responsibly.
      - contentinfo [ref=e573]:
        - navigation [ref=e574]:
          - list [ref=e575]:
            - listitem [ref=e576]:
              - button "Home" [ref=e577] [cursor=pointer]:
                - generic [ref=e578]:
                  - img [ref=e579]
                  - generic [ref=e580]: Home
            - listitem [ref=e581]:
              - button "Entries 169" [ref=e582] [cursor=pointer]:
                - generic [ref=e583]:
                  - img [ref=e584]
                  - generic [ref=e585]: Entries
                - generic [ref=e586]: "169"
            - listitem [ref=e587]:
              - button "Feed" [ref=e588] [cursor=pointer]:
                - generic [ref=e589]:
                  - img [ref=e590]
                  - generic [ref=e591]: Feed
            - listitem [ref=e592]:
              - button "Rewards 56" [ref=e593] [cursor=pointer]:
                - generic [ref=e594]:
                  - img [ref=e595]
                  - generic [ref=e596]: Rewards
                - generic [ref=e597]: "56"
            - listitem [ref=e598]:
              - button "Free2Play 2" [ref=e599] [cursor=pointer]:
                - generic [ref=e600]:
                  - img [ref=e601]
                  - generic [ref=e602]: Free2Play
                - generic [ref=e603]: "2"
    - region "Notifications Alt+T"
  - alert [ref=e604]
```

# Test source

```ts
  220 |             lastPick &&
  221 |             lastPickId
  222 |           ) {
  223 |             await this.deselectPick(lastPick);
  224 |             selected.delete(lastPickId);
  225 |             recentlyFailed.add(lastPickId);
  226 | 
  227 |             let replaced = false;
  228 |             for (const nextPick of picks) {
  229 |               const nextId = await nextPick
  230 |                 .locator(">div[id]")
  231 |                 .getAttribute("id");
  232 |               if (!nextId || selected.has(nextId) || recentlyFailed.has(nextId))
  233 |                 continue;
  234 |               if (nextId === lastPickId) continue;
  235 |               if (await this.trySelectPick(nextPick)) {
  236 |                 selected.add(nextId);
  237 |                 lastPick = nextPick;
  238 |                 lastPickId = nextId;
  239 |                 replaced = true;
  240 |                 break;
  241 |               }
  242 |             }
  243 |             if (!replaced) {
  244 |               throw new Error(
  245 |                 `Unable to find replacement pick when Continue is disabled (target: ${count})`
  246 |               );
  247 |             }
  248 |             continueFlag = await this.isContinueEnabled();
  249 |           }
  250 | 
  251 |           if (continueFlag && selected.size == count)
  252 |             return Array.from(selected);
  253 |           if (continueFlag) recentlyFailed.clear();
  254 |         }
  255 |       }
  256 |     }
  257 | 
  258 |     if (selected.size < count)
  259 |       throw new Error(`Could not select ${count} valid picks`);
  260 |     return Array.from(selected);
  261 |   }
  262 | 
  263 |   async pickFivePlayers(): Promise<string[]> {
  264 |     return this.pickPlayers(5);
  265 |   }
  266 | 
  267 |   /**
  268 |    * Walks every non-combo league tab and returns the player-card IDs that
  269 |    * currently have a highlighted (bg-playYellow) grid-button. Used to verify
  270 |    * slip persistence after navigation or reload.
  271 |    *
  272 |    * A player card only renders grid-buttons for the currently active stat
  273 |    * tab, so a pick made on Assists is invisible when the league lands on
  274 |    * Points. We iterate every stat tab per league and union the matches.
  275 |    */
  276 |   async getSelectedPickIds(): Promise<string[]> {
  277 |     const leagueButtons = await this.listLeagueButtons();
  278 |     const ids = new Set<string>();
  279 | 
  280 |     for (const leagueButton of leagueButtons) {
  281 |       const leagueId = (await leagueButton.getAttribute("id")) ?? "";
  282 |       if (leagueId.toLowerCase().includes("combo")) continue;
  283 | 
  284 |       await leagueButton.click();
  285 |       await this.waitForFeedReady().catch(() => undefined);
  286 |       if (await this.isEmptyState()) continue;
  287 | 
  288 |       const statTabs = this.statsSelector.locator("li button");
  289 |       const statCount = await statTabs.count().catch(() => 0);
  290 |       // Always do at least one pass: a league with no stat selector
  291 |       // still has cards we need to scan with whatever's currently shown.
  292 |       const tabsToVisit = Math.max(statCount, 1);
  293 | 
  294 |       for (let s = 0; s < tabsToVisit; s++) {
  295 |         if (statCount > 0) {
  296 |           try {
  297 |             await statTabs.nth(s).click({ timeout: 5_000 });
  298 |             await this.waitForPlayersGrid();
  299 |           } catch {
  300 |             // Disabled / off-screen / overlapped tab — skip rather
  301 |             // than fail the whole scan; another stat may still
  302 |             // surface the pick.
  303 |             continue;
  304 |           }
  305 |         }
  306 | 
  307 |         await this.collectHighlightedCardIds(ids);
  308 |       }
  309 |     }
  310 | 
  311 |     return Array.from(ids);
  312 |   }
  313 | 
  314 |   private async collectHighlightedCardIds(into: Set<string>): Promise<void> {
  315 |     const cards = this.playerCardsVisible;
  316 |     const n = await cards.count();
  317 |     for (let i = 0; i < n; i++) {
  318 |       const card = cards.nth(i);
  319 |       const buttons = card.getByTestId("grid-button");
> 320 |       const btnCount = await buttons.count();
      |                                      ^ Error: locator.count: Target page, context or browser has been closed
  321 |       for (let j = 0; j < btnCount; j++) {
  322 |         const cls = (await buttons.nth(j).getAttribute("class")) ?? "";
  323 |         if (cls.includes("bg-playYellow")) {
  324 |           const id = await card.locator(">div[id]").getAttribute("id");
  325 |           if (id) into.add(id);
  326 |           break;
  327 |         }
  328 |       }
  329 |     }
  330 |   }
  331 | 
  332 |   async assertPicksPersist(expectedIds: string[]): Promise<void> {
  333 |     const currentIds = await this.getSelectedPickIds();
  334 |     expect(
  335 |       new Set(currentIds),
  336 |       `Expected picks ${JSON.stringify(
  337 |         expectedIds
  338 |       )} to persist, got ${JSON.stringify(currentIds)}`
  339 |     ).toEqual(new Set(expectedIds));
  340 |   }
  341 | 
  342 |   async waitForSlipPersisted(
  343 |     expectedPickCount: number,
  344 |     timeout = 5_000
  345 |   ): Promise<void> {
  346 |     await expect
  347 |       .poll(
  348 |         async () =>
  349 |           this.page.evaluate(() => {
  350 |             const raw = localStorage.getItem("pp_persistent_slip:v1");
  351 |             if (!raw) return 0;
  352 |             try {
  353 |               return JSON.parse(raw).nrOfPicks ?? 0;
  354 |             } catch {
  355 |               return 0;
  356 |             }
  357 |           }),
  358 |         {
  359 |           timeout,
  360 |           message: `Slip with ${expectedPickCount} picks was never written to localStorage`,
  361 |         }
  362 |       )
  363 |       .toBe(expectedPickCount);
  364 |   }
  365 | 
  366 |   async enterFinalContestPage() {
  367 |     await this.continueBtn.click();
  368 |   }
  369 | 
  370 |   async clearSlip(): Promise<void> {
  371 |     await this.page.evaluate(() =>
  372 |       localStorage.removeItem("pp_persistent_slip:v1")
  373 |     );
  374 |     await this.page.goto("/");
  375 |     await this.waitForFeedReady();
  376 |   }
  377 | 
  378 |   async selectStatByIndex(idx: number): Promise<void> {
  379 |     const tab = this.statsSelector.locator("li button").nth(idx);
  380 |     await expect(tab).toBeVisible();
  381 |     await tab.click();
  382 |     await this.waitForFeedReady();
  383 |   }
  384 | 
  385 |   async enterEntriesPage() {
  386 |     await this.entriesTab.click();
  387 |   }
  388 | 
  389 |   async enterHomePage(): Promise<void> {
  390 |     await this.homeTab.click();
  391 |     await this.waitForFeedReady();
  392 |     await expect(this.leagueSelector).toBeVisible();
  393 |   }
  394 | 
  395 |   async enterMenu() {
  396 |     // Some specs land here without an explicit goto('/'), so the global
  397 |     // header may not be mounted yet. Wait briefly for Toggle Menu before
  398 |     // clicking — fail fast (15s) instead of letting the test-level timeout
  399 |     // (10 min) absorb a hung locator.
  400 |     await this.toggleMenu.waitFor({ state: "visible", timeout: 15_000 });
  401 |     await this.toggleMenu.click({ timeout: 15_000 });
  402 |   }
  403 | 
  404 |   async assertHomePage() {
  405 |     await expect(this.leagueSelector).toBeVisible();
  406 |   }
  407 | 
  408 |   async enterRewarsdsPage() {
  409 |     await this.rewardsTab.click();
  410 |   }
  411 | 
  412 |   async fullGameLeagueCount() {
  413 |     return await this.fgleagueTabs.count();
  414 |   }
  415 | 
  416 |   async statsTabCount() {
  417 |     return await this.statsTabs.count();
  418 |   }
  419 | }
  420 | 
```