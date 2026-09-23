# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: slip-persistence/slip-persistence.spec.ts >> Slip persistence - navigation and reload >> Slip persists through a hard page reload
- Location: tests/slip-persistence/slip-persistence.spec.ts:83:5

# Error details

```
Test timeout of 240000ms exceeded.
```

```
Error: locator.getAttribute: Target page, context or browser has been closed
Call log:
  - waiting for locator('button[id^="league-"]').filter({ visible: true }).nth(8)

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
                - link "Rewards 1" [ref=e24] [cursor=pointer]:
                  - /url: /rewards
                  - generic [ref=e25]:
                    - generic [ref=e26]: Rewards
                    - generic [ref=e27]: "1"
              - listitem [ref=e28]:
                - link "Track Picks 150" [ref=e29] [cursor=pointer]:
                  - /url: /challenges/pending
                  - generic [ref=e30]:
                    - generic [ref=e31]: Track Picks
                    - generic [ref=e32]: "150"
            - button "Claim your $100 Deposit Match" [ref=e33] [cursor=pointer]
            - generic [ref=e34]:
              - generic [ref=e37]: $732.48
              - button "Toggle Menu" [ref=e38]:
                - img [ref=e39]
      - main [ref=e41]:
        - generic [ref=e43]:
          - generic [ref=e47]:
            - button "previous slide" [ref=e48] [cursor=pointer]:
              - img [ref=e49]
            - generic [ref=e52]:
              - generic [ref=e54]:
                - generic [ref=e55]:
                  - generic [ref=e56]: Receive a referral Bonus!
                  - generic [ref=e57]: $20
                - generic [ref=e58]:
                  - text: Refer a Friend
                  - text: when they make their first deposit
                  - button "Invite Now" [ref=e60] [cursor=pointer]
              - generic [ref=e62]:
                - generic [ref=e63]:
                  - text: $100
                  - img "black lightning bol" [ref=e64]
                - generic [ref=e66]: =
                - generic [ref=e67]:
                  - text: $200
                  - img "black lightning bol" [ref=e68]
                - generic [ref=e69]:
                  - text: We match your 1st deposit
                  - text: We match your first deposit up to $100.
                  - button "Deposit Now" [ref=e71] [cursor=pointer]
            - button "next slide" [ref=e72] [cursor=pointer]:
              - img [ref=e73]
          - generic [ref=e76]:
            - generic [ref=e78]:
              - generic [ref=e81]:
                - generic:
                  - img
                - textbox "Search player or team" [ref=e82]
              - generic [ref=e83]:
                - button "All" [ref=e84] [cursor=pointer]
                - button "MLB" [ref=e85] [cursor=pointer]
                - button "NHL" [ref=e86] [cursor=pointer]
                - button "WNBA" [ref=e87] [cursor=pointer]
                - button "WNBA H1" [ref=e88] [cursor=pointer]
                - button "WNBA Q1" [ref=e89] [cursor=pointer]
                - button "MLS" [ref=e90] [cursor=pointer]
                - button "UFC" [ref=e91] [cursor=pointer]
              - button "right chevron sign Filter" [ref=e93] [cursor=pointer]:
                - img "right chevron sign" [ref=e94]
                - text: Filter
            - generic [ref=e95]:
              - generic [ref=e98]:
                - generic [ref=e101]:
                  - generic [ref=e102]:
                    - img "Yazmin Jauregui" [ref=e104]
                    - generic [ref=e105]:
                      - generic [ref=e106]: Y. Jauregui
                      - generic [ref=e107]: FI -
                      - generic [ref=e110]: "@ Sep 26th 5:00 PM"
                    - button "Open expert opinion for Yazmin Jauregui" [ref=e111]:
                      - img [ref=e112]
                  - generic [ref=e116]:
                    - generic [ref=e117]:
                      - generic [ref=e118]:
                        - generic [ref=e120] [cursor=pointer]:
                          - text: Less
                          - img [ref=e121]
                        - generic [ref=e123]: Significant Strikes
                        - generic [ref=e125] [cursor=pointer]:
                          - text: More
                          - img [ref=e126]
                      - generic [ref=e129]:
                        - button "Select over 40.5 Significant Strikes for 1.77 times" [ref=e130]: 1.77x
                        - generic [ref=e131]: 40.5 S. STR
                        - button "Select over 40.5 Significant Strikes for 1.77 times" [ref=e132]: 1.77x
                    - generic [ref=e133]:
                      - generic [ref=e134]:
                        - generic [ref=e136] [cursor=pointer]:
                          - text: Less
                          - img [ref=e137]
                        - generic [ref=e139]: Strikes Landed
                        - generic [ref=e141] [cursor=pointer]:
                          - text: More
                          - img [ref=e142]
                      - generic [ref=e145]:
                        - button "Select over 60.5 Strikes Landed for 1.77 times" [ref=e146]: 1.77x
                        - generic [ref=e147]: 60.5 Strikes Landed
                        - button "Select over 60.5 Strikes Landed for 1.77 times" [ref=e148]: 1.77x
                  - button "Show More Stats" [ref=e150]:
                    - img [ref=e151]
                - generic [ref=e155]:
                  - generic [ref=e156]:
                    - img "Mickey Gall" [ref=e158]
                    - generic [ref=e159]:
                      - generic [ref=e160]: Mickey Gall
                      - generic [ref=e161]: FI -
                      - generic [ref=e164]: "@ Sep 26th 5:20 PM"
                    - button "Open expert opinion for Mickey Gall" [ref=e165]:
                      - img [ref=e166]
                  - generic [ref=e170]:
                    - generic [ref=e171]:
                      - generic [ref=e172]:
                        - generic [ref=e174] [cursor=pointer]:
                          - text: Less
                          - img [ref=e175]
                        - generic [ref=e177]: Significant Strikes
                        - generic [ref=e179] [cursor=pointer]:
                          - text: More
                          - img [ref=e180]
                      - generic [ref=e183]:
                        - button "Select over 20.5 Significant Strikes for 1.77 times" [active] [ref=e184]: 1.77x
                        - generic [ref=e185]: 20.5 S. STR
                        - button "Select over 20.5 Significant Strikes for 1.77 times" [ref=e186]: 1.77x
                    - generic [ref=e187]:
                      - generic [ref=e188]:
                        - generic [ref=e190] [cursor=pointer]:
                          - text: Less
                          - img [ref=e191]
                        - generic [ref=e193]: Strikes Landed
                        - generic [ref=e195] [cursor=pointer]:
                          - text: More
                          - img [ref=e196]
                      - generic [ref=e199]:
                        - button "Select over 34.5 Strikes Landed for 1.77 times" [ref=e200]: 1.77x
                        - generic [ref=e201]: 34.5 Strikes Landed
                        - button "Select over 34.5 Strikes Landed for 1.77 times" [ref=e202]: 1.77x
                  - button "Show More Stats" [ref=e204]:
                    - img [ref=e205]
              - generic [ref=e306]:
                - generic [ref=e308]:
                  - generic [ref=e309]: 3.89x
                  - generic [ref=e310]:
                    - button "+ 5% Boost 🚀" [ref=e315]:
                      - generic [ref=e316]: + 5% Boost 🚀
                    - generic [ref=e327]: "Add 3rd Pick: 5% Boost"
                - generic [ref=e329]:
                  - generic [ref=e331]:
                    - generic [ref=e332]:
                      - generic [ref=e334]: "1"
                      - button [ref=e337]:
                        - img [ref=e339]
                      - generic [ref=e341]: 3DMAX - misutaaa
                      - generic [ref=e342]: Today 12:10 PM vs Luminosi
                      - generic [ref=e343]:
                        - button "1.94 x Less 13.5 Map 1 Kills" [disabled] [ref=e345]:
                          - generic [ref=e347]: 1.94 x
                          - generic [ref=e348]: Less
                          - generic [ref=e349]: "13.5"
                          - generic [ref=e350]: Map 1 Kills
                          - img [ref=e353]
                        - button "1.56 x More 13.5 Map 1 Kills" [disabled] [ref=e356]:
                          - generic [ref=e358]: 1.56 x
                          - generic [ref=e359]: More
                          - generic [ref=e360]: "13.5"
                          - generic [ref=e361]: Map 1 Kills
                    - generic:
                      - generic:
                        - img
                        - text: Unavailable
                      - generic: This player is no longer available for this projection.
                    - img "misutaaa" [ref=e364]
                  - generic [ref=e366]:
                    - generic [ref=e367]:
                      - generic [ref=e369]: "2"
                      - button [ref=e372]:
                        - img [ref=e374]
                      - generic [ref=e376]: Luminosity Gaming - Rainwaker
                      - generic [ref=e377]: Today 12:10 PM vs 3DMAX
                      - generic [ref=e378]:
                        - button "2.17 x Less 12.5 Map 1 Kills" [disabled] [ref=e380]:
                          - generic [ref=e382]: 2.17 x
                          - generic [ref=e383]: Less
                          - generic [ref=e384]: "12.5"
                          - generic [ref=e385]: Map 1 Kills
                          - img [ref=e388]
                        - button "1.46 x More 12.5 Map 1 Kills" [disabled] [ref=e391]:
                          - generic [ref=e393]: 1.46 x
                          - generic [ref=e394]: More
                          - generic [ref=e395]: "12.5"
                          - generic [ref=e396]: Map 1 Kills
                    - generic:
                      - generic:
                        - img
                        - text: Unavailable
                      - generic: This player is no longer available for this projection.
                    - img "Rainwaker" [ref=e399]
                  - generic [ref=e401]:
                    - generic [ref=e402]:
                      - generic [ref=e403]:
                        - img [ref=e404]
                        - generic [ref=e406]: "You have 2 unavailable projections:"
                      - generic [ref=e407]: misutaaa is no longer available for this projection.
                    - button "Remove" [ref=e409] [cursor=pointer]
                    - button "Dismiss warning banner" [ref=e410]:
                      - img [ref=e411]
                  - generic [ref=e413]:
                    - generic [ref=e414]:
                      - generic [ref=e416]:
                        - radio "$25"
                        - generic [ref=e417] [cursor=pointer]: $25
                        - radio "$75"
                        - generic [ref=e418] [cursor=pointer]: $75
                        - radio "$300"
                        - generic [ref=e419] [cursor=pointer]: $300
                      - generic [ref=e421]:
                        - generic [ref=e422]: $
                        - spinbutton [ref=e426]: "3"
                      - button [ref=e427] [cursor=pointer]:
                        - img [ref=e428]
                    - generic [ref=e430]:
                      - generic [ref=e431]:
                        - generic [ref=e432]:
                          - button "Insured" [ref=e433]
                          - button "All In" [ref=e434]
                        - generic [ref=e436]: 3.89x
                      - generic [ref=e438]:
                        - generic [ref=e439]:
                          - paragraph [ref=e440]: Perfect line-up
                          - paragraph [ref=e441]: $11.67
                        - generic [ref=e443]:
                          - paragraph [ref=e444]: Or 1st place in group
                          - generic [ref=e445]: $1 + $11.67
                    - generic [ref=e447]:
                      - button "Place" [disabled] [ref=e449]:
                        - text: Place
                        - img [ref=e450]
                      - button "Remove locked picks from your slip" [ref=e452]
          - generic [ref=e455]:
            - generic [ref=e456]:
              - link "Parlay Play Logo" [ref=e457] [cursor=pointer]:
                - /url: /
                - img "Parlay Play Logo" [ref=e459]
              - generic [ref=e460]:
                - generic [ref=e461]: Improve your experience. Download our app.
                - generic [ref=e462]:
                  - link "Apple Store" [ref=e463] [cursor=pointer]:
                    - /url: https://parlayplay.onelink.me/oLJk/gnqpwjha
                    - img "Apple Store" [ref=e464]
                  - link "Google Play Store" [ref=e465] [cursor=pointer]:
                    - /url: https://parlayplay.onelink.me/oLJk/fh7u6juo
                    - img "Google Play Store" [ref=e466]
            - generic [ref=e467]:
              - link "Privacy" [ref=e468] [cursor=pointer]:
                - /url: /privacy-policy
              - link "Fantasy Terms" [ref=e469] [cursor=pointer]:
                - /url: /terms
              - link "Packs Terms" [ref=e470] [cursor=pointer]:
                - /url: /terms/packs
              - link "Responsible Gaming" [ref=e471] [cursor=pointer]:
                - /url: /responsible-gaming
              - link "Gaming Rules" [ref=e472] [cursor=pointer]:
                - /url: /rules
              - link "FAQ" [ref=e473] [cursor=pointer]:
                - /url: https://intercom.help/parlayplay/en/
              - link "Contact Us" [ref=e474] [cursor=pointer]:
                - /url: /
              - paragraph [ref=e475]: © ParlayPlay 2026 - All Rights Reserved
            - list [ref=e476]:
              - listitem [ref=e477]:
                - generic [ref=e478]:
                  - log [ref=e480]
                  - generic [ref=e481]:
                    - generic [ref=e482]:
                      - generic [ref=e483]: 🇺🇸English
                      - combobox "Select language" [ref=e484]
                    - img [ref=e488]
              - listitem [ref=e490]:
                - img "18+-icon" [ref=e491]
              - listitem [ref=e492]:
                - link "ParlayPlay on Twitter" [ref=e493] [cursor=pointer]:
                  - /url: https://twitter.com/parlay_play?lang=en
                  - img [ref=e494]
              - listitem [ref=e496]:
                - link "ParlayPlay on Facebook" [ref=e497] [cursor=pointer]:
                  - /url: https://www.facebook.com/ParlayPlay.io/
                  - img [ref=e498]
              - listitem [ref=e500]:
                - link "ParlayPlay on Instagram" [ref=e501] [cursor=pointer]:
                  - /url: https://www.instagram.com/parlayplay_?igsh=bHBldWQyMmV2b3Y4
                  - img [ref=e502]
              - listitem [ref=e504]:
                - link "ParlayPlay on Discord" [ref=e505] [cursor=pointer]:
                  - /url: https://discord.com/invite/parlayplay
                  - img [ref=e506]
    - generic:
      - region "Notifications Alt+T"
  - alert [ref=e508]
  - iframe [ref=e509]:
    
```

# Test source

```ts
  220 |       await btn.click({ timeout: 10_000 });
  221 |       return;
  222 |     } catch {
  223 |       /* still intercepted — last resort below */
  224 |     }
  225 |     await btn.click({ force: true, timeout: 10_000 });
  226 |   }
  227 | 
  228 |   async listLeagueButtons(): Promise<Locator[]> {
  229 |     const n = await this.leagueButtons.count();
  230 |     const leagueButtonsLocator: Locator[] = [];
  231 |     for (let i = 0; i < n; i++) {
  232 |       leagueButtonsLocator.push(this.leagueButtons.nth(i));
  233 |     }
  234 |     return leagueButtonsLocator;
  235 |   }
  236 | 
  237 |   /**
  238 |    * "Is the slip valid?" oracle for pickPlayers. Mobile: the Continue button.
  239 |    * Desktop has no Continue — the persistent panel mounts `#place-pick` once
  240 |    * the slip is playable and shows the "Let's Start" box otherwise.
  241 |    */
  242 |   async isContinueEnabled(): Promise<boolean> {
  243 |     if (await this.continueBtn.isVisible().catch(() => false)) {
  244 |       return this.continueBtn.isEnabled().catch(() => false);
  245 |     }
  246 |     if (await this.placePickBtn.isVisible().catch(() => false)) {
  247 |       // Payout/metadata loading briefly disables place-pick right after a
  248 |       // pick lands — give that a moment before reading the slip as invalid.
  249 |       return expect(this.placePickBtn)
  250 |         .toBeEnabled({ timeout: 3_000 })
  251 |         .then(
  252 |           () => true,
  253 |           () => false,
  254 |         );
  255 |     }
  256 |     return false;
  257 |   }
  258 | 
  259 |   async trySelectPick(card: Locator): Promise<boolean> {
  260 |     const buttons = this.pickButtons(card);
  261 |     const lessButton = buttons.first();
  262 |     // Filter updates run in useTransition and the grid is virtualised, so a
  263 |     // card from listVisiblePlayerIds can unmount before we act on it. With no
  264 |     // actionTimeout configured that would hang — treat "gone" as unpickable.
  265 |     let isEnabled: boolean;
  266 |     try {
  267 |       isEnabled = await lessButton.isEnabled({ timeout: 5000 });
  268 |     } catch {
  269 |       return false;
  270 |     }
  271 | 
  272 |     try {
  273 |       await buttons.nth(isEnabled ? 0 : 1).click({ timeout: 10_000 });
  274 |     } catch {
  275 |       return false;
  276 |     }
  277 | 
  278 |     try {
  279 |       const modal = this.warningModal;
  280 |       if (await modal.isVisible({ timeout: 2000 }).catch(() => false)) {
  281 |         await modal.getByRole('button', { name: 'Understood' }).click();
  282 |         return false;
  283 |       }
  284 |     } catch {
  285 |       /* modal probe failed — treat as no modal */
  286 |     }
  287 |     return true;
  288 |   }
  289 | 
  290 |   async deselectPick(card: Locator): Promise<void> {
  291 |     const buttons = this.pickButtons(card);
  292 |     const count = await buttons.count();
  293 | 
  294 |     for (let i = 0; i < count; i++) {
  295 |       const btn = buttons.nth(i);
  296 |       const classes = (await btn.getAttribute('class')) ?? '';
  297 |       if (classes.includes('bg-playYellow')) {
  298 |         await btn.click();
  299 |         return;
  300 |       }
  301 |     }
  302 |     throw new Error('No selected button found with bg-yellow class.');
  303 |   }
  304 | 
  305 |   /**
  306 |    * `excludeIds`: retries (e.g. after "multiple promos cannot be applied")
  307 |    * pass the failed slip's players so the deterministic pick order doesn't
  308 |    * re-select the same promo-bearing cards.
  309 |    */
  310 |   async pickPlayers(count: number, statIdx?: number, excludeIds?: Set<string>): Promise<string[]> {
  311 |     const leagueButtons = await this.listLeagueButtons();
  312 | 
  313 |     const selected = new Set<string>();
  314 |     let lastPickId: string | null = null;
  315 |     // Kept separate from recentlyFailed (cleared once a valid combo is found)
  316 |     // so retries never re-pick a player a prior attempt already tried.
  317 |     const excluded = new Set<string>(excludeIds ?? []);
  318 |     const recentlyFailed = new Set<string>();
  319 |     for (const leagueButton of leagueButtons) {
> 320 |       const leagueId = (await leagueButton.getAttribute('id')) ?? '';
      |                                            ^ Error: locator.getAttribute: Target page, context or browser has been closed
  321 |       // Every card in the Combo and Promo leagues carries a promo, so picking
  322 |       // >1 always trips "multiple promos cannot be applied" and re-picking
  323 |       // never escapes it.
  324 |       const lid = leagueId.toLowerCase();
  325 |       if (lid.includes('combo') || lid.includes('promo')) continue;
  326 | 
  327 |       await this.clickLeagueTab(leagueButton);
  328 |       await this.waitForPlayersGrid();
  329 | 
  330 |       // Each league resets to its default stat tab on click.
  331 |       if (statIdx !== undefined) {
  332 |         const statTab = this.statsSelector.locator('li button').nth(statIdx);
  333 |         if (await statTab.isVisible().catch(() => false)) {
  334 |           await statTab.click();
  335 |           await this.waitForPlayersGrid();
  336 |         }
  337 |       }
  338 | 
  339 |       if (await this.noPlayerLabel.isVisible().catch(() => false)) {
  340 |         continue;
  341 |       }
  342 | 
  343 |       const playerIds = await this.listVisiblePlayerIds();
  344 |       // The virtualised grid mounts only a handful of cards on desktop, so a
  345 |       // small league can run dry with valid picks still selected — carry them
  346 |       // into the next league instead of aborting.
  347 |       let leagueExhausted = false;
  348 |       for (const playerId of playerIds) {
  349 |         if (selected.has(playerId) || recentlyFailed.has(playerId) || excluded.has(playerId))
  350 |           continue;
  351 | 
  352 |         if (await this.trySelectPick(this.playerCardById(playerId))) {
  353 |           selected.add(playerId);
  354 |           lastPickId = playerId;
  355 | 
  356 |           let continueFlag = await this.isContinueEnabled();
  357 |           if (selected.size >= count && continueFlag) return Array.from(selected);
  358 | 
  359 |           while (!continueFlag && selected.size == count && lastPickId) {
  360 |             await this.deselectPick(this.playerCardById(lastPickId));
  361 |             selected.delete(lastPickId);
  362 |             recentlyFailed.add(lastPickId);
  363 | 
  364 |             let replaced = false;
  365 |             for (const nextId of playerIds) {
  366 |               if (selected.has(nextId) || recentlyFailed.has(nextId) || excluded.has(nextId))
  367 |                 continue;
  368 |               if (await this.trySelectPick(this.playerCardById(nextId))) {
  369 |                 selected.add(nextId);
  370 |                 lastPickId = nextId;
  371 |                 replaced = true;
  372 |                 break;
  373 |               }
  374 |             }
  375 |             if (!replaced) {
  376 |               leagueExhausted = true;
  377 |               break;
  378 |             }
  379 |             continueFlag = await this.isContinueEnabled();
  380 |           }
  381 |           if (leagueExhausted) break;
  382 | 
  383 |           if (continueFlag && selected.size == count) return Array.from(selected);
  384 |           if (continueFlag) recentlyFailed.clear();
  385 |         }
  386 |       }
  387 |     }
  388 | 
  389 |     if (selected.size < count) throw new Error(`Could not select ${count} valid picks`);
  390 |     return Array.from(selected);
  391 |   }
  392 | 
  393 |   async pickFivePlayers(): Promise<string[]> {
  394 |     return this.pickPlayers(5);
  395 |   }
  396 | 
  397 |   /**
  398 |    * Reads picks from the slip the app persists via `slipPersistence.saveSlip`
  399 |    * rather than the DOM: when the backend omits a player's main/default
  400 |    * altLine flag the card boots on a fallback line and the highlight isn't
  401 |    * visible even though the pick is persisted.
  402 |    */
  403 |   async getPersistedPickIds(): Promise<string[]> {
  404 |     return this.page.evaluate(() => {
  405 |       const raw = localStorage.getItem('pp_persistent_slip:v1');
  406 |       if (!raw) return [];
  407 |       try {
  408 |         const parsed = JSON.parse(raw);
  409 |         return Object.keys(parsed.selectedPicks ?? {});
  410 |       } catch {
  411 |         return [];
  412 |       }
  413 |     });
  414 |   }
  415 | 
  416 |   async assertPicksPersist(expectedIds: string[], timeout = 10_000): Promise<void> {
  417 |     // Storage holds bare ids ("1089"); pickPlayers returns "player-1089".
  418 |     const normalise = (id: string) => id.replace(/^player-/, '');
  419 |     const expected = new Set(expectedIds.map(normalise));
  420 | 
```