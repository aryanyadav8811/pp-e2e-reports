# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: menu/account-center.spec.ts >> Account Center menu (DFS-1667) >> Groups items under Account, Rewards and Support
- Location: tests/menu/account-center.spec.ts:47:5

# Error details

```
TimeoutError: locator.waitFor: Timeout 15000ms exceeded.
Call log:
  - waiting for getByRole('button', { name: 'Toggle Menu' }).filter({ visible: true }).first() to be visible

```

# Page snapshot

```yaml
- generic [active] [ref=e1]:
  - generic [ref=e2]:
    - generic [ref=e3]:
      - banner [ref=e4]:
        - navigation [ref=e5]:
          - link "Parlay Play LogoParlay Play text" [ref=e6] [cursor=pointer]:
            - /url: /
            - generic [ref=e7]:
              - img "Parlay Play Logo" [ref=e8]
              - img "Parlay Play text" [ref=e9]
          - generic [ref=e10]:
            - link "Join Now" [ref=e11] [cursor=pointer]:
              - /url: /account/signup
              - generic [ref=e13]: Join Now
            - link "Login" [ref=e14] [cursor=pointer]:
              - /url: /account/login
              - generic [ref=e16]: Login
      - main [ref=e17]:
        - generic [ref=e22]:
          - generic [ref=e23]:
            - generic [ref=e24]:
              - list [ref=e26]:
                - button "Live" [ref=e27] [cursor=pointer]:
                  - generic [ref=e31]: Live
                - button "MLB" [ref=e32] [cursor=pointer]
                - button "MLB-Combos" [ref=e33] [cursor=pointer]
                - button "NFL" [ref=e34] [cursor=pointer]
                - button "WNBA" [ref=e35] [cursor=pointer]
                - button "WNBA-Combos" [ref=e36] [cursor=pointer]
                - button "WNBA H1" [ref=e37] [cursor=pointer]
                - button "WNBA Q1" [ref=e38] [cursor=pointer]
                - button "MLS" [ref=e39] [cursor=pointer]
                - button "NFLSZN" [ref=e40] [cursor=pointer]
                - button "UFC" [ref=e41] [cursor=pointer]
                - button "Aussie Rules" [ref=e42] [cursor=pointer]
                - button "Lacrosse" [ref=e43] [cursor=pointer]
              - list [ref=e45]:
                - listitem [ref=e46]:
                  - button "ALL" [ref=e47] [cursor=pointer]:
                    - generic [ref=e48]: ALL
                - listitem [ref=e49]:
                  - button "PHI@MIN 7:30PM" [ref=e50] [cursor=pointer]:
                    - text: PHI@MIN
                    - generic [ref=e51]: 7:30PM
                - listitem [ref=e52]:
                  - button "TEX@LAA 10:07PM" [ref=e53] [cursor=pointer]:
                    - text: TEX@LAA
                    - generic [ref=e54]: 10:07PM
                - listitem [ref=e55]:
                  - button "MIL@LAD 10:10PM" [ref=e56] [cursor=pointer]:
                    - text: MIL@LAD
                    - generic [ref=e57]: 10:10PM
                - listitem [ref=e58]:
                  - button "BOS@PIT Fri 6PM" [ref=e59] [cursor=pointer]:
                    - text: BOS@PIT
                    - generic [ref=e60]: Fri 6PM
              - generic [ref=e61]:
                - generic [ref=e62]:
                  - generic [ref=e65]:
                    - img [ref=e67]
                    - textbox "Search player or team" [ref=e69]
                  - button "Change card style from grid" [ref=e71]
                - list [ref=e73]:
                  - listitem [ref=e74]:
                    - button "Strikeouts (K)" [ref=e75]
                  - listitem [ref=e76]:
                    - button "Hits" [ref=e77]
                  - listitem [ref=e78]:
                    - button "Hits + Runs + RBIs" [ref=e79]
                  - listitem [ref=e80]:
                    - button "Singles" [ref=e81]
                  - listitem [ref=e82]:
                    - button "Doubles" [ref=e83]
                  - listitem [ref=e84]:
                    - button "Triples" [ref=e85]
                  - listitem [ref=e86]:
                    - button "Runs" [ref=e87]
                  - listitem [ref=e88]:
                    - button "RBIs" [ref=e89]
                  - listitem [ref=e90]:
                    - button "Hits Allowed" [ref=e91]
                  - listitem [ref=e92]:
                    - button "Pitching Outs" [ref=e93]
                  - listitem [ref=e94]:
                    - button "Pitches Thrown" [ref=e95]
                  - listitem [ref=e96]:
                    - button "Earned Runs" [ref=e97]
                  - listitem [ref=e98]:
                    - button "Homeruns" [ref=e99]
                  - listitem [ref=e100]:
                    - button "Total Bases" [ref=e101]
                  - listitem [ref=e102]:
                    - button "Strikeouts" [ref=e103]
                  - listitem [ref=e104]:
                    - button "Fantasy Points" [ref=e105]
            - generic [ref=e106]:
              - generic [ref=e111]:
                - generic [ref=e114] [cursor=pointer]:
                  - generic [ref=e115]:
                    - generic [ref=e116]:
                      - generic [ref=e117]: 100%
                      - generic [ref=e118]: Deposit Match
                    - generic [ref=e119]: New User Promotion
                  - button "Sign Up" [ref=e121]
                - generic [ref=e125] [cursor=pointer]:
                  - generic [ref=e126]: Pull real graded cards worth up to $10,000
                  - generic [ref=e127]: Sell or ship instantly
                  - button "Rip a pack" [ref=e128]:
                    - generic [ref=e129]:
                      - img [ref=e130]
                      - text: Rip a pack
                - generic [ref=e135] [cursor=pointer]:
                  - generic [ref=e136]:
                    - generic [ref=e137]:
                      - img [ref=e138]
                      - generic [ref=e142]: Boosted Picks
                    - generic [ref=e143]: "Every Pick Pays: Up to a 35% Boost!"
                  - button "Details" [ref=e145]
              - generic [ref=e149]:
                - generic [ref=e152]:
                  - generic [ref=e155]:
                    - button "Open expert opinion for Shane Drohan" [ref=e156]:
                      - img [ref=e157]
                    - img "Shane Drohan" [ref=e160]
                  - generic [ref=e161]:
                    - generic [ref=e162]: Shane Drohan
                    - button "4.5 SO (K)" [ref=e163]:
                      - generic [ref=e164]:
                        - img [ref=e165]
                        - img [ref=e167]
                      - generic [ref=e169]: "4.5"
                      - generic [ref=e170]: SO (K)
                    - generic [ref=e171]:
                      - generic [ref=e172]: MIL@LAD
                      - generic [ref=e173]: 10:10PM
                    - generic [ref=e174]:
                      - button "Select over 4.5 Strikeouts (K) for 1.84 times" [ref=e175]:
                        - img [ref=e176]
                        - generic [ref=e178]: 1.84x
                      - button "Select over 4.5 Strikeouts (K) for 1.79 times" [ref=e179]:
                        - generic [ref=e180]: 1.79x
                        - img [ref=e181]
                - generic [ref=e185]:
                  - generic [ref=e188]:
                    - button "Open expert opinion for Roki Sasaki" [ref=e189]:
                      - img [ref=e190]
                    - img "Roki Sasaki" [ref=e193]
                  - generic [ref=e194]:
                    - generic [ref=e195]: Roki Sasaki
                    - button "5.5 SO (K)" [ref=e196]:
                      - generic [ref=e197]:
                        - img [ref=e198]
                        - img [ref=e200]
                      - generic [ref=e202]: "5.5"
                      - generic [ref=e203]: SO (K)
                    - generic [ref=e204]:
                      - generic [ref=e205]: MIL@LAD
                      - generic [ref=e206]: 10:10PM
                    - generic [ref=e207]:
                      - button "Select over 5.5 Strikeouts (K) for 2 times" [ref=e208]:
                        - img [ref=e209]
                        - generic [ref=e211]: 2x
                      - button "Select over 5.5 Strikeouts (K) for 1.67 times" [ref=e212]:
                        - generic [ref=e213]: 1.67x
                        - img [ref=e214]
          - generic [ref=e217]:
            - generic [ref=e219]:
              - link "Download ParlayPlay On The Play Store" [ref=e220] [cursor=pointer]:
                - /url: https://parlayplay.onelink.me/oLJk/fh7u6juo
                - img "Download ParlayPlay On The Play Store" [ref=e221]
              - paragraph [ref=e222]:
                - text: Get the app.
                - text: Better. Faster. Convenient
            - navigation [ref=e223]:
              - link "Privacy" [ref=e224] [cursor=pointer]:
                - /url: /privacy-policy
              - link "Fantasy Terms" [ref=e225] [cursor=pointer]:
                - /url: /terms
              - link "Packs Terms" [ref=e226] [cursor=pointer]:
                - /url: /terms/packs
              - link "Responsible Gaming" [ref=e227] [cursor=pointer]:
                - /url: /responsible-gaming
              - link "Gaming Rules" [ref=e228] [cursor=pointer]:
                - /url: /rules
              - link "FAQ" [ref=e229] [cursor=pointer]:
                - /url: https://intercom.help/parlayplay/en/
            - navigation [ref=e230]:
              - generic [ref=e231]:
                - paragraph [ref=e232]: © ParlayPlay 2026
                - generic [ref=e233]:
                  - link "ParlayPlay on Facebook" [ref=e234] [cursor=pointer]:
                    - /url: https://www.facebook.com/parlayplay.io
                    - img [ref=e235]
                  - link "ParlayPlay on Instagram" [ref=e237] [cursor=pointer]:
                    - /url: https://www.instagram.com/parlayplay_?igsh=bHBldWQyMmV2b3Y4
                    - img [ref=e238]
                  - link "ParlayPlay on Twitter" [ref=e240] [cursor=pointer]:
                    - /url: https://www.twitter.com/parlay_play
                    - img [ref=e241]
                  - link "ParlayPlay on Discord" [ref=e243] [cursor=pointer]:
                    - /url: https://discord.com/invite/parlayplay
                    - img [ref=e244]
                - img "18+ icon" [ref=e246]
            - paragraph [ref=e248]
      - contentinfo [ref=e249]:
        - navigation [ref=e250]:
          - list [ref=e251]:
            - listitem [ref=e252]:
              - button "Home" [ref=e253] [cursor=pointer]:
                - generic [ref=e254]:
                  - img [ref=e255]
                  - generic [ref=e256]: Home
            - listitem [ref=e257]:
              - button "Entries" [ref=e258] [cursor=pointer]:
                - generic [ref=e259]:
                  - img [ref=e260]
                  - generic [ref=e261]: Entries
            - listitem [ref=e262]:
              - button "Feed" [ref=e263] [cursor=pointer]:
                - generic [ref=e264]:
                  - img [ref=e265]
                  - generic [ref=e266]: Feed
            - listitem [ref=e267]:
              - button "Rewards" [ref=e268] [cursor=pointer]:
                - generic [ref=e269]:
                  - img [ref=e270]
                  - generic [ref=e271]: Rewards
            - listitem [ref=e272]:
              - button "Packs" [ref=e273] [cursor=pointer]:
                - generic [ref=e274]:
                  - img [ref=e275]
                  - generic [ref=e276]: Packs
    - region "Notifications Alt+T"
  - alert [ref=e277]
  - iframe [ref=e278]:
    
```

# Test source

```ts
  416 |    * persistence assertion from the render path.
  417 |    */
  418 |   async getPersistedPickIds(): Promise<string[]> {
  419 |     return this.page.evaluate(() => {
  420 |       const raw = localStorage.getItem("pp_persistent_slip:v1");
  421 |       if (!raw) return [];
  422 |       try {
  423 |         const parsed = JSON.parse(raw);
  424 |         return Object.keys(parsed.selectedPicks ?? {});
  425 |       } catch {
  426 |         return [];
  427 |       }
  428 |     });
  429 |   }
  430 | 
  431 |   async assertPicksPersist(
  432 |     expectedIds: string[],
  433 |     timeout = 10_000,
  434 |   ): Promise<void> {
  435 |     // Storage IDs are bare player IDs ("1089"); pickPlayers returns the DOM
  436 |     // attribute form ("player-1089"). Normalise both sides.
  437 |     const normalise = (id: string) => id.replace(/^player-/, "");
  438 |     const expected = new Set(expectedIds.map(normalise));
  439 | 
  440 |     // Auto-save is debounced ~1s and the post-reload restore writes its
  441 |     // reconciled state back asynchronously, so poll rather than read once.
  442 |     await expect
  443 |       .poll(
  444 |         async () => {
  445 |           const ids = await this.getPersistedPickIds();
  446 |           return Array.from(new Set(ids.map(normalise))).sort();
  447 |         },
  448 |         {
  449 |           timeout,
  450 |           message: `Expected persisted picks ${JSON.stringify(
  451 |             Array.from(expected).sort(),
  452 |           )} in localStorage`,
  453 |         },
  454 |       )
  455 |       .toEqual(Array.from(expected).sort());
  456 |   }
  457 | 
  458 |   async waitForSlipPersisted(
  459 |     expectedPickCount: number,
  460 |     timeout = 5_000
  461 |   ): Promise<void> {
  462 |     await expect
  463 |       .poll(
  464 |         async () =>
  465 |           this.page.evaluate(() => {
  466 |             const raw = localStorage.getItem("pp_persistent_slip:v1");
  467 |             if (!raw) return 0;
  468 |             try {
  469 |               return JSON.parse(raw).nrOfPicks ?? 0;
  470 |             } catch {
  471 |               return 0;
  472 |             }
  473 |           }),
  474 |         {
  475 |           timeout,
  476 |           message: `Slip with ${expectedPickCount} picks was never written to localStorage`,
  477 |         }
  478 |       )
  479 |       .toBe(expectedPickCount);
  480 |   }
  481 | 
  482 |   async enterFinalContestPage() {
  483 |     await this.continueBtn.click();
  484 |   }
  485 | 
  486 |   async clearSlip(): Promise<void> {
  487 |     await this.page.evaluate(() =>
  488 |       localStorage.removeItem("pp_persistent_slip:v1")
  489 |     );
  490 |     await this.page.goto("/");
  491 |     await this.waitForFeedReady();
  492 |   }
  493 | 
  494 |   async selectStatByIndex(idx: number): Promise<void> {
  495 |     const tab = this.statsSelector.locator("li button").nth(idx);
  496 |     await expect(tab).toBeVisible();
  497 |     await tab.click();
  498 |     await this.waitForFeedReady();
  499 |   }
  500 | 
  501 |   async enterEntriesPage() {
  502 |     await this.entriesTab.click();
  503 |   }
  504 | 
  505 |   async enterHomePage(): Promise<void> {
  506 |     await this.homeTab.click();
  507 |     await this.waitForFeedReady();
  508 |     await expect(this.leagueSelector).toBeVisible();
  509 |   }
  510 | 
  511 |   async enterMenu() {
  512 |     // Some specs land here without an explicit goto('/'), so the global
  513 |     // header may not be mounted yet. Wait briefly for Toggle Menu before
  514 |     // clicking — fail fast (15s) instead of letting the test-level timeout
  515 |     // (10 min) absorb a hung locator.
> 516 |     await this.toggleMenu.waitFor({ state: "visible", timeout: 15_000 });
      |                           ^ TimeoutError: locator.waitFor: Timeout 15000ms exceeded.
  517 |     await this.toggleMenu.click({ timeout: 15_000 });
  518 |   }
  519 | 
  520 |   async assertHomePage() {
  521 |     await expect(this.leagueSelector).toBeVisible();
  522 |   }
  523 | 
  524 |   async enterRewarsdsPage() {
  525 |     await this.rewardsTab.click();
  526 |   }
  527 | 
  528 |   /**
  529 |    * The active-tab underline in the bottom nav. Every tab label <span> carries
  530 |    * `border-playYellow`; the active one additionally gets `border-b-2`, so tests
  531 |    * assert on that class. Scoped to `bottomNav` so it never resolves to page
  532 |    * content that happens to share the tab's label.
  533 |    */
  534 |   navIndicator(label: string): Locator {
  535 |     return this.bottomNav
  536 |       .getByRole("button", { name: label })
  537 |       .locator("span.border-playYellow");
  538 |   }
  539 | 
  540 |   async enterFeedPage() {
  541 |     await this.feedTab.click();
  542 |   }
  543 | 
  544 |   /**
  545 |    * DFS-2115: the footer's fifth slot is a kill switch (see packsTab). When
  546 |    * Packs occupies it, Free2Play moves into the burger menu (Account Center →
  547 |    * Rewards). Prefer the footer tab, fall back to the menu entry — exactly
  548 |    * one of the two placements exists for a given user.
  549 |    */
  550 |   async enterFree2PlayPage() {
  551 |     if (await this.free2PlayTab.isVisible().catch(() => false)) {
  552 |       await this.free2PlayTab.click();
  553 |       return;
  554 |     }
  555 |     await this.enterMenu();
  556 |     await this.visible(
  557 |       this.page.getByRole("link", { name: "Free2Play", exact: true })
  558 |     ).click();
  559 |   }
  560 | 
  561 |   /** Type into the feed search box. `onSearch` is debounced by the feed, so
  562 |    * callers should assert on the resulting grid/empty state rather than a
  563 |    * fixed wait. */
  564 |   async searchPlayers(term: string): Promise<void> {
  565 |     await expect(this.searchInput).toBeVisible();
  566 |     await this.searchInput.fill(term);
  567 |   }
  568 | 
  569 |   /** Clear the feed search via the in-field × button so the grid resets. */
  570 |   async clearSearch(): Promise<void> {
  571 |     await this.searchClearBtn.click();
  572 |   }
  573 | 
  574 |   async fullGameLeagueCount() {
  575 |     return await this.fgleagueTabs.count();
  576 |   }
  577 | 
  578 |   async statsTabCount() {
  579 |     return await this.statsTabs.count();
  580 |   }
  581 | }
  582 | 
```