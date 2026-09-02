# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: entries/entry-card-redesign.spec.ts >> My Entries card redesign — cancel flow >> Freshly placed entry is cancellable with a live countdown, and confirming Cancel Entry removes it from Active and History (refund + hard delete)
- Location: tests/entries/entry-card-redesign.spec.ts:250:5

# Error details

```
Error: Could not place contest after 5 attempts (last error: 400 You have reached your limit for in-game contests for this match.)

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
          - generic [ref=e10]:
            - generic [ref=e12]:
              - generic [ref=e13]: $861.00
              - generic [ref=e14]:
                - img "gift-icon" [ref=e15]
                - text: "51.00"
            - button "Toggle Menu" [ref=e16]:
              - img [ref=e17]
      - main [ref=e19]:
        - generic [ref=e24]:
          - generic [ref=e25]:
            - generic [ref=e26]:
              - list [ref=e28]:
                - button "Live" [ref=e29] [cursor=pointer]:
                  - generic [ref=e33]: Live
                - button "MLB" [ref=e34] [cursor=pointer]
                - button "EPL" [ref=e35] [cursor=pointer]
                - button "MLS" [ref=e36] [cursor=pointer]
                - button "NFLSZN" [ref=e37] [cursor=pointer]
                - button "LaLiga" [ref=e38] [cursor=pointer]
                - button "UFC" [ref=e39] [cursor=pointer]
              - list [ref=e41]:
                - listitem [ref=e42]:
                  - button "ALL" [ref=e43] [cursor=pointer]:
                    - generic [ref=e44]: ALL
                - listitem [ref=e45]:
                  - button "MIL@CHC 7:40PM" [ref=e46] [cursor=pointer]:
                    - text: MIL@CHC
                    - generic [ref=e47]: 7:40PM
                - listitem [ref=e48]:
                  - button "MIA@KC 7:40PM" [ref=e49] [cursor=pointer]:
                    - text: MIA@KC
                    - generic [ref=e50]: 7:40PM
                - listitem [ref=e51]:
                  - button "DET@MIN 7:40PM" [ref=e52] [cursor=pointer]:
                    - text: DET@MIN
                    - generic [ref=e53]: 7:40PM
                - listitem [ref=e54]:
                  - button "OAK@TEX 8:05PM" [ref=e55] [cursor=pointer]:
                    - text: OAK@TEX
                    - generic [ref=e56]: 8:05PM
                - listitem [ref=e57]:
                  - button "CWS@HOU 8:10PM" [ref=e58] [cursor=pointer]:
                    - text: CWS@HOU
                    - generic [ref=e59]: 8:10PM
                - listitem [ref=e60]:
                  - button "BAL@COL 8:40PM" [ref=e61] [cursor=pointer]:
                    - text: BAL@COL
                    - generic [ref=e62]: 8:40PM
                - listitem [ref=e63]:
                  - button "NYY@LAA 9:38PM" [ref=e64] [cursor=pointer]:
                    - text: NYY@LAA
                    - generic [ref=e65]: 9:38PM
                - listitem [ref=e66]:
                  - button "PHI@ARI 9:40PM" [ref=e67] [cursor=pointer]:
                    - text: PHI@ARI
                    - generic [ref=e68]: 9:40PM
                - listitem [ref=e69]:
                  - button "STL@LAD 10:10PM" [ref=e70] [cursor=pointer]:
                    - text: STL@LAD
                    - generic [ref=e71]: 10:10PM
              - generic [ref=e72]:
                - generic [ref=e73]:
                  - generic [ref=e76]:
                    - generic:
                      - img
                    - textbox "Search player or team" [ref=e77]
                  - button "Change card style from grid" [ref=e79]
                - list [ref=e81]:
                  - listitem [ref=e82]:
                    - button "Strikeouts (K)" [ref=e83]
                  - listitem [ref=e84]:
                    - button "Hits" [ref=e85]
                  - listitem [ref=e86]:
                    - button "Hits + Runs + RBIs" [ref=e87]
                  - listitem [ref=e88]:
                    - button "Singles" [ref=e89]
                  - listitem [ref=e90]:
                    - button "Doubles" [ref=e91]
                  - listitem [ref=e92]:
                    - button "Triples" [ref=e93]
                  - listitem [ref=e94]:
                    - button "Runs" [ref=e95]
                  - listitem [ref=e96]:
                    - button "RBIs" [ref=e97]
                  - listitem [ref=e98]:
                    - button "Hits Allowed" [ref=e99]
                  - listitem [ref=e100]:
                    - button "Pitching Outs" [ref=e101]
                  - listitem [ref=e102]:
                    - button "Pitches Thrown" [ref=e103]
                  - listitem [ref=e104]:
                    - button "Earned Runs" [ref=e105]
                  - listitem [ref=e106]:
                    - button "Homeruns" [ref=e107]
                  - listitem [ref=e108]:
                    - button "Total Bases" [ref=e109]
                  - listitem [ref=e110]:
                    - button "Strikeouts" [ref=e111]
                  - listitem [ref=e112]:
                    - button "Fantasy Points" [ref=e113]
            - generic [ref=e114]:
              - generic [ref=e119]:
                - generic [ref=e122] [cursor=pointer]:
                  - generic [ref=e123]:
                    - generic [ref=e124]:
                      - generic [ref=e125]: 100%
                      - generic [ref=e126]: Deposit Match
                    - generic [ref=e127]: New User Promotion
                  - button "Deposit" [ref=e129]
                - generic [ref=e133] [cursor=pointer]:
                  - generic [ref=e134]: Pull real graded cards worth up to $10,000
                  - generic [ref=e135]: Sell or ship instantly
                  - button "Rip a pack" [ref=e136]:
                    - generic [ref=e137]:
                      - img [ref=e138]
                      - text: Rip a pack
                - generic [ref=e143] [cursor=pointer]:
                  - generic [ref=e144]:
                    - generic [ref=e145]: Refer a friend, get a $20 Free Entry
                    - generic [ref=e146]: Referral bonus
                  - button "Refer" [ref=e147]
                - generic [ref=e150] [cursor=pointer]:
                  - generic [ref=e151]:
                    - generic [ref=e152]:
                      - img [ref=e153]
                      - generic [ref=e157]: Boosted Picks
                    - generic [ref=e158]: "Every Pick Pays: Up to a 35% Boost!"
                  - button "Details" [ref=e160]
              - generic [ref=e164]:
                - generic [ref=e167]:
                  - generic [ref=e170]:
                    - button "Open expert opinion for Brice Turang" [ref=e171]:
                      - img [ref=e172]
                    - img "Brice Turang" [ref=e175]
                  - generic [ref=e176]:
                    - generic [ref=e177]: Brice Turang
                    - button "0.5 Doubles" [ref=e178]:
                      - generic [ref=e179]:
                        - img [ref=e180]
                        - img [ref=e182]
                      - generic [ref=e184]: "0.5"
                      - generic [ref=e185]: Doubles
                    - generic [ref=e186]:
                      - generic [ref=e187]: MIL@CHC
                      - generic [ref=e188]:
                        - img "clock" [ref=e189]
                        - text: 37:43
                    - generic [ref=e190]:
                      - button "Select over 0.5 Doubles for 1.06 times" [ref=e191]:
                        - img [ref=e192]
                        - generic [ref=e194]: 1.06x
                      - button "Select over 0.5 Doubles for 4.32 times" [ref=e195]:
                        - generic [ref=e196]: 4.32x
                        - img [ref=e197]
                - generic [ref=e201]:
                  - generic [ref=e204]:
                    - button "Open expert opinion for William Contreras" [ref=e205]:
                      - img [ref=e206]
                    - img "William Contreras" [ref=e209]
                  - generic [ref=e210]:
                    - generic [ref=e211]: W. Contreras
                    - button "0.5 Doubles" [ref=e212]:
                      - generic [ref=e213]:
                        - img [ref=e214]
                        - img [ref=e216]
                      - generic [ref=e218]: "0.5"
                      - generic [ref=e219]: Doubles
                    - generic [ref=e220]:
                      - generic [ref=e221]: MIL@CHC
                      - generic [ref=e222]:
                        - img "clock" [ref=e223]
                        - text: 37:43
                    - generic [ref=e224]:
                      - button "Select over 0.5 Doubles for 1.08 times" [ref=e225]:
                        - img [ref=e226]
                        - img [ref=e230]
                        - generic [ref=e232]: 1.08x
                      - button "Select over 0.5 Doubles for 4 times" [ref=e233]:
                        - generic [ref=e234]: 4x
                        - img [ref=e235]
                - generic [ref=e239]:
                  - generic [ref=e242]:
                    - button "Open expert opinion for Joseph Ortiz" [ref=e243]:
                      - img [ref=e244]
                    - img "Joseph Ortiz" [ref=e247]
                  - generic [ref=e248]:
                    - generic [ref=e249]: Joseph Ortiz
                    - button "0.5 Doubles" [ref=e250]:
                      - generic [ref=e251]:
                        - img [ref=e252]
                        - img [ref=e254]
                      - generic [ref=e256]: "0.5"
                      - generic [ref=e257]: Doubles
                    - generic [ref=e258]:
                      - generic [ref=e259]: MIL@CHC
                      - generic [ref=e260]:
                        - img "clock" [ref=e261]
                        - text: 37:43
                    - generic [ref=e262]:
                      - button "Select over 0.5 Doubles for 0 times" [disabled] [ref=e263]
                      - button "Select over 0.5 Doubles for 4.68 times" [ref=e265]:
                        - img [ref=e268]
                        - generic [ref=e270]: 4.68x
                        - img [ref=e271]
                - generic [ref=e275]:
                  - generic [ref=e278]:
                    - button "Open expert opinion for Jackson Chourio" [ref=e279]:
                      - img [ref=e280]
                    - img "Jackson Chourio" [ref=e283]
                  - generic [ref=e284]:
                    - generic [ref=e285]: J. Chourio
                    - button "0.5 Doubles" [ref=e286]:
                      - generic [ref=e287]:
                        - img [ref=e288]
                        - img [ref=e290]
                      - generic [ref=e292]: "0.5"
                      - generic [ref=e293]: Doubles
                    - generic [ref=e294]:
                      - generic [ref=e295]: MIL@CHC
                      - generic [ref=e296]:
                        - img "clock" [ref=e297]
                        - text: 37:43
                    - generic [ref=e298]:
                      - button "Select over 0.5 Doubles for 1.11 times" [ref=e299]:
                        - img [ref=e300]
                        - generic [ref=e302]: 1.11x
                      - button "Select over 0.5 Doubles for 3.76 times" [ref=e303]:
                        - generic [ref=e304]: 3.76x
                        - img [ref=e305]
                - generic [ref=e309]:
                  - generic [ref=e312]:
                    - button "Open expert opinion for Jake Bauers" [ref=e313]:
                      - img [ref=e314]
                    - img "Jake Bauers" [ref=e317]
                  - generic [ref=e318]:
                    - generic [ref=e319]: Jake Bauers
                    - button "0.5 Doubles" [ref=e320]:
                      - generic [ref=e321]:
                        - img [ref=e322]
                        - img [ref=e324]
                      - generic [ref=e326]: "0.5"
                      - generic [ref=e327]: Doubles
                    - generic [ref=e328]:
                      - generic [ref=e329]: MIL@CHC
                      - generic [ref=e330]:
                        - img "clock" [ref=e331]
                        - text: 37:43
                    - generic [ref=e332]:
                      - button "Select over 0.5 Doubles for 1.06 times" [ref=e333]:
                        - img [ref=e334]
                        - generic [ref=e336]: 1.06x
                      - button "Select over 0.5 Doubles for 4.56 times" [ref=e337]:
                        - generic [ref=e338]: 4.56x
                        - img [ref=e339]
                - generic [ref=e343]:
                  - generic [ref=e346]:
                    - button "Open expert opinion for Andrew Vaughn" [ref=e347]:
                      - img [ref=e348]
                    - img "Andrew Vaughn" [ref=e351]
                  - generic [ref=e352]:
                    - generic [ref=e353]: Andrew Vaughn
                    - button "0.5 Doubles" [ref=e354]:
                      - generic [ref=e355]:
                        - img [ref=e356]
                        - img [ref=e358]
                      - generic [ref=e360]: "0.5"
                      - generic [ref=e361]: Doubles
                    - generic [ref=e362]:
                      - generic [ref=e363]: MIL@CHC
                      - generic [ref=e364]:
                        - img "clock" [ref=e365]
                        - text: 37:43
                    - generic [ref=e366]:
                      - button "Select over 0.5 Doubles for 1.07 times" [ref=e367]:
                        - img [ref=e368]
                        - generic [ref=e370]: 1.07x
                      - button "Select over 0.5 Doubles for 4.26 times" [ref=e371]:
                        - generic [ref=e372]: 4.26x
                        - img [ref=e373]
                - generic [ref=e377]:
                  - generic [ref=e380]:
                    - button "Open expert opinion for Pete Crow-Armstrong" [ref=e381]:
                      - img [ref=e382]
                    - img "Pete Crow-Armstrong" [ref=e385]
                  - generic [ref=e386]:
                    - generic [ref=e387]: P. Crow-Armstrong
                    - button "0.5 Doubles" [ref=e388]:
                      - generic [ref=e389]:
                        - img [ref=e390]
                        - img [ref=e392]
                      - generic [ref=e394]: "0.5"
                      - generic [ref=e395]: Doubles
                    - generic [ref=e396]:
                      - generic [ref=e397]: MIL@CHC
                      - generic [ref=e398]:
                        - img "clock" [ref=e399]
                        - text: 37:43
                    - generic [ref=e400]:
                      - button "Select over 0.5 Doubles for 1.07 times" [ref=e401]:
                        - img [ref=e402]
                        - generic [ref=e404]: 1.07x
                      - button "Select over 0.5 Doubles for 4.2 times" [ref=e405]:
                        - generic [ref=e406]: 4.2x
                        - img [ref=e407]
                - generic [ref=e411]:
                  - generic [ref=e414]:
                    - button "Open expert opinion for Seiya Suzuki" [ref=e415]:
                      - img [ref=e416]
                    - img "Seiya Suzuki" [ref=e419]
                  - generic [ref=e420]:
                    - generic [ref=e421]: Seiya Suzuki
                    - button "0.5 Doubles" [ref=e422]:
                      - generic [ref=e423]:
                        - img [ref=e424]
                        - img [ref=e426]
                      - generic [ref=e428]: "0.5"
                      - generic [ref=e429]: Doubles
                    - generic [ref=e430]:
                      - generic [ref=e431]: MIL@CHC
                      - generic [ref=e432]:
                        - img "clock" [ref=e433]
                        - text: 37:43
                    - generic [ref=e434]:
                      - button "Select over 0.5 Doubles for 1.11 times" [ref=e435]:
                        - img [ref=e436]
                        - generic [ref=e438]: 1.11x
                      - button "Select over 0.5 Doubles for 3.84 times" [ref=e439]:
                        - generic [ref=e440]: 3.84x
                        - img [ref=e441]
            - generic [ref=e444]:
              - img [ref=e446]
              - generic [ref=e448]:
                - generic [ref=e450]:
                  - generic [ref=e451]: 18.2x
                  - generic [ref=e452]: 19.11x
                - generic [ref=e453]:
                  - button "+ 10% Boost 🚀" [ref=e459]:
                    - generic [ref=e460]: + 10% Boost 🚀
                  - generic [ref=e470]: "Add 4th Pick: 10% Boost"
              - button "Continue" [ref=e471] [cursor=pointer]
            - generic [ref=e473]:
              - generic [ref=e474]:
                - button [ref=e475]:
                  - img [ref=e476]
                - generic [ref=e478]: Make Your More/Less Picks
              - generic [ref=e479]:
                - generic [ref=e481]:
                  - img "Jackson Merrill" [ref=e483]
                  - generic [ref=e484]:
                    - paragraph [ref=e485]: Jackson Merrill
                    - paragraph [ref=e486]:
                      - generic [ref=e487]: SD
                      - text: "- CIN"
                    - paragraph [ref=e488]: Today 6:40 PM
                  - generic [ref=e489]:
                    - paragraph [ref=e490]:
                      - text: "0.5"
                      - generic [ref=e491]: Doubles
                    - generic [ref=e492]:
                      - button "Less" [disabled] [ref=e493]:
                        - generic [ref=e494]: Less
                      - button "More 4.8 x" [ref=e495]:
                        - generic [ref=e496]: More
                        - generic [ref=e497]: 4.8 x
                  - button [ref=e498]:
                    - img [ref=e499]
                - generic [ref=e503]:
                  - img "William Contreras" [ref=e505]
                  - generic [ref=e506]:
                    - paragraph [ref=e507]: William Contreras
                    - paragraph [ref=e508]:
                      - generic [ref=e509]: MIL
                      - text: "- CHC"
                    - paragraph [ref=e510]: Today 7:40 PM
                  - generic [ref=e511]:
                    - paragraph [ref=e512]:
                      - text: "0.5"
                      - generic [ref=e513]: Doubles
                    - generic [ref=e514]:
                      - button "Less 1.08 x" [ref=e515]:
                        - generic [ref=e516]: Less
                        - generic [ref=e517]: 1.08 x
                      - button "More 4 x" [ref=e518]:
                        - generic [ref=e519]: More
                        - generic [ref=e520]: 4 x
                  - button [ref=e521]:
                    - img [ref=e522]
                - generic [ref=e526]:
                  - img "Joseph Ortiz" [ref=e528]
                  - generic [ref=e529]:
                    - paragraph [ref=e530]: Joseph Ortiz
                    - paragraph [ref=e531]:
                      - generic [ref=e532]: MIL
                      - text: "- CHC"
                    - paragraph [ref=e533]: Today 7:40 PM
                  - generic [ref=e534]:
                    - paragraph [ref=e535]:
                      - text: "0.5"
                      - generic [ref=e536]: Doubles
                    - generic [ref=e537]:
                      - button "Less" [disabled] [ref=e538]:
                        - generic [ref=e539]: Less
                      - button "More 4.68 x" [ref=e540]:
                        - generic [ref=e541]: More
                        - generic [ref=e542]: 4.68 x
                  - button [ref=e543]:
                    - img [ref=e544]
                - button "Add Icon Add Player Add 1 More Pick for a 10% Boost Boost Icon" [ref=e548]:
                  - generic [ref=e549]:
                    - img "Add Icon" [ref=e551]
                    - generic [ref=e552]: Add Player
                  - generic [ref=e553]:
                    - generic [ref=e554]: Add 1 More Pick for a 10% Boost
                    - img "Boost Icon" [ref=e556]
              - generic [ref=e558]:
                - generic [ref=e559]:
                  - generic [ref=e561]:
                    - radio
                    - generic [ref=e562] [cursor=pointer]: $25
                    - radio
                    - generic [ref=e563] [cursor=pointer]: $75
                    - radio
                    - generic [ref=e564] [cursor=pointer]: $300
                  - generic [ref=e566]:
                    - generic [ref=e567]: $
                    - spinbutton [ref=e571]: "3"
                  - button "51" [ref=e572] [cursor=pointer]:
                    - img [ref=e573]
                    - generic [ref=e575]: "51"
                - generic [ref=e576]:
                  - generic [ref=e577]:
                    - generic [ref=e578]:
                      - button "Insured" [ref=e579]
                      - button "All In" [ref=e580]
                    - generic [ref=e581]:
                      - generic [ref=e582]: 18.2x
                      - generic [ref=e583]: 19.11x
                  - generic [ref=e585]:
                    - generic [ref=e586]:
                      - paragraph [ref=e587]: Perfect line-up
                      - paragraph [ref=e588]: $57.33
                    - generic [ref=e590]:
                      - paragraph [ref=e591]: Or 1st place in group
                      - generic [ref=e592]: $1 + $57.33
                - button "Place" [active] [ref=e596] [cursor=pointer]:
                  - text: Place
                  - img [ref=e597]
          - generic [ref=e600]:
            - generic [ref=e602]:
              - link "Download ParlayPlay On The Play Store" [ref=e603] [cursor=pointer]:
                - /url: https://parlayplay.onelink.me/oLJk/fh7u6juo
                - img "Download ParlayPlay On The Play Store" [ref=e604]
              - paragraph [ref=e605]:
                - text: Get the app.
                - text: Better. Faster. Convenient
            - navigation [ref=e606]:
              - link "Privacy" [ref=e607] [cursor=pointer]:
                - /url: /privacy-policy
              - link "Fantasy Terms" [ref=e608] [cursor=pointer]:
                - /url: /terms
              - link "Packs Terms" [ref=e609] [cursor=pointer]:
                - /url: /terms/packs
              - link "Responsible Gaming" [ref=e610] [cursor=pointer]:
                - /url: /responsible-gaming
              - link "Gaming Rules" [ref=e611] [cursor=pointer]:
                - /url: /rules
              - link "FAQ" [ref=e612] [cursor=pointer]:
                - /url: https://intercom.help/parlayplay/en/
            - navigation [ref=e613]:
              - generic [ref=e614]:
                - paragraph [ref=e615]: © ParlayPlay 2026
                - generic [ref=e616]:
                  - link "ParlayPlay on Facebook" [ref=e617] [cursor=pointer]:
                    - /url: https://www.facebook.com/parlayplay.io
                    - img [ref=e618]
                  - link "ParlayPlay on Instagram" [ref=e620] [cursor=pointer]:
                    - /url: https://www.instagram.com/parlayplay_?igsh=bHBldWQyMmV2b3Y4
                    - img [ref=e621]
                  - link "ParlayPlay on Twitter" [ref=e623] [cursor=pointer]:
                    - /url: https://www.twitter.com/parlay_play
                    - img [ref=e624]
                  - link "ParlayPlay on Discord" [ref=e626] [cursor=pointer]:
                    - /url: https://discord.com/invite/parlayplay
                    - img [ref=e627]
                - img "18+ icon" [ref=e629]
            - paragraph [ref=e631]
    - generic:
      - region "Notifications Alt+T":
        - alert [ref=e633] [cursor=pointer]:
          - img [ref=e635]
          - text: You have reached your limit for in-game contests for this match.
          - button "close" [ref=e637]:
            - img [ref=e638]
          - progressbar "notification timer" [ref=e642]
  - alert [ref=e643]
  - iframe [ref=e644]:
    
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
      |       ^ Error: Could not place contest after 5 attempts (last error: 400 You have reached your limit for in-game contests for this match.)
  185 | 
  186 |     return { pickIds };
  187 | }
  188 | 
```