# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: contests/user-enter-contest.spec.ts >> User Enter Contest >> Five player contest Submission @smoke
- Location: tests/contests/user-enter-contest.spec.ts:18:5

# Error details

```
Test timeout of 120000ms exceeded.
```

```
Error: locator.click: Target page, context or browser has been closed
Call log:
  - waiting for getByTestId('league-selector').locator('>button').first()
    - locator resolved to <button type="button" id="league-MLB" class="py-2 px-4 font-thin text-sm text-white  bg-black  rounded-full  flex-row justify-center items-center whitespace-nowrap text-sm bg-opacity-100 border border-black mr-2 cursor-pointer">…</button>
  - attempting click action
    2 × waiting for element to be visible, enabled and stable
      - element is visible, enabled and stable
      - scrolling into view if needed
      - done scrolling
      - <nextjs-portal></nextjs-portal> intercepts pointer events
    - retrying click action
    - waiting 20ms
    2 × waiting for element to be visible, enabled and stable
      - element is visible, enabled and stable
      - scrolling into view if needed
      - done scrolling
      - <nextjs-portal></nextjs-portal> intercepts pointer events
    - retrying click action
      - waiting 100ms
    196 × waiting for element to be visible, enabled and stable
        - element is visible, enabled and stable
        - scrolling into view if needed
        - done scrolling
        - <nextjs-portal></nextjs-portal> intercepts pointer events
      - retrying click action
        - waiting 500ms
    - waiting for element to be visible, enabled and stable
    - element is visible, enabled and stable
    - scrolling into view if needed
    - done scrolling

```

# Page snapshot

```yaml
- generic [ref=e1]:
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
              - generic [ref=e17]: $649.13
              - button "Toggle Menu" [ref=e18]:
                - img [ref=e19]
      - main [ref=e21]:
        - generic [ref=e24]:
          - generic [ref=e25]:
            - generic [ref=e26]:
              - list [ref=e28]:
                - button "MLB" [ref=e29] [cursor=pointer]
                - button "NBA" [ref=e30] [cursor=pointer]
                - button "NBA-Combos" [ref=e31] [cursor=pointer]
                - button "NBA Q1" [ref=e32] [cursor=pointer]
                - button "NBA H1" [ref=e33] [cursor=pointer]
                - button "NHL" [ref=e34] [cursor=pointer]
                - button "NHL-Combos" [ref=e35] [cursor=pointer]
                - button "WNBA" [ref=e36] [cursor=pointer]
                - button "WNBA-Combos" [ref=e37] [cursor=pointer]
                - button "WNBA Q1" [ref=e38] [cursor=pointer]
                - button "WNBA H1" [ref=e39] [cursor=pointer]
                - button "Cricket" [ref=e40] [cursor=pointer]
              - list [ref=e42]:
                - listitem [ref=e43]:
                  - button "ALL" [ref=e44] [cursor=pointer]:
                    - generic [ref=e45]: ALL
                - listitem [ref=e46]:
                  - button "SF@LAD 10:10PM" [ref=e47] [cursor=pointer]:
                    - text: SF@LAD
                    - generic [ref=e48]: 10:10PM
                - listitem [ref=e49]:
                  - button "PHI@BOS 6:45PM" [ref=e50] [cursor=pointer]:
                    - text: PHI@BOS
                    - generic [ref=e51]: 6:45PM
                - listitem [ref=e52]:
                  - button "CHC@ATL 7:15PM" [ref=e53] [cursor=pointer]:
                    - text: CHC@ATL
                    - generic [ref=e54]: 7:15PM
              - generic [ref=e55]:
                - generic [ref=e56]:
                  - generic [ref=e59]:
                    - img [ref=e61]
                    - textbox "Search player or team" [ref=e63]
                  - button "Change card style from grid" [ref=e65]
                - list [ref=e67]:
                  - listitem [ref=e68]:
                    - button "Hits" [ref=e69]
                  - listitem [ref=e70]:
                    - button "Hits + Runs + RBIs" [ref=e71]
                  - listitem [ref=e72]:
                    - button "Singles" [ref=e73]
                  - listitem [ref=e74]:
                    - button "Doubles" [ref=e75]
                  - listitem [ref=e76]:
                    - button "Triples" [ref=e77]
                  - listitem [ref=e78]:
                    - button "Runs" [ref=e79]
                  - listitem [ref=e80]:
                    - button "RBIs" [ref=e81]
                  - listitem [ref=e82]:
                    - button "Homeruns" [ref=e83]
                  - listitem [ref=e84]:
                    - button "Total Bases" [ref=e85]
                  - listitem [ref=e86]:
                    - button "Strikeouts" [ref=e87]
                  - listitem [ref=e88]:
                    - button "Fantasy Points" [ref=e89]
            - generic [ref=e90]:
              - generic [ref=e94]:
                - button "previous slide / item" [ref=e95] [cursor=pointer]:
                  - img [ref=e96]
                - list [ref=e99]:
                  - listitem [ref=e100]:
                    - link "Win or Lose! Earn SpinPals Coins with Every Entry! SpinPals" [ref=e101] [cursor=pointer]:
                      - /url: https://www.spinpals.com/
                      - generic [ref=e103]:
                        - generic [ref=e105]: Win or Lose!
                        - generic [ref=e106]: Earn SpinPals Coins with Every Entry!
                      - generic [ref=e107]:
                        - img "SpinPals"
                  - listitem [ref=e108]:
                    - 'button "Boosted Picks 🚀 Every Pick Pays: Up to a 35% Boost! lightning-bolt-yellow" [ref=e109] [cursor=pointer]':
                      - generic [ref=e110]:
                        - generic [ref=e112]: Boosted Picks 🚀
                        - generic [ref=e113]: "Every Pick Pays: Up to a 35% Boost!"
                      - img "lightning-bolt-yellow"
                  - listitem [ref=e114]:
                    - button "Get $20 By referring a friend making a first $10 deposit. lightning-bolt-yellow" [ref=e115] [cursor=pointer]:
                      - generic [ref=e116]:
                        - generic [ref=e118]: Get $20
                        - generic [ref=e119]: By referring a friend making a first $10 deposit.
                      - img "lightning-bolt-yellow"
                  - listitem [ref=e120]:
                    - link "Win or Lose! Earn SpinPals Coins with Every Entry! SpinPals" [ref=e121] [cursor=pointer]:
                      - /url: https://www.spinpals.com/
                      - generic [ref=e123]:
                        - generic [ref=e125]: Win or Lose!
                        - generic [ref=e126]: Earn SpinPals Coins with Every Entry!
                      - generic [ref=e127]:
                        - img "SpinPals"
                  - listitem [ref=e128]:
                    - 'button "Boosted Picks 🚀 Every Pick Pays: Up to a 35% Boost! lightning-bolt-yellow" [ref=e129] [cursor=pointer]':
                      - generic [ref=e130]:
                        - generic [ref=e132]: Boosted Picks 🚀
                        - generic [ref=e133]: "Every Pick Pays: Up to a 35% Boost!"
                      - img "lightning-bolt-yellow"
                - button "next slide / item" [ref=e134] [cursor=pointer]:
                  - img [ref=e135]
              - generic [ref=e137]:
                - generic [ref=e140]:
                  - generic [ref=e143]:
                    - button "Open expert opinion for Ceddanne Rafaela" [ref=e144]:
                      - img [ref=e145]
                    - img "Ceddanne Rafaela" [ref=e148]
                  - generic [ref=e149]:
                    - generic [ref=e150]: C. Rafaela
                    - button "0.5 Hits" [ref=e151]:
                      - generic [ref=e152]:
                        - img [ref=e153]
                        - img [ref=e155]
                      - generic [ref=e157]: "0.5"
                      - generic [ref=e158]: Hits
                    - generic [ref=e159]:
                      - generic [ref=e160]: PHI@BOS
                      - generic [ref=e161]: 6:45PM
                    - generic [ref=e162]:
                      - button "Select over 0.5 Hits for 2.17 times" [ref=e163]:
                        - img [ref=e164]
                        - generic [ref=e166]: 2.17x
                      - button "Select over 0.5 Hits for 1.5 times" [ref=e167]:
                        - generic [ref=e168]: 1.5x
                        - img [ref=e169]
                - generic [ref=e173]:
                  - generic [ref=e176]:
                    - button "Open expert opinion for Jarren Duran" [ref=e177]:
                      - img [ref=e178]
                    - img "Jarren Duran" [ref=e181]
                  - generic [ref=e182]:
                    - generic [ref=e183]: Jarren Duran
                    - button "0.5 Hits" [ref=e184]:
                      - generic [ref=e185]:
                        - img [ref=e186]
                        - img [ref=e188]
                      - generic [ref=e190]: "0.5"
                      - generic [ref=e191]: Hits
                    - generic [ref=e192]:
                      - generic [ref=e193]: PHI@BOS
                      - generic [ref=e194]: 6:45PM
                    - generic [ref=e195]:
                      - button "Select over 0.5 Hits for 2.34 times" [ref=e196]:
                        - img [ref=e197]
                        - generic [ref=e199]: 2.34x
                      - button "Select over 0.5 Hits for 1.44 times" [ref=e200]:
                        - generic [ref=e201]: 1.44x
                        - img [ref=e202]
                - generic [ref=e206]:
                  - generic [ref=e209]:
                    - button "Open expert opinion for Trevor Story" [ref=e210]:
                      - img [ref=e211]
                    - img "Trevor Story" [ref=e214]
                  - generic [ref=e215]:
                    - generic [ref=e216]: Trevor Story
                    - button "0.5 Hits" [ref=e217]:
                      - generic [ref=e218]:
                        - img [ref=e219]
                        - img [ref=e221]
                      - generic [ref=e223]: "0.5"
                      - generic [ref=e224]: Hits
                    - generic [ref=e225]:
                      - generic [ref=e226]: PHI@BOS
                      - generic [ref=e227]: 6:45PM
                    - generic [ref=e228]:
                      - button "Select over 0.5 Hits for 2.15 times" [ref=e229]:
                        - img [ref=e230]
                        - generic [ref=e232]: 2.15x
                      - button "Select over 0.5 Hits for 1.53 times" [ref=e233]:
                        - generic [ref=e234]: 1.53x
                        - img [ref=e235]
                - generic [ref=e239]:
                  - generic [ref=e242]:
                    - button "Open expert opinion for Pete Crow-Armstrong" [ref=e243]:
                      - img [ref=e244]
                    - img "Pete Crow-Armstrong" [ref=e247]
                  - generic [ref=e248]:
                    - generic [ref=e249]: P. Crow-Armstrong
                    - button "0.5 Hits" [ref=e250]:
                      - generic [ref=e251]:
                        - img [ref=e252]
                        - img [ref=e254]
                      - generic [ref=e256]: "0.5"
                      - generic [ref=e257]: Hits
                    - generic [ref=e258]:
                      - generic [ref=e259]: CHC@ATL
                      - generic [ref=e260]: 7:15PM
                    - generic [ref=e261]:
                      - button "Select over 0.5 Hits for 1.85 times" [ref=e262]:
                        - img [ref=e263]
                        - generic [ref=e265]: 1.85x
                      - button "Select over 0.5 Hits for 1.75 times" [ref=e266]:
                        - generic [ref=e267]: 1.75x
                        - img [ref=e268]
          - generic [ref=e361]:
            - generic [ref=e363]:
              - link "Download ParlayPlay On The App Store" [ref=e364]:
                - /url: https://parlayplay.onelink.me/oLJk/gnqpwjha
                - img "Download ParlayPlay On The App Store" [ref=e365]
              - paragraph [ref=e366]:
                - text: Get the app.
                - text: Better. Faster. Convenient
            - navigation [ref=e367]:
              - link "Privacy" [ref=e368]:
                - /url: /privacy-policy
              - link "Terms" [ref=e369]:
                - /url: /terms
              - link "Responsible Gaming" [ref=e370]:
                - /url: /responsible-gaming
              - link "Gaming Rules" [ref=e371]:
                - /url: /rules
              - link "FAQ" [ref=e372]:
                - /url: https://intercom.help/parlayplay/en/
            - navigation [ref=e373]:
              - generic [ref=e374]:
                - paragraph [ref=e375]: © ParlayPlay 2026
                - generic [ref=e376]:
                  - link [ref=e377]:
                    - /url: https://www.facebook.com/parlayplay.io
                    - img [ref=e378]
                  - link [ref=e380]:
                    - /url: https://www.instagram.com/parlayplay_?igsh=bHBldWQyMmV2b3Y4
                    - img [ref=e381]
                  - link [ref=e383]:
                    - /url: https://www.twitter.com/parlay_play
                    - img [ref=e384]
                  - link [ref=e386]:
                    - /url: https://discord.com/invite/parlayplay
                    - img [ref=e387]
                - img "Under 18 Logo" [ref=e389]
      - contentinfo [ref=e390]:
        - navigation [ref=e391]:
          - list [ref=e392]:
            - listitem [ref=e393]:
              - button "Home" [ref=e394] [cursor=pointer]
            - listitem [ref=e395]:
              - button "Free2Play 2" [ref=e396] [cursor=pointer]:
                - text: Free2Play
                - generic [ref=e397]: "2"
            - listitem [ref=e398]:
              - button "Rewards" [ref=e399] [cursor=pointer]
            - listitem [ref=e400]:
              - button "Entries 86" [ref=e401] [cursor=pointer]:
                - text: Entries
                - generic [ref=e402]: "86"
    - region "Notifications Alt+T"
  - generic [active]:
    - generic [ref=e405]:
      - generic [ref=e406]:
        - navigation [ref=e408]:
          - button "previous" [disabled] [ref=e409]:
            - img "previous" [ref=e410]
          - generic [ref=e412]:
            - generic [ref=e413]: 1/
            - text: "1"
          - button "next" [disabled] [ref=e414]:
            - img "next" [ref=e415]
        - link "Next.js 16.1.6 (stale) Webpack" [ref=e418]:
          - /url: https://nextjs.org/docs/messages/version-staleness
          - img [ref=e419]
          - generic "There is a newer version (16.2.6) available, upgrade recommended!" [ref=e421]: Next.js 16.1.6 (stale)
          - generic [ref=e422]: Webpack
      - dialog "Runtime TypeError" [ref=e424]:
        - generic [ref=e427]:
          - generic [ref=e428]:
            - generic [ref=e429]:
              - generic [ref=e431]: Runtime TypeError
              - generic [ref=e432]:
                - button "Copy Error Info" [ref=e433] [cursor=pointer]:
                  - img [ref=e434]
                - button "No related documentation found" [disabled] [ref=e436]:
                  - img [ref=e437]
                - button "Attach Node.js inspector" [ref=e439] [cursor=pointer]:
                  - img [ref=e440]
            - generic [ref=e452]: window.safari?.pushNotification?.permission is not a function. (In 'window.safari?.pushNotification?.permission(t)', 'window.safari?.pushNotification?.permission' is undefined)
          - generic [ref=e455]:
            - paragraph [ref=e456]:
              - text: Call Stack
              - generic [ref=e457]: "4"
            - button "Show 4 ignore-listed frame(s)" [ref=e458] [cursor=pointer]:
              - text: Show 4 ignore-listed frame(s)
              - img [ref=e459]
        - generic [ref=e461]: "1"
        - generic [ref=e462]: "2"
    - generic [ref=e467] [cursor=pointer]:
      - button "Open Next.js Dev Tools" [ref=e468]:
        - img [ref=e469]
      - generic [ref=e474]:
        - button "Open issues overlay" [ref=e475]:
          - generic [ref=e476]:
            - generic [ref=e477]: "0"
            - generic [ref=e478]: "1"
          - generic [ref=e479]: Issue
        - button "Collapse issues badge" [ref=e480]:
          - img [ref=e481]
  - alert [ref=e483]
```

# Test source

```ts
  84  |     await expect(this.playersGrid).toBeVisible();
  85  |   }
  86  | 
  87  |   async waitForFeedReady(timeout = 30_000): Promise<void> {
  88  |     await Promise.race([
  89  |       this.crossGameCardWrapper.waitFor({ state: "visible", timeout }),
  90  |       this.noPlayerFoundVisible.waitFor({ state: "visible", timeout }),
  91  |     ]);
  92  |   }
  93  | 
  94  |   async isEmptyState(): Promise<boolean> {
  95  |     return this.noPlayerFoundVisible.isVisible().catch(() => false);
  96  |   }
  97  | 
  98  |   async getPlayerCardCount(): Promise<number> {
  99  |     await this.waitForPlayersGrid();
  100 |     const cards = this.playerCardsVisible;
  101 |     await expect(cards.first()).toBeVisible();
  102 |     return await cards.count();
  103 |   }
  104 | 
  105 |   async listPlayersCard(): Promise<Locator[]> {
  106 |     await this.waitForPlayersGrid();
  107 |     const cards = this.playerCardsVisible;
  108 |     await expect(cards.first()).toBeVisible();
  109 |     const count = await cards.count();
  110 |     const result: Locator[] = [];
  111 |     for (let i = 0; i < count; i++) {
  112 |       result.push(cards.nth(i));
  113 |     }
  114 |     return result;
  115 |   }
  116 | 
  117 |   async getLeagueCount(): Promise<number> {
  118 |     return await this.leagueButtons.count();
  119 |   }
  120 | 
  121 |   async listLeagueButtons(): Promise<Locator[]> {
  122 |     const n = await this.leagueButtons.count();
  123 |     const leagueButtonsLocator: Locator[] = [];
  124 |     for (let i = 0; i < n; i++) {
  125 |       leagueButtonsLocator.push(this.leagueButtons.nth(i));
  126 |     }
  127 |     return leagueButtonsLocator;
  128 |   }
  129 | 
  130 |   async isContinueEnabled(): Promise<boolean> {
  131 |     const button = this.continueBtn;
  132 |     const isPresent = await button.isVisible().catch(() => false);
  133 |     if (!isPresent) return false;
  134 |     const enabled = await button.isEnabled().catch(() => false);
  135 |     return enabled;
  136 |   }
  137 | 
  138 |   async trySelectPick(card: Locator): Promise<boolean> {
  139 |     const buttons = card.getByTestId("grid-button");
  140 |     const lessButton = buttons.first();
  141 |     const isEnabled = await lessButton.isEnabled();
  142 | 
  143 |     await buttons.nth(isEnabled ? 0 : 1).click();
  144 | 
  145 |     //warning modal check
  146 |     try {
  147 |       const modal = this.warningModal;
  148 |       if (await modal.isVisible({ timeout: 2000 }).catch(() => false)) {
  149 |         await modal.getByRole("button", { name: "Understood" }).click();
  150 |         return false;
  151 |       }
  152 |     } catch {
  153 |       // log will be added
  154 |     }
  155 |     return true;
  156 |   }
  157 | 
  158 |   async deselectPick(card: Locator): Promise<void> {
  159 |     const buttons = card.getByTestId("grid-button");
  160 |     const count = await buttons.count();
  161 | 
  162 |     for (let i = 0; i < count; i++) {
  163 |       const btn = buttons.nth(i);
  164 |       const classes = (await btn.getAttribute("class")) ?? "";
  165 |       if (classes.includes("bg-playYellow")) {
  166 |         await btn.click(); // Deselects the selected button
  167 |         return;
  168 |       }
  169 |     }
  170 |     throw new Error("No selected button found with bg-yellow class.");
  171 |   }
  172 | 
  173 |   async pickPlayers(count: number, statIdx?: number): Promise<string[]> {
  174 |     const leagueButtons = await this.listLeagueButtons();
  175 | 
  176 |     const selected = new Set<string>();
  177 |     let lastPick: Locator | null = null;
  178 |     let lastPickId: string | null = null;
  179 |     const recentlyFailed = new Set<string>();
  180 |     for (const leagueButton of leagueButtons) {
  181 |       const leagueId = (await leagueButton.getAttribute("id")) ?? "";
  182 |       if (leagueId.toLowerCase().includes("combo")) continue;
  183 | 
> 184 |       await leagueButton.click();
      |                          ^ Error: locator.click: Target page, context or browser has been closed
  185 |       await this.waitForPlayersGrid();
  186 | 
  187 |       // Each league resets to its default stat tab on click, so re-pin
  188 |       // the requested stat after navigating into the league.
  189 |       if (statIdx !== undefined) {
  190 |         const statTab = this.statsSelector.locator("li button").nth(statIdx);
  191 |         if (await statTab.isVisible().catch(() => false)) {
  192 |           await statTab.click();
  193 |           await this.waitForPlayersGrid();
  194 |         }
  195 |       }
  196 | 
  197 |       if (await this.noPlayerLabel.isVisible().catch(() => false)) {
  198 |         continue;
  199 |       }
  200 | 
  201 |       const picks = await this.listPlayersCard();
  202 |       for (const pick of picks) {
  203 |         const playerId = await pick.locator(">div[id]").getAttribute("id");
  204 | 
  205 |         if (!playerId || selected.has(playerId)) continue;
  206 | 
  207 |         if (await this.trySelectPick(pick)) {
  208 |           selected.add(playerId);
  209 |           lastPick = pick;
  210 |           lastPickId = playerId;
  211 | 
  212 |           let continueFlag = await this.isContinueEnabled();
  213 |           if (selected.size >= count && continueFlag)
  214 |             return Array.from(selected);
  215 | 
  216 |           // Warning modal continuation
  217 |           while (
  218 |             !continueFlag &&
  219 |             selected.size == count &&
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
```