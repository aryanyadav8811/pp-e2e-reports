# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: entries/entry-card-redesign.spec.ts >> My Entries card redesign — cancel flow >> Freshly placed entry is cancellable with a live countdown, and Cancel Entry opens a confirmation
- Location: tests/entries/entry-card-redesign.spec.ts:247:5

# Error details

```
Error: Could not place contest after 5 attempts (last error: 429 Request was throttled. Expected available in 1 second.)

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
                - generic [ref=e17]: $793.37
                - generic [ref=e18]:
                  - img "gift-icon" [ref=e19]
                  - text: "6.00"
              - button "Toggle Menu" [ref=e20]:
                - img [ref=e21]
      - main [ref=e23]:
        - generic [ref=e28]:
          - generic [ref=e29]:
            - generic [ref=e30]:
              - list [ref=e32]:
                - button "Live" [ref=e33] [cursor=pointer]:
                  - generic [ref=e37]: Live
                - button "MLB" [ref=e38] [cursor=pointer]
                - button "WNBA" [ref=e39] [cursor=pointer]
                - button "WNBA-Combos" [ref=e40] [cursor=pointer]
                - button "WNBA Q1" [ref=e41] [cursor=pointer]
                - button "WNBA H1" [ref=e42] [cursor=pointer]
                - button "Valorant" [ref=e43] [cursor=pointer]
                - button "UFC" [ref=e44] [cursor=pointer]
              - list [ref=e46]:
                - button "WNBA" [ref=e47] [cursor=pointer]
              - generic [ref=e48]:
                - generic [ref=e49]:
                  - generic [ref=e52]:
                    - img [ref=e54]
                    - textbox "Search player or team" [ref=e56]
                  - button "Change card style from grid" [ref=e58]
                - list [ref=e60]:
                  - listitem [ref=e61]:
                    - button "Points" [ref=e62]
                  - listitem [ref=e63]:
                    - button "Rebounds" [ref=e64]
                  - listitem [ref=e65]:
                    - button "Assists" [ref=e66]
                  - listitem [ref=e67]:
                    - button "3PT Made" [ref=e68]
                  - listitem [ref=e69]:
                    - button "Pts + Reb + Ast" [ref=e70]
                  - listitem [ref=e71]:
                    - button "Double Double" [ref=e72]
                  - listitem [ref=e73]:
                    - button "Pts + Reb" [ref=e74]
                  - listitem [ref=e75]:
                    - button "Pts + Ast" [ref=e76]
                  - listitem [ref=e77]:
                    - button "Reb + Ast" [ref=e78]
            - generic [ref=e79]:
              - generic [ref=e82]:
                - button "previous slide" [ref=e83] [cursor=pointer]:
                  - img [ref=e84]
                - generic [ref=e87]:
                  - 'button "Boosted Picks 🚀 Every Pick Pays: Up to a 35% Boost! lightning-bolt-yellow" [ref=e89] [cursor=pointer]':
                    - generic [ref=e90]:
                      - generic [ref=e92]: Boosted Picks 🚀
                      - generic [ref=e93]: "Every Pick Pays: Up to a 35% Boost!"
                    - img "lightning-bolt-yellow" [ref=e94]
                  - button "Get $20 By referring a friend making a first $10 deposit. lightning-bolt-yellow" [ref=e96] [cursor=pointer]:
                    - generic [ref=e97]:
                      - generic [ref=e99]: Get $20
                      - generic [ref=e100]: By referring a friend making a first $10 deposit.
                    - img "lightning-bolt-yellow" [ref=e101]
                - button "next slide" [ref=e102] [cursor=pointer]:
                  - img [ref=e103]
              - generic [ref=e105]:
                - generic [ref=e108]:
                  - generic [ref=e111]:
                    - button "Open expert opinion for Chelsea Gray" [ref=e112]:
                      - img [ref=e113]
                    - img "Chelsea Gray" [ref=e116]
                  - generic [ref=e117]:
                    - generic [ref=e118]: Chelsea Gray
                    - button "2.5 3PT Made" [ref=e119]:
                      - generic [ref=e120]:
                        - img [ref=e121]
                        - img [ref=e123]
                      - generic [ref=e125]: "2.5"
                      - generic [ref=e126]: 3PT Made
                    - generic [ref=e128]:
                      - generic [ref=e129]:
                        - paragraph [ref=e130]
                        - paragraph [ref=e131]: "Current: 2"
                      - generic [ref=e133]:
                        - generic [ref=e134]: Q4 - 00:28
                        - text: LVA 99 vs 83 DAL
                    - generic [ref=e135]:
                      - button "Select over 2.5 3PT Made for 0 times" [disabled] [ref=e136]
                      - button "Select over 2.5 3PT Made for 2.32 times" [ref=e138]:
                        - img [ref=e141]
                        - generic [ref=e143]: 2.32x
                        - img [ref=e144]
                - generic [ref=e148]:
                  - generic [ref=e151]:
                    - button "Open expert opinion for Jackie Young" [ref=e152]:
                      - img [ref=e153]
                    - img "Jackie Young" [ref=e156]
                  - generic [ref=e157]:
                    - generic [ref=e158]: Jackie Young
                    - button "2.5 3PT Made" [ref=e159]:
                      - generic [ref=e160]:
                        - img [ref=e161]
                        - img [ref=e163]
                      - generic [ref=e165]: "2.5"
                      - generic [ref=e166]: 3PT Made
                    - generic [ref=e168]:
                      - generic [ref=e169]:
                        - paragraph [ref=e170]
                        - paragraph [ref=e171]: "Current: 2"
                      - generic [ref=e173]:
                        - generic [ref=e174]: Q4 - 00:28
                        - text: LVA 99 vs 83 DAL
                    - generic [ref=e175]:
                      - button "Select over 2.5 3PT Made for 0 times" [disabled] [ref=e176]
                      - button "Select over 2.5 3PT Made for 5.56 times" [ref=e178]:
                        - img [ref=e181]
                        - generic [ref=e183]: 5.56x
                        - img [ref=e184]
                - generic [ref=e188]:
                  - generic [ref=e191]:
                    - button "Open expert opinion for Aja Wilson" [ref=e192]:
                      - img [ref=e193]
                    - img "Aja Wilson" [ref=e196]
                  - generic [ref=e197]:
                    - generic [ref=e198]: Aja Wilson
                    - button "0.5 3PT Made" [ref=e199]:
                      - generic [ref=e200]:
                        - img [ref=e201]
                        - img [ref=e203]
                      - generic [ref=e205]: "0.5"
                      - generic [ref=e206]: 3PT Made
                    - generic [ref=e208]:
                      - generic [ref=e209]:
                        - paragraph [ref=e210]
                        - paragraph [ref=e211]: "Current: 0"
                      - generic [ref=e213]:
                        - generic [ref=e214]: Q4 - 00:28
                        - text: LVA 99 vs 83 DAL
                    - generic [ref=e215]:
                      - button "Select over 0.5 3PT Made for 0 times" [disabled] [ref=e216]
                      - button "Select over 0.5 3PT Made for 3.6 times" [ref=e218]:
                        - generic [ref=e219]: 3.6x
                        - img [ref=e220]
                - generic [ref=e224]:
                  - generic [ref=e227]:
                    - button "Open expert opinion for Jewell Loyd" [ref=e228]:
                      - img [ref=e229]
                    - img "Jewell Loyd" [ref=e232]
                  - generic [ref=e233]:
                    - generic [ref=e234]: Jewell Loyd
                    - button "2.5 3PT Made" [ref=e235]:
                      - generic [ref=e236]:
                        - img [ref=e237]
                        - img [ref=e239]
                      - generic [ref=e241]: "2.5"
                      - generic [ref=e242]: 3PT Made
                    - generic [ref=e244]:
                      - generic [ref=e245]:
                        - paragraph [ref=e246]
                        - paragraph [ref=e247]: "Current: 2"
                      - generic [ref=e249]:
                        - generic [ref=e250]: Q4 - 00:28
                        - text: LVA 99 vs 83 DAL
                    - generic [ref=e251]:
                      - button "Select over 2.5 3PT Made for 0 times" [disabled] [ref=e252]
                      - button "Select over 2.5 3PT Made for 1.9 times" [ref=e254]:
                        - generic [ref=e255]: 1.9x
                        - img [ref=e256]
                - generic [ref=e260]:
                  - generic [ref=e263]:
                    - button "Open expert opinion for Paige Bueckers" [ref=e264]:
                      - img [ref=e265]
                    - img "Paige Bueckers" [ref=e268]
                  - generic [ref=e269]:
                    - generic [ref=e270]: P. Bueckers
                    - button "0.5 3PT Made" [ref=e271]:
                      - generic [ref=e272]:
                        - img [ref=e273]
                        - img [ref=e275]
                      - generic [ref=e277]: "0.5"
                      - generic [ref=e278]: 3PT Made
                    - generic [ref=e280]:
                      - generic [ref=e281]:
                        - paragraph [ref=e282]
                        - paragraph [ref=e283]: "Current: 0"
                      - generic [ref=e285]:
                        - generic [ref=e286]: Q4 - 00:28
                        - text: LVA 99 vs 83 DAL
                    - generic [ref=e287]:
                      - button "Select over 0.5 3PT Made for 0 times" [disabled] [ref=e288]
                      - button "Select over 0.5 3PT Made for 2.37 times" [ref=e290]:
                        - img [ref=e293]
                        - generic [ref=e295]: 2.37x
                        - img [ref=e296]
            - generic [ref=e299]:
              - img [ref=e301]
              - generic [ref=e303]:
                - generic [ref=e305]:
                  - generic [ref=e306]: 20.71x
                  - generic [ref=e307]: 21.75x
                - generic [ref=e308]:
                  - button "+ 10% Boost 🚀" [ref=e314]:
                    - generic [ref=e315]: + 10% Boost 🚀
                  - generic [ref=e325]: "Add 4th Pick: 10% Boost"
              - button "Continue" [ref=e326] [cursor=pointer]
            - generic [ref=e328]:
              - generic [ref=e329]:
                - button [ref=e330]:
                  - img [ref=e331]
                - generic [ref=e333]: Make Your More/Less Picks
              - generic [ref=e334]:
                - generic [ref=e336]:
                  - img "Chelsea Gray" [ref=e338]
                  - generic [ref=e339]:
                    - paragraph [ref=e340]: Chelsea Gray
                    - paragraph [ref=e341]:
                      - generic [ref=e342]: LVA
                      - text: "- DAL"
                    - paragraph [ref=e343]: Jun 25th 10:00 PM
                  - generic [ref=e344]:
                    - paragraph [ref=e345]:
                      - text: "2.5"
                      - generic [ref=e346]: 3PT Made
                    - generic [ref=e347]:
                      - button "Less" [disabled] [ref=e348]:
                        - generic [ref=e349]: Less
                      - button "More 2.32 x" [ref=e350]:
                        - generic [ref=e351]: More
                        - generic [ref=e352]: 2.32 x
                  - button [ref=e353]:
                    - img [ref=e354]
                - generic [ref=e358]:
                  - img "Jackie Young" [ref=e360]
                  - generic [ref=e361]:
                    - paragraph [ref=e362]: Jackie Young
                    - paragraph [ref=e363]:
                      - generic [ref=e364]: LVA
                      - text: "- DAL"
                    - paragraph [ref=e365]: Jun 25th 10:00 PM
                  - generic [ref=e366]:
                    - paragraph [ref=e367]:
                      - text: "2.5"
                      - generic [ref=e368]: 3PT Made
                    - generic [ref=e369]:
                      - button "Less" [disabled] [ref=e370]:
                        - generic [ref=e371]: Less
                      - button "More 5.56 x" [ref=e372]:
                        - generic [ref=e373]: More
                        - generic [ref=e374]: 5.56 x
                  - button [ref=e375]:
                    - img [ref=e376]
                - generic [ref=e380]:
                  - img "Paige Bueckers" [ref=e382]
                  - generic [ref=e383]:
                    - paragraph [ref=e384]: Paige Bueckers
                    - paragraph [ref=e385]:
                      - generic [ref=e386]: DAL
                      - text: "- LVA"
                    - paragraph [ref=e387]: Jun 25th 10:00 PM
                  - generic [ref=e388]:
                    - paragraph [ref=e389]:
                      - text: "0.5"
                      - generic [ref=e390]: 3PT Made
                    - generic [ref=e391]:
                      - button "Less" [disabled] [ref=e392]:
                        - generic [ref=e393]: Less
                      - button "More 2.37 x" [ref=e394]:
                        - generic [ref=e395]: More
                        - generic [ref=e396]: 2.37 x
                  - button [ref=e397]:
                    - img [ref=e398]
                - button "Add Icon Add Player Add 1 More Pick for a 10% Boost Boost Icon" [ref=e402]:
                  - generic [ref=e403]:
                    - img "Add Icon" [ref=e405]
                    - generic [ref=e406]: Add Player
                  - generic [ref=e407]:
                    - generic [ref=e408]: Add 1 More Pick for a 10% Boost
                    - img "Boost Icon" [ref=e410]
              - generic [ref=e412]:
                - generic [ref=e413]:
                  - generic [ref=e415]:
                    - radio
                    - generic [ref=e416] [cursor=pointer]: $25
                    - radio
                    - generic [ref=e417] [cursor=pointer]: $75
                    - radio
                    - generic [ref=e418] [cursor=pointer]: $300
                  - generic [ref=e420]:
                    - generic [ref=e421]: $
                    - spinbutton [ref=e425]: "3"
                  - button "2" [ref=e426] [cursor=pointer]:
                    - img [ref=e427]
                    - generic [ref=e429]: "2"
                - generic [ref=e430]:
                  - generic [ref=e431]:
                    - generic [ref=e432]:
                      - button "Insured" [ref=e433]
                      - button "All In" [ref=e434]
                    - generic [ref=e435]:
                      - generic [ref=e436]: 20.71x
                      - generic [ref=e437]: 21.75x
                  - generic [ref=e439]:
                    - generic [ref=e440]:
                      - paragraph [ref=e441]: Perfect line-up
                      - paragraph [ref=e442]: $65.25
                    - generic [ref=e444]:
                      - paragraph [ref=e445]: Or 1st place in group
                      - generic [ref=e446]: $5 + $65.25
                - button "Place" [active] [ref=e450] [cursor=pointer]:
                  - text: Place
                  - img [ref=e451]
          - generic [ref=e454]:
            - generic [ref=e456]:
              - link "Download ParlayPlay On The Play Store" [ref=e457] [cursor=pointer]:
                - /url: https://parlayplay.onelink.me/oLJk/fh7u6juo
                - img "Download ParlayPlay On The Play Store" [ref=e458]
              - paragraph [ref=e459]:
                - text: Get the app.
                - text: Better. Faster. Convenient
            - navigation [ref=e460]:
              - link "Privacy" [ref=e461] [cursor=pointer]:
                - /url: /privacy-policy
              - link "Terms" [ref=e462] [cursor=pointer]:
                - /url: /terms
              - link "Responsible Gaming" [ref=e463] [cursor=pointer]:
                - /url: /responsible-gaming
              - link "Gaming Rules" [ref=e464] [cursor=pointer]:
                - /url: /rules
              - link "FAQ" [ref=e465] [cursor=pointer]:
                - /url: https://intercom.help/parlayplay/en/
            - navigation [ref=e466]:
              - generic [ref=e467]:
                - paragraph [ref=e468]: © ParlayPlay 2026
                - generic [ref=e469]:
                  - link [ref=e470] [cursor=pointer]:
                    - /url: https://www.facebook.com/parlayplay.io
                    - img [ref=e471]
                  - link [ref=e473] [cursor=pointer]:
                    - /url: https://www.instagram.com/parlayplay_?igsh=bHBldWQyMmV2b3Y4
                    - img [ref=e474]
                  - link [ref=e476] [cursor=pointer]:
                    - /url: https://www.twitter.com/parlay_play
                    - img [ref=e477]
                  - link [ref=e479] [cursor=pointer]:
                    - /url: https://discord.com/invite/parlayplay
                    - img [ref=e480]
                - img "21+-icon" [ref=e482]
              - paragraph [ref=e484]: Gambling can be addictive. Please play responsibly.
    - region "Notifications Alt+T":
      - alert [ref=e486] [cursor=pointer]:
        - img [ref=e488]
        - text: Request was throttled. Expected available in 1 second.
        - button "close" [ref=e490]:
          - img [ref=e491]
        - progressbar "notification timer" [ref=e495]
  - alert [ref=e496]
  - iframe [ref=e497]:
    
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
      |       ^ Error: Could not place contest after 5 attempts (last error: 429 Request was throttled. Expected available in 1 second.)
  103 | 
  104 |     return { pickIds };
  105 | }
  106 | 
```