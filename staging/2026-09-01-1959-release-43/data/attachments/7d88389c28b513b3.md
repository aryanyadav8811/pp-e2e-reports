# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: contests/user-enter-contest.spec.ts >> User Enter Contest >> Five player contest Submission
- Location: tests/contests/user-enter-contest.spec.ts:26:5

# Error details

```
Error: Could not place contest after 5 attempts (last error: Could not select 5 valid picks) — every attempted stat tab ran out of selectable cards; the environment's offering is likely too thin for this pick count

expect(received).toBe(expected) // Object.is equality

Expected: true
Received: false
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
                - link "Rewards 51" [ref=e24] [cursor=pointer]:
                  - /url: /rewards
                  - generic [ref=e25]:
                    - generic [ref=e26]: Rewards
                    - generic [ref=e27]: "51"
              - listitem [ref=e28]:
                - link "Track Picks 32" [ref=e29] [cursor=pointer]:
                  - /url: /challenges/pending
                  - generic [ref=e30]:
                    - generic [ref=e31]: Track Picks
                    - generic [ref=e32]: "32"
            - button "Claim your $100 Deposit Match" [ref=e33] [cursor=pointer]
            - generic [ref=e34]:
              - generic [ref=e36]:
                - generic [ref=e37]: $942.00
                - generic [ref=e38]:
                  - img "gift-icon" [ref=e39]
                  - text: "51.00"
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
                - button "MLB-Combos" [ref=e88] [cursor=pointer]
                - button "EPL" [ref=e89] [cursor=pointer]
                - button "MLS" [ref=e90] [cursor=pointer]
                - button "NFLSZN" [ref=e91] [cursor=pointer]
                - button "LaLiga" [ref=e92] [cursor=pointer]
                - button "UFC" [ref=e93] [cursor=pointer]
              - button "right chevron sign Filter" [ref=e95] [cursor=pointer]:
                - img "right chevron sign" [ref=e96]
                - text: Filter
            - generic [ref=e97]:
              - generic [ref=e100]:
                - generic [ref=e103]:
                  - generic [ref=e104]:
                    - img "Charlie Cleveland" [ref=e106]
                    - generic [ref=e107]:
                      - generic [ref=e108]: C. Cleveland
                      - generic [ref=e109]: FI - CClevela
                      - generic [ref=e112]: CClevela @ GLourenc 7:20 PM
                    - button "Open expert opinion for Charlie Cleveland" [ref=e113]:
                      - img [ref=e114]
                  - generic [ref=e118]:
                    - generic [ref=e119]:
                      - generic [ref=e120]:
                        - generic [ref=e122] [cursor=pointer]:
                          - text: Less
                          - img [ref=e123]
                        - generic [ref=e125]: Significant Strikes
                        - generic [ref=e127] [cursor=pointer]:
                          - text: More
                          - img [ref=e128]
                      - generic [ref=e131]:
                        - button "Select over 40.5 Significant Strikes for 1.77 times" [ref=e132]:
                          - img [ref=e135]
                          - text: 1.77x
                        - generic [ref=e137]: 40.5 S. STR
                        - button "Select over 40.5 Significant Strikes for 1.77 times" [ref=e138]: 1.77x
                    - generic [ref=e139]:
                      - generic [ref=e140]:
                        - generic [ref=e142] [cursor=pointer]:
                          - text: Less
                          - img [ref=e143]
                        - generic [ref=e145]: Strikes Landed
                        - generic [ref=e147] [cursor=pointer]:
                          - text: More
                          - img [ref=e148]
                      - generic [ref=e151]:
                        - button "Select over 60.5 Strikes Landed for 1.77 times" [ref=e152]: 1.77x
                        - generic [ref=e153]: 60.5 Strikes Landed
                        - button "Select over 60.5 Strikes Landed for 1.77 times" [ref=e154]: 1.77x
                  - button "Show More Stats" [ref=e156]:
                    - img [ref=e157]
                - generic [ref=e161]:
                  - generic [ref=e162]:
                    - img "Gabriel Lourenco" [ref=e164]
                    - generic [ref=e165]:
                      - generic [ref=e166]: G. Lourenco
                      - generic [ref=e167]: FI - GLourenc
                      - generic [ref=e170]: CClevela @ GLourenc 7:20 PM
                    - button "Open expert opinion for Gabriel Lourenco" [ref=e171]:
                      - img [ref=e172]
                  - generic [ref=e176]:
                    - generic [ref=e177]:
                      - generic [ref=e178]:
                        - generic [ref=e180] [cursor=pointer]:
                          - text: Less
                          - img [ref=e181]
                        - generic [ref=e183]: Significant Strikes
                        - generic [ref=e185] [cursor=pointer]:
                          - text: More
                          - img [ref=e186]
                      - generic [ref=e189]:
                        - button "Select over 40.5 Significant Strikes for 1.77 times" [active] [ref=e190]:
                          - img [ref=e193]
                          - text: 1.77x
                        - generic [ref=e195]: 40.5 S. STR
                        - button "Select over 40.5 Significant Strikes for 1.77 times" [ref=e196]: 1.77x
                    - generic [ref=e197]:
                      - generic [ref=e198]:
                        - generic [ref=e200] [cursor=pointer]:
                          - text: Less
                          - img [ref=e201]
                        - generic [ref=e203]: Strikes Landed
                        - generic [ref=e205] [cursor=pointer]:
                          - text: More
                          - img [ref=e206]
                      - generic [ref=e209]:
                        - button "Select over 60.5 Strikes Landed for 1.77 times" [ref=e210]: 1.77x
                        - generic [ref=e211]: 60.5 Strikes Landed
                        - button "Select over 60.5 Strikes Landed for 1.77 times" [ref=e212]: 1.77x
                  - button "Show More Stats" [ref=e214]:
                    - img [ref=e215]
              - generic [ref=e415]:
                - generic [ref=e417]:
                  - generic [ref=e418]: 2.7x
                  - generic [ref=e419]:
                    - button "+ 5% Boost 🚀" [ref=e424]:
                      - generic [ref=e425]: + 5% Boost 🚀
                    - generic [ref=e436]: "Add 3rd Pick: 5% Boost"
                - generic [ref=e438]:
                  - generic [ref=e440]:
                    - generic [ref=e441]:
                      - generic [ref=e443]: "1"
                      - button [ref=e446]:
                        - img [ref=e448]
                      - generic [ref=e450]: Cleveland - Charlie Cleveland
                      - generic [ref=e451]: Today 7:20 PM vs GLourenc
                      - generic [ref=e452]:
                        - button "1.77 x Less 40.5 Significant Strikes" [ref=e454]:
                          - generic [ref=e456]: 1.77 x
                          - generic [ref=e457]: Less
                          - generic [ref=e458]: "40.5"
                          - generic [ref=e459]: Significant Strikes
                          - img [ref=e462]
                        - button "1.77 x More 40.5 Significant Strikes" [ref=e465]:
                          - generic [ref=e467]: 1.77 x
                          - generic [ref=e468]: More
                          - generic [ref=e469]: "40.5"
                          - generic [ref=e470]: Significant Strikes
                    - img "Charlie Cleveland" [ref=e473]
                  - generic [ref=e475]:
                    - generic [ref=e476]:
                      - generic [ref=e478]: "2"
                      - button [ref=e481]:
                        - img [ref=e483]
                      - generic [ref=e485]: Lourenco - Gabriel Lourenco
                      - generic [ref=e486]: Today 7:20 PM vs CClevela
                      - generic [ref=e487]:
                        - button "1.77 x Less 40.5 Significant Strikes" [ref=e489]:
                          - generic [ref=e491]: 1.77 x
                          - generic [ref=e492]: Less
                          - generic [ref=e493]: "40.5"
                          - generic [ref=e494]: Significant Strikes
                          - img [ref=e497]
                        - button "1.77 x More 40.5 Significant Strikes" [ref=e500]:
                          - generic [ref=e502]: 1.77 x
                          - generic [ref=e503]: More
                          - generic [ref=e504]: "40.5"
                          - generic [ref=e505]: Significant Strikes
                    - img "Gabriel Lourenco" [ref=e508]
                  - generic [ref=e509]:
                    - generic [ref=e510]:
                      - generic [ref=e512]:
                        - radio "$25"
                        - generic [ref=e513] [cursor=pointer]: $25
                        - radio "$75"
                        - generic [ref=e514] [cursor=pointer]: $75
                        - radio "$300"
                        - generic [ref=e515] [cursor=pointer]: $300
                      - generic [ref=e517]:
                        - generic [ref=e518]: $
                        - spinbutton [ref=e522]: "3"
                      - button "51" [ref=e523] [cursor=pointer]:
                        - img [ref=e524]
                        - generic [ref=e526]: "51"
                    - generic [ref=e527]:
                      - generic [ref=e528]:
                        - generic [ref=e529]:
                          - button "Insured" [ref=e530]
                          - button "All In" [ref=e531]
                        - generic [ref=e533]: 2.7x
                      - generic [ref=e535]:
                        - generic [ref=e536]:
                          - paragraph [ref=e537]: Perfect line-up
                          - paragraph [ref=e538]: $8.1
                        - generic [ref=e540]:
                          - paragraph [ref=e541]: Or 1st place in group
                          - generic [ref=e542]: $1 + $8.1
                    - button "Place" [ref=e546] [cursor=pointer]:
                      - text: Place
                      - img [ref=e547]
          - generic [ref=e551]:
            - generic [ref=e552]:
              - link "Parlay Play Logo" [ref=e553] [cursor=pointer]:
                - /url: /
                - img "Parlay Play Logo" [ref=e555]
              - generic [ref=e556]:
                - generic [ref=e557]: Improve your experience. Download our app.
                - generic [ref=e558]:
                  - link "Apple Store" [ref=e559] [cursor=pointer]:
                    - /url: https://parlayplay.onelink.me/oLJk/gnqpwjha
                    - img "Apple Store" [ref=e560]
                  - link "Google Play Store" [ref=e561] [cursor=pointer]:
                    - /url: https://parlayplay.onelink.me/oLJk/fh7u6juo
                    - img "Google Play Store" [ref=e562]
            - generic [ref=e563]:
              - link "Privacy" [ref=e564] [cursor=pointer]:
                - /url: /privacy-policy
              - link "Fantasy Terms" [ref=e565] [cursor=pointer]:
                - /url: /terms
              - link "Packs Terms" [ref=e566] [cursor=pointer]:
                - /url: /terms/packs
              - link "Responsible Gaming" [ref=e567] [cursor=pointer]:
                - /url: /responsible-gaming
              - link "Gaming Rules" [ref=e568] [cursor=pointer]:
                - /url: /rules
              - link "FAQ" [ref=e569] [cursor=pointer]:
                - /url: https://intercom.help/parlayplay/en/
              - link "Contact Us" [ref=e570] [cursor=pointer]:
                - /url: /
              - paragraph [ref=e571]: © ParlayPlay 2026 - All Rights Reserved
            - list [ref=e572]:
              - listitem [ref=e573]:
                - generic [ref=e574]:
                  - log [ref=e576]
                  - generic [ref=e577]:
                    - generic [ref=e578]:
                      - generic [ref=e579]: 🇺🇸English
                      - combobox "Select language" [ref=e580]
                    - img [ref=e584]
              - listitem [ref=e586]:
                - img "18+-icon" [ref=e587]
              - listitem [ref=e588]:
                - link "ParlayPlay on Twitter" [ref=e589] [cursor=pointer]:
                  - /url: https://twitter.com/parlay_play?lang=en
                  - img [ref=e590]
              - listitem [ref=e592]:
                - link "ParlayPlay on Facebook" [ref=e593] [cursor=pointer]:
                  - /url: https://www.facebook.com/ParlayPlay.io/
                  - img [ref=e594]
              - listitem [ref=e596]:
                - link "ParlayPlay on Instagram" [ref=e597] [cursor=pointer]:
                  - /url: https://www.instagram.com/parlayplay_?igsh=bHBldWQyMmV2b3Y4
                  - img [ref=e598]
              - listitem [ref=e600]:
                - link "ParlayPlay on Discord" [ref=e601] [cursor=pointer]:
                  - /url: https://discord.com/invite/parlayplay
                  - img [ref=e602]
    - generic:
      - region "Notifications Alt+T"
  - alert [ref=e604]
  - iframe [ref=e605]:
    
```

# Test source

```ts
  84  |  * Picks N players, advances to the contest page, and submits — retrying on
  85  |  * a different stat tab when a user limit (or other submission error) trips.
  86  |  *
  87  |  * Used by both the contest-submission specs and the slip-sharing flow, since
  88  |  * any user can hit a per-stat limit on the first try.
  89  |  */
  90  | export async function placeContestWithRetry(
  91  |     opts: PlaceContestWithRetryOptions,
  92  | ): Promise<PlaceContestWithRetryResult> {
  93  |     const { homePage, contestPage, pickCount, entryAmount } = opts;
  94  |     const maxAttempts = resolveMaxAttempts(opts.maxAttempts);
  95  |     const submit = opts.submit ?? (() => contestPage.submitAndAwaitResult());
  96  | 
  97  |     let pickIds: string[] = [];
  98  |     let placed = false;
  99  |     let lastError: string | null = null;
  100 |     let statIdx = 0;
  101 |     // Players any prior attempt already tried. Passed to pickPlayers so each
  102 |     // retry selects genuinely new cards — the fix for a slip that keeps
  103 |     // tripping "multiple promos cannot be applied" on the same promo players.
  104 |     const triedPickIds = new Set<string>();
  105 |     // 429s are contention (parallel workers sharing one user), not a problem
  106 |     // with the picks — don't let them consume the stat-rotation attempts.
  107 |     // Bounded separately so a hard-stuck throttle still terminates.
  108 |     let throttleRetries = 0;
  109 |     const maxThrottleRetries = 8;
  110 | 
  111 |     for (let attempt = 1; attempt <= maxAttempts && !placed; attempt++) {
  112 |         // Reset after *any* failed attempt — keyed on lastError, not the attempt
  113 |         // counter, because a 429 refunds the attempt (attempt-- below) and the
  114 |         // loop re-enters at attempt === 1. Gating on `attempt > 1` skipped this
  115 |         // block on that path: no clearSlip, no backoff, and the still-open
  116 |         // submission sheet then intercepted every pick click (10s timeout
  117 |         // each) until the test timed out.
  118 |         if (lastError !== null) {
  119 |             // Always reset back to home — pickPlayers below needs the grid.
  120 |             // But only rotate the stat tab on a per-stat user limit. On a 429,
  121 |             // the picks were fine; rotating wastes stat tabs (we can run out
  122 |             // before the throttle window even closes), so we sleep instead.
  123 |             // A multiple-promo rejection isn't stat-specific either — the fresh
  124 |             // cards (via triedPickIds below) are what break the loop, so leave
  125 |             // the stat tab put.
  126 |             await homePage.clearSlip();
  127 |             if (isThrottleError(lastError)) {
  128 |                 await new Promise((r) => setTimeout(r, throttleBackoffMs(lastError)));
  129 |             } else if (!isMultiplePromoError(lastError)) {
  130 |                 statIdx++;
  131 |             }
  132 |         }
  133 |         await homePage.waitForPlayersGrid();
  134 |         try {
  135 |             pickIds = await homePage.pickPlayers(
  136 |                 pickCount,
  137 |                 attempt > 1 ? statIdx : undefined,
  138 |                 triedPickIds,
  139 |             );
  140 |         } catch (err) {
  141 |             const msg = err instanceof Error ? err.message : String(err);
  142 |             if (!isPickExhaustionError(msg)) throw err;
  143 |             // Dry pick pool on this stat tab — burn the attempt and let the
  144 |             // next iteration rotate to the next tab (clearSlip + statIdx++).
  145 |             lastError = msg;
  146 |             continue;
  147 |         }
  148 |         await homePage.enterFinalContestPage();
  149 |         await contestPage.verifyPage();
  150 |         await contestPage.setEntryAmountIfEditable(entryAmount);
  151 | 
  152 |         const result = await submit();
  153 |         if (!result.success) {
  154 |             lastError = result.error;
  155 | 
  156 |             // The account's rolling daily/weekly/monthly cap is exhausted —
  157 |             // no retry strategy can place an entry. Skip with the reason
  158 |             // rather than burning attempts and failing on account state.
  159 |             test.skip(
  160 |                 isAccountLimitError(result.error),
  161 |                 `Test user hit an account-level contest limit — cannot place entries (${result.error}). ` +
  162 |                     'Reset the user limits (POST /account/information/reset-limits/) or use a different TEST_USER.',
  163 |             );
  164 | 
  165 |             // On a throttle the picks themselves were fine — keep them reusable
  166 |             // and refund the attempt (bounded by maxThrottleRetries).
  167 |             if (isThrottleError(result.error)) {
  168 |                 if (throttleRetries++ < maxThrottleRetries) attempt--;
  169 |             } else {
  170 |                 for (const id of pickIds) triedPickIds.add(id);
  171 |             }
  172 |             continue;
  173 |         }
  174 |         placed = true;
  175 |     }
  176 | 
  177 |     expect(
  178 |         placed,
  179 |         `Could not place contest after ${maxAttempts} attempts (last error: ${lastError})` +
  180 |             (isPickExhaustionError(lastError)
  181 |                 ? " — every attempted stat tab ran out of selectable cards; the " +
  182 |                   "environment's offering is likely too thin for this pick count"
  183 |                 : ""),
> 184 |     ).toBe(true);
      |       ^ Error: Could not place contest after 5 attempts (last error: Could not select 5 valid picks) — every attempted stat tab ran out of selectable cards; the environment's offering is likely too thin for this pick count
  185 | 
  186 |     return { pickIds };
  187 | }
  188 | 
```