# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: settings/settings.spec.ts >> My Settings >> Verify user data renders correctly
- Location: tests/settings/settings.spec.ts:17:5

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
          - link "Parlay Play LogoParlay Play text" [ref=e6]:
            - /url: /
            - generic [ref=e7]:
              - img "Parlay Play Logo" [ref=e8]
              - img "Parlay Play text" [ref=e9]
          - generic [ref=e10]:
            - link "Join Now" [ref=e11]:
              - /url: /account/signup
              - generic [ref=e13]: Join Now
            - link "Login" [ref=e14]:
              - /url: /account/login
              - generic [ref=e16]: Login
      - main [ref=e17]:
        - generic [ref=e22]:
          - generic [ref=e23]:
            - generic [ref=e24]:
              - list [ref=e26]:
                - button "MLB" [ref=e27] [cursor=pointer]
                - button "MLB-Combos" [ref=e28] [cursor=pointer]
                - button "NFL" [ref=e29] [cursor=pointer]
                - button "WNBA" [ref=e30] [cursor=pointer]
                - button "WNBA-Combos" [ref=e31] [cursor=pointer]
                - button "WNBA H1" [ref=e32] [cursor=pointer]
                - button "WNBA Q1" [ref=e33] [cursor=pointer]
                - button "MLS" [ref=e34] [cursor=pointer]
                - button "UFC" [ref=e35] [cursor=pointer]
                - button "Aussie Rules" [ref=e36] [cursor=pointer]
                - button "Lacrosse" [ref=e37] [cursor=pointer]
              - list [ref=e39]:
                - listitem [ref=e40]:
                  - button "ALL" [ref=e41] [cursor=pointer]:
                    - generic [ref=e42]: ALL
                - listitem [ref=e43]:
                  - button "PHI@MIN 7:30PM" [ref=e44] [cursor=pointer]:
                    - text: PHI@MIN
                    - generic [ref=e45]: 7:30PM
                - listitem [ref=e46]:
                  - button "TEX@LAA 10:07PM" [ref=e47] [cursor=pointer]:
                    - text: TEX@LAA
                    - generic [ref=e48]: 10:07PM
                - listitem [ref=e49]:
                  - button "MIL@LAD 10:10PM" [ref=e50] [cursor=pointer]:
                    - text: MIL@LAD
                    - generic [ref=e51]: 10:10PM
              - generic [ref=e52]:
                - generic [ref=e53]:
                  - generic [ref=e56]:
                    - img [ref=e58]
                    - textbox "Search player or team" [ref=e60]
                  - button "Change card style from grid" [ref=e62]
                - list [ref=e64]:
                  - listitem [ref=e65]:
                    - button "Strikeouts (K)" [ref=e66]
                  - listitem [ref=e67]:
                    - button "Hits" [ref=e68]
                  - listitem [ref=e69]:
                    - button "Hits + Runs + RBIs" [ref=e70]
                  - listitem [ref=e71]:
                    - button "Singles" [ref=e72]
                  - listitem [ref=e73]:
                    - button "Doubles" [ref=e74]
                  - listitem [ref=e75]:
                    - button "Triples" [ref=e76]
                  - listitem [ref=e77]:
                    - button "Runs" [ref=e78]
                  - listitem [ref=e79]:
                    - button "RBIs" [ref=e80]
                  - listitem [ref=e81]:
                    - button "Hits Allowed" [ref=e82]
                  - listitem [ref=e83]:
                    - button "Pitching Outs" [ref=e84]
                  - listitem [ref=e85]:
                    - button "Pitches Thrown" [ref=e86]
                  - listitem [ref=e87]:
                    - button "Earned Runs" [ref=e88]
                  - listitem [ref=e89]:
                    - button "Homeruns" [ref=e90]
                  - listitem [ref=e91]:
                    - button "Total Bases" [ref=e92]
                  - listitem [ref=e93]:
                    - button "Strikeouts" [ref=e94]
                  - listitem [ref=e95]:
                    - button "Fantasy Points" [ref=e96]
            - generic [ref=e97]:
              - generic [ref=e102]:
                - generic [ref=e105] [cursor=pointer]:
                  - generic [ref=e106]:
                    - generic [ref=e107]:
                      - generic [ref=e108]: 100%
                      - generic [ref=e109]: Deposit Match
                    - generic [ref=e110]: New User Promotion
                  - button "Sign Up" [ref=e112]
                - generic [ref=e116] [cursor=pointer]:
                  - generic [ref=e117]: Pull real graded cards worth up to $10,000
                  - generic [ref=e118]: Sell or ship instantly
                  - button "Rip a pack" [ref=e119]:
                    - generic [ref=e120]:
                      - img [ref=e121]
                      - text: Rip a pack
                - generic [ref=e126] [cursor=pointer]:
                  - generic [ref=e127]:
                    - generic [ref=e128]:
                      - img [ref=e129]
                      - generic [ref=e133]: Boosted Picks
                    - generic [ref=e134]: "Every Pick Pays: Up to a 35% Boost!"
                  - button "Details" [ref=e136]
              - generic [ref=e140]:
                - generic [ref=e143]:
                  - generic [ref=e146]:
                    - button "Open expert opinion for Shane Drohan" [ref=e147]:
                      - img [ref=e148]
                    - img "Shane Drohan" [ref=e151]
                  - generic [ref=e152]:
                    - generic [ref=e153]: Shane Drohan
                    - button "4.5 SO (K)" [ref=e154]:
                      - generic [ref=e155]:
                        - img [ref=e156]
                        - img [ref=e158]
                      - generic [ref=e160]: "4.5"
                      - generic [ref=e161]: SO (K)
                    - generic [ref=e162]:
                      - generic [ref=e163]: MIL@LAD
                      - generic [ref=e164]: 10:10PM
                    - generic [ref=e165]:
                      - button "Select over 4.5 Strikeouts (K) for 1.78 times" [ref=e166]:
                        - img [ref=e167]
                        - generic [ref=e169]: 1.78x
                      - button "Select over 4.5 Strikeouts (K) for 1.86 times" [ref=e170]:
                        - generic [ref=e171]: 1.86x
                        - img [ref=e172]
                - generic [ref=e176]:
                  - generic [ref=e179]:
                    - button "Open expert opinion for Roki Sasaki" [ref=e180]:
                      - img [ref=e181]
                    - img "Roki Sasaki" [ref=e184]
                  - generic [ref=e185]:
                    - generic [ref=e186]: Roki Sasaki
                    - button "5.5 SO (K)" [ref=e187]:
                      - generic [ref=e188]:
                        - img [ref=e189]
                        - img [ref=e191]
                      - generic [ref=e193]: "5.5"
                      - generic [ref=e194]: SO (K)
                    - generic [ref=e195]:
                      - generic [ref=e196]: MIL@LAD
                      - generic [ref=e197]: 10:10PM
                    - generic [ref=e198]:
                      - button "Select over 5.5 Strikeouts (K) for 2 times" [ref=e199]:
                        - img [ref=e200]
                        - generic [ref=e202]: 2x
                      - button "Select over 5.5 Strikeouts (K) for 1.66 times" [ref=e203]:
                        - generic [ref=e204]: 1.66x
                        - img [ref=e205]
          - generic [ref=e208]:
            - generic [ref=e210]:
              - link "Download ParlayPlay On The App Store" [ref=e211]:
                - /url: https://parlayplay.onelink.me/oLJk/gnqpwjha
                - img "Download ParlayPlay On The App Store" [ref=e212]
              - paragraph [ref=e213]:
                - text: Get the app.
                - text: Better. Faster. Convenient
            - navigation [ref=e214]:
              - link "Privacy" [ref=e215]:
                - /url: /privacy-policy
              - link "Fantasy Terms" [ref=e216]:
                - /url: /terms
              - link "Packs Terms" [ref=e217]:
                - /url: /terms/packs
              - link "Responsible Gaming" [ref=e218]:
                - /url: /responsible-gaming
              - link "Gaming Rules" [ref=e219]:
                - /url: /rules
              - link "FAQ" [ref=e220]:
                - /url: https://intercom.help/parlayplay/en/
            - navigation [ref=e221]:
              - generic [ref=e222]:
                - paragraph [ref=e223]: © ParlayPlay 2026
                - generic [ref=e224]:
                  - link "ParlayPlay on Facebook" [ref=e225]:
                    - /url: https://www.facebook.com/parlayplay.io
                    - img [ref=e226]
                  - link "ParlayPlay on Instagram" [ref=e228]:
                    - /url: https://www.instagram.com/parlayplay_?igsh=bHBldWQyMmV2b3Y4
                    - img [ref=e229]
                  - link "ParlayPlay on Twitter" [ref=e231]:
                    - /url: https://www.twitter.com/parlay_play
                    - img [ref=e232]
                  - link "ParlayPlay on Discord" [ref=e234]:
                    - /url: https://discord.com/invite/parlayplay
                    - img [ref=e235]
                - img "18+ icon" [ref=e237]
            - paragraph [ref=e239]
      - contentinfo [ref=e240]:
        - navigation [ref=e241]:
          - list [ref=e242]:
            - listitem [ref=e243]:
              - button "Home" [ref=e244] [cursor=pointer]:
                - generic [ref=e245]:
                  - img [ref=e246]
                  - generic [ref=e247]: Home
            - listitem [ref=e248]:
              - button "Entries" [ref=e249] [cursor=pointer]:
                - generic [ref=e250]:
                  - img [ref=e251]
                  - generic [ref=e252]: Entries
            - listitem [ref=e253]:
              - button "Feed" [ref=e254] [cursor=pointer]:
                - generic [ref=e255]:
                  - img [ref=e256]
                  - generic [ref=e257]: Feed
            - listitem [ref=e258]:
              - button "Rewards" [ref=e259] [cursor=pointer]:
                - generic [ref=e260]:
                  - img [ref=e261]
                  - generic [ref=e262]: Rewards
            - listitem [ref=e263]:
              - button "Packs" [ref=e264] [cursor=pointer]:
                - generic [ref=e265]:
                  - img [ref=e266]
                  - generic [ref=e267]: Packs
    - region "Notifications Alt+T"
  - alert [ref=e268]
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