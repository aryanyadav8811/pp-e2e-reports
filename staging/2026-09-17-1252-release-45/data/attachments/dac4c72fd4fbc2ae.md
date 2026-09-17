# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: entries/entry-card.spec.ts >> My Entries - cancel entry >> Fresh entry shows a live cancel countdown and confirming Cancel Entry removes it everywhere
- Location: tests/entries/entry-card.spec.ts:261:5

# Error details

```
Error: No selected button found with bg-yellow class.
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
              - generic [ref=e13]: $693.00
              - generic [ref=e14]:
                - img "gift-icon" [ref=e15]
                - text: "17.00"
            - button "Toggle Menu" [ref=e16]:
              - img [ref=e17]
      - main [ref=e19]:
        - generic [ref=e24]:
          - generic [ref=e25]:
            - generic [ref=e26]:
              - list [ref=e28]:
                - button "MLB" [ref=e29] [cursor=pointer]
                - button "NHL" [ref=e30] [cursor=pointer]
                - button "SerieA" [ref=e31] [cursor=pointer]
                - button "EPL" [ref=e32] [cursor=pointer]
                - button "CSGO" [ref=e33] [cursor=pointer]
                - button "CSGO MAP1" [ref=e34] [cursor=pointer]
                - button "WNBA" [ref=e35] [cursor=pointer]
                - button "WNBA-Combos" [ref=e36] [cursor=pointer]
                - button "WNBA H1" [ref=e37] [cursor=pointer]
                - button "WNBA Q1" [ref=e38] [cursor=pointer]
                - button "MLS" [ref=e39] [cursor=pointer]
                - button "LaLiga" [ref=e40] [cursor=pointer]
                - button "UFC" [ref=e41] [cursor=pointer]
                - button "Bundes" [ref=e42] [cursor=pointer]
              - list [ref=e44]:
                - listitem [ref=e45]:
                  - button "ALL" [ref=e46] [cursor=pointer]:
                    - generic [ref=e47]: ALL
                - listitem [ref=e48]:
                  - button "TOR@BOL Sat 9AM" [ref=e49] [cursor=pointer]:
                    - text: TOR@BOL
                    - generic [ref=e50]: Sat 9AM
                - listitem [ref=e51]:
                  - button "INT@ROM Sat 12PM" [ref=e52] [cursor=pointer]:
                    - text: INT@ROM
                    - generic [ref=e53]: Sat 12PM
                - listitem [ref=e54]:
                  - button "LAZ@VEN Sat 2PM" [ref=e55] [cursor=pointer]:
                    - text: LAZ@VEN
                    - generic [ref=e56]: Sat 2PM
                - listitem [ref=e57]:
                  - button "NAP@FIO Sun 6AM" [ref=e58] [cursor=pointer]:
                    - text: NAP@FIO
                    - generic [ref=e59]: Sun 6AM
                - listitem [ref=e60]:
                  - button "GEN@PAR Sun 9AM" [ref=e61] [cursor=pointer]:
                    - text: GEN@PAR
                    - generic [ref=e62]: Sun 9AM
                - listitem [ref=e63]:
                  - button "ATA@JUV Sun 12PM" [ref=e64] [cursor=pointer]:
                    - text: ATA@JUV
                    - generic [ref=e65]: Sun 12PM
              - generic [ref=e66]:
                - generic [ref=e67]:
                  - generic [ref=e70]:
                    - generic:
                      - img
                    - textbox "Search player or team" [ref=e71]
                  - button "Change card style from grid" [ref=e73]
                - list [ref=e75]:
                  - listitem [ref=e76]:
                    - button "Shots" [ref=e77]
                  - listitem [ref=e78]:
                    - button "Goals" [ref=e79]
                  - listitem [ref=e80]:
                    - button "Shots on Goal" [ref=e81]
                  - listitem [ref=e82]:
                    - button "Assists" [ref=e83]
                  - listitem [ref=e84]:
                    - button "Gls + Ast" [ref=e85]
                  - listitem [ref=e86]:
                    - button "Fouls Drawn" [ref=e87]
                  - listitem [ref=e88]:
                    - button "Fouls Committed" [ref=e89]
            - generic [ref=e90]:
              - generic [ref=e95]:
                - generic [ref=e99] [cursor=pointer]:
                  - generic [ref=e100]: Pull real graded cards worth up to $10,000
                  - generic [ref=e101]: Sell or ship instantly
                  - button "Rip a pack" [ref=e102]:
                    - generic [ref=e103]:
                      - img [ref=e104]
                      - text: Rip a pack
                - generic [ref=e109] [cursor=pointer]:
                  - generic [ref=e110]:
                    - generic [ref=e111]: Refer a friend, get a $20 Free Entry
                    - generic [ref=e112]: Referral bonus
                  - button "Refer" [ref=e113]
                - generic [ref=e116] [cursor=pointer]:
                  - generic [ref=e117]:
                    - generic [ref=e118]:
                      - img [ref=e119]
                      - generic [ref=e123]: Boosted Picks
                    - generic [ref=e124]: "Every Pick Pays: Up to a 35% Boost!"
                  - button "Details" [ref=e126]
                - generic [ref=e129] [cursor=pointer]:
                  - generic [ref=e130]:
                    - generic [ref=e131]:
                      - generic [ref=e132]: 100%
                      - generic [ref=e133]: Deposit Match
                    - generic [ref=e134]: New User Promotion
                  - button "Deposit" [ref=e136]
              - generic [ref=e140]:
                - generic [ref=e143]:
                  - generic [ref=e146]:
                    - button "Open expert opinion for Jens Odgaard" [ref=e147]:
                      - img [ref=e148]
                    - img "Jens Odgaard" [ref=e151]
                  - generic [ref=e152]:
                    - generic [ref=e153]: Jens Odgaard
                    - button "2.5 Shots" [ref=e154]:
                      - generic [ref=e155]:
                        - img [ref=e156]
                        - img [ref=e158]
                      - generic [ref=e160]: "2.5"
                      - generic [ref=e161]: Shots
                    - generic [ref=e162]:
                      - generic [ref=e163]: TOR@BOL
                      - generic [ref=e164]: Sat 9AM
                    - generic [ref=e165]:
                      - button "Select over 2.5 Shots for 0 times" [disabled] [ref=e166]
                      - button "Select over 2.5 Shots for 1.51 times" [active] [ref=e168]:
                        - generic [ref=e169]: 1.51x
                        - img [ref=e170]
                - generic [ref=e174]:
                  - generic [ref=e177]:
                    - button "Open expert opinion for Riccardo Orsolini" [ref=e178]:
                      - img [ref=e179]
                    - img "Riccardo Orsolini" [ref=e182]
                  - generic [ref=e183]:
                    - generic [ref=e184]: R. Orsolini
                    - button "3.5 Shots" [ref=e185]:
                      - generic [ref=e186]:
                        - img [ref=e187]
                        - img [ref=e189]
                      - generic [ref=e191]: "3.5"
                      - generic [ref=e192]: Shots
                    - generic [ref=e193]:
                      - generic [ref=e194]: TOR@BOL
                      - generic [ref=e195]: Sat 9AM
                    - generic [ref=e196]:
                      - button "Select over 3.5 Shots for 0 times" [disabled] [ref=e197]
                      - button "Select over 3.5 Shots for 1.55 times" [ref=e199]:
                        - generic [ref=e200]: 1.55x
                        - img [ref=e201]
                - generic [ref=e205]:
                  - generic [ref=e208]:
                    - button "Open expert opinion for Tommaso Pobega" [ref=e209]:
                      - img [ref=e210]
                    - img "Tommaso Pobega" [ref=e213]
                  - generic [ref=e214]:
                    - generic [ref=e215]: T. Pobega
                    - button "1.5 Shots" [ref=e216]:
                      - generic [ref=e217]:
                        - img [ref=e218]
                        - img [ref=e220]
                      - generic [ref=e222]: "1.5"
                      - generic [ref=e223]: Shots
                    - generic [ref=e224]:
                      - generic [ref=e225]: TOR@BOL
                      - generic [ref=e226]: Sat 9AM
                    - generic [ref=e227]:
                      - button "Select over 1.5 Shots for 0 times" [disabled] [ref=e228]
                      - button "Select over 1.5 Shots for 1.35 times" [ref=e230]:
                        - generic [ref=e231]: 1.35x
                        - img [ref=e232]
                - generic [ref=e236]:
                  - generic [ref=e239]:
                    - button "Open expert opinion for Martin Vitík" [ref=e240]:
                      - img [ref=e241]
                    - img "Martin Vitík" [ref=e244]
                  - generic [ref=e245]:
                    - generic [ref=e246]: Martin Vitík
                    - button "0.5 Shots" [ref=e247]:
                      - generic [ref=e248]:
                        - img [ref=e249]
                        - img [ref=e251]
                      - generic [ref=e253]: "0.5"
                      - generic [ref=e254]: Shots
                    - generic [ref=e255]:
                      - generic [ref=e256]: TOR@BOL
                      - generic [ref=e257]: Sat 9AM
                    - generic [ref=e258]:
                      - button "Select over 0.5 Shots for 0 times" [disabled] [ref=e259]
                      - button "Select over 0.5 Shots for 1.45 times" [ref=e261]:
                        - generic [ref=e262]: 1.45x
                        - img [ref=e263]
                - generic [ref=e267]:
                  - generic [ref=e270]:
                    - button "Open expert opinion for Juan Miranda González" [ref=e271]:
                      - img [ref=e272]
                    - img "Juan Miranda González" [ref=e275]
                  - generic [ref=e276]:
                    - generic [ref=e277]: J. Miranda González
                    - button "0.5 Shots" [ref=e278]:
                      - generic [ref=e279]:
                        - img [ref=e280]
                        - img [ref=e282]
                      - generic [ref=e284]: "0.5"
                      - generic [ref=e285]: Shots
                    - generic [ref=e286]:
                      - generic [ref=e287]: TOR@BOL
                      - generic [ref=e288]: Sat 9AM
                    - generic [ref=e289]:
                      - button "Select over 0.5 Shots for 0 times" [disabled] [ref=e290]
                      - button "Select over 0.5 Shots for 1.88 times" [ref=e292]:
                        - generic [ref=e293]: 1.88x
                        - img [ref=e294]
                - generic [ref=e298]:
                  - generic [ref=e301]:
                    - button "Open expert opinion for Francesco Pio Esposito" [ref=e302]:
                      - img [ref=e303]
                    - img "Francesco Pio Esposito" [ref=e306]
                  - generic [ref=e307]:
                    - generic [ref=e308]: F. Esposito
                    - button "2.5 Shots" [ref=e309]:
                      - generic [ref=e310]:
                        - img [ref=e311]
                        - img [ref=e313]
                      - generic [ref=e315]: "2.5"
                      - generic [ref=e316]: Shots
                    - generic [ref=e317]:
                      - generic [ref=e318]: INT@ROM
                      - generic [ref=e319]: Sat 12PM
                    - generic [ref=e320]:
                      - button "Select over 2.5 Shots for 0 times" [disabled] [ref=e321]
                      - button "Select over 2.5 Shots for 1.68 times" [ref=e323]:
                        - generic [ref=e324]: 1.68x
                        - img [ref=e325]
                - generic [ref=e329]:
                  - generic [ref=e332]:
                    - button "Open expert opinion for Luis Henrique Tomaz de Lima" [ref=e333]:
                      - img [ref=e334]
                    - img "Luis Henrique Tomaz de Lima" [ref=e337]
                  - generic [ref=e338]:
                    - generic [ref=e339]: L. Tomaz de Lima
                    - button "0.5 Shots" [ref=e340]:
                      - generic [ref=e341]:
                        - img [ref=e342]
                        - img [ref=e344]
                      - generic [ref=e346]: "0.5"
                      - generic [ref=e347]: Shots
                    - generic [ref=e348]:
                      - generic [ref=e349]: INT@ROM
                      - generic [ref=e350]: Sat 12PM
                    - generic [ref=e351]:
                      - button "Select over 0.5 Shots for 0 times" [disabled] [ref=e352]
                      - button "Select over 0.5 Shots for 1.19 times" [ref=e354]:
                        - generic [ref=e355]: 1.19x
                        - img [ref=e356]
                - generic [ref=e360]:
                  - generic [ref=e363]:
                    - button "Open expert opinion for Nicolò Barella" [ref=e364]:
                      - img [ref=e365]
                    - img "Nicolò Barella" [ref=e368]
                  - generic [ref=e369]:
                    - generic [ref=e370]: N. Barella
                    - button "0.5 Shots" [ref=e371]:
                      - generic [ref=e372]:
                        - img [ref=e373]
                        - img [ref=e375]
                      - generic [ref=e377]: "0.5"
                      - generic [ref=e378]: Shots
                    - generic [ref=e379]:
                      - generic [ref=e380]: INT@ROM
                      - generic [ref=e381]: Sat 12PM
                    - generic [ref=e382]:
                      - button "Select over 0.5 Shots for 0 times" [disabled] [ref=e383]
                      - button "Select over 0.5 Shots for 1.25 times" [ref=e385]:
                        - generic [ref=e386]: 1.25x
                        - img [ref=e387]
          - generic [ref=e390]:
            - generic [ref=e392]:
              - link "Download ParlayPlay On The App Store" [ref=e393]:
                - /url: https://parlayplay.onelink.me/oLJk/gnqpwjha
                - img "Download ParlayPlay On The App Store" [ref=e394]
              - paragraph [ref=e395]:
                - text: Get the app.
                - text: Better. Faster. Convenient
            - navigation [ref=e396]:
              - link "Privacy" [ref=e397]:
                - /url: /privacy-policy
              - link "Fantasy Terms" [ref=e398]:
                - /url: /terms
              - link "Packs Terms" [ref=e399]:
                - /url: /terms/packs
              - link "Responsible Gaming" [ref=e400]:
                - /url: /responsible-gaming
              - link "Gaming Rules" [ref=e401]:
                - /url: /rules
              - link "FAQ" [ref=e402]:
                - /url: https://intercom.help/parlayplay/en/
            - navigation [ref=e403]:
              - generic [ref=e404]:
                - paragraph [ref=e405]: © ParlayPlay 2026
                - generic [ref=e406]:
                  - link "ParlayPlay on Facebook" [ref=e407]:
                    - /url: https://www.facebook.com/parlayplay.io
                    - img [ref=e408]
                  - link "ParlayPlay on Instagram" [ref=e410]:
                    - /url: https://www.instagram.com/parlayplay_?igsh=bHBldWQyMmV2b3Y4
                    - img [ref=e411]
                  - link "ParlayPlay on Twitter" [ref=e413]:
                    - /url: https://www.twitter.com/parlay_play
                    - img [ref=e414]
                  - link "ParlayPlay on Discord" [ref=e416]:
                    - /url: https://discord.com/invite/parlayplay
                    - img [ref=e417]
                - img "18+ icon" [ref=e419]
            - paragraph [ref=e421]
      - contentinfo [ref=e422]:
        - navigation [ref=e423]:
          - list [ref=e424]:
            - listitem [ref=e425]:
              - button "Home" [ref=e426] [cursor=pointer]:
                - generic [ref=e427]:
                  - img [ref=e428]
                  - generic [ref=e429]: Home
            - listitem [ref=e430]:
              - button "Entries 104" [ref=e431] [cursor=pointer]:
                - generic [ref=e432]:
                  - img [ref=e433]
                  - generic [ref=e434]: Entries
                - generic [ref=e435]: "104"
            - listitem [ref=e436]:
              - button "Feed" [ref=e437] [cursor=pointer]:
                - generic [ref=e438]:
                  - img [ref=e439]
                  - generic [ref=e440]: Feed
            - listitem [ref=e441]:
              - button "Rewards 18" [ref=e442] [cursor=pointer]:
                - generic [ref=e443]:
                  - img [ref=e444]
                  - generic [ref=e445]: Rewards
                - generic [ref=e446]: "18"
            - listitem [ref=e447]:
              - button "Packs" [ref=e448] [cursor=pointer]:
                - generic [ref=e449]:
                  - img [ref=e450]
                  - generic [ref=e451]: Packs
    - generic:
      - region "Notifications Alt+T"
  - alert [ref=e452]
```

# Test source

```ts
  202 |   async getLeagueCount(): Promise<number> {
  203 |     return await this.leagueButtons.count();
  204 |   }
  205 | 
  206 |   /**
  207 |    * WebKit occasionally leaves a card image overlapping the league pill row
  208 |    * after submit → home, and an unbounded click retries against it until the
  209 |    * test times out. Scrolling to the top restores the row's hit area.
  210 |    */
  211 |   async clickLeagueTab(btn: Locator): Promise<void> {
  212 |     try {
  213 |       await btn.click({ timeout: 10_000 });
  214 |       return;
  215 |     } catch {
  216 |       /* intercepted — try to restore the layout */
  217 |     }
  218 |     await this.page.evaluate(() => window.scrollTo(0, 0));
  219 |     try {
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
> 302 |     throw new Error('No selected button found with bg-yellow class.');
      |           ^ Error: No selected button found with bg-yellow class.
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
  320 |       const leagueId = (await leagueButton.getAttribute('id')) ?? '';
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
```