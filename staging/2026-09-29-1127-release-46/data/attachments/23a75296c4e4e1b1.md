# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: modals/userlimits.spec.ts >> User Limits - Limit Exceeded Modal >> Exceeding the daily entry limit shows the Limit Exceeded modal and Reset Limits clears it
- Location: tests/modals/userlimits.spec.ts:46:3

# Error details

```
Error: Could not select 5 valid picks
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
          - generic [ref=e9]:
            - list [ref=e10]:
              - listitem [ref=e11]:
                - link "Home" [ref=e12] [cursor=pointer]:
                  - /url: /
                  - generic [ref=e14]: Home
              - listitem [ref=e15]:
                - link "Packs" [ref=e16] [cursor=pointer]:
                  - /url: /packs
                  - generic [ref=e18]: Packs
              - listitem [ref=e19]:
                - link "Feed" [ref=e20] [cursor=pointer]:
                  - /url: /challenges/feed
                  - generic [ref=e22]: Feed
              - listitem [ref=e23]:
                - link "Rewards 9" [ref=e24] [cursor=pointer]:
                  - /url: /rewards
                  - generic [ref=e25]:
                    - generic [ref=e26]: Rewards
                    - generic [ref=e27]: "9"
              - listitem [ref=e28]:
                - link "Track Picks 170" [ref=e29] [cursor=pointer]:
                  - /url: /challenges/pending
                  - generic [ref=e30]:
                    - generic [ref=e31]: Track Picks
                    - generic [ref=e32]: "170"
            - button "Claim your $100 Deposit Match" [ref=e33] [cursor=pointer]
            - generic [ref=e34]:
              - generic [ref=e36]:
                - generic [ref=e37]: $604.77
                - generic [ref=e38]:
                  - img "gift-icon" [ref=e39]
                  - text: "9.00"
              - button "Toggle Menu" [ref=e40]:
                - img [ref=e41]
      - main [ref=e43]:
        - generic [ref=e45]:
          - generic [ref=e49]:
            - button "previous slide" [ref=e50] [cursor=pointer]:
              - img [ref=e51]
            - generic [ref=e54]:
              - generic [ref=e56]:
                - generic [ref=e57]:
                  - generic [ref=e58]: Receive a referral Bonus!
                  - generic [ref=e59]: $20
                - generic [ref=e60]:
                  - text: Refer a Friend
                  - text: when they make their first deposit
                  - button "Invite Now" [ref=e62] [cursor=pointer]
              - generic [ref=e64]:
                - generic [ref=e65]:
                  - text: $100
                  - img "black lightning bol" [ref=e66]
                - generic [ref=e68]: =
                - generic [ref=e69]:
                  - text: $200
                  - img "black lightning bol" [ref=e70]
                - generic [ref=e71]:
                  - text: We match your 1st deposit
                  - text: We match your first deposit up to $100.
                  - button "Deposit Now" [ref=e73] [cursor=pointer]
            - button "next slide" [ref=e74] [cursor=pointer]:
              - img [ref=e75]
          - generic [ref=e78]:
            - generic [ref=e80]:
              - generic [ref=e83]:
                - generic:
                  - img
                - textbox "Search player or team" [ref=e84]
              - generic [ref=e85]:
                - button "All" [ref=e86] [cursor=pointer]
                - button "MLB" [ref=e87] [cursor=pointer]
                - button "UFC" [ref=e88] [cursor=pointer]
              - button "right chevron sign Filter" [ref=e90] [cursor=pointer]:
                - img "right chevron sign" [ref=e91]
                - text: Filter
            - generic [ref=e92]:
              - generic [ref=e95]:
                - generic [ref=e98]:
                  - generic [ref=e99]:
                    - img "Ilias Bulaid" [ref=e101]
                    - generic [ref=e102]:
                      - generic [ref=e103]: Ilias Bulaid
                      - generic [ref=e104]: FI - IBulaid
                      - generic [ref=e107]: EViscond @ IBulaid 7:00 PM
                    - button "Open expert opinion for Ilias Bulaid" [ref=e108]:
                      - img [ref=e109]
                  - generic [ref=e113]:
                    - generic [ref=e114]:
                      - generic [ref=e115]:
                        - generic [ref=e117] [cursor=pointer]:
                          - text: Less
                          - img [ref=e118]
                        - generic [ref=e120]: Significant Strikes
                        - generic [ref=e122] [cursor=pointer]:
                          - text: More
                          - img [ref=e123]
                      - generic [ref=e126]:
                        - button "Select over 40.5 Significant Strikes for 1.77 times" [ref=e127]:
                          - img [ref=e130]
                          - text: 1.77x
                        - generic [ref=e132]: 40.5 S. STR
                        - button "Select over 40.5 Significant Strikes for 1.77 times" [ref=e133]: 1.77x
                    - generic [ref=e134]:
                      - generic [ref=e135]:
                        - generic [ref=e137] [cursor=pointer]:
                          - text: Less
                          - img [ref=e138]
                        - generic [ref=e140]: Strikes Landed
                        - generic [ref=e142] [cursor=pointer]:
                          - text: More
                          - img [ref=e143]
                      - generic [ref=e146]:
                        - button "Select over 60.5 Strikes Landed for 1.77 times" [ref=e147]: 1.77x
                        - generic [ref=e148]: 60.5 Strikes Landed
                        - button "Select over 60.5 Strikes Landed for 1.77 times" [ref=e149]: 1.77x
                  - button "Show More Stats" [ref=e151]:
                    - img [ref=e152]
                - generic [ref=e156]:
                  - generic [ref=e157]:
                    - img "Erick Visconde" [ref=e159]
                    - generic [ref=e160]:
                      - generic [ref=e161]: E. Visconde
                      - generic [ref=e162]: FI - EViscond
                      - generic [ref=e165]: EViscond @ IBulaid 7:00 PM
                    - button "Open expert opinion for Erick Visconde" [ref=e166]:
                      - img [ref=e167]
                  - generic [ref=e171]:
                    - generic [ref=e172]:
                      - generic [ref=e173]:
                        - generic [ref=e175] [cursor=pointer]:
                          - text: Less
                          - img [ref=e176]
                        - generic [ref=e178]: Significant Strikes
                        - generic [ref=e180] [cursor=pointer]:
                          - text: More
                          - img [ref=e181]
                      - generic [ref=e184]:
                        - button "Select over 40.5 Significant Strikes for 1.77 times" [active] [ref=e185]:
                          - img [ref=e188]
                          - text: 1.77x
                        - generic [ref=e190]: 40.5 S. STR
                        - button "Select over 40.5 Significant Strikes for 1.77 times" [ref=e191]: 1.77x
                    - generic [ref=e192]:
                      - generic [ref=e193]:
                        - generic [ref=e195] [cursor=pointer]:
                          - text: Less
                          - img [ref=e196]
                        - generic [ref=e198]: Strikes Landed
                        - generic [ref=e200] [cursor=pointer]:
                          - text: More
                          - img [ref=e201]
                      - generic [ref=e204]:
                        - button "Select over 60.5 Strikes Landed for 1.77 times" [ref=e205]: 1.77x
                        - generic [ref=e206]: 60.5 Strikes Landed
                        - button "Select over 60.5 Strikes Landed for 1.77 times" [ref=e207]: 1.77x
                  - button "Show More Stats" [ref=e209]:
                    - img [ref=e210]
              - generic [ref=e284]:
                - generic [ref=e286]:
                  - generic [ref=e288]:
                    - generic [ref=e289]: 10.28x
                    - generic [ref=e290]: 11.31x
                  - generic [ref=e291]:
                    - button "+ 15% Boost 🚀" [ref=e298]:
                      - generic [ref=e299]: + 15% Boost 🚀
                    - generic [ref=e308]: "Add 5th Pick: 15% Boost"
                - generic [ref=e310]:
                  - generic [ref=e312]:
                    - generic [ref=e313]:
                      - generic [ref=e315]: "1"
                      - button [ref=e318]:
                        - img [ref=e320]
                      - generic [ref=e322]: Braves - Matt Olson
                      - generic [ref=e323]: Today 2:00 PM vs PHI
                      - generic [ref=e324]:
                        - button "2.5 x Less 0.5 Hits" [ref=e326]:
                          - generic [ref=e328]: 2.5 x
                          - generic [ref=e329]: Less
                          - generic [ref=e330]: "0.5"
                          - generic [ref=e331]: Hits
                          - img [ref=e334]
                        - button "1.38 x More 0.5 Hits" [ref=e337]:
                          - generic [ref=e339]: 1.38 x
                          - generic [ref=e340]: More
                          - generic [ref=e341]: "0.5"
                          - generic [ref=e342]: Hits
                    - img "Matt Olson" [ref=e345]
                  - generic [ref=e347]:
                    - generic [ref=e348]:
                      - generic [ref=e350]: "2"
                      - button [ref=e353]:
                        - img [ref=e355]
                      - generic [ref=e357]: Braves - Ozzie Albies
                      - generic [ref=e358]: Today 2:00 PM vs PHI
                      - generic [ref=e359]:
                        - button "2.5 x Less 0.5 Hits" [ref=e361]:
                          - generic [ref=e363]: 2.5 x
                          - generic [ref=e364]: Less
                          - generic [ref=e365]: "0.5"
                          - generic [ref=e366]: Hits
                          - img [ref=e369]
                        - button "1.34 x More 0.5 Hits" [ref=e372]:
                          - generic [ref=e374]: 1.34 x
                          - generic [ref=e375]: More
                          - generic [ref=e376]: "0.5"
                          - generic [ref=e377]: Hits
                    - img "Ozzie Albies" [ref=e380]
                  - generic [ref=e382]:
                    - generic [ref=e383]:
                      - generic [ref=e385]: "3"
                      - button [ref=e388]:
                        - img [ref=e390]
                      - generic [ref=e392]: Bulaid - Ilias Bulaid
                      - generic [ref=e393]: Today 7:00 PM vs EViscond
                      - generic [ref=e394]:
                        - button "1.77 x Less 40.5 Significant Strikes" [ref=e396]:
                          - generic [ref=e398]: 1.77 x
                          - generic [ref=e399]: Less
                          - generic [ref=e400]: "40.5"
                          - generic [ref=e401]: Significant Strikes
                          - img [ref=e404]
                        - button "1.77 x More 40.5 Significant Strikes" [ref=e407]:
                          - generic [ref=e409]: 1.77 x
                          - generic [ref=e410]: More
                          - generic [ref=e411]: "40.5"
                          - generic [ref=e412]: Significant Strikes
                    - img "Ilias Bulaid" [ref=e415]
                  - generic [ref=e417]:
                    - generic [ref=e418]:
                      - generic [ref=e420]: "4"
                      - button [ref=e423]:
                        - img [ref=e425]
                      - generic [ref=e427]: Visconde - Erick Visconde
                      - generic [ref=e428]: Today 7:00 PM vs IBulaid
                      - generic [ref=e429]:
                        - button "1.77 x Less 40.5 Significant Strikes" [ref=e431]:
                          - generic [ref=e433]: 1.77 x
                          - generic [ref=e434]: Less
                          - generic [ref=e435]: "40.5"
                          - generic [ref=e436]: Significant Strikes
                          - img [ref=e439]
                        - button "1.77 x More 40.5 Significant Strikes" [ref=e442]:
                          - generic [ref=e444]: 1.77 x
                          - generic [ref=e445]: More
                          - generic [ref=e446]: "40.5"
                          - generic [ref=e447]: Significant Strikes
                    - img "Erick Visconde" [ref=e450]
                  - generic [ref=e451]:
                    - generic [ref=e452]:
                      - generic [ref=e454]:
                        - radio "$25"
                        - generic [ref=e455] [cursor=pointer]: $25
                        - radio "$75"
                        - generic [ref=e456] [cursor=pointer]: $75
                        - radio "$300" [disabled]
                        - generic: $300
                      - generic [ref=e458]:
                        - generic [ref=e459]: $
                        - spinbutton [ref=e463]: "3"
                      - button "9" [ref=e464] [cursor=pointer]:
                        - img [ref=e465]
                        - generic [ref=e467]: "9"
                    - generic [ref=e468]:
                      - generic [ref=e469]:
                        - generic [ref=e470]:
                          - button "Insured" [ref=e471]
                          - button "All In" [ref=e472]
                        - generic [ref=e473]:
                          - generic [ref=e474]: 10.28x
                          - generic [ref=e475]: 11.31x
                      - generic [ref=e477]:
                        - generic [ref=e478]:
                          - paragraph [ref=e479]: Perfect line-up
                          - paragraph [ref=e480]: $33.93
                        - generic [ref=e482]:
                          - paragraph [ref=e483]: Or 1st place in group
                          - generic [ref=e484]: $1 + $33.93
                    - button "Place" [ref=e488] [cursor=pointer]:
                      - text: Place
                      - img [ref=e489]
          - generic [ref=e493]:
            - generic [ref=e494]:
              - link "Parlay Play Logo" [ref=e495] [cursor=pointer]:
                - /url: /
                - img "Parlay Play Logo" [ref=e497]
              - generic [ref=e498]:
                - generic [ref=e499]: Improve your experience. Download our app.
                - generic [ref=e500]:
                  - link "Apple Store" [ref=e501] [cursor=pointer]:
                    - /url: https://apps.apple.com/us/app/parlayplay-fantasy-sports-game/id1634803703
                    - img "Apple Store" [ref=e502]
                  - link "Google Play Store" [ref=e503] [cursor=pointer]:
                    - /url: https://play.google.com/store/apps/details?id=com.parlayplay.app&hl=en_US
                    - img "Google Play Store" [ref=e504]
            - generic [ref=e505]:
              - link "Privacy" [ref=e506] [cursor=pointer]:
                - /url: /privacy-policy
              - link "Fantasy Terms" [ref=e507] [cursor=pointer]:
                - /url: /terms
              - link "Packs Terms" [ref=e508] [cursor=pointer]:
                - /url: /terms/packs
              - link "Responsible Gaming" [ref=e509] [cursor=pointer]:
                - /url: /responsible-gaming
              - link "Gaming Rules" [ref=e510] [cursor=pointer]:
                - /url: /rules
              - link "FAQ" [ref=e511] [cursor=pointer]:
                - /url: https://intercom.help/parlayplay/en/
              - link "Contact Us" [ref=e512] [cursor=pointer]:
                - /url: /
              - paragraph [ref=e513]: © ParlayPlay 2026 - All Rights Reserved
            - list [ref=e514]:
              - listitem [ref=e515]:
                - generic [ref=e516]:
                  - log [ref=e518]
                  - generic [ref=e519]:
                    - generic [ref=e520]:
                      - generic [ref=e521]: 🇺🇸English
                      - combobox "Select language" [ref=e522]
                    - img [ref=e526]
              - listitem [ref=e528]:
                - img "18+-icon" [ref=e529]
              - listitem [ref=e530]:
                - link "ParlayPlay on Twitter" [ref=e531] [cursor=pointer]:
                  - /url: https://twitter.com/parlay_play?lang=en
                  - img [ref=e532]
              - listitem [ref=e534]:
                - link "ParlayPlay on Facebook" [ref=e535] [cursor=pointer]:
                  - /url: https://www.facebook.com/ParlayPlay.io/
                  - img [ref=e536]
              - listitem [ref=e538]:
                - link "ParlayPlay on Instagram" [ref=e539] [cursor=pointer]:
                  - /url: https://www.instagram.com/parlayplay_?igsh=bHBldWQyMmV2b3Y4
                  - img [ref=e540]
              - listitem [ref=e542]:
                - link "ParlayPlay on Discord" [ref=e543] [cursor=pointer]:
                  - /url: https://discord.com/invite/parlayplay
                  - img [ref=e544]
    - generic:
      - region "Notifications Alt+T"
  - alert [ref=e546]: ParlayPlay | Fun Fantasy Sports
  - iframe [ref=e547]:
    
```

# Test source

```ts
  302 | 
  303 |   async deselectPick(card: Locator): Promise<void> {
  304 |     const buttons = this.pickButtons(card);
  305 |     const count = await buttons.count();
  306 | 
  307 |     for (let i = 0; i < count; i++) {
  308 |       const btn = buttons.nth(i);
  309 |       const classes = (await btn.getAttribute('class')) ?? '';
  310 |       if (classes.includes('bg-playYellow')) {
  311 |         await btn.click();
  312 |         return;
  313 |       }
  314 |     }
  315 |     throw new Error('No selected button found with bg-yellow class.');
  316 |   }
  317 | 
  318 |   /**
  319 |    * `excludeIds`: retries (e.g. after "multiple promos cannot be applied")
  320 |    * pass the failed slip's players so the deterministic pick order doesn't
  321 |    * re-select the same promo-bearing cards.
  322 |    */
  323 |   async pickPlayers(count: number, statIdx?: number, excludeIds?: Set<string>): Promise<string[]> {
  324 |     const leagueButtons = await this.listLeagueButtons();
  325 | 
  326 |     const selected = new Set<string>();
  327 |     let lastPickId: string | null = null;
  328 |     // Kept separate from recentlyFailed (cleared once a valid combo is found)
  329 |     // so retries never re-pick a player a prior attempt already tried.
  330 |     const excluded = new Set<string>(excludeIds ?? []);
  331 |     const recentlyFailed = new Set<string>();
  332 |     for (const leagueButton of leagueButtons) {
  333 |       const leagueId = (await leagueButton.getAttribute('id')) ?? '';
  334 |       // Every card in the Combo and Promo leagues carries a promo, so picking
  335 |       // >1 always trips "multiple promos cannot be applied" and re-picking
  336 |       // never escapes it.
  337 |       const lid = leagueId.toLowerCase();
  338 |       if (lid.includes('combo') || lid.includes('promo')) continue;
  339 | 
  340 |       await this.clickLeagueTab(leagueButton);
  341 |       await this.waitForPlayersGrid();
  342 | 
  343 |       // Each league resets to its default stat tab on click.
  344 |       if (statIdx !== undefined) {
  345 |         const statTab = this.statsSelector.locator('li button').nth(statIdx);
  346 |         if (await statTab.isVisible().catch(() => false)) {
  347 |           await statTab.click();
  348 |           await this.waitForPlayersGrid();
  349 |         }
  350 |       }
  351 | 
  352 |       if (await this.noPlayerLabel.isVisible().catch(() => false)) {
  353 |         continue;
  354 |       }
  355 | 
  356 |       const playerIds = await this.listVisiblePlayerIds();
  357 |       // The virtualised grid mounts only a handful of cards on desktop, so a
  358 |       // small league can run dry with valid picks still selected — carry them
  359 |       // into the next league instead of aborting.
  360 |       let leagueExhausted = false;
  361 |       for (const playerId of playerIds) {
  362 |         if (selected.has(playerId) || recentlyFailed.has(playerId) || excluded.has(playerId))
  363 |           continue;
  364 | 
  365 |         if (await this.trySelectPick(this.playerCardById(playerId))) {
  366 |           selected.add(playerId);
  367 |           lastPickId = playerId;
  368 | 
  369 |           let continueFlag = await this.isContinueEnabled();
  370 |           if (selected.size >= count && continueFlag) return Array.from(selected);
  371 | 
  372 |           while (!continueFlag && selected.size == count && lastPickId) {
  373 |             await this.deselectPick(this.playerCardById(lastPickId));
  374 |             selected.delete(lastPickId);
  375 |             recentlyFailed.add(lastPickId);
  376 | 
  377 |             let replaced = false;
  378 |             for (const nextId of playerIds) {
  379 |               if (selected.has(nextId) || recentlyFailed.has(nextId) || excluded.has(nextId))
  380 |                 continue;
  381 |               if (await this.trySelectPick(this.playerCardById(nextId))) {
  382 |                 selected.add(nextId);
  383 |                 lastPickId = nextId;
  384 |                 replaced = true;
  385 |                 break;
  386 |               }
  387 |             }
  388 |             if (!replaced) {
  389 |               leagueExhausted = true;
  390 |               break;
  391 |             }
  392 |             continueFlag = await this.isContinueEnabled();
  393 |           }
  394 |           if (leagueExhausted) break;
  395 | 
  396 |           if (continueFlag && selected.size == count) return Array.from(selected);
  397 |           if (continueFlag) recentlyFailed.clear();
  398 |         }
  399 |       }
  400 |     }
  401 | 
> 402 |     if (selected.size < count) throw new Error(`Could not select ${count} valid picks`);
      |                                      ^ Error: Could not select 5 valid picks
  403 |     return Array.from(selected);
  404 |   }
  405 | 
  406 |   async pickFivePlayers(): Promise<string[]> {
  407 |     return this.pickPlayers(5);
  408 |   }
  409 | 
  410 |   /**
  411 |    * Reads picks from the slip the app persists via `slipPersistence.saveSlip`
  412 |    * rather than the DOM: when the backend omits a player's main/default
  413 |    * altLine flag the card boots on a fallback line and the highlight isn't
  414 |    * visible even though the pick is persisted.
  415 |    */
  416 |   async getPersistedPickIds(): Promise<string[]> {
  417 |     return this.page.evaluate(() => {
  418 |       const raw = localStorage.getItem('pp_persistent_slip:v1');
  419 |       if (!raw) return [];
  420 |       try {
  421 |         const parsed = JSON.parse(raw);
  422 |         return Object.keys(parsed.selectedPicks ?? {});
  423 |       } catch {
  424 |         return [];
  425 |       }
  426 |     });
  427 |   }
  428 | 
  429 |   async assertPicksPersist(expectedIds: string[], timeout = 10_000): Promise<void> {
  430 |     // Storage holds bare ids ("1089"); pickPlayers returns "player-1089".
  431 |     const normalise = (id: string) => id.replace(/^player-/, '');
  432 |     const expected = new Set(expectedIds.map(normalise));
  433 | 
  434 |     // Auto-save is debounced ~1s and the post-reload restore writes back
  435 |     // asynchronously, so poll.
  436 |     await expect
  437 |       .poll(
  438 |         async () => {
  439 |           const ids = await this.getPersistedPickIds();
  440 |           return Array.from(new Set(ids.map(normalise))).sort();
  441 |         },
  442 |         {
  443 |           timeout,
  444 |           message: `Expected persisted picks ${JSON.stringify(
  445 |             Array.from(expected).sort(),
  446 |           )} in localStorage`,
  447 |         },
  448 |       )
  449 |       .toEqual(Array.from(expected).sort());
  450 |   }
  451 | 
  452 |   async waitForSlipPersisted(expectedPickCount: number, timeout = 5_000): Promise<void> {
  453 |     await expect
  454 |       .poll(
  455 |         async () =>
  456 |           this.page.evaluate(() => {
  457 |             const raw = localStorage.getItem('pp_persistent_slip:v1');
  458 |             if (!raw) return 0;
  459 |             try {
  460 |               return JSON.parse(raw).nrOfPicks ?? 0;
  461 |             } catch {
  462 |               return 0;
  463 |             }
  464 |           }),
  465 |         {
  466 |           timeout,
  467 |           message: `Slip with ${expectedPickCount} picks was never written to localStorage`,
  468 |         },
  469 |       )
  470 |       .toBe(expectedPickCount);
  471 |   }
  472 | 
  473 |   async enterFinalContestPage() {
  474 |     // Desktop already shows the submission form — no Continue hop.
  475 |     if (await this.placePickBtn.isVisible().catch(() => false)) return;
  476 |     await this.continueBtn.click();
  477 |   }
  478 | 
  479 |   async clearSlip(): Promise<void> {
  480 |     await this.page.evaluate(() => localStorage.removeItem('pp_persistent_slip:v1'));
  481 |     await this.page.goto('/');
  482 |     await this.waitForFeedReady();
  483 |   }
  484 | 
  485 |   async selectStatByIndex(idx: number): Promise<void> {
  486 |     const tab = this.statsSelector.locator('li button').nth(idx);
  487 |     await expect(tab).toBeVisible();
  488 |     await tab.click();
  489 |     await this.waitForFeedReady();
  490 |   }
  491 | 
  492 |   async enterEntriesPage() {
  493 |     await this.entriesTab.click();
  494 |   }
  495 | 
  496 |   async enterHomePage(): Promise<void> {
  497 |     await this.homeTab.click();
  498 |     await this.waitForFeedReady();
  499 |     await expect(this.leagueSelector).toBeVisible();
  500 |   }
  501 | 
  502 |   async enterMenu() {
```