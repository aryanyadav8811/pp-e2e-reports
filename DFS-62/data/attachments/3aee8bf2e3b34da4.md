# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: slip_sharing/tail_feed.spec.ts >> Tail Feed >> Share toggle OFF — newly-placed contest does NOT appear on the You tab
- Location: tests/slip_sharing/tail_feed.spec.ts:135:5

# Error details

```
Error: Could not place contest after 5 attempts (last error: 400 Entering this contest will cause you to exceed your daily contest limit.)

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
          - link "Parlay Play LogoParlay Play text" [ref=e6] [cursor=pointer]:
            - /url: /
            - generic [ref=e7]:
              - img "Parlay Play Logo" [ref=e8]
              - img "Parlay Play text" [ref=e9]
          - generic [ref=e10]:
            - button "Switch to dark mode" [ref=e11]:
              - img [ref=e12]
            - generic [ref=e14]:
              - generic [ref=e16]:
                - generic [ref=e17]: $97.99
                - generic [ref=e18]:
                  - img "gift-icon" [ref=e19]
                  - text: "51.00"
              - button "Toggle Menu" [ref=e20]:
                - img [ref=e21]
      - main [ref=e23]:
        - generic [ref=e24]:
          - generic [ref=e26]:
            - generic [ref=e27]:
              - generic [ref=e28]:
                - list [ref=e30]:
                  - button "NBA" [ref=e31] [cursor=pointer]
                  - button "NBA-Combos" [ref=e32] [cursor=pointer]
                  - button "NBA Q1" [ref=e33] [cursor=pointer]
                  - button "MLB" [ref=e34] [cursor=pointer]
                  - button "MLB-Combos" [ref=e35] [cursor=pointer]
                  - button "NHL" [ref=e36] [cursor=pointer]
                  - button "UCL" [ref=e37] [cursor=pointer]
                  - button "CSGO" [ref=e38] [cursor=pointer]
                  - button "Valorant" [ref=e39] [cursor=pointer]
                  - button "Cricket" [ref=e40] [cursor=pointer]
                  - button "UFC" [ref=e41] [cursor=pointer]
                - list [ref=e43]:
                  - listitem [ref=e44]:
                    - button "ALL" [ref=e45] [cursor=pointer]:
                      - generic [ref=e46]: ALL
                  - listitem [ref=e47]:
                    - button "SAS@OKC Sat 8PM" [ref=e48] [cursor=pointer]:
                      - text: SAS@OKC
                      - generic [ref=e49]: Sat 8PM
                - generic [ref=e50]:
                  - generic [ref=e51]:
                    - generic [ref=e54]:
                      - img [ref=e56]
                      - textbox "Search player or team" [ref=e58]
                    - button "Change card style from grid" [ref=e60]
                  - list [ref=e62]:
                    - listitem [ref=e63]:
                      - button "Points" [ref=e64]
                    - listitem [ref=e65]:
                      - button "Rebounds" [ref=e66]
                    - listitem [ref=e67]:
                      - button "Assists" [ref=e68]
                    - listitem [ref=e69]:
                      - button "Triple Double" [ref=e70]
                    - listitem [ref=e71]:
                      - button "3PT Made" [ref=e72]
                    - listitem [ref=e73]:
                      - button "Pts + Reb + Ast" [ref=e74]
                    - listitem [ref=e75]:
                      - button "Double Double" [ref=e76]
                    - listitem [ref=e77]:
                      - button "Pts + Reb" [ref=e78]
                    - listitem [ref=e79]:
                      - button "Pts + Ast" [ref=e80]
                    - listitem [ref=e81]:
                      - button "Reb + Ast" [ref=e82]
                    - listitem [ref=e83]:
                      - button "Stl + Blk" [ref=e84]
                    - listitem [ref=e85]:
                      - button "3PT Attempted" [ref=e86]
                    - listitem [ref=e87]:
                      - button "FT Made" [ref=e88]
                    - listitem [ref=e89]:
                      - button "FG Made" [ref=e90]
                    - listitem [ref=e91]:
                      - button "FG Attempted" [ref=e92]
                    - listitem [ref=e93]:
                      - button "First Point Scorer" [ref=e94]
                    - listitem [ref=e95]:
                      - button "Steals" [ref=e96]
                    - listitem [ref=e97]:
                      - button "Blocks" [ref=e98]
                    - listitem [ref=e99]:
                      - button "Turnovers" [ref=e100]
              - generic [ref=e101]:
                - generic [ref=e105]:
                  - button "previous slide / item" [ref=e106] [cursor=pointer]:
                    - img [ref=e107]
                  - list [ref=e110]:
                    - listitem [ref=e111]:
                      - generic [ref=e113] [cursor=pointer]:
                        - img "huddle-bg-small"
                        - generic [ref=e114]:
                          - generic [ref=e115]:
                            - generic [ref=e116]: Pistons
                            - generic [ref=e119]: VS
                            - generic [ref=e120]: Magic
                          - generic [ref=e121]: Huddle
                          - generic [ref=e122]:
                            - generic [ref=e123]:
                              - generic [ref=e124]:
                                - text: Win
                                - generic [ref=e125]: $1000
                              - generic [ref=e126]: + many more prizes
                            - button "Enter" [ref=e128]
                    - listitem [ref=e129]:
                      - 'button "Boosted Picks 🚀 Every Pick Pays: Up to a 35% Boost! lightning-bolt-yellow" [ref=e130] [cursor=pointer]':
                        - generic [ref=e131]:
                          - generic [ref=e133]: Boosted Picks 🚀
                          - generic [ref=e134]: "Every Pick Pays: Up to a 35% Boost!"
                        - img "lightning-bolt-yellow"
                    - listitem [ref=e135]:
                      - button "Get $20 By referring a friend making a first $10 deposit. lightning-bolt-yellow" [ref=e136] [cursor=pointer]:
                        - generic [ref=e137]:
                          - generic [ref=e139]: Get $20
                          - generic [ref=e140]: By referring a friend making a first $10 deposit.
                        - img "lightning-bolt-yellow"
                    - listitem [ref=e141]:
                      - generic [ref=e143] [cursor=pointer]:
                        - img "huddle-bg-small"
                        - generic [ref=e144]:
                          - generic [ref=e145]:
                            - generic [ref=e146]: Pistons
                            - generic [ref=e149]: VS
                            - generic [ref=e150]: Magic
                          - generic [ref=e151]: Huddle
                          - generic [ref=e152]:
                            - generic [ref=e153]:
                              - generic [ref=e154]:
                                - text: Win
                                - generic [ref=e155]: $1000
                              - generic [ref=e156]: + many more prizes
                            - button "Enter" [ref=e158]
                    - listitem [ref=e159]:
                      - 'button "Boosted Picks 🚀 Every Pick Pays: Up to a 35% Boost! lightning-bolt-yellow" [ref=e160] [cursor=pointer]':
                        - generic [ref=e161]:
                          - generic [ref=e163]: Boosted Picks 🚀
                          - generic [ref=e164]: "Every Pick Pays: Up to a 35% Boost!"
                        - img "lightning-bolt-yellow"
                  - button "next slide / item" [ref=e165] [cursor=pointer]:
                    - img [ref=e166]
                - generic [ref=e168]:
                  - generic [ref=e171]:
                    - generic [ref=e174]:
                      - button "Open expert opinion for De'Aaron Fox" [ref=e175]:
                        - img [ref=e176]
                      - img "De'Aaron Fox" [ref=e179]
                    - generic [ref=e180]:
                      - generic [ref=e181]: De'Aaron Fox
                      - button "5.5 Assists" [ref=e182]:
                        - generic [ref=e183]:
                          - img [ref=e184]
                          - img [ref=e186]
                        - generic [ref=e188]: "5.5"
                        - generic [ref=e189]: Assists
                      - generic [ref=e190]:
                        - generic [ref=e191]: SAS@OKC
                        - generic [ref=e192]: Sat 8PM
                      - generic [ref=e193]:
                        - button "Select over 5.5 Assists for 1.82 times" [ref=e194]:
                          - img [ref=e195]
                          - generic [ref=e197]: 1.82x
                        - button "Select over 5.5 Assists for 1.8 times" [ref=e198]:
                          - generic [ref=e199]: 1.8x
                          - img [ref=e200]
                  - generic [ref=e204]:
                    - generic [ref=e207]:
                      - button "Open expert opinion for Dylan Harper" [ref=e208]:
                        - img [ref=e209]
                      - img "Dylan Harper" [ref=e212]
                    - generic [ref=e213]:
                      - generic [ref=e214]: Dylan Harper
                      - button "2.5 Assists" [ref=e215]:
                        - generic [ref=e216]:
                          - img [ref=e217]
                          - img [ref=e219]
                        - generic [ref=e221]: "2.5"
                        - generic [ref=e222]: Assists
                      - generic [ref=e223]:
                        - generic [ref=e224]: SAS@OKC
                        - generic [ref=e225]: Sat 8PM
                      - generic [ref=e226]:
                        - button "Select over 2.5 Assists for 1.86 times" [ref=e227]:
                          - img [ref=e228]
                          - generic [ref=e230]: 1.86x
                        - button "Select over 2.5 Assists for 1.76 times" [ref=e231]:
                          - generic [ref=e232]: 1.76x
                          - img [ref=e233]
                  - generic [ref=e237]:
                    - generic [ref=e240]:
                      - button "Open expert opinion for Devin Vassell" [ref=e241]:
                        - img [ref=e242]
                      - img "Devin Vassell" [ref=e245]
                    - generic [ref=e246]:
                      - generic [ref=e247]: Devin Vassell
                      - button "2.5 Assists" [ref=e248]:
                        - generic [ref=e249]:
                          - img [ref=e250]
                          - img [ref=e252]
                        - generic [ref=e254]: "2.5"
                        - generic [ref=e255]: Assists
                      - generic [ref=e256]:
                        - generic [ref=e257]: SAS@OKC
                        - generic [ref=e258]: Sat 8PM
                      - generic [ref=e259]:
                        - button "Select over 2.5 Assists for 1.49 times" [ref=e260]:
                          - img [ref=e261]
                          - img [ref=e265]
                          - generic [ref=e267]: 1.49x
                        - button "Select over 2.5 Assists for 2.22 times" [ref=e268]:
                          - generic [ref=e269]: 2.22x
                          - img [ref=e270]
                  - generic [ref=e274]:
                    - generic [ref=e277]:
                      - button "Open expert opinion for Stephon Castle" [ref=e278]:
                        - img [ref=e279]
                      - img "Stephon Castle" [ref=e282]
                    - generic [ref=e283]:
                      - generic [ref=e284]: S. Castle
                      - button "6.5 Assists" [ref=e285]:
                        - generic [ref=e286]:
                          - img [ref=e287]
                          - img [ref=e289]
                        - generic [ref=e291]: "6.5"
                        - generic [ref=e292]: Assists
                      - generic [ref=e293]:
                        - generic [ref=e294]: SAS@OKC
                        - generic [ref=e295]: Sat 8PM
                      - generic [ref=e296]:
                        - button "Select over 6.5 Assists for 2.03 times" [ref=e297]:
                          - img [ref=e298]
                          - generic [ref=e300]: 2.03x
                        - button "Select over 6.5 Assists for 1.58 times" [ref=e301]:
                          - generic [ref=e302]: 1.58x
                          - img [ref=e303]
                  - generic [ref=e307]:
                    - generic [ref=e310]:
                      - button "Open expert opinion for Victor Wembanyama" [ref=e311]:
                        - img [ref=e312]
                      - img "Victor Wembanyama" [ref=e315]
                    - generic [ref=e316]:
                      - generic [ref=e317]: V. Wembanyama
                      - button "3.5 Assists" [ref=e318]:
                        - generic [ref=e319]:
                          - img [ref=e320]
                          - img [ref=e322]
                        - generic [ref=e324]: "3.5"
                        - generic [ref=e325]: Assists
                      - generic [ref=e326]:
                        - generic [ref=e327]: SAS@OKC
                        - generic [ref=e328]: Sat 8PM
                      - generic [ref=e329]:
                        - button "Select over 3.5 Assists for 1.54 times" [ref=e330]:
                          - img [ref=e331]
                          - generic [ref=e333]: 1.54x
                        - button "Select over 3.5 Assists for 2.12 times" [ref=e334]:
                          - generic [ref=e335]: 2.12x
                          - img [ref=e336]
                  - generic [ref=e340]:
                    - generic [ref=e343]:
                      - button "Open expert opinion for Keldon Johnson" [ref=e344]:
                        - img [ref=e345]
                      - img "Keldon Johnson" [ref=e348]
                    - generic [ref=e349]:
                      - generic [ref=e350]: K. Johnson
                      - button "0.5 Assists" [ref=e351]:
                        - generic [ref=e352]:
                          - img [ref=e353]
                          - img [ref=e355]
                        - generic [ref=e357]: "0.5"
                        - generic [ref=e358]: Assists
                      - generic [ref=e359]:
                        - generic [ref=e360]: SAS@OKC
                        - generic [ref=e361]: Sat 8PM
                      - generic [ref=e362]:
                        - button "Select over 0.5 Assists for 1.99 times" [ref=e363]:
                          - img [ref=e364]
                          - generic [ref=e366]: 1.99x
                        - button "Select over 0.5 Assists for 1.65 times" [ref=e367]:
                          - generic [ref=e368]: 1.65x
                          - img [ref=e369]
                  - generic [ref=e373]:
                    - generic [ref=e376]:
                      - button "Open expert opinion for Julian Champagnie" [ref=e377]:
                        - img [ref=e378]
                      - img "Julian Champagnie" [ref=e381]
                    - generic [ref=e382]:
                      - generic [ref=e383]: J. Champagnie
                      - button "1.5 Assists" [ref=e384]:
                        - generic [ref=e385]:
                          - img [ref=e386]
                          - img [ref=e388]
                        - generic [ref=e390]: "1.5"
                        - generic [ref=e391]: Assists
                      - generic [ref=e392]:
                        - generic [ref=e393]: SAS@OKC
                        - generic [ref=e394]: Sat 8PM
                      - generic [ref=e395]:
                        - button "Select over 1.5 Assists for 1.6 times" [ref=e396]:
                          - img [ref=e397]
                          - generic [ref=e399]: 1.6x
                        - button "Select over 1.5 Assists for 2.05 times" [ref=e400]:
                          - generic [ref=e401]: 2.05x
                          - img [ref=e402]
                  - generic [ref=e406]:
                    - generic [ref=e409]:
                      - button "Open expert opinion for Shai Gilgeous-Alexander" [ref=e410]:
                        - img [ref=e411]
                      - img "Shai Gilgeous-Alexander" [ref=e414]
                    - generic [ref=e415]:
                      - generic [ref=e416]: S. Gilgeous-Alexander
                      - button "7.5 Assists" [ref=e417]:
                        - generic [ref=e418]:
                          - img [ref=e419]
                          - img [ref=e421]
                        - generic [ref=e423]: "7.5"
                        - generic [ref=e424]: Assists
                      - generic [ref=e425]:
                        - generic [ref=e426]: SAS@OKC
                        - generic [ref=e427]: Sat 8PM
                      - generic [ref=e428]:
                        - button "Select over 7.5 Assists for 1.96 times" [ref=e429]:
                          - img [ref=e430]
                          - img [ref=e434]
                          - generic [ref=e436]: 1.96x
                        - button "Select over 7.5 Assists for 1.66 times" [ref=e437]:
                          - generic [ref=e438]: 1.66x
                          - img [ref=e439]
              - generic [ref=e505]:
                - generic [ref=e506]:
                  - img [ref=e508]
                  - generic [ref=e510]:
                    - generic [ref=e511]: 2.73x
                    - generic [ref=e512]:
                      - button "+ 5% Boost 🚀" [ref=e517]:
                        - generic [ref=e518]: + 5% Boost 🚀
                      - generic [ref=e529]: "Add 3rd Pick: 5% Boost"
                  - button "Continue" [ref=e530] [cursor=pointer]
                - generic [ref=e531]:
                  - generic [ref=e532]:
                    - generic [ref=e533]: Your Selection
                    - generic [ref=e534]:
                      - generic [ref=e535]:
                        - generic [ref=e536]:
                          - img [ref=e537]
                          - generic [ref=e539]:
                            - text: D. Vassell (2.5 Assists - Less - FG)
                            - generic [ref=e540]: 1.49x
                        - img [ref=e542]
                      - generic [ref=e544]:
                        - generic [ref=e545]:
                          - img [ref=e546]
                          - generic [ref=e548]:
                            - text: S. Gilgeous-Alexander (7.5 Assists - Less - FG)
                            - generic [ref=e549]: 1.96x
                        - img [ref=e551]
                  - generic [ref=e553]:
                    - img [ref=e554]
                    - generic [ref=e556]: Clear All
              - generic [ref=e558]:
                - generic [ref=e559]:
                  - button [ref=e560]:
                    - img [ref=e561]
                  - generic [ref=e563]: Make Your More/Less Picks
                - generic [ref=e564]:
                  - generic [ref=e566]:
                    - img "Devin Vassell" [ref=e568]
                    - generic [ref=e569]:
                      - paragraph [ref=e570]: Devin Vassell
                      - paragraph [ref=e571]:
                        - generic [ref=e572]: SAS
                        - text: "- OKC"
                      - paragraph [ref=e573]: May 30th 8:10 PM
                    - generic [ref=e574]:
                      - paragraph [ref=e575]:
                        - text: "2.5"
                        - generic [ref=e576]: Assists
                      - generic [ref=e577]:
                        - button "Less 1.49 x" [ref=e578]:
                          - generic [ref=e579]: Less
                          - generic [ref=e580]: 1.49 x
                        - button "More 2.22 x" [ref=e581]:
                          - generic [ref=e582]: More
                          - generic [ref=e583]: 2.22 x
                    - button [ref=e584]:
                      - img [ref=e585]
                  - generic [ref=e589]:
                    - img "Shai Gilgeous-Alexander" [ref=e591]
                    - generic [ref=e592]:
                      - paragraph [ref=e593]: Shai Gilgeous-Alexander
                      - paragraph [ref=e594]:
                        - generic [ref=e595]: OKC
                        - text: "- SAS"
                      - paragraph [ref=e596]: May 30th 8:10 PM
                    - generic [ref=e597]:
                      - paragraph [ref=e598]:
                        - text: "7.5"
                        - generic [ref=e599]: Assists
                      - generic [ref=e600]:
                        - button "Less 1.96 x" [ref=e601]:
                          - generic [ref=e602]: Less
                          - generic [ref=e603]: 1.96 x
                        - button "More 1.66 x" [ref=e604]:
                          - generic [ref=e605]: More
                          - generic [ref=e606]: 1.66 x
                    - button [ref=e607]:
                      - img [ref=e608]
                  - button "Add Icon Add Player Add 1 More Pick for a 5% Boost Boost Icon" [ref=e612]:
                    - generic [ref=e613]:
                      - img "Add Icon" [ref=e615]
                      - generic [ref=e616]: Add Player
                    - generic [ref=e617]:
                      - generic [ref=e618]: Add 1 More Pick for a 5% Boost
                      - img "Boost Icon" [ref=e620]
                - generic [ref=e622]:
                  - generic [ref=e623]:
                    - generic [ref=e625]:
                      - radio
                      - generic [ref=e626] [cursor=pointer]: $25
                      - radio
                      - generic [ref=e627] [cursor=pointer]: $75
                      - radio [disabled]
                      - generic: $300
                    - generic [ref=e629]:
                      - generic [ref=e630]: $
                      - spinbutton [ref=e634]: "3"
                    - button "31" [ref=e635] [cursor=pointer]:
                      - img [ref=e636]
                      - generic [ref=e638]: "31"
                  - generic [ref=e639]:
                    - generic [ref=e640]:
                      - generic [ref=e641]:
                        - button "Insured" [ref=e642]
                        - button "All In" [ref=e643]
                      - generic [ref=e645]: 2.73x
                    - generic [ref=e647]:
                      - generic [ref=e648]:
                        - paragraph [ref=e649]: Perfect line-up
                        - paragraph [ref=e650]: $8.19
                      - generic [ref=e652]:
                        - paragraph [ref=e653]: Or 1st place in group
                        - generic [ref=e654]: $5 + $8.19
                  - button "Place" [ref=e658] [cursor=pointer]:
                    - text: Place
                    - img [ref=e659]
            - generic [ref=e662]:
              - generic [ref=e664]:
                - link "Download ParlayPlay On The Play Store" [ref=e665] [cursor=pointer]:
                  - /url: https://parlayplay.onelink.me/oLJk/fh7u6juo
                  - img "Download ParlayPlay On The Play Store" [ref=e666]
                - paragraph [ref=e667]:
                  - text: Get the app.
                  - text: Better. Faster. Convenient
              - navigation [ref=e668]:
                - link "Privacy" [ref=e669] [cursor=pointer]:
                  - /url: /privacy-policy
                - link "Terms" [ref=e670] [cursor=pointer]:
                  - /url: /terms
                - link "Responsible Gaming" [ref=e671] [cursor=pointer]:
                  - /url: /responsible-gaming
                - link "Gaming Rules" [ref=e672] [cursor=pointer]:
                  - /url: /rules
                - link "FAQ" [ref=e673] [cursor=pointer]:
                  - /url: https://intercom.help/parlayplay/en/
              - navigation [ref=e674]:
                - generic [ref=e675]:
                  - paragraph [ref=e676]: © ParlayPlay 2026
                  - generic [ref=e677]:
                    - link [ref=e678] [cursor=pointer]:
                      - /url: https://www.facebook.com/parlayplay.io
                      - img [ref=e679]
                    - link [ref=e681] [cursor=pointer]:
                      - /url: https://www.instagram.com/parlayplay_?igsh=bHBldWQyMmV2b3Y4
                      - img [ref=e682]
                    - link [ref=e684] [cursor=pointer]:
                      - /url: https://www.twitter.com/parlay_play
                      - img [ref=e685]
                    - link [ref=e687] [cursor=pointer]:
                      - /url: https://discord.com/invite/parlayplay
                      - img [ref=e688]
                  - img "21+-icon" [ref=e690]
                - paragraph [ref=e692]: Gambling can be addictive. Please play responsibly.
          - generic [ref=e694]:
            - button [ref=e695]
            - dialog "User Limit Exceeded" [ref=e697]:
              - generic [ref=e698]:
                - generic [ref=e699]:
                  - img [ref=e701]
                  - button [active] [ref=e703]:
                    - img [ref=e704]
                - heading "User Limit Exceeded" [level=1] [ref=e706]
                - heading "Daily Amount Limit" [level=1] [ref=e707]
                - generic [ref=e708]:
                  - paragraph [ref=e709]: Placing this contest will cause you to exceed your Daily Amount Limit
                  - generic [ref=e710]:
                    - paragraph [ref=e711]:
                      - strong [ref=e712]: "Current limit:"
                      - text: $5
                    - paragraph [ref=e713]:
                      - strong [ref=e714]: "Can reset to:"
                      - text: $5,000
                  - paragraph [ref=e715]: Click the button below to change your limits or to reset them back to the defaults.
                  - generic [ref=e716]:
                    - button "Go to Settings" [ref=e717] [cursor=pointer]
                    - button "Reset Limits" [ref=e718] [cursor=pointer]
    - region "Notifications Alt+T"
  - alert [ref=e719]
  - iframe [ref=e720]:
    
```

# Test source

```ts
  2   | import type { ContestPage } from '../pages/contest.page';
  3   | import type { HomePage } from '../pages/home.page';
  4   | 
  5   | export interface PlaceContestWithRetryOptions {
  6   |     homePage: HomePage;
  7   |     contestPage: ContestPage;
  8   |     pickCount: number;
  9   |     entryAmount: number;
  10  |     /**
  11  |      * Max attempts before giving up. Falls back to the `CONTEST_RETRY_ATTEMPTS`
  12  |      * env var so each environment (local/dev/staging) can tune how many stat
  13  |      * rotations to try before failing. Defaults to 3.
  14  |      */
  15  |     maxAttempts?: number;
  16  |     /**
  17  |      * Submission step. Runs after picks are selected and the entry amount is set.
  18  |      * Return `{ success: false, error }` to trigger a retry on a different stat tab.
  19  |      * Defaults to `contestPage.submitAndAwaitResult()`.
  20  |      */
  21  |     submit?: () => Promise<{ success: boolean; error: string | null }>;
  22  | }
  23  | 
  24  | function resolveMaxAttempts(explicit?: number): number {
  25  |     if (explicit !== undefined) return explicit;
  26  |     const raw = process.env.CONTEST_RETRY_ATTEMPTS;
  27  |     if (!raw) return 5;
  28  |     const parsed = parseInt(raw, 10);
  29  |     return Number.isFinite(parsed) && parsed > 0 ? parsed : 5;
  30  | }
  31  | 
  32  | function isThrottleError(err: string | null): boolean {
  33  |     return /\b429\b|throttled|too many requests/i.test(err ?? "");
  34  | }
  35  | 
  36  | // DRF emits "Expected available in N second(s)". Parse that and wait at least
  37  | // that long, capped to keep a single throttle from eating the whole suite.
  38  | function throttleBackoffMs(err: string | null): number {
  39  |     const match = (err ?? "").match(/in\s+(\d+)\s+second/i);
  40  |     const seconds = match ? parseInt(match[1], 10) : 0;
  41  |     const buffered = Math.max(seconds, 10) + 3;
  42  |     return Math.min(buffered, 30) * 1000;
  43  | }
  44  | 
  45  | export interface PlaceContestWithRetryResult {
  46  |     /** Picks from the successful attempt. */
  47  |     pickIds: string[];
  48  | }
  49  | 
  50  | /**
  51  |  * Picks N players, advances to the contest page, and submits — retrying on
  52  |  * a different stat tab when a user limit (or other submission error) trips.
  53  |  *
  54  |  * Used by both the contest-submission specs and the slip-sharing flow, since
  55  |  * any user can hit a per-stat limit on the first try.
  56  |  */
  57  | export async function placeContestWithRetry(
  58  |     opts: PlaceContestWithRetryOptions,
  59  | ): Promise<PlaceContestWithRetryResult> {
  60  |     const { homePage, contestPage, pickCount, entryAmount } = opts;
  61  |     const maxAttempts = resolveMaxAttempts(opts.maxAttempts);
  62  |     const submit = opts.submit ?? (() => contestPage.submitAndAwaitResult());
  63  | 
  64  |     let pickIds: string[] = [];
  65  |     let placed = false;
  66  |     let lastError: string | null = null;
  67  |     let statIdx = 0;
  68  | 
  69  |     for (let attempt = 1; attempt <= maxAttempts && !placed; attempt++) {
  70  |         if (attempt > 1) {
  71  |             // Always reset back to home — pickPlayers below needs the grid.
  72  |             // But only rotate the stat tab on a per-stat user limit. On a 429,
  73  |             // the picks were fine; rotating wastes stat tabs (we can run out
  74  |             // before the throttle window even closes), so we sleep instead.
  75  |             await homePage.clearSlip();
  76  |             if (isThrottleError(lastError)) {
  77  |                 await new Promise((r) => setTimeout(r, throttleBackoffMs(lastError)));
  78  |             } else {
  79  |                 statIdx++;
  80  |             }
  81  |         }
  82  |         await homePage.waitForPlayersGrid();
  83  |         pickIds = await homePage.pickPlayers(
  84  |             pickCount,
  85  |             attempt > 1 ? statIdx : undefined,
  86  |         );
  87  |         await homePage.enterFinalContestPage();
  88  |         await contestPage.verifyPage();
  89  |         await contestPage.setEntryAmountIfEditable(entryAmount);
  90  | 
  91  |         const result = await submit();
  92  |         if (!result.success) {
  93  |             lastError = result.error;
  94  |             continue;
  95  |         }
  96  |         placed = true;
  97  |     }
  98  | 
  99  |     expect(
  100 |         placed,
  101 |         `Could not place contest after ${maxAttempts} attempts (last error: ${lastError})`,
> 102 |     ).toBe(true);
      |       ^ Error: Could not place contest after 5 attempts (last error: 400 Entering this contest will cause you to exceed your daily contest limit.)
  103 | 
  104 |     return { pickIds };
  105 | }
  106 | 
```