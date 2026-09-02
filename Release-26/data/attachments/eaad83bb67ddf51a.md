# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: slipPersistent/slip_persistent.spec.ts >> Slip persistence >> slip persists through Rewards tab round-trip
- Location: tests/slipPersistent/slip_persistent.spec.ts:49:5

# Error details

```
Error: Expected picks ["player-1089","player-878910","player-1363"] to persist, got ["player-1089","player-878910"]

expect(received).toEqual(expected) // deep equality

- Expected  - 1
+ Received  + 0

  Set {
    "player-1089",
-   "player-1363",
    "player-878910",
  }
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
                - generic [ref=e17]: $278.45
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
                  - button "OSA@GET Sat 3PM" [ref=e54] [cursor=pointer]:
                    - text: OSA@GET
                    - generic [ref=e55]: Sat 3PM
                - listitem [ref=e56]:
                  - button "LEV@BET Sat 3PM" [ref=e57] [cursor=pointer]:
                    - text: LEV@BET
                    - generic [ref=e58]: Sat 3PM
                - listitem [ref=e59]:
                  - button "FCB@VAL Sat 3PM" [ref=e60] [cursor=pointer]:
                    - text: FCB@VAL
                    - generic [ref=e61]: Sat 3PM
                - listitem [ref=e62]:
                  - button "RAY@ALA Sat 3PM" [ref=e63] [cursor=pointer]:
                    - text: RAY@ALA
                    - generic [ref=e64]: Sat 3PM
                - listitem [ref=e65]:
                  - button "ELC@GIR Sat 3PM" [ref=e66] [cursor=pointer]:
                    - text: ELC@GIR
                    - generic [ref=e67]: Sat 3PM
                - listitem [ref=e68]:
                  - button "SEV@CEL Sat 3PM" [ref=e69] [cursor=pointer]:
                    - text: SEV@CEL
                    - generic [ref=e70]: Sat 3PM
                - listitem [ref=e71]:
                  - button "RSO@ESP Sat 3PM" [ref=e72] [cursor=pointer]:
                    - text: RSO@ESP
                    - generic [ref=e73]: Sat 3PM
                - listitem [ref=e74]:
                  - button "ATH@RMA Sat 3PM" [ref=e75] [cursor=pointer]:
                    - text: ATH@RMA
                    - generic [ref=e76]: Sat 3PM
                - listitem [ref=e77]:
                  - button "ATM@VIL Sun 3PM" [ref=e78] [cursor=pointer]:
                    - text: ATM@VIL
                    - generic [ref=e79]: Sun 3PM
                - listitem [ref=e80]:
                  - button "OVI@MAL Sat 3PM" [ref=e81] [cursor=pointer]:
                    - text: OVI@MAL
                    - generic [ref=e82]: Sat 3PM
              - generic [ref=e83]:
                - generic [ref=e84]:
                  - generic [ref=e87]:
                    - img [ref=e89]
                    - textbox "Search player or team" [ref=e91]
                  - button "Change card style from grid" [ref=e93]
                - list [ref=e95]:
                  - listitem [ref=e96]:
                    - button "Shots" [ref=e97]
                  - listitem [ref=e98]:
                    - button "Goals" [ref=e99]
                  - listitem [ref=e100]:
                    - button "Shots on Goal" [ref=e101]
                  - listitem [ref=e102]:
                    - button "Assists" [ref=e103]
                  - listitem [ref=e104]:
                    - button "Saves" [ref=e105]
                  - listitem [ref=e106]:
                    - button "Gls + Ast" [ref=e107]
                  - listitem [ref=e108]:
                    - button "Offsides" [ref=e109]
                  - listitem [ref=e110]:
                    - button "Fouls Drawn" [ref=e111]
                  - listitem [ref=e112]:
                    - button "Fouls Committed" [ref=e113]
            - generic [ref=e114]:
              - generic [ref=e118]:
                - button "previous slide / item" [ref=e119] [cursor=pointer]:
                  - img [ref=e120]
                - list [ref=e123]:
                  - listitem [ref=e124]:
                    - button "Get $20 By referring a friend making a first $10 deposit. lightning-bolt-yellow" [ref=e125] [cursor=pointer]:
                      - generic [ref=e126]:
                        - generic [ref=e128]: Get $20
                        - generic [ref=e129]: By referring a friend making a first $10 deposit.
                      - img "lightning-bolt-yellow"
                  - listitem [ref=e130]:
                    - 'button "Boosted Picks 🚀 Every Pick Pays: Up to a 35% Boost! lightning-bolt-yellow" [ref=e131] [cursor=pointer]':
                      - generic [ref=e132]:
                        - generic [ref=e134]: Boosted Picks 🚀
                        - generic [ref=e135]: "Every Pick Pays: Up to a 35% Boost!"
                      - img "lightning-bolt-yellow"
                  - listitem [ref=e136]:
                    - button "Get $20 By referring a friend making a first $10 deposit. lightning-bolt-yellow" [ref=e137] [cursor=pointer]:
                      - generic [ref=e138]:
                        - generic [ref=e140]: Get $20
                        - generic [ref=e141]: By referring a friend making a first $10 deposit.
                      - img "lightning-bolt-yellow"
                  - listitem [ref=e142]:
                    - 'button "Boosted Picks 🚀 Every Pick Pays: Up to a 35% Boost! lightning-bolt-yellow" [ref=e143] [cursor=pointer]':
                      - generic [ref=e144]:
                        - generic [ref=e146]: Boosted Picks 🚀
                        - generic [ref=e147]: "Every Pick Pays: Up to a 35% Boost!"
                      - img "lightning-bolt-yellow"
                - button "next slide / item" [ref=e148] [cursor=pointer]:
                  - img [ref=e149]
              - generic [ref=e151]:
                - generic [ref=e154]:
                  - generic [ref=e157]:
                    - button "Open expert opinion for Lucas Boyé" [ref=e158]:
                      - img [ref=e159]
                    - img "Lucas Boyé" [ref=e162]
                  - generic [ref=e163]:
                    - generic [ref=e164]: Lucas Boyé
                    - button "1.5 FL C" [ref=e165]:
                      - generic [ref=e166]:
                        - img [ref=e167]
                        - img [ref=e169]
                      - generic [ref=e171]: "1.5"
                      - generic [ref=e172]: FL C
                    - generic [ref=e173]:
                      - generic [ref=e174]: RAY@ALA
                      - generic [ref=e175]: Sat 3PM
                    - generic [ref=e176]:
                      - button "Select over 1.5 Fouls Committed for 0 times" [disabled] [ref=e177]
                      - button "Select over 1.5 Fouls Committed for 1.26 times" [ref=e179]:
                        - generic [ref=e180]: 1.26x
                        - img [ref=e181]
                - generic [ref=e185]:
                  - generic [ref=e188]:
                    - button "Open expert opinion for Nahuel Tenaglia" [ref=e189]:
                      - img [ref=e190]
                    - img "Nahuel Tenaglia" [ref=e193]
                  - generic [ref=e194]:
                    - generic [ref=e195]: N. Tenaglia
                    - button "0.5 FL C" [ref=e196]:
                      - generic [ref=e197]:
                        - img [ref=e198]
                        - img [ref=e200]
                      - generic [ref=e202]: "0.5"
                      - generic [ref=e203]: FL C
                    - generic [ref=e204]:
                      - generic [ref=e205]: RAY@ALA
                      - generic [ref=e206]: Sat 3PM
                    - generic [ref=e207]:
                      - button "Select over 0.5 Fouls Committed for 0 times" [disabled] [ref=e208]
                      - button "Select over 0.5 Fouls Committed for 1.2 times" [ref=e210]:
                        - generic [ref=e211]: 1.2x
                        - img [ref=e212]
                - generic [ref=e216]:
                  - generic [ref=e219]:
                    - button "Open expert opinion for Jorge de Frutos" [ref=e220]:
                      - img [ref=e221]
                    - img "Jorge de Frutos" [ref=e224]
                  - generic [ref=e225]:
                    - generic [ref=e226]: J. de Frutos
                    - button "1.5 FL C" [ref=e227]:
                      - generic [ref=e228]:
                        - img [ref=e229]
                        - img [ref=e231]
                      - generic [ref=e233]: "1.5"
                      - generic [ref=e234]: FL C
                    - generic [ref=e235]:
                      - generic [ref=e236]: RAY@ALA
                      - generic [ref=e237]: Sat 3PM
                    - generic [ref=e238]:
                      - button "Select over 1.5 Fouls Committed for 0 times" [disabled] [ref=e239]
                      - button "Select over 1.5 Fouls Committed for 1.7 times" [ref=e241]:
                        - generic [ref=e242]: 1.7x
                        - img [ref=e243]
                - generic [ref=e247]:
                  - generic [ref=e250]:
                    - button "Open expert opinion for Pathé Ciss" [ref=e251]:
                      - img [ref=e252]
                    - img "Pathé Ciss" [ref=e255]
                  - generic [ref=e256]:
                    - generic [ref=e257]: Pathé Ciss
                    - button "1.5 FL C" [ref=e258]:
                      - generic [ref=e259]:
                        - img [ref=e260]
                        - img [ref=e262]
                      - generic [ref=e264]: "1.5"
                      - generic [ref=e265]: FL C
                    - generic [ref=e266]:
                      - generic [ref=e267]: RAY@ALA
                      - generic [ref=e268]: Sat 3PM
                    - generic [ref=e269]:
                      - button "Select over 1.5 Fouls Committed for 0 times" [disabled] [ref=e270]
                      - button "Select over 1.5 Fouls Committed for 1.43 times" [ref=e272]:
                        - generic [ref=e273]: 1.43x
                        - img [ref=e274]
            - generic [ref=e673]:
              - img [ref=e675]
              - generic [ref=e677]:
                - generic [ref=e679]:
                  - generic [ref=e680]: 7.22x
                  - generic [ref=e681]: 7.58x
                - generic [ref=e682]:
                  - button "+ 10% Boost 🚀" [ref=e688]:
                    - generic [ref=e689]: + 10% Boost 🚀
                  - generic [ref=e699]: "Add 4th Pick: 10% Boost"
              - button "Continue" [ref=e700] [cursor=pointer]
          - generic [ref=e702]:
            - generic [ref=e704]:
              - link "Download ParlayPlay On The App Store" [ref=e705]:
                - /url: https://parlayplay.onelink.me/oLJk/gnqpwjha
                - img "Download ParlayPlay On The App Store" [ref=e706]
              - paragraph [ref=e707]:
                - text: Get the app.
                - text: Better. Faster. Convenient
            - navigation [ref=e708]:
              - link "Privacy" [ref=e709]:
                - /url: /privacy-policy
              - link "Terms" [ref=e710]:
                - /url: /terms
              - link "Responsible Gaming" [ref=e711]:
                - /url: /responsible-gaming
              - link "Gaming Rules" [ref=e712]:
                - /url: /rules
              - link "FAQ" [ref=e713]:
                - /url: https://intercom.help/parlayplay/en/
            - navigation [ref=e714]:
              - generic [ref=e715]:
                - paragraph [ref=e716]: © ParlayPlay 2026
                - generic [ref=e717]:
                  - link [ref=e718]:
                    - /url: https://www.facebook.com/parlayplay.io
                    - img [ref=e719]
                  - link [ref=e721]:
                    - /url: https://www.instagram.com/parlayplay_?igsh=bHBldWQyMmV2b3Y4
                    - img [ref=e722]
                  - link [ref=e724]:
                    - /url: https://www.twitter.com/parlay_play
                    - img [ref=e725]
                  - link [ref=e727]:
                    - /url: https://discord.com/invite/parlayplay
                    - img [ref=e728]
                - img "21+-icon" [ref=e730]
              - paragraph [ref=e732]: Gambling can be addictive. Please play responsibly.
      - contentinfo [ref=e733]:
        - navigation [ref=e734]:
          - list [ref=e735]:
            - listitem [ref=e736]:
              - button "Home" [ref=e737] [cursor=pointer]:
                - generic [ref=e738]:
                  - img [ref=e739]
                  - generic [ref=e740]: Home
            - listitem [ref=e741]:
              - button "Entries 160" [ref=e742] [cursor=pointer]:
                - generic [ref=e743]:
                  - img [ref=e744]
                  - generic [ref=e745]: Entries
                - generic [ref=e746]: "160"
            - listitem [ref=e747]:
              - button "Feed" [ref=e748] [cursor=pointer]:
                - generic [ref=e749]:
                  - img [ref=e750]
                  - generic [ref=e751]: Feed
            - listitem [ref=e752]:
              - button "Rewards 56" [ref=e753] [cursor=pointer]:
                - generic [ref=e754]:
                  - img [ref=e755]
                  - generic [ref=e756]: Rewards
                - generic [ref=e757]: "56"
            - listitem [ref=e758]:
              - button "Free2Play 2" [ref=e759] [cursor=pointer]:
                - generic [ref=e760]:
                  - img [ref=e761]
                  - generic [ref=e762]: Free2Play
                - generic [ref=e763]: "2"
    - region "Notifications Alt+T"
  - alert [ref=e764]: ParlayPlay | Fun Fantasy Sports
```

# Test source

```ts
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
  320 |       const btnCount = await buttons.count();
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
> 339 |     ).toEqual(new Set(expectedIds));
      |       ^ Error: Expected picks ["player-1089","player-878910","player-1363"] to persist, got ["player-1089","player-878910"]
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