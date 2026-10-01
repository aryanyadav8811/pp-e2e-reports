# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: slip-persistence/slip-persistence.spec.ts >> Slip persistence - navigation and reload >> Slip persists through an Entries tab round-trip
- Location: tests/slip-persistence/slip-persistence.spec.ts:28:5

# Error details

```
Error: Expected persisted picks ["638127","638174","638176"] in localStorage

expect(received).toEqual(expected) // deep equality

- Expected  - 1
+ Received  + 1

  Array [
-   "638127",
+   "1275518",
    "638174",
    "638176",
  ]

Call Log:
- Timeout 10000ms exceeded while waiting on the predicate
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
            - generic [ref=e12]:
              - generic [ref=e13]: $503.03
              - generic [ref=e14]:
                - img "gift-icon" [ref=e15]
                - text: "12.00"
            - button "Toggle Menu" [ref=e16]:
              - img [ref=e17]
      - main [ref=e19]:
        - generic [ref=e24]:
          - generic [ref=e25]:
            - generic [ref=e26]:
              - list [ref=e28]:
                - button "MLB" [ref=e29] [cursor=pointer]
                - button "NHL" [ref=e30] [cursor=pointer]
                - button "CSGO" [ref=e31] [cursor=pointer]
                - button "UFC" [ref=e32] [cursor=pointer]
              - list [ref=e34]:
                - listitem [ref=e35]:
                  - button "ALL" [ref=e36] [cursor=pointer]:
                    - generic [ref=e37]: ALL
                - listitem [ref=e38]:
                  - button "PHI@ATL 8:00PM" [ref=e39] [cursor=pointer]:
                    - text: PHI@ATL
                    - generic [ref=e40]: 8:00PM
              - generic [ref=e41]:
                - generic [ref=e42]:
                  - generic [ref=e45]:
                    - generic:
                      - img
                    - textbox "Search player or team" [ref=e46]
                  - button "Change card style from grid" [ref=e48]
                - list [ref=e50]:
                  - listitem [ref=e51]:
                    - button "Hits" [ref=e52]
                  - listitem [ref=e53]:
                    - button "Hits + Runs + RBIs" [ref=e54]
                  - listitem [ref=e55]:
                    - button "Singles" [ref=e56]
                  - listitem [ref=e57]:
                    - button "Doubles" [ref=e58]
                  - listitem [ref=e59]:
                    - button "Triples" [ref=e60]
                  - listitem [ref=e61]:
                    - button "Runs" [ref=e62]
                  - listitem [ref=e63]:
                    - button "RBIs" [ref=e64]
                  - listitem [ref=e65]:
                    - button "Homeruns" [ref=e66]
                  - listitem [ref=e67]:
                    - button "Total Bases" [ref=e68]
                  - listitem [ref=e69]:
                    - button "Strikeouts" [ref=e70]
                  - listitem [ref=e71]:
                    - button "Fantasy Points" [ref=e72]
            - generic [ref=e73]:
              - generic [ref=e78]:
                - generic [ref=e81] [cursor=pointer]:
                  - generic [ref=e82]:
                    - generic [ref=e83]:
                      - generic [ref=e84]: 100%
                      - generic [ref=e85]: Deposit Match
                    - generic [ref=e86]: New User Promotion
                  - button "Deposit" [ref=e88]
                - generic [ref=e92] [cursor=pointer]:
                  - generic [ref=e93]: Pull real graded cards worth up to $10,000
                  - generic [ref=e94]: Sell or ship instantly
                  - button "Rip a pack" [ref=e95]:
                    - generic [ref=e96]:
                      - img [ref=e97]
                      - text: Rip a pack
                - generic [ref=e102] [cursor=pointer]:
                  - generic [ref=e103]:
                    - generic [ref=e104]: Refer a friend, get a $20 Free Entry
                    - generic [ref=e105]: Referral bonus
                  - button "Refer" [ref=e106]
                - generic [ref=e109] [cursor=pointer]:
                  - generic [ref=e110]:
                    - generic [ref=e111]:
                      - img [ref=e112]
                      - generic [ref=e116]: Boosted Picks
                    - generic [ref=e117]: "Every Pick Pays: Up to a 35% Boost!"
                  - button "Details" [ref=e119]
              - generic [ref=e123]:
                - generic [ref=e126]:
                  - generic [ref=e129]:
                    - button "Open expert opinion for Matt Olson" [ref=e130]:
                      - img [ref=e131]
                    - img "Matt Olson" [ref=e134]
                  - generic [ref=e135]:
                    - generic [ref=e136]: Matt Olson
                    - button "0.5 Hits" [ref=e137]:
                      - generic [ref=e138]:
                        - img [ref=e139]
                        - img [ref=e141]
                      - generic [ref=e143]: "0.5"
                      - generic [ref=e144]: Hits
                    - generic [ref=e145]:
                      - generic [ref=e146]: PHI@ATL
                      - generic [ref=e147]: 8:00PM
                    - generic [ref=e148]:
                      - button "Select over 0.5 Hits for 2.38 times" [ref=e149]:
                        - img [ref=e150]
                        - img [ref=e154]
                        - generic [ref=e156]: 2.38x
                      - button "Select over 0.5 Hits for 1.42 times" [ref=e157]:
                        - generic [ref=e158]: 1.42x
                        - img [ref=e159]
                - generic [ref=e163]:
                  - generic [ref=e166]:
                    - button "Open expert opinion for Ozzie Albies" [ref=e167]:
                      - img [ref=e168]
                    - img "Ozzie Albies" [ref=e171]
                  - generic [ref=e172]:
                    - generic [ref=e173]: Ozzie Albies
                    - button "0.5 Hits" [ref=e174]:
                      - generic [ref=e175]:
                        - img [ref=e176]
                        - img [ref=e178]
                      - generic [ref=e180]: "0.5"
                      - generic [ref=e181]: Hits
                    - generic [ref=e182]:
                      - generic [ref=e183]: PHI@ATL
                      - generic [ref=e184]: 8:00PM
                    - generic [ref=e185]:
                      - button "Select over 0.5 Hits for 2.18 times" [ref=e186]:
                        - img [ref=e187]
                        - img [ref=e191]
                        - generic [ref=e193]: 2.18x
                      - button "Select over 0.5 Hits for 1.51 times" [ref=e194]:
                        - generic [ref=e195]: 1.51x
                        - img [ref=e196]
                - generic [ref=e200]:
                  - generic [ref=e203]:
                    - button "Open expert opinion for Sean Murphy" [ref=e204]:
                      - img [ref=e205]
                    - img "Sean Murphy" [ref=e208]
                  - generic [ref=e209]:
                    - generic [ref=e210]: Sean Murphy
                    - button "0.5 Hits" [ref=e211]:
                      - generic [ref=e212]:
                        - img [ref=e213]
                        - img [ref=e215]
                      - generic [ref=e217]: "0.5"
                      - generic [ref=e218]: Hits
                    - generic [ref=e219]:
                      - generic [ref=e220]: PHI@ATL
                      - generic [ref=e221]: 8:00PM
                    - generic [ref=e222]:
                      - button "Select over 0.5 Hits for 1.75 times" [ref=e223]:
                        - img [ref=e224]
                        - generic [ref=e226]: 1.75x
                      - button "Select over 0.5 Hits for 1.85 times" [ref=e227]:
                        - generic [ref=e228]: 1.85x
                        - img [ref=e229]
                - generic [ref=e233]:
                  - generic [ref=e236]:
                    - button "Open expert opinion for Michael Harris" [ref=e237]:
                      - img [ref=e238]
                    - img "Michael Harris" [ref=e241]
                  - generic [ref=e242]:
                    - generic [ref=e243]: M. Harris
                    - button "0.5 Hits" [ref=e244]:
                      - generic [ref=e245]:
                        - img [ref=e246]
                        - img [ref=e248]
                      - generic [ref=e250]: "0.5"
                      - generic [ref=e251]: Hits
                    - generic [ref=e252]:
                      - generic [ref=e253]: PHI@ATL
                      - generic [ref=e254]: 8:00PM
                    - generic [ref=e255]:
                      - button "Select over 0.5 Hits for 2.64 times" [ref=e256]:
                        - img [ref=e257]
                        - generic [ref=e259]: 2.64x
                      - button "Select over 0.5 Hits for 1.32 times" [ref=e260]:
                        - generic [ref=e261]: 1.32x
                        - img [ref=e262]
                - generic [ref=e266]:
                  - generic [ref=e269]:
                    - button "Open expert opinion for Drake Baldwin" [ref=e270]:
                      - img [ref=e271]
                    - img "Drake Baldwin" [ref=e274]
                  - generic [ref=e275]:
                    - generic [ref=e276]: Drake Baldwin
                    - button "0.5 Hits" [ref=e277]:
                      - generic [ref=e278]:
                        - img [ref=e279]
                        - img [ref=e281]
                      - generic [ref=e283]: "0.5"
                      - generic [ref=e284]: Hits
                    - generic [ref=e285]:
                      - generic [ref=e286]: PHI@ATL
                      - generic [ref=e287]: 8:00PM
                    - generic [ref=e288]:
                      - button "Select over 0.5 Hits for 2.7 times" [ref=e289]:
                        - img [ref=e290]
                        - generic [ref=e292]: 2.7x
                      - button "Select over 0.5 Hits for 1.3 times" [ref=e293]:
                        - generic [ref=e294]: 1.3x
                        - img [ref=e295]
                - generic [ref=e299]:
                  - generic [ref=e302]:
                    - button "Open expert opinion for J.T. Realmuto" [ref=e303]:
                      - img [ref=e304]
                    - img "J.T. Realmuto" [ref=e307]
                  - generic [ref=e308]:
                    - generic [ref=e309]: J.T. Realmuto
                    - button "0.5 Hits" [ref=e310]:
                      - generic [ref=e311]:
                        - img [ref=e312]
                        - img [ref=e314]
                      - generic [ref=e316]: "0.5"
                      - generic [ref=e317]: Hits
                    - generic [ref=e318]:
                      - generic [ref=e319]: PHI@ATL
                      - generic [ref=e320]: 8:00PM
                    - generic [ref=e321]:
                      - button "Select over 0.5 Hits for 2.15 times" [ref=e322]:
                        - img [ref=e323]
                        - img [ref=e327]
                        - generic [ref=e329]: 2.15x
                      - button "Select over 0.5 Hits for 1.53 times" [ref=e330]:
                        - generic [ref=e331]: 1.53x
                        - img [ref=e332]
                - generic [ref=e336]:
                  - generic [ref=e339]:
                    - button "Open expert opinion for Kyle Schwarber" [ref=e340]:
                      - img [ref=e341]
                    - img "Kyle Schwarber" [ref=e344]
                  - generic [ref=e345]:
                    - generic [ref=e346]: K. Schwarber
                    - button "0.5 Hits" [ref=e347]:
                      - generic [ref=e348]:
                        - img [ref=e349]
                        - img [ref=e351]
                      - generic [ref=e353]: "0.5"
                      - generic [ref=e354]: Hits
                    - generic [ref=e355]:
                      - generic [ref=e356]: PHI@ATL
                      - generic [ref=e357]: 8:00PM
                    - generic [ref=e358]:
                      - button "Select over 0.5 Hits for 2.22 times" [ref=e359]:
                        - img [ref=e360]
                        - generic [ref=e362]: 2.22x
                      - button "Select over 0.5 Hits for 1.5 times" [ref=e363]:
                        - generic [ref=e364]: 1.5x
                        - img [ref=e365]
                - generic [ref=e369]:
                  - generic [ref=e372]:
                    - button "Open expert opinion for Bryson Stott" [ref=e373]:
                      - img [ref=e374]
                    - img "Bryson Stott" [ref=e377]
                  - generic [ref=e378]:
                    - generic [ref=e379]: Bryson Stott
                    - button "0.5 Hits" [ref=e380]:
                      - generic [ref=e381]:
                        - img [ref=e382]
                        - img [ref=e384]
                      - generic [ref=e386]: "0.5"
                      - generic [ref=e387]: Hits
                    - generic [ref=e388]:
                      - generic [ref=e389]: PHI@ATL
                      - generic [ref=e390]: 8:00PM
                    - generic [ref=e391]:
                      - button "Select over 0.5 Hits for 2.52 times" [ref=e392]:
                        - img [ref=e393]
                        - generic [ref=e395]: 2.52x
                      - button "Select over 0.5 Hits for 1.38 times" [ref=e396]:
                        - generic [ref=e397]: 1.38x
                        - img [ref=e398]
            - generic [ref=e401]:
              - img [ref=e403]
              - generic [ref=e405]:
                - generic [ref=e407]:
                  - generic [ref=e408]: 6.85x
                  - generic [ref=e409]: 7.19x
                - generic [ref=e410]:
                  - button "+ 10% Boost 🚀" [ref=e416]:
                    - generic [ref=e417]: + 10% Boost 🚀
                  - generic [ref=e427]: "Add 4th Pick: 10% Boost"
              - button "Continue" [ref=e428] [cursor=pointer]
          - generic [ref=e430]:
            - generic [ref=e432]:
              - link "Download ParlayPlay On The Play Store" [ref=e433] [cursor=pointer]:
                - /url: https://parlayplay.onelink.me/oLJk/fh7u6juo
                - img "Download ParlayPlay On The Play Store" [ref=e434]
              - paragraph [ref=e435]:
                - text: Get the app.
                - text: Better. Faster. Convenient
            - navigation [ref=e436]:
              - link "Privacy" [ref=e437] [cursor=pointer]:
                - /url: /privacy-policy
              - link "Fantasy Terms" [ref=e438] [cursor=pointer]:
                - /url: /terms
              - link "Packs Terms" [ref=e439] [cursor=pointer]:
                - /url: /terms/packs
              - link "Responsible Gaming" [ref=e440] [cursor=pointer]:
                - /url: /responsible-gaming
              - link "Gaming Rules" [ref=e441] [cursor=pointer]:
                - /url: /rules
              - link "FAQ" [ref=e442] [cursor=pointer]:
                - /url: https://intercom.help/parlayplay/en/
            - navigation [ref=e443]:
              - generic [ref=e444]:
                - paragraph [ref=e445]: © ParlayPlay 2026
                - generic [ref=e446]:
                  - link "ParlayPlay on Facebook" [ref=e447] [cursor=pointer]:
                    - /url: https://www.facebook.com/parlayplay.io
                    - img [ref=e448]
                  - link "ParlayPlay on Instagram" [ref=e450] [cursor=pointer]:
                    - /url: https://www.instagram.com/parlayplay_?igsh=bHBldWQyMmV2b3Y4
                    - img [ref=e451]
                  - link "ParlayPlay on Twitter" [ref=e453] [cursor=pointer]:
                    - /url: https://www.twitter.com/parlay_play
                    - img [ref=e454]
                  - link "ParlayPlay on Discord" [ref=e456] [cursor=pointer]:
                    - /url: https://discord.com/invite/parlayplay
                    - img [ref=e457]
                - img "18+ icon" [ref=e459]
            - paragraph [ref=e461]
      - contentinfo [ref=e462]:
        - navigation [ref=e463]:
          - list [ref=e464]:
            - listitem [ref=e465]:
              - button "Home" [active] [ref=e466] [cursor=pointer]:
                - generic [ref=e467]:
                  - img [ref=e468]
                  - generic [ref=e469]: Home
            - listitem [ref=e470]:
              - button "Entries 158" [ref=e471] [cursor=pointer]:
                - generic [ref=e472]:
                  - img [ref=e473]
                  - generic [ref=e474]: Entries
                - generic [ref=e475]: "158"
            - listitem [ref=e476]:
              - button "Feed" [ref=e477] [cursor=pointer]:
                - generic [ref=e478]:
                  - img [ref=e479]
                  - generic [ref=e480]: Feed
            - listitem [ref=e481]:
              - button "Rewards 12" [ref=e482] [cursor=pointer]:
                - generic [ref=e483]:
                  - img [ref=e484]
                  - generic [ref=e485]: Rewards
                - generic [ref=e486]: "12"
            - listitem [ref=e487]:
              - button "Packs" [ref=e488] [cursor=pointer]:
                - generic [ref=e489]:
                  - img [ref=e490]
                  - generic [ref=e491]: Packs
    - generic:
      - region "Notifications Alt+T"
  - alert [ref=e492]: ParlayPlay | Fun Fantasy Sports
  - iframe [ref=e493]:
    
```

# Test source

```ts
  382 |         }
  383 |       }
  384 | 
  385 |       if (await this.noPlayerLabel.isVisible().catch(() => false)) {
  386 |         continue;
  387 |       }
  388 | 
  389 |       // Only cards near the viewport carry an id (desktop lazy-loads each card,
  390 |       // mobile virtualises the grid), so a league can look dry after two cards.
  391 |       // Scroll to mount more before moving on, carrying valid picks along.
  392 |       const enumerated = new Set<string>();
  393 |       let leagueExhausted = false;
  394 |       let scrolls = 0;
  395 |       while (!leagueExhausted) {
  396 |         const playerIds = (await this.listVisiblePlayerIds()).filter((id) => !enumerated.has(id));
  397 |         if (playerIds.length === 0) {
  398 |           if (scrolls >= MAX_GRID_SCROLLS || !(await this.scrollGridForMoreCards())) break;
  399 |           scrolls++;
  400 |           continue;
  401 |         }
  402 |         playerIds.forEach((id) => enumerated.add(id));
  403 | 
  404 |         for (const playerId of playerIds) {
  405 |           if (selected.has(playerId) || recentlyFailed.has(playerId) || excluded.has(playerId))
  406 |             continue;
  407 | 
  408 |           if (await this.trySelectPick(this.playerCardById(playerId))) {
  409 |             selected.add(playerId);
  410 |             lastPickId = playerId;
  411 | 
  412 |             let continueFlag = await this.isContinueEnabled();
  413 |             if (selected.size >= count && continueFlag) return Array.from(selected);
  414 | 
  415 |             while (!continueFlag && selected.size == count && lastPickId) {
  416 |               await this.deselectPick(this.playerCardById(lastPickId));
  417 |               selected.delete(lastPickId);
  418 |               recentlyFailed.add(lastPickId);
  419 | 
  420 |               let replaced = false;
  421 |               for (const nextId of playerIds) {
  422 |                 if (selected.has(nextId) || recentlyFailed.has(nextId) || excluded.has(nextId))
  423 |                   continue;
  424 |                 if (await this.trySelectPick(this.playerCardById(nextId))) {
  425 |                   selected.add(nextId);
  426 |                   lastPickId = nextId;
  427 |                   replaced = true;
  428 |                   break;
  429 |                 }
  430 |               }
  431 |               if (!replaced) {
  432 |                 leagueExhausted = true;
  433 |                 break;
  434 |               }
  435 |               continueFlag = await this.isContinueEnabled();
  436 |             }
  437 |             if (leagueExhausted) break;
  438 | 
  439 |             if (continueFlag && selected.size == count) return Array.from(selected);
  440 |             if (continueFlag) recentlyFailed.clear();
  441 |           }
  442 |         }
  443 |       }
  444 |       // League pills sit above the grid; restore their hit area for the next tab.
  445 |       if (scrolls > 0) await this.page.evaluate(() => window.scrollTo(0, 0));
  446 |     }
  447 | 
  448 |     if (selected.size < count) throw new Error(`Could not select ${count} valid picks`);
  449 |     return Array.from(selected);
  450 |   }
  451 | 
  452 |   async pickFivePlayers(): Promise<string[]> {
  453 |     return this.pickPlayers(5);
  454 |   }
  455 | 
  456 |   /**
  457 |    * Reads picks from the slip the app persists via `slipPersistence.saveSlip`
  458 |    * rather than the DOM: when the backend omits a player's main/default
  459 |    * altLine flag the card boots on a fallback line and the highlight isn't
  460 |    * visible even though the pick is persisted.
  461 |    */
  462 |   async getPersistedPickIds(): Promise<string[]> {
  463 |     return this.page.evaluate(() => {
  464 |       const raw = localStorage.getItem('pp_persistent_slip:v1');
  465 |       if (!raw) return [];
  466 |       try {
  467 |         const parsed = JSON.parse(raw);
  468 |         return Object.keys(parsed.selectedPicks ?? {});
  469 |       } catch {
  470 |         return [];
  471 |       }
  472 |     });
  473 |   }
  474 | 
  475 |   async assertPicksPersist(expectedIds: string[], timeout = 10_000): Promise<void> {
  476 |     // Storage holds bare ids ("1089"); pickPlayers returns "player-1089".
  477 |     const normalise = (id: string) => id.replace(/^player-/, '');
  478 |     const expected = new Set(expectedIds.map(normalise));
  479 | 
  480 |     // Auto-save is debounced ~1s and the post-reload restore writes back
  481 |     // asynchronously, so poll.
> 482 |     await expect
      |     ^ Error: Expected persisted picks ["638127","638174","638176"] in localStorage
  483 |       .poll(
  484 |         async () => {
  485 |           const ids = await this.getPersistedPickIds();
  486 |           return Array.from(new Set(ids.map(normalise))).sort();
  487 |         },
  488 |         {
  489 |           timeout,
  490 |           message: `Expected persisted picks ${JSON.stringify(
  491 |             Array.from(expected).sort(),
  492 |           )} in localStorage`,
  493 |         },
  494 |       )
  495 |       .toEqual(Array.from(expected).sort());
  496 |   }
  497 | 
  498 |   async waitForSlipPersisted(expectedPickCount: number, timeout = 5_000): Promise<void> {
  499 |     await expect
  500 |       .poll(
  501 |         async () =>
  502 |           this.page.evaluate(() => {
  503 |             const raw = localStorage.getItem('pp_persistent_slip:v1');
  504 |             if (!raw) return 0;
  505 |             try {
  506 |               return JSON.parse(raw).nrOfPicks ?? 0;
  507 |             } catch {
  508 |               return 0;
  509 |             }
  510 |           }),
  511 |         {
  512 |           timeout,
  513 |           message: `Slip with ${expectedPickCount} picks was never written to localStorage`,
  514 |         },
  515 |       )
  516 |       .toBe(expectedPickCount);
  517 |   }
  518 | 
  519 |   async enterFinalContestPage() {
  520 |     // Desktop already shows the submission form — no Continue hop.
  521 |     if (await this.placePickBtn.isVisible().catch(() => false)) return;
  522 |     await this.continueBtn.click();
  523 |   }
  524 | 
  525 |   async clearSlip(): Promise<void> {
  526 |     await this.page.evaluate(() => localStorage.removeItem('pp_persistent_slip:v1'));
  527 |     await this.page.goto('/');
  528 |     await this.waitForFeedReady();
  529 |   }
  530 | 
  531 |   async selectStatByIndex(idx: number): Promise<void> {
  532 |     const tab = this.statsSelector.locator('li button').nth(idx);
  533 |     await expect(tab).toBeVisible();
  534 |     await tab.click();
  535 |     await this.waitForFeedReady();
  536 |   }
  537 | 
  538 |   async enterEntriesPage() {
  539 |     await this.entriesTab.click();
  540 |   }
  541 | 
  542 |   async enterHomePage(): Promise<void> {
  543 |     await this.homeTab.click();
  544 |     await this.waitForFeedReady();
  545 |     await expect(this.leagueSelector).toBeVisible();
  546 |   }
  547 | 
  548 |   async enterMenu() {
  549 |     // Specs can land here before the header mounts; bounded so a hung locator
  550 |     // fails fast instead of absorbing the 10-min test timeout.
  551 |     await this.toggleMenu.waitFor({ state: 'visible', timeout: 15_000 });
  552 |     await this.toggleMenu.click({ timeout: 15_000 });
  553 |   }
  554 | 
  555 |   async assertHomePage() {
  556 |     await expect(this.leagueSelector).toBeVisible();
  557 |   }
  558 | 
  559 |   async enterRewarsdsPage() {
  560 |     await this.rewardsTab.click();
  561 |   }
  562 | 
  563 |   // Every tab label span carries `border-playYellow`; the active one adds
  564 |   // `border-b-2`, so assert on that class.
  565 |   navIndicator(label: string): Locator {
  566 |     return this.bottomNav.getByRole('button', { name: label }).locator('span.border-playYellow');
  567 |   }
  568 | 
  569 |   async enterFeedPage() {
  570 |     await this.feedTab.click();
  571 |   }
  572 | 
  573 |   // When Packs occupies the fifth footer slot (see packsTab), Free2Play moves
  574 |   // into the burger menu — exactly one of the two placements exists.
  575 |   async enterFree2PlayPage() {
  576 |     if (await this.free2PlayTab.isVisible().catch(() => false)) {
  577 |       await this.free2PlayTab.click();
  578 |       return;
  579 |     }
  580 |     await this.enterMenu();
  581 |     await this.visible(this.page.getByRole('link', { name: 'Free2Play', exact: true })).click();
  582 |   }
```