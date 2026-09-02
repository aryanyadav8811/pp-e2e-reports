# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: slip_sharing/tail_feed.spec.ts >> Tail Feed >> Share toggle OFF — newly-placed contest does NOT appear on the You tab
- Location: tests/slip_sharing/tail_feed.spec.ts:135:5

# Error details

```
TimeoutError: page.waitForResponse: Timeout 60000ms exceeded while waiting for event "response"
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
                - generic [ref=e17]: $0.00
                - generic [ref=e18]:
                  - img "gift-icon" [ref=e19]
                  - text: "23.00"
              - button "Toggle Menu" [ref=e20]:
                - img [ref=e21]
      - main [ref=e23]:
        - generic [ref=e26]:
          - generic [ref=e27]:
            - generic [ref=e28]:
              - list [ref=e30]:
                - button "NBA" [ref=e31] [cursor=pointer]
                - button "NBA-Combos" [ref=e32] [cursor=pointer]
                - button "NBA Q1" [ref=e33] [cursor=pointer]
                - button "NBA H1" [ref=e34] [cursor=pointer]
                - button "MLB" [ref=e35] [cursor=pointer]
                - button "MLB-Combos" [ref=e36] [cursor=pointer]
                - button "NHL" [ref=e37] [cursor=pointer]
                - button "CSGO" [ref=e38] [cursor=pointer]
                - button "Valorant" [ref=e39] [cursor=pointer]
              - list [ref=e41]:
                - listitem [ref=e42]:
                  - button "ALL" [ref=e43] [cursor=pointer]:
                    - generic [ref=e44]: ALL
                - listitem [ref=e45]:
                  - button "SAS@NYK 8:40PM" [ref=e46] [cursor=pointer]:
                    - text: SAS@NYK
                    - generic [ref=e47]: 8:40PM
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
                    - button "Triple Double" [ref=e68]
                  - listitem [ref=e69]:
                    - button "3PT Made" [ref=e70]
                  - listitem [ref=e71]:
                    - button "Pts + Reb + Ast" [ref=e72]
                  - listitem [ref=e73]:
                    - button "Double Double" [ref=e74]
                  - listitem [ref=e75]:
                    - button "Pts + Reb" [ref=e76]
                  - listitem [ref=e77]:
                    - button "Pts + Ast" [ref=e78]
                  - listitem [ref=e79]:
                    - button "Reb + Ast" [ref=e80]
                  - listitem [ref=e81]:
                    - button "Stl + Blk" [ref=e82]
                  - listitem [ref=e83]:
                    - button "3PT Attempted" [ref=e84]
                  - listitem [ref=e85]:
                    - button "FT Made" [ref=e86]
                  - listitem [ref=e87]:
                    - button "FG Made" [ref=e88]
                  - listitem [ref=e89]:
                    - button "FG Attempted" [ref=e90]
                  - listitem [ref=e91]:
                    - button "First Point Scorer" [ref=e92]
                  - listitem [ref=e93]:
                    - button "Fantasy Points" [ref=e94]
                  - listitem [ref=e95]:
                    - button "Blocks" [ref=e96]
                  - listitem [ref=e97]:
                    - button "Steals" [ref=e98]
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
                    - button "Open expert opinion for Jalen Brunson" [ref=e175]:
                      - img [ref=e176]
                    - img "Jalen Brunson" [ref=e179]
                  - generic [ref=e180]:
                    - generic [ref=e181]: Jalen Brunson
                    - button "0.5 TD" [ref=e182]:
                      - generic [ref=e183]:
                        - img [ref=e184]
                        - img [ref=e186]
                      - generic [ref=e188]: "0.5"
                      - generic [ref=e189]: TD
                    - generic [ref=e190]:
                      - generic [ref=e191]: SAS@NYK
                      - generic [ref=e192]: 8:40PM
                    - generic [ref=e193]:
                      - button "Select over 0.5 Triple Double for 0 times" [disabled] [ref=e194]
                      - button "Select over 0.5 Triple Double for 51.4 times" [ref=e196]:
                        - img [ref=e199]
                        - generic [ref=e201]: 51.4x
                        - img [ref=e202]
                - generic [ref=e206]:
                  - generic [ref=e209]:
                    - button "Open expert opinion for Josh Hart" [ref=e210]:
                      - img [ref=e211]
                    - img "Josh Hart" [ref=e214]
                  - generic [ref=e215]:
                    - generic [ref=e216]: Josh Hart
                    - button "0.5 TD" [ref=e217]:
                      - generic [ref=e218]:
                        - img [ref=e219]
                        - img [ref=e221]
                      - generic [ref=e223]: "0.5"
                      - generic [ref=e224]: TD
                    - generic [ref=e225]:
                      - generic [ref=e226]: SAS@NYK
                      - generic [ref=e227]: 8:40PM
                    - generic [ref=e228]:
                      - button "Select over 0.5 Triple Double for 0 times" [disabled] [ref=e229]
                      - button "Select over 0.5 Triple Double for 25.9 times" [ref=e231]:
                        - img [ref=e234]
                        - generic [ref=e236]: 25.9x
                        - img [ref=e237]
                - generic [ref=e241]:
                  - generic [ref=e244]:
                    - button "Open expert opinion for Karl-Anthony Towns" [ref=e245]:
                      - img [ref=e246]
                    - img "Karl-Anthony Towns" [ref=e249]
                  - generic [ref=e250]:
                    - generic [ref=e251]: K. Towns
                    - button "0.5 TD" [ref=e252]:
                      - generic [ref=e253]:
                        - img [ref=e254]
                        - img [ref=e256]
                      - generic [ref=e258]: "0.5"
                      - generic [ref=e259]: TD
                    - generic [ref=e260]:
                      - generic [ref=e261]: SAS@NYK
                      - generic [ref=e262]: 8:40PM
                    - generic [ref=e263]:
                      - button "Select over 0.5 Triple Double for 0 times" [disabled] [ref=e264]
                      - button "Select over 0.5 Triple Double for 28.6 times" [ref=e266]:
                        - generic [ref=e267]: 28.6x
                        - img [ref=e268]
                - generic [ref=e272]:
                  - generic [ref=e275]:
                    - button "Open expert opinion for De'Aaron Fox" [ref=e276]:
                      - img [ref=e277]
                    - img "De'Aaron Fox" [ref=e280]
                  - generic [ref=e281]:
                    - generic [ref=e282]: De'Aaron Fox
                    - button "0.5 TD" [ref=e283]:
                      - generic [ref=e284]:
                        - img [ref=e285]
                        - img [ref=e287]
                      - generic [ref=e289]: "0.5"
                      - generic [ref=e290]: TD
                    - generic [ref=e291]:
                      - generic [ref=e292]: SAS@NYK
                      - generic [ref=e293]: 8:40PM
                    - generic [ref=e294]:
                      - button "Select over 0.5 Triple Double for 0 times" [disabled] [ref=e295]
                      - button "Select over 0.5 Triple Double for 52 times" [ref=e297]:
                        - img [ref=e300]
                        - generic [ref=e302]: 52x
                        - img [ref=e303]
                - generic [ref=e307]:
                  - generic [ref=e310]:
                    - button "Open expert opinion for Dylan Harper" [ref=e311]:
                      - img [ref=e312]
                    - img "Dylan Harper" [ref=e315]
                  - generic [ref=e316]:
                    - generic [ref=e317]: Dylan Harper
                    - button "0.5 TD" [ref=e318]:
                      - generic [ref=e319]:
                        - img [ref=e320]
                        - img [ref=e322]
                      - generic [ref=e324]: "0.5"
                      - generic [ref=e325]: TD
                    - generic [ref=e326]:
                      - generic [ref=e327]: SAS@NYK
                      - generic [ref=e328]: 8:40PM
                    - generic [ref=e329]:
                      - button "Select over 0.5 Triple Double for 0 times" [disabled] [ref=e330]
                      - button "Select over 0.5 Triple Double for 49 times" [ref=e332]:
                        - generic [ref=e333]: 49x
                        - img [ref=e334]
                - generic [ref=e338]:
                  - generic [ref=e341]:
                    - button "Open expert opinion for Devin Vassell" [ref=e342]:
                      - img [ref=e343]
                    - img "Devin Vassell" [ref=e346]
                  - generic [ref=e347]:
                    - generic [ref=e348]: Devin Vassell
                    - button "0.5 TD" [ref=e349]:
                      - generic [ref=e350]:
                        - img [ref=e351]
                        - img [ref=e353]
                      - generic [ref=e355]: "0.5"
                      - generic [ref=e356]: TD
                    - generic [ref=e357]:
                      - generic [ref=e358]: SAS@NYK
                      - generic [ref=e359]: 8:40PM
                    - generic [ref=e360]:
                      - button "Select over 0.5 Triple Double for 0 times" [disabled] [ref=e361]
                      - button "Select over 0.5 Triple Double for 57.4 times" [ref=e363]:
                        - generic [ref=e364]: 57.4x
                        - img [ref=e365]
                - generic [ref=e369]:
                  - generic [ref=e372]:
                    - button "Open expert opinion for Stephon Castle" [ref=e373]:
                      - img [ref=e374]
                    - img "Stephon Castle" [ref=e377]
                  - generic [ref=e378]:
                    - generic [ref=e379]: S. Castle
                    - button "0.5 TD" [ref=e380]:
                      - generic [ref=e381]:
                        - img [ref=e382]
                        - img [ref=e384]
                      - generic [ref=e386]: "0.5"
                      - generic [ref=e387]: TD
                    - generic [ref=e388]:
                      - generic [ref=e389]: SAS@NYK
                      - generic [ref=e390]: 8:40PM
                    - generic [ref=e391]:
                      - button "Select over 0.5 Triple Double for 0 times" [disabled] [ref=e392]
                      - button "Select over 0.5 Triple Double for 27.4 times" [ref=e394]:
                        - generic [ref=e395]: 27.4x
                        - img [ref=e396]
                - generic [ref=e400]:
                  - generic [ref=e403]:
                    - button "Open expert opinion for Victor Wembanyama" [ref=e404]:
                      - img [ref=e405]
                    - img "Victor Wembanyama" [ref=e408]
                  - generic [ref=e409]:
                    - generic [ref=e410]: V. Wembanyama
                    - button "0.5 TD" [ref=e411]:
                      - generic [ref=e412]:
                        - img [ref=e413]
                        - img [ref=e415]
                      - generic [ref=e417]: "0.5"
                      - generic [ref=e418]: TD
                    - generic [ref=e419]:
                      - generic [ref=e420]: SAS@NYK
                      - generic [ref=e421]: 8:40PM
                    - generic [ref=e422]:
                      - button "Select over 0.5 Triple Double for 0 times" [disabled] [ref=e423]
                      - button "Select over 0.5 Triple Double for 32.8 times" [ref=e425]:
                        - generic [ref=e426]: 32.8x
                        - img [ref=e427]
            - generic [ref=e430]:
              - generic [ref=e431]:
                - img [ref=e433]
                - generic [ref=e435]:
                  - generic [ref=e436]: 1000.00x
                  - generic [ref=e451]: 3 picks
                - button "Continue" [ref=e452] [cursor=pointer]
              - generic [ref=e453]:
                - generic [ref=e454]:
                  - generic [ref=e455]: Your Selection
                  - generic [ref=e456]:
                    - generic [ref=e457]:
                      - generic [ref=e458]:
                        - img [ref=e459]
                        - generic [ref=e461]:
                          - text: J. Brunson (0.5 Triple Double - More - FG)
                          - generic [ref=e462]: 51.4x
                      - img [ref=e464]
                    - generic [ref=e466]:
                      - generic [ref=e467]:
                        - img [ref=e468]
                        - generic [ref=e470]:
                          - text: J. Hart (0.5 Triple Double - More - FG)
                          - generic [ref=e471]: 25.9x
                      - img [ref=e473]
                    - generic [ref=e475]:
                      - generic [ref=e476]:
                        - img [ref=e477]
                        - generic [ref=e479]:
                          - text: D. Fox (0.5 Triple Double - More - FG)
                          - generic [ref=e480]: 52x
                      - img [ref=e482]
                - generic [ref=e484]:
                  - img [ref=e485]
                  - generic [ref=e487]: Clear All
            - generic [ref=e489]:
              - generic [ref=e490]:
                - button [ref=e491]:
                  - img [ref=e492]
                - generic [ref=e494]: Make Your More/Less Picks
              - generic [ref=e495]:
                - generic [ref=e497]:
                  - img "Jalen Brunson" [ref=e499]
                  - generic [ref=e500]:
                    - paragraph [ref=e501]: Jalen Brunson
                    - paragraph [ref=e502]:
                      - generic [ref=e503]: NYK
                      - text: "- SAS"
                    - paragraph [ref=e504]: Today 8:40 PM
                  - generic [ref=e505]:
                    - paragraph [ref=e506]:
                      - text: "0.5"
                      - generic [ref=e507]: TD
                    - generic [ref=e508]:
                      - button "Less" [disabled] [ref=e509]:
                        - generic [ref=e510]: Less
                      - button "More 51.4 x" [ref=e511]:
                        - generic [ref=e512]: More
                        - generic [ref=e513]: 51.4 x
                  - button [ref=e514]:
                    - img [ref=e515]
                - generic [ref=e519]:
                  - img "Josh Hart" [ref=e521]
                  - generic [ref=e522]:
                    - paragraph [ref=e523]: Josh Hart
                    - paragraph [ref=e524]:
                      - generic [ref=e525]: NYK
                      - text: "- SAS"
                    - paragraph [ref=e526]: Today 8:40 PM
                  - generic [ref=e527]:
                    - paragraph [ref=e528]:
                      - text: "0.5"
                      - generic [ref=e529]: TD
                    - generic [ref=e530]:
                      - button "Less" [disabled] [ref=e531]:
                        - generic [ref=e532]: Less
                      - button "More 25.9 x" [ref=e533]:
                        - generic [ref=e534]: More
                        - generic [ref=e535]: 25.9 x
                  - button [ref=e536]:
                    - img [ref=e537]
                - generic [ref=e541]:
                  - img "De'Aaron Fox" [ref=e543]
                  - generic [ref=e544]:
                    - paragraph [ref=e545]: De'Aaron Fox
                    - paragraph [ref=e546]:
                      - generic [ref=e547]: SAS
                      - text: "- NYK"
                    - paragraph [ref=e548]: Today 8:40 PM
                  - generic [ref=e549]:
                    - paragraph [ref=e550]:
                      - text: "0.5"
                      - generic [ref=e551]: TD
                    - generic [ref=e552]:
                      - button "Less" [disabled] [ref=e553]:
                        - generic [ref=e554]: Less
                      - button "More 52 x" [ref=e555]:
                        - generic [ref=e556]: More
                        - generic [ref=e557]: 52 x
                  - button [ref=e558]:
                    - img [ref=e559]
                - button "+ Add Player" [ref=e563] [cursor=pointer]
              - generic [ref=e564]:
                - generic [ref=e565]:
                  - generic [ref=e566]:
                    - img [ref=e567]
                    - text: Your balance is insufficient - use your Promo Balance or Free Entry to enter
                  - button "Apply Promo" [ref=e569] [cursor=pointer]
                - generic [ref=e570]:
                  - generic [ref=e571]:
                    - generic [ref=e573]:
                      - radio [disabled]
                      - generic: $25
                      - radio [disabled]
                      - generic: $75
                      - radio [disabled]
                      - generic: $300
                    - generic [ref=e575]:
                      - generic [ref=e576]: $
                      - spinbutton [ref=e580]: "0"
                    - button "4" [ref=e581] [cursor=pointer]:
                      - img [ref=e582]
                      - generic [ref=e584]: "4"
                  - generic [ref=e585]:
                    - generic [ref=e586]:
                      - generic [ref=e587]:
                        - button [ref=e588]:
                          - img [ref=e589]
                        - button "All In" [ref=e591]
                      - generic [ref=e593]: 1000x
                    - generic [ref=e595]:
                      - generic [ref=e596]:
                        - paragraph [ref=e597]: Perfect line-up
                        - paragraph [ref=e598]: $0
                      - generic [ref=e600]:
                        - paragraph [ref=e601]: Or 1st place in group
                        - generic [ref=e602]: $5 +
                  - button "Place" [active] [ref=e606] [cursor=pointer]:
                    - text: Place
                    - img [ref=e607]
          - generic [ref=e610]:
            - generic [ref=e612]:
              - link "Download ParlayPlay On The Play Store" [ref=e613] [cursor=pointer]:
                - /url: https://parlayplay.onelink.me/oLJk/fh7u6juo
                - img "Download ParlayPlay On The Play Store" [ref=e614]
              - paragraph [ref=e615]:
                - text: Get the app.
                - text: Better. Faster. Convenient
            - navigation [ref=e616]:
              - link "Privacy" [ref=e617] [cursor=pointer]:
                - /url: /privacy-policy
              - link "Terms" [ref=e618] [cursor=pointer]:
                - /url: /terms
              - link "Responsible Gaming" [ref=e619] [cursor=pointer]:
                - /url: /responsible-gaming
              - link "Gaming Rules" [ref=e620] [cursor=pointer]:
                - /url: /rules
              - link "FAQ" [ref=e621] [cursor=pointer]:
                - /url: https://intercom.help/parlayplay/en/
            - navigation [ref=e622]:
              - generic [ref=e623]:
                - paragraph [ref=e624]: © ParlayPlay 2026
                - generic [ref=e625]:
                  - link [ref=e626] [cursor=pointer]:
                    - /url: https://www.facebook.com/parlayplay.io
                    - img [ref=e627]
                  - link [ref=e629] [cursor=pointer]:
                    - /url: https://www.instagram.com/parlayplay_?igsh=bHBldWQyMmV2b3Y4
                    - img [ref=e630]
                  - link [ref=e632] [cursor=pointer]:
                    - /url: https://www.twitter.com/parlay_play
                    - img [ref=e633]
                  - link [ref=e635] [cursor=pointer]:
                    - /url: https://discord.com/invite/parlayplay
                    - img [ref=e636]
                - img "21+-icon" [ref=e638]
              - paragraph [ref=e640]: Gambling can be addictive. Please play responsibly.
    - region "Notifications Alt+T":
      - alert [ref=e642] [cursor=pointer]:
        - img [ref=e644]
        - text: Your entry amount must be greater than $0
        - button "close" [ref=e646]:
          - img [ref=e647]
        - progressbar "notification timer" [ref=e651]
  - alert [ref=e652]
  - iframe [ref=e653]:
    
```

# Test source

```ts
  1   | /*
  2   |  Tail Feed end-to-end coverage for the soft-launched /challenges/feed page:
  3   |    - For You tab — empty state (single-user environment)
  4   |    - Following tab — empty state (no followed users)
  5   |    - Share toggle OFF in My Settings → newly-placed contest is not added to
  6   |      the You tab (the feed signal skips users with is_feed_visible=False)
  7   |    - Share toggle ON  → newly-placed contest appears on the You tab and the
  8   |      Tail Entry button on its card auto-tails (mirrors the existing
  9   |      slip_sharing_and_tailing flow, but driven from the feed surface)
  10  | 
  11  |  Required env vars: PPUSERNAME / PPPASSWORD (primary user). The tests assume
  12  |  the primary user is the only relevant author in the environment, so the
  13  |  public For You / Following tabs render their empty states.
  14  | */
  15  | 
  16  | import { test, expect } from '../../fixtures/test.extend';
  17  | import { ContestPage } from '../../pages/contest.page';
  18  | import { FeedPage } from '../../pages/feed.page';
  19  | import { HomePage } from '../../pages/home.page';
  20  | import { SettingsPage } from '../../pages/settings.page';
  21  | import { TailPage } from '../../pages/tail.page';
  22  | import { placeContestWithRetry } from '../../utils/contestFlow';
  23  | 
  24  | const PICK_COUNT = 3;
  25  | const ENTRY_AMOUNT = 3;
  26  | const SLIP_STORAGE_KEY = 'pp_persistent_slip:v1';
  27  | const CROSSGAME_API_PATH = /\/api\/v1\/challenges-sp\/crossgame\/?$/;
  28  | 
  29  | type PlacedContest = { uuid: string; pickIds: string[] };
  30  | 
  31  | /**
  32  |  * Drive the standard pick-then-submit flow, sniffing the
  33  |  * POST /challenges-sp/crossgame/ response so we can return the new
  34  |  * SinglePlayerContest.uuid. The uuid is what the feed envelope keys cards
  35  |  * by, so identifying our card via the network is more reliable than
  36  |  * scraping DOM that doesn't expose the id.
  37  |  */
  38  | async function placeContestAndCaptureUuid(
  39  |     homePage: HomePage,
  40  |     contestPage: ContestPage,
  41  |     page: import('@playwright/test').Page,
  42  | ): Promise<PlacedContest> {
  43  |     let uuid = '';
  44  |     const { pickIds } = await placeContestWithRetry({
  45  |         homePage,
  46  |         contestPage,
  47  |         pickCount: PICK_COUNT,
  48  |         entryAmount: ENTRY_AMOUNT,
  49  |         submit: async () => {
> 50  |             const respPromise = page.waitForResponse(
      |                                      ^ TimeoutError: page.waitForResponse: Timeout 60000ms exceeded while waiting for event "response"
  51  |                 (resp) =>
  52  |                     CROSSGAME_API_PATH.test(new URL(resp.url()).pathname) &&
  53  |                     resp.request().method() === 'POST',
  54  |                 { timeout: 60_000 },
  55  |             );
  56  | 
  57  |             const submitResult = await contestPage.submitAndAwaitResult();
  58  |             if (submitResult.success) {
  59  |                 const resp = await respPromise;
  60  |                 const body = await resp.json().catch(() => null);
  61  |                 // Server returns { redirectUrl: "/challenges/contest/<uuid>" }
  62  |                 // — see challenges/views.py:place_single_contest. CamelCase
  63  |                 // renderer rewrites snake_case before it hits the wire.
  64  |                 const redirectUrl: string = body?.redirectUrl ?? body?.redirect_url ?? '';
  65  |                 const match = redirectUrl.match(/\/challenges\/contest\/([^/?#]+)/);
  66  |                 uuid = match?.[1] ?? '';
  67  |                 expect(
  68  |                     uuid,
  69  |                     `crossgame POST should expose the new contest uuid in redirectUrl (got ${JSON.stringify(redirectUrl)})`,
  70  |                 ).toBeTruthy();
  71  |             }
  72  |             return submitResult;
  73  |         },
  74  |     });
  75  | 
  76  |     return { uuid, pickIds };
  77  | }
  78  | 
  79  | async function openSettings(page: import('@playwright/test').Page): Promise<SettingsPage> {
  80  |     // Direct navigation — we're already authenticated via storage state, and
  81  |     // routing through the home page → hamburger → settings adds two
  82  |     // dev-server compile waits and a race against the UserContext fetch
  83  |     // (the home shell briefly renders the anonymous "Join" CTA on slow
  84  |     // hydrations, which masks the Toggle Menu button).
  85  |     await page.goto('/account/update');
  86  |     const settings = new SettingsPage(page);
  87  |     // The feedVisible checkbox lives near the bottom of the form, which
  88  |     // mounts only after the user/limits/notifications GETs resolve.
  89  |     await expect(settings.feedVisibleCheckbox).toBeVisible({ timeout: 60_000 });
  90  |     return settings;
  91  | }
  92  | 
  93  | test.describe('Tail Feed', { tag: '@tailFeed' }, () => {
  94  |     // Toggling is_feed_visible mutates server-side user state, and the
  95  |     // OFF/ON tests are deliberately ordered (OFF first so any leftover
  96  |     // entry from ON doesn't pollute the OFF assertion). Serial keeps
  97  |     // those mutations from racing each other across workers.
  98  |     test.describe.configure({ mode: 'serial' });
  99  | 
  100 |     test('For You tab renders (empty hero in single-user envs, cards otherwise)', async ({
  101 |         loggedInPage: page,
  102 |     }) => {
  103 |         test.setTimeout(120_000);
  104 |         const feed = new FeedPage(page);
  105 | 
  106 |         await test.step('Open /challenges/feed (For You is the default tab)', async () => {
  107 |             await feed.open('for_you');
  108 |         });
  109 | 
  110 |         // Strict empty-state assertion is the "single user only" case in the
  111 |         // ticket. The dev DB often carries stray entries from other users,
  112 |         // so we accept either: empty hero OR at least one feed card. The
  113 |         // network 200 is verified inside FeedPage.open.
  114 |         await test.step('Tab loads — empty hero OR at least one card visible', async () => {
  115 |             await feed.assertForYouRendered();
  116 |         });
  117 |     });
  118 | 
  119 |     test('Following tab shows the empty state (single user, no follows)', async ({
  120 |         loggedInPage: page,
  121 |     }) => {
  122 |         test.setTimeout(120_000);
  123 |         const feed = new FeedPage(page);
  124 | 
  125 |         await test.step('Open feed and switch to Following', async () => {
  126 |             await feed.open('for_you');
  127 |             await feed.switchTab('following');
  128 |         });
  129 | 
  130 |         await test.step('Empty-state hero + zero feed cards', async () => {
  131 |             await feed.assertFollowingEmpty();
  132 |         });
  133 |     });
  134 | 
  135 |     test('Share toggle OFF — newly-placed contest does NOT appear on the You tab', async ({
  136 |         loggedInPage: page,
  137 |     }) => {
  138 |         test.setTimeout(360_000);
  139 |         const home = new HomePage(page);
  140 |         const contest = new ContestPage(page);
  141 |         const feed = new FeedPage(page);
  142 | 
  143 |         await test.step('Uncheck "Show My Entries In The Feed" and persist', async () => {
  144 |             // UI-level proof the toggle is exposed on the settings page,
  145 |             // then server-side toggle via the same endpoint the form posts
  146 |             // to. Going through the form would fail in dev envs where an
  147 |             // unrelated limit field is in a cross-field-invalid state and
  148 |             // react-hook-form blocks the whole save.
  149 |             const settings = await openSettings(page);
  150 |             await settings.setFeedVisibleViaAPI(false);
```