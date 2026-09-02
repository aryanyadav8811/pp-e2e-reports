# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: contests/user-enter-contest.spec.ts >> User Enter Contest >> Submit multiple contests back to back
- Location: tests/contests/user-enter-contest.spec.ts:183:5

# Error details

```
Test timeout of 240000ms exceeded.
```

```
Error: locator.click: Target page, context or browser has been closed
Call log:
  - waiting for locator('button[id^="league-"]').filter({ visible: true }).first()
    - locator resolved to <button type="button" id="league-MLB" class="py-2 px-4 font-thin text-sm text-black  bg-playYellow  rounded-full  flex-row justify-center items-center whitespace-nowrap text-sm border-white border mr-2 cursor-pointer">…</button>
  - attempting click action
    2 × waiting for element to be visible, enabled and stable
      - element is visible, enabled and stable
      - scrolling into view if needed
      - done scrolling
      - <img loading="lazy" decoding="async" alt="Gavin Williams" class="mx-auto self-end" src="https://cdn.staging.parlayplay.io/media/players/williams.png"/> from <div class="fixed inset-0 z-50 flex items-center justify-center bg-black/50">…</div> subtree intercepts pointer events
    - retrying click action
    - waiting 20ms
    - waiting for element to be visible, enabled and stable
    - element is visible, enabled and stable
    - scrolling into view if needed
    - done scrolling
    - <img loading="lazy" decoding="async" alt="Gavin Williams" class="mx-auto self-end" src="https://cdn.staging.parlayplay.io/media/players/williams.png"/> from <div class="fixed inset-0 z-50 flex items-center justify-center bg-black/50">…</div> subtree intercepts pointer events
  2 × retrying click action
      - waiting 100ms
      - waiting for element to be visible, enabled and stable
      - element is visible, enabled and stable
      - scrolling into view if needed
      - done scrolling
      - <button class="w-10 h-10 rounded-full bg-bgTertiary/40 dark:bg-bgSecondary/40">…</button> from <div class="fixed inset-0 z-50 flex items-center justify-center bg-black/50">…</div> subtree intercepts pointer events
  97 × retrying click action
       - waiting 500ms
       - waiting for element to be visible, enabled and stable
       - element is visible, enabled and stable
       - scrolling into view if needed
       - done scrolling
       - <img loading="lazy" decoding="async" alt="Gavin Williams" class="mx-auto self-end" src="https://cdn.staging.parlayplay.io/media/players/williams.png"/> from <div class="fixed inset-0 z-50 flex items-center justify-center bg-black/50">…</div> subtree intercepts pointer events
     - retrying click action
       - waiting 500ms
       - waiting for element to be visible, enabled and stable
       - element is visible, enabled and stable
       - scrolling into view if needed
       - done scrolling
       - <img loading="lazy" decoding="async" alt="Gavin Williams" class="mx-auto self-end" src="https://cdn.staging.parlayplay.io/media/players/williams.png"/> from <div class="fixed inset-0 z-50 flex items-center justify-center bg-black/50">…</div> subtree intercepts pointer events
     - retrying click action
       - waiting 500ms
       - waiting for element to be visible, enabled and stable
       - element is visible, enabled and stable
       - scrolling into view if needed
       - done scrolling
       - <button class="w-10 h-10 rounded-full bg-bgTertiary/40 dark:bg-bgSecondary/40">…</button> from <div class="fixed inset-0 z-50 flex items-center justify-center bg-black/50">…</div> subtree intercepts pointer events
     - retrying click action
       - waiting 500ms
       - waiting for element to be visible, enabled and stable
       - element is visible, enabled and stable
       - scrolling into view if needed
       - done scrolling
       - <button class="w-10 h-10 rounded-full bg-bgTertiary/40 dark:bg-bgSecondary/40">…</button> from <div class="fixed inset-0 z-50 flex items-center justify-center bg-black/50">…</div> subtree intercepts pointer events
  2 × retrying click action
      - waiting 500ms
      - waiting for element to be visible, enabled and stable
      - element is visible, enabled and stable
      - scrolling into view if needed
      - done scrolling
      - <img loading="lazy" decoding="async" alt="Gavin Williams" class="mx-auto self-end" src="https://cdn.staging.parlayplay.io/media/players/williams.png"/> from <div class="fixed inset-0 z-50 flex items-center justify-center bg-black/50">…</div> subtree intercepts pointer events
  - retrying click action
    - waiting 500ms
    - waiting for element to be visible, enabled and stable
    - element is visible, enabled and stable
    - scrolling into view if needed
    - done scrolling
    - <button class="w-10 h-10 rounded-full bg-bgTertiary/40 dark:bg-bgSecondary/40">…</button> from <div class="fixed inset-0 z-50 flex items-center justify-center bg-black/50">…</div> subtree intercepts pointer events
  - retrying click action
    - waiting 500ms
    - waiting for element to be visible, enabled and stable
    - element is visible, enabled and stable
    - scrolling into view if needed
    - done scrolling

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
            - button "Switch to dark mode" [ref=e11]:
              - img [ref=e12]
            - generic [ref=e14]:
              - generic [ref=e16]:
                - generic [ref=e17]: $220.04
                - generic [ref=e18]:
                  - img "gift-icon" [ref=e19]
                  - text: "1.00"
              - button "Toggle Menu" [ref=e20]:
                - img [ref=e21]
      - main [ref=e23]:
        - generic [ref=e28]:
          - generic [ref=e29]:
            - generic [ref=e30]:
              - list [ref=e32]:
                - button "MLB" [ref=e33] [cursor=pointer]
                - button "NFL" [ref=e34] [cursor=pointer]
                - button "WNBA" [ref=e35] [cursor=pointer]
                - button "WNBA-Combos" [ref=e36] [cursor=pointer]
                - button "WNBA Q1" [ref=e37] [cursor=pointer]
                - button "WNBA H1" [ref=e38] [cursor=pointer]
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
                  - button "NE@SEA Wed 8PM" [ref=e50] [cursor=pointer]:
                    - text: NE@SEA
                    - generic [ref=e51]: Wed 8PM
                - listitem [ref=e52]:
                  - button "SF@LAR Thu 8PM" [ref=e53] [cursor=pointer]:
                    - text: SF@LAR
                    - generic [ref=e54]: Thu 8PM
                - listitem [ref=e55]:
                  - button "CHI@CAR Sun 1PM" [ref=e56] [cursor=pointer]:
                    - text: CHI@CAR
                    - generic [ref=e57]: Sun 1PM
                - listitem [ref=e58]:
                  - button "TB@CIN Sun 1PM" [ref=e59] [cursor=pointer]:
                    - text: TB@CIN
                    - generic [ref=e60]: Sun 1PM
                - listitem [ref=e61]:
                  - button "NO@DET Sun 1PM" [ref=e62] [cursor=pointer]:
                    - text: NO@DET
                    - generic [ref=e63]: Sun 1PM
                - listitem [ref=e64]:
                  - button "BUF@HOU Sun 1PM" [ref=e65] [cursor=pointer]:
                    - text: BUF@HOU
                    - generic [ref=e66]: Sun 1PM
                - listitem [ref=e67]:
                  - button "BAL@IND Sun 1PM" [ref=e68] [cursor=pointer]:
                    - text: BAL@IND
                    - generic [ref=e69]: Sun 1PM
                - listitem [ref=e70]:
                  - button "CLE@JAX Sun 1PM" [ref=e71] [cursor=pointer]:
                    - text: CLE@JAX
                    - generic [ref=e72]: Sun 1PM
                - listitem [ref=e73]:
                  - button "ATL@PIT Sun 1PM" [ref=e74] [cursor=pointer]:
                    - text: ATL@PIT
                    - generic [ref=e75]: Sun 1PM
                - listitem [ref=e76]:
                  - button "NYJ@TEN Sun 1PM" [ref=e77] [cursor=pointer]:
                    - text: NYJ@TEN
                    - generic [ref=e78]: Sun 1PM
                - listitem [ref=e79]:
                  - button "ARI@LAC Sun 4PM" [ref=e80] [cursor=pointer]:
                    - text: ARI@LAC
                    - generic [ref=e81]: Sun 4PM
                - listitem [ref=e82]:
                  - button "MIA@LV Sun 4PM" [ref=e83] [cursor=pointer]:
                    - text: MIA@LV
                    - generic [ref=e84]: Sun 4PM
                - listitem [ref=e85]:
                  - button "GB@MIN Sun 4PM" [ref=e86] [cursor=pointer]:
                    - text: GB@MIN
                    - generic [ref=e87]: Sun 4PM
                - listitem [ref=e88]:
                  - button "WAS@PHI Sun 4PM" [ref=e89] [cursor=pointer]:
                    - text: WAS@PHI
                    - generic [ref=e90]: Sun 4PM
                - listitem [ref=e91]:
                  - button "DAL@NYG Sun 8PM" [ref=e92] [cursor=pointer]:
                    - text: DAL@NYG
                    - generic [ref=e93]: Sun 8PM
                - listitem [ref=e94]:
                  - button "DEN@KC Mon 8PM" [ref=e95] [cursor=pointer]:
                    - text: DEN@KC
                    - generic [ref=e96]: Mon 8PM
              - generic [ref=e97]:
                - generic [ref=e98]:
                  - generic [ref=e101]:
                    - img [ref=e103]
                    - textbox "Search player or team" [ref=e105]
                  - button "Change card style from grid" [ref=e107]
                - list [ref=e109]:
                  - listitem [ref=e110]:
                    - button "Passing Yards" [ref=e111]
                  - listitem [ref=e112]:
                    - button "Passing TDs" [ref=e113]
                  - listitem [ref=e114]:
                    - button "Interception" [ref=e115]
                  - listitem [ref=e116]:
                    - button "Rushing Yards" [ref=e117]
                  - listitem [ref=e118]:
                    - button "Receiving Yards" [ref=e119]
                  - listitem [ref=e120]:
                    - button "Receptions" [ref=e121]
                  - listitem [ref=e122]:
                    - button "Pass + Rush + Rec TD" [ref=e123]
            - generic [ref=e124]:
              - generic [ref=e129]:
                - generic [ref=e132] [cursor=pointer]:
                  - generic [ref=e133]:
                    - generic [ref=e134]: Refer a friend, get a $20 Free Entry
                    - generic [ref=e135]: Referral bonus
                  - button "Refer" [ref=e136]
                - generic [ref=e139] [cursor=pointer]:
                  - generic [ref=e140]:
                    - generic [ref=e141]:
                      - img [ref=e142]
                      - generic [ref=e146]: Boosted Picks
                    - generic [ref=e147]: "Every Pick Pays: Up to a 35% Boost!"
                  - button "Details" [ref=e149]
                - generic [ref=e152] [cursor=pointer]:
                  - generic [ref=e153]:
                    - generic [ref=e154]:
                      - generic [ref=e155]: $5
                      - generic [ref=e156]: Free Entry
                    - generic [ref=e157]: $5 Free WNBA Entry
                  - generic [ref=e158]:
                    - button "Claim" [ref=e159]
                    - generic [ref=e160]:
                      - img [ref=e161]
                      - generic [ref=e163]: 75h
                      - button "more info" [ref=e164]
                - generic [ref=e167] [cursor=pointer]:
                  - generic [ref=e168]:
                    - generic [ref=e169]:
                      - generic [ref=e170]: $7
                      - generic [ref=e171]: Protected Pick
                    - generic [ref=e172]: PP Aug 13
                  - generic [ref=e173]:
                    - button "Claim" [ref=e174]
                    - generic [ref=e175]:
                      - img [ref=e176]
                      - generic [ref=e178]: 3h
                      - button "more info" [ref=e179]
                - generic [ref=e182] [cursor=pointer]:
                  - generic [ref=e183]:
                    - generic [ref=e184]:
                      - generic [ref=e185]: 100%
                      - generic [ref=e186]: Deposit Match
                    - generic [ref=e187]: New User Promotion
                  - button "Deposit" [ref=e189]
                - generic [ref=e193] [cursor=pointer]:
                  - generic [ref=e194]: Pull real graded cards worth up to $10,000
                  - generic [ref=e195]: Sell or ship instantly
                  - button "Rip a pack" [ref=e196]:
                    - generic [ref=e197]:
                      - img [ref=e198]
                      - text: Rip a pack
              - generic [ref=e204]:
                - generic [ref=e207]:
                  - generic [ref=e210]:
                    - button "Open expert opinion for Drake Maye" [ref=e211]:
                      - img [ref=e212]
                    - img "Drake Maye" [ref=e215]
                  - generic [ref=e216]:
                    - generic [ref=e217]: Drake Maye
                    - button "221.5 Ps Yd" [ref=e218]:
                      - generic [ref=e219]:
                        - img [ref=e220]
                        - img [ref=e222]
                      - generic [ref=e224]: "221.5"
                      - generic [ref=e225]: Ps Yd
                    - generic [ref=e226]:
                      - generic [ref=e227]: NE@SEA
                      - generic [ref=e228]: Wed 8PM
                    - generic [ref=e229]:
                      - button "Select over 221.5 Passing Yards for 1.78 times" [ref=e230]:
                        - img [ref=e231]
                        - img [ref=e235]
                        - generic [ref=e237]: 1.78x
                      - button "Select over 221.5 Passing Yards for 1.78 times" [ref=e238]:
                        - generic [ref=e239]: 1.78x
                        - img [ref=e240]
                - generic [ref=e244]:
                  - generic [ref=e247]:
                    - button "Open expert opinion for Brock Purdy" [ref=e248]:
                      - img [ref=e249]
                    - img "Brock Purdy" [ref=e252]
                  - generic [ref=e253]:
                    - generic [ref=e254]: Brock Purdy
                    - button "242.5 Ps Yd" [ref=e255]:
                      - generic [ref=e256]:
                        - img [ref=e257]
                        - img [ref=e259]
                      - generic [ref=e261]: "242.5"
                      - generic [ref=e262]: Ps Yd
                    - generic [ref=e263]:
                      - generic [ref=e264]: SF@LAR
                      - generic [ref=e265]: Thu 8PM
                    - generic [ref=e266]:
                      - button "Select over 242.5 Passing Yards for 1.78 times" [ref=e267]:
                        - img [ref=e268]
                        - generic [ref=e270]: 1.78x
                      - button "Select over 242.5 Passing Yards for 1.78 times" [ref=e271]:
                        - generic [ref=e272]: 1.78x
                        - img [ref=e273]
                - generic [ref=e277]:
                  - generic [ref=e280]:
                    - button "Open expert opinion for Matthew Stafford" [ref=e281]:
                      - img [ref=e282]
                    - img "Matthew Stafford" [ref=e285]
                  - generic [ref=e286]:
                    - generic [ref=e287]: M. Stafford
                    - button "263.5 Ps Yd" [ref=e288]:
                      - generic [ref=e289]:
                        - img [ref=e290]
                        - img [ref=e292]
                      - generic [ref=e294]: "263.5"
                      - generic [ref=e295]: Ps Yd
                    - generic [ref=e296]:
                      - generic [ref=e297]: SF@LAR
                      - generic [ref=e298]: Thu 8PM
                    - generic [ref=e299]:
                      - button "Select over 263.5 Passing Yards for 1.78 times" [ref=e300]:
                        - img [ref=e301]
                        - generic [ref=e303]: 1.78x
                      - button "Select over 263.5 Passing Yards for 1.78 times" [ref=e304]:
                        - generic [ref=e305]: 1.78x
                        - img [ref=e306]
                - generic [ref=e310]:
                  - generic [ref=e313]:
                    - button "Open expert opinion for Caleb Williams" [ref=e314]:
                      - img [ref=e315]
                    - img "Caleb Williams" [ref=e318]
                  - generic [ref=e319]:
                    - generic [ref=e320]: C. Williams
                    - button "239.5 Ps Yd" [ref=e321]:
                      - generic [ref=e322]:
                        - img [ref=e323]
                        - img [ref=e325]
                      - generic [ref=e327]: "239.5"
                      - generic [ref=e328]: Ps Yd
                    - generic [ref=e329]:
                      - generic [ref=e330]: CHI@CAR
                      - generic [ref=e331]: Sun 1PM
                    - generic [ref=e332]:
                      - button "Select over 239.5 Passing Yards for 1.78 times" [ref=e333]:
                        - img [ref=e334]
                        - generic [ref=e336]: 1.78x
                      - button "Select over 239.5 Passing Yards for 1.78 times" [ref=e337]:
                        - generic [ref=e338]: 1.78x
                        - img [ref=e339]
                - generic [ref=e343]:
                  - generic [ref=e346]:
                    - button "Open expert opinion for Bryce Young" [ref=e347]:
                      - img [ref=e348]
                    - img "Bryce Young" [ref=e351]
                  - generic [ref=e352]:
                    - generic [ref=e353]: Bryce Young
                    - button "196.5 Ps Yd" [ref=e354]:
                      - generic [ref=e355]:
                        - img [ref=e356]
                        - img [ref=e358]
                      - generic [ref=e360]: "196.5"
                      - generic [ref=e361]: Ps Yd
                    - generic [ref=e362]:
                      - generic [ref=e363]: CHI@CAR
                      - generic [ref=e364]: Sun 1PM
                    - generic [ref=e365]:
                      - button "Select over 196.5 Passing Yards for 1.78 times" [ref=e366]:
                        - img [ref=e367]
                        - generic [ref=e369]: 1.78x
                      - button "Select over 196.5 Passing Yards for 1.78 times" [ref=e370]:
                        - generic [ref=e371]: 1.78x
                        - img [ref=e372]
                - generic [ref=e376]:
                  - generic [ref=e379]:
                    - button "Open expert opinion for Joe Burrow" [ref=e380]:
                      - img [ref=e381]
                    - img "Joe Burrow" [ref=e384]
                  - generic [ref=e385]:
                    - generic [ref=e386]: Joe Burrow
                    - button "265.5 Ps Yd" [ref=e387]:
                      - generic [ref=e388]:
                        - img [ref=e389]
                        - img [ref=e391]
                      - generic [ref=e393]: "265.5"
                      - generic [ref=e394]: Ps Yd
                    - generic [ref=e395]:
                      - generic [ref=e396]: TB@CIN
                      - generic [ref=e397]: Sun 1PM
                    - generic [ref=e398]:
                      - button "Select over 265.5 Passing Yards for 1.78 times" [ref=e399]:
                        - img [ref=e400]
                        - generic [ref=e402]: 1.78x
                      - button "Select over 265.5 Passing Yards for 1.78 times" [ref=e403]:
                        - generic [ref=e404]: 1.78x
                        - img [ref=e405]
                - generic [ref=e409]:
                  - generic [ref=e412]:
                    - button "Open expert opinion for Baker Mayfield" [ref=e413]:
                      - img [ref=e414]
                    - img "Baker Mayfield" [ref=e417]
                  - generic [ref=e418]:
                    - generic [ref=e419]: B. Mayfield
                    - button "248.5 Ps Yd" [ref=e420]:
                      - generic [ref=e421]:
                        - img [ref=e422]
                        - img [ref=e424]
                      - generic [ref=e426]: "248.5"
                      - generic [ref=e427]: Ps Yd
                    - generic [ref=e428]:
                      - generic [ref=e429]: TB@CIN
                      - generic [ref=e430]: Sun 1PM
                    - generic [ref=e431]:
                      - button "Select over 248.5 Passing Yards for 1.78 times" [ref=e432]:
                        - img [ref=e433]
                        - generic [ref=e435]: 1.78x
                      - button "Select over 248.5 Passing Yards for 1.78 times" [ref=e436]:
                        - generic [ref=e437]: 1.78x
                        - img [ref=e438]
                - generic [ref=e442]:
                  - generic [ref=e445]:
                    - button "Open expert opinion for Jared Goff" [ref=e446]:
                      - img [ref=e447]
                    - img "Jared Goff" [ref=e450]
                  - generic [ref=e451]:
                    - generic [ref=e452]: Jared Goff
                    - button "271.5 Ps Yd" [ref=e453]:
                      - generic [ref=e454]:
                        - img [ref=e455]
                        - img [ref=e457]
                      - generic [ref=e459]: "271.5"
                      - generic [ref=e460]: Ps Yd
                    - generic [ref=e461]:
                      - generic [ref=e462]: NO@DET
                      - generic [ref=e463]: Sun 1PM
                    - generic [ref=e464]:
                      - button "Select over 271.5 Passing Yards for 1.78 times" [ref=e465]:
                        - img [ref=e466]
                        - generic [ref=e468]: 1.78x
                      - button "Select over 271.5 Passing Yards for 1.78 times" [ref=e469]:
                        - generic [ref=e470]: 1.78x
                        - img [ref=e471]
                - generic [ref=e475]:
                  - generic [ref=e478]:
                    - button "Open expert opinion for Tyler Shough" [ref=e479]:
                      - img [ref=e480]
                    - img "Tyler Shough" [ref=e483]
                  - generic [ref=e484]:
                    - generic [ref=e485]: Tyler Shough
                    - button "249.5 Ps Yd" [ref=e486]:
                      - generic [ref=e487]:
                        - img [ref=e488]
                        - img [ref=e490]
                      - generic [ref=e492]: "249.5"
                      - generic [ref=e493]: Ps Yd
                    - generic [ref=e494]:
                      - generic [ref=e495]: NO@DET
                      - generic [ref=e496]: Sun 1PM
                    - generic [ref=e497]:
                      - button "Select over 249.5 Passing Yards for 1.78 times" [ref=e498]:
                        - img [ref=e499]
                        - generic [ref=e501]: 1.78x
                      - button "Select over 249.5 Passing Yards for 1.78 times" [ref=e502]:
                        - generic [ref=e503]: 1.78x
                        - img [ref=e504]
                - generic [ref=e508]:
                  - generic [ref=e511]:
                    - button "Open expert opinion for Josh Allen" [ref=e512]:
                      - img [ref=e513]
                    - img "Josh Allen" [ref=e516]
                  - generic [ref=e517]:
                    - generic [ref=e518]: Josh Allen
                    - button "223.5 Ps Yd" [ref=e519]:
                      - generic [ref=e520]:
                        - img [ref=e521]
                        - img [ref=e523]
                      - generic [ref=e525]: "223.5"
                      - generic [ref=e526]: Ps Yd
                    - generic [ref=e527]:
                      - generic [ref=e528]: BUF@HOU
                      - generic [ref=e529]: Sun 1PM
                    - generic [ref=e530]:
                      - button "Select over 223.5 Passing Yards for 1.78 times" [ref=e531]:
                        - img [ref=e532]
                        - generic [ref=e534]: 1.78x
                      - button "Select over 223.5 Passing Yards for 1.78 times" [ref=e535]:
                        - generic [ref=e536]: 1.78x
                        - img [ref=e537]
                - generic [ref=e541]:
                  - generic [ref=e544]:
                    - button "Open expert opinion for C.J. Stroud" [ref=e545]:
                      - img [ref=e546]
                    - img "C.J. Stroud" [ref=e549]
                  - generic [ref=e550]:
                    - generic [ref=e551]: C.J. Stroud
                    - button "228.5 Ps Yd" [ref=e552]:
                      - generic [ref=e553]:
                        - img [ref=e554]
                        - img [ref=e556]
                      - generic [ref=e558]: "228.5"
                      - generic [ref=e559]: Ps Yd
                    - generic [ref=e560]:
                      - generic [ref=e561]: BUF@HOU
                      - generic [ref=e562]: Sun 1PM
                    - generic [ref=e563]:
                      - button "Select over 228.5 Passing Yards for 1.78 times" [ref=e564]:
                        - img [ref=e565]
                        - generic [ref=e567]: 1.78x
                      - button "Select over 228.5 Passing Yards for 1.78 times" [ref=e568]:
                        - generic [ref=e569]: 1.78x
                        - img [ref=e570]
                - generic [ref=e574]:
                  - generic [ref=e577]:
                    - button "Open expert opinion for Lamar Jackson" [ref=e578]:
                      - img [ref=e579]
                    - img "Lamar Jackson" [ref=e582]
                  - generic [ref=e583]:
                    - generic [ref=e584]: Lamar Jackson
                    - button "219.5 Ps Yd" [ref=e585]:
                      - generic [ref=e586]:
                        - img [ref=e587]
                        - img [ref=e589]
                      - generic [ref=e591]: "219.5"
                      - generic [ref=e592]: Ps Yd
                    - generic [ref=e593]:
                      - generic [ref=e594]: BAL@IND
                      - generic [ref=e595]: Sun 1PM
                    - generic [ref=e596]:
                      - button "Select over 219.5 Passing Yards for 1.78 times" [ref=e597]:
                        - img [ref=e598]
                        - generic [ref=e600]: 1.78x
                      - button "Select over 219.5 Passing Yards for 1.78 times" [ref=e601]:
                        - generic [ref=e602]: 1.78x
                        - img [ref=e603]
            - generic [ref=e606]:
              - img [ref=e608]
              - generic [ref=e610]:
                - generic [ref=e612]:
                  - generic [ref=e613]: 15.37x
                  - generic [ref=e614]: 17.68x
                - generic [ref=e615]:
                  - button "+ 20% Boost 🚀" [ref=e623]:
                    - generic [ref=e624]: + 20% Boost 🚀
                  - generic [ref=e632]: "Add 6th Pick: 20% Boost"
              - button "Continue" [ref=e633] [cursor=pointer]
            - generic [ref=e635]:
              - generic [ref=e636]:
                - button [ref=e637]:
                  - img [ref=e638]
                - generic [ref=e640]: Make Your More/Less Picks
              - generic [ref=e641]:
                - generic [ref=e643]:
                  - img "Gavin Williams" [ref=e645]
                  - generic [ref=e646]:
                    - paragraph [ref=e647]: Gavin Williams
                    - paragraph [ref=e648]:
                      - generic [ref=e649]: CLE
                      - text: "- SD"
                    - paragraph [ref=e650]: Today 7:10 PM
                  - generic [ref=e651]:
                    - paragraph [ref=e652]:
                      - text: "7.5"
                      - generic [ref=e653]: SO (K)
                    - generic [ref=e654]:
                      - button "Less 1.56 x" [ref=e655]:
                        - generic [ref=e656]: Less
                        - generic [ref=e657]: 1.56 x
                      - button "More 2.12 x" [ref=e658]:
                        - generic [ref=e659]: More
                        - generic [ref=e660]: 2.12 x
                  - button [ref=e661]:
                    - img [ref=e662]
                - generic [ref=e666]:
                  - img "Shane Bieber" [ref=e668]
                  - generic [ref=e669]:
                    - paragraph [ref=e670]: Shane Bieber
                    - paragraph [ref=e671]:
                      - generic [ref=e672]: TOR
                      - text: "- NYY"
                    - paragraph [ref=e673]: Today 7:15 PM
                  - generic [ref=e674]:
                    - paragraph [ref=e675]:
                      - text: "5.5"
                      - generic [ref=e676]: SO (K)
                    - generic [ref=e677]:
                      - button "Less 1.56 x" [ref=e678]:
                        - generic [ref=e679]: Less
                        - generic [ref=e680]: 1.56 x
                      - button "More 2.14 x" [ref=e681]:
                        - generic [ref=e682]: More
                        - generic [ref=e683]: 2.14 x
                  - button [ref=e684]:
                    - img [ref=e685]
                - generic [ref=e689]:
                  - img "George Kirby" [ref=e691]
                  - generic [ref=e692]:
                    - paragraph [ref=e693]: George Kirby
                    - paragraph [ref=e694]:
                      - generic [ref=e695]: SEA
                      - text: "- HOU"
                    - paragraph [ref=e696]: Today 8:10 PM
                  - generic [ref=e697]:
                    - paragraph [ref=e698]:
                      - text: "4.5"
                      - generic [ref=e699]: SO (K)
                    - generic [ref=e700]:
                      - button "Less 2.19 x" [ref=e701]:
                        - generic [ref=e702]: Less
                        - generic [ref=e703]: 2.19 x
                      - button "More 1.52 x" [ref=e704]:
                        - generic [ref=e705]: More
                        - generic [ref=e706]: 1.52 x
                  - button [ref=e707]:
                    - img [ref=e708]
                - generic [ref=e712]:
                  - img "Kyle Freeland" [ref=e714]
                  - generic [ref=e715]:
                    - paragraph [ref=e716]: Kyle Freeland
                    - paragraph [ref=e717]:
                      - generic [ref=e718]: COL
                      - text: "- SF"
                    - paragraph [ref=e719]: Today 10:15 PM
                  - generic [ref=e720]:
                    - paragraph [ref=e721]:
                      - text: "5.5"
                      - generic [ref=e722]: SO (K)
                    - generic [ref=e723]:
                      - button "Less 1.62 x" [ref=e724]:
                        - generic [ref=e725]: Less
                        - generic [ref=e726]: 1.62 x
                      - button "More 2.04 x" [ref=e727]:
                        - generic [ref=e728]: More
                        - generic [ref=e729]: 2.04 x
                  - button [ref=e730]:
                    - img [ref=e731]
                - generic [ref=e735]:
                  - img "Drake Maye" [ref=e737]
                  - generic [ref=e738]:
                    - paragraph [ref=e739]: Drake Maye
                    - paragraph [ref=e740]:
                      - generic [ref=e741]: NE
                      - text: "- SEA"
                    - paragraph [ref=e742]: Sep 9th 8:20 PM
                  - generic [ref=e743]:
                    - paragraph [ref=e744]:
                      - text: "221.5"
                      - generic [ref=e745]: Ps Yd
                    - generic [ref=e746]:
                      - button "Less 1.78 x" [ref=e747]:
                        - generic [ref=e748]: Less
                        - generic [ref=e749]: 1.78 x
                      - button "More 1.78 x" [ref=e750]:
                        - generic [ref=e751]: More
                        - generic [ref=e752]: 1.78 x
                  - button [ref=e753]:
                    - img [ref=e754]
                - button "Add Icon Add Player Add 1 More Pick for a 20% Boost Boost Icon" [ref=e758]:
                  - generic [ref=e759]:
                    - img "Add Icon" [ref=e761]
                    - generic [ref=e762]: Add Player
                  - generic [ref=e763]:
                    - generic [ref=e764]: Add 1 More Pick for a 20% Boost
                    - img "Boost Icon" [ref=e766]
              - generic [ref=e768]:
                - generic [ref=e769]:
                  - generic [ref=e771]:
                    - radio
                    - generic [ref=e772] [cursor=pointer]: $25
                    - radio
                    - generic [ref=e773] [cursor=pointer]: $75
                    - radio [disabled]
                    - generic: $300
                  - generic [ref=e775]:
                    - generic [ref=e776]: $
                    - spinbutton [ref=e780]: "3"
                  - button "1" [ref=e781] [cursor=pointer]:
                    - img [ref=e782]
                    - generic [ref=e784]: "1"
                - generic [ref=e785]:
                  - generic [ref=e786]:
                    - generic [ref=e787]:
                      - button "Insured" [ref=e788]
                      - button "All In" [ref=e789]
                    - generic [ref=e790]:
                      - generic [ref=e791]: 15.37x
                      - generic [ref=e792]: 17.68x
                  - generic [ref=e794]:
                    - generic [ref=e795]:
                      - paragraph [ref=e796]: Perfect line-up
                      - paragraph [ref=e797]: $53.04
                    - generic [ref=e799]:
                      - paragraph [ref=e800]: Or 1st place in group
                      - generic [ref=e801]: $1 + $53.04
                - button "Place" [ref=e805] [cursor=pointer]:
                  - text: Place
                  - img [ref=e806]
          - generic [ref=e809]:
            - generic [ref=e811]:
              - link "Download ParlayPlay On The App Store" [ref=e812]:
                - /url: https://parlayplay.onelink.me/oLJk/gnqpwjha
                - img "Download ParlayPlay On The App Store" [ref=e813]
              - paragraph [ref=e814]:
                - text: Get the app.
                - text: Better. Faster. Convenient
            - navigation [ref=e815]:
              - link "Privacy" [ref=e816]:
                - /url: /privacy-policy
              - link "Fantasy Terms" [ref=e817]:
                - /url: /terms
              - link "Packs Terms" [ref=e818]:
                - /url: /terms/packs
              - link "Responsible Gaming" [ref=e819]:
                - /url: /responsible-gaming
              - link "Gaming Rules" [ref=e820]:
                - /url: /rules
              - link "FAQ" [ref=e821]:
                - /url: https://intercom.help/parlayplay/en/
            - navigation [ref=e822]:
              - generic [ref=e823]:
                - paragraph [ref=e824]: © ParlayPlay 2026
                - generic [ref=e825]:
                  - link "ParlayPlay on Facebook" [ref=e826]:
                    - /url: https://www.facebook.com/parlayplay.io
                    - img [ref=e827]
                  - link "ParlayPlay on Instagram" [ref=e829]:
                    - /url: https://www.instagram.com/parlayplay_?igsh=bHBldWQyMmV2b3Y4
                    - img [ref=e830]
                  - link "ParlayPlay on Twitter" [ref=e832]:
                    - /url: https://www.twitter.com/parlay_play
                    - img [ref=e833]
                  - link "ParlayPlay on Discord" [ref=e835]:
                    - /url: https://discord.com/invite/parlayplay
                    - img [ref=e836]
                - img "18+ icon" [ref=e838]
            - paragraph [ref=e840]
    - region "Notifications Alt+T"
  - alert [ref=e841]: ParlayPlay | Fun Fantasy Sports
```

# Test source

```ts
  227 |   }
  228 | 
  229 |   async listLeagueButtons(): Promise<Locator[]> {
  230 |     const n = await this.leagueButtons.count();
  231 |     const leagueButtonsLocator: Locator[] = [];
  232 |     for (let i = 0; i < n; i++) {
  233 |       leagueButtonsLocator.push(this.leagueButtons.nth(i));
  234 |     }
  235 |     return leagueButtonsLocator;
  236 |   }
  237 | 
  238 |   async isContinueEnabled(): Promise<boolean> {
  239 |     const button = this.continueBtn;
  240 |     const isPresent = await button.isVisible().catch(() => false);
  241 |     if (!isPresent) return false;
  242 |     const enabled = await button.isEnabled().catch(() => false);
  243 |     return enabled;
  244 |   }
  245 | 
  246 |   async trySelectPick(card: Locator): Promise<boolean> {
  247 |     const buttons = this.pickButtons(card);
  248 |     const lessButton = buttons.first();
  249 |     // Bounded checks: league/stat filter updates run inside useTransition and
  250 |     // the grid is virtualised, so a card captured from listVisiblePlayerIds
  251 |     // can unmount before we act on it. With no actionTimeout configured, an
  252 |     // unbounded isEnabled()/click() on a gone card would hang the test —
  253 |     // treat "card no longer there" as an unpickable card instead.
  254 |     let isEnabled: boolean;
  255 |     try {
  256 |       isEnabled = await lessButton.isEnabled({ timeout: 5000 });
  257 |     } catch {
  258 |       return false;
  259 |     }
  260 | 
  261 |     try {
  262 |       await buttons.nth(isEnabled ? 0 : 1).click({ timeout: 10_000 });
  263 |     } catch {
  264 |       return false;
  265 |     }
  266 | 
  267 |     //warning modal check
  268 |     try {
  269 |       const modal = this.warningModal;
  270 |       if (await modal.isVisible({ timeout: 2000 }).catch(() => false)) {
  271 |         await modal.getByRole("button", { name: "Understood" }).click();
  272 |         return false;
  273 |       }
  274 |     } catch {
  275 |       // log will be added
  276 |     }
  277 |     return true;
  278 |   }
  279 | 
  280 |   async deselectPick(card: Locator): Promise<void> {
  281 |     const buttons = this.pickButtons(card);
  282 |     const count = await buttons.count();
  283 | 
  284 |     for (let i = 0; i < count; i++) {
  285 |       const btn = buttons.nth(i);
  286 |       const classes = (await btn.getAttribute("class")) ?? "";
  287 |       if (classes.includes("bg-playYellow")) {
  288 |         await btn.click(); // Deselects the selected button
  289 |         return;
  290 |       }
  291 |     }
  292 |     throw new Error("No selected button found with bg-yellow class.");
  293 |   }
  294 | 
  295 |   /**
  296 |    * Picks `count` players.
  297 |    *
  298 |    * `excludeIds` skips players that a previous attempt already tried. Retries
  299 |    * (e.g. after "multiple promos cannot be applied") pass the players from the
  300 |    * failed slip so the next attempt selects genuinely new cards instead of
  301 |    * re-picking the same promo-bearing players in the same deterministic order.
  302 |    */
  303 |   async pickPlayers(
  304 |     count: number,
  305 |     statIdx?: number,
  306 |     excludeIds?: Set<string>,
  307 |   ): Promise<string[]> {
  308 |     const leagueButtons = await this.listLeagueButtons();
  309 | 
  310 |     const selected = new Set<string>();
  311 |     let lastPickId: string | null = null;
  312 |     // Caller-provided players to skip for the whole call. Kept separate from
  313 |     // recentlyFailed (which is cleared once a valid combo is found) so retries
  314 |     // never re-pick a player a prior attempt already tried.
  315 |     const excluded = new Set<string>(excludeIds ?? []);
  316 |     const recentlyFailed = new Set<string>();
  317 |     for (const leagueButton of leagueButtons) {
  318 |       const leagueId = (await leagueButton.getAttribute("id")) ?? "";
  319 |       // Skip the Combo (`league-*-combo`) and Promo (`league-Promo`) leagues:
  320 |       // every card in them carries a promo, so picking >1 always trips
  321 |       // "multiple promos cannot be applied" — and since the whole league is
  322 |       // promos, re-picking never escapes it. Regular sport leagues almost
  323 |       // never stack two promos (the exclusion retry handles the rare case).
  324 |       const lid = leagueId.toLowerCase();
  325 |       if (lid.includes("combo") || lid.includes("promo")) continue;
  326 | 
> 327 |       await leagueButton.click();
      |                          ^ Error: locator.click: Target page, context or browser has been closed
  328 |       await this.waitForPlayersGrid();
  329 | 
  330 |       // Each league resets to its default stat tab on click, so re-pin
  331 |       // the requested stat after navigating into the league.
  332 |       if (statIdx !== undefined) {
  333 |         const statTab = this.statsSelector.locator("li button").nth(statIdx);
  334 |         if (await statTab.isVisible().catch(() => false)) {
  335 |           await statTab.click();
  336 |           await this.waitForPlayersGrid();
  337 |         }
  338 |       }
  339 | 
  340 |       if (await this.noPlayerLabel.isVisible().catch(() => false)) {
  341 |         continue;
  342 |       }
  343 | 
  344 |       const playerIds = await this.listVisiblePlayerIds();
  345 |       for (const playerId of playerIds) {
  346 |         if (
  347 |           selected.has(playerId) ||
  348 |           recentlyFailed.has(playerId) ||
  349 |           excluded.has(playerId)
  350 |         )
  351 |           continue;
  352 | 
  353 |         if (await this.trySelectPick(this.playerCardById(playerId))) {
  354 |           selected.add(playerId);
  355 |           lastPickId = playerId;
  356 | 
  357 |           let continueFlag = await this.isContinueEnabled();
  358 |           if (selected.size >= count && continueFlag)
  359 |             return Array.from(selected);
  360 | 
  361 |           // Warning modal continuation
  362 |           while (!continueFlag && selected.size == count && lastPickId) {
  363 |             await this.deselectPick(this.playerCardById(lastPickId));
  364 |             selected.delete(lastPickId);
  365 |             recentlyFailed.add(lastPickId);
  366 | 
  367 |             let replaced = false;
  368 |             for (const nextId of playerIds) {
  369 |               if (
  370 |                 selected.has(nextId) ||
  371 |                 recentlyFailed.has(nextId) ||
  372 |                 excluded.has(nextId)
  373 |               )
  374 |                 continue;
  375 |               if (await this.trySelectPick(this.playerCardById(nextId))) {
  376 |                 selected.add(nextId);
  377 |                 lastPickId = nextId;
  378 |                 replaced = true;
  379 |                 break;
  380 |               }
  381 |             }
  382 |             if (!replaced) {
  383 |               throw new Error(
  384 |                 `Unable to find replacement pick when Continue is disabled (target: ${count})`
  385 |               );
  386 |             }
  387 |             continueFlag = await this.isContinueEnabled();
  388 |           }
  389 | 
  390 |           if (continueFlag && selected.size == count)
  391 |             return Array.from(selected);
  392 |           if (continueFlag) recentlyFailed.clear();
  393 |         }
  394 |       }
  395 |     }
  396 | 
  397 |     if (selected.size < count)
  398 |       throw new Error(`Could not select ${count} valid picks`);
  399 |     return Array.from(selected);
  400 |   }
  401 | 
  402 |   async pickFivePlayers(): Promise<string[]> {
  403 |     return this.pickPlayers(5);
  404 |   }
  405 | 
  406 |   /**
  407 |    * Reads the persisted slip from localStorage and returns the set of player
  408 |    * IDs it currently contains. Source of truth is the storage key the app
  409 |    * writes via `slipPersistence.saveSlip` — see `utils/slipPersistence.ts`.
  410 |    *
  411 |    * Why this over scraping the DOM: card visualisation depends on the offering
  412 |    * having a flagged main/default altLine. When the backend omits those flags
  413 |    * for a player (e.g. Cunningham bb_points), the card boots on a fallback
  414 |    * line that doesn't match the picked one, and the highlight isn't visible
  415 |    * even though the pick is correctly persisted. Reading storage decouples the
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
```