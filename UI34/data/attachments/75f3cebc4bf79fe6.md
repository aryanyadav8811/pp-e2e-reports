# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: contests/user-enter-contest.spec.ts >> User Enter Contest >> Contest creation and validate in entries section
- Location: tests/contests/user-enter-contest.spec.ts:74:5

# Error details

```
Test timeout of 300000ms exceeded.
```

```
Error: locator.click: Target page, context or browser has been closed
Call log:
  - waiting for getByTestId('stats-selector').filter({ visible: true }).first().locator('li button').nth(1)
    - locator resolved to <button class="mx-2 border-b-2 border-transparent">…</button>
  - attempting click action
    2 × waiting for element to be visible, enabled and stable
      - element is visible, enabled and stable
      - scrolling into view if needed
      - done scrolling
      - <div class="flex flex-row items-center justify-start min-w-16 pr-1 whitespace-nowrap text-base text-grey-vDark font-museo">1000x</div> from <div class="fixed z-40 flex flex-row w-full text-white rounded-tl-lg rounded-tr-lg bg-playYellow shadow-footer px-4 items-start justify-start h-fit pb-4 bottom-16 md:w-112">…</div> subtree intercepts pointer events
    - retrying click action
    - waiting 20ms
    - waiting for element to be visible, enabled and stable
    - element is visible, enabled and stable
    - scrolling into view if needed
    - done scrolling
    - <div class="flex flex-row items-center justify-start min-w-16 pr-1 whitespace-nowrap text-base text-grey-vDark font-museo">1000x</div> from <div class="fixed z-40 flex flex-row w-full text-white rounded-tl-lg rounded-tr-lg bg-playYellow shadow-footer px-4 items-start justify-start h-fit pb-4 bottom-16 md:w-112">…</div> subtree intercepts pointer events
  - retrying click action
    - waiting 100ms
    - waiting for element to be visible, enabled and stable
    - element is visible, enabled and stable
    - scrolling into view if needed
    - done scrolling
    - <img width="30px" height="30px" class="inline mr-3" alt="Parlay Play Logo" src="https://cdn.staging.parlayplay.io/static/svgs/ParlayPlayLogo_w_y_v2.svg"/> from <header class="fixed z-50 w-full py-2 bg-transparent md:w-112 desk:w-full desk:flex desk:justify-center desk:sticky md:mx-auto tb:bg-playYellow desk:z-100">…</header> subtree intercepts pointer events
  - retrying click action
    - waiting 100ms
    34 × waiting for element to be visible, enabled and stable
       - element is visible, enabled and stable
       - scrolling into view if needed
       - done scrolling
       - <img width="30px" height="30px" class="inline mr-3" alt="Parlay Play Logo" src="https://cdn.staging.parlayplay.io/static/svgs/ParlayPlayLogo_w_y_v2.svg"/> from <header class="fixed z-50 w-full py-2 bg-playYellow md:w-112 desk:w-full desk:flex desk:justify-center desk:sticky md:mx-auto tb:bg-playYellow desk:z-100">…</header> subtree intercepts pointer events
     - retrying click action
       - waiting 500ms
       - waiting for element to be visible, enabled and stable
       - element is visible, enabled and stable
       - scrolling into view if needed
       - done scrolling
       - <div class="flex flex-row items-center justify-start min-w-16 pr-1 whitespace-nowrap text-base text-grey-vDark font-museo">1000x</div> from <div class="fixed z-40 flex flex-row w-full text-white rounded-tl-lg rounded-tr-lg bg-playYellow shadow-footer px-4 items-start justify-start h-fit pb-4 bottom-16 md:w-112">…</div> subtree intercepts pointer events
     - retrying click action
       - waiting 500ms
       - waiting for element to be visible, enabled and stable
       - element is visible, enabled and stable
       - scrolling into view if needed
       - done scrolling
       - <div class="flex flex-row items-center justify-start min-w-16 pr-1 whitespace-nowrap text-base text-grey-vDark font-museo">1000x</div> from <div class="fixed z-40 flex flex-row w-full text-white rounded-tl-lg rounded-tr-lg bg-playYellow shadow-footer px-4 items-start justify-start h-fit pb-4 bottom-16 md:w-112">…</div> subtree intercepts pointer events
     - retrying click action
       - waiting 500ms
       - waiting for element to be visible, enabled and stable
       - element is visible, enabled and stable
       - scrolling into view if needed
       - done scrolling
       - <img width="30px" height="30px" class="inline mr-3" alt="Parlay Play Logo" src="https://cdn.staging.parlayplay.io/static/svgs/ParlayPlayLogo_w_y_v2.svg"/> from <header class="fixed z-50 w-full py-2 bg-transparent md:w-112 desk:w-full desk:flex desk:justify-center desk:sticky md:mx-auto tb:bg-playYellow desk:z-100">…</header> subtree intercepts pointer events
     - retrying click action
       - waiting 500ms

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
              - generic [ref=e17]: $911.58
              - button "Toggle Menu" [ref=e18]:
                - img [ref=e19]
      - main [ref=e21]:
        - generic [ref=e26]:
          - generic [ref=e27]:
            - generic [ref=e28]:
              - list [ref=e30]:
                - button "FIFA" [ref=e31] [cursor=pointer]
                - button "MLB" [ref=e32] [cursor=pointer]
                - button "WNBA" [active] [ref=e33] [cursor=pointer]
                - button "WNBA-Combos" [ref=e34] [cursor=pointer]
                - button "WNBA Q1" [ref=e35] [cursor=pointer]
                - button "WNBA H1" [ref=e36] [cursor=pointer]
                - button "MLS" [ref=e37] [cursor=pointer]
              - list [ref=e39]:
                - listitem [ref=e40]:
                  - button "ALL" [ref=e41] [cursor=pointer]:
                    - generic [ref=e42]: ALL
                - listitem [ref=e43]:
                  - button "SEA@IND 7:30PM" [ref=e44] [cursor=pointer]:
                    - text: SEA@IND
                    - generic [ref=e45]: 7:30PM
                - listitem [ref=e46]:
                  - button "LAS@CHI 7:30PM" [ref=e47] [cursor=pointer]:
                    - text: LAS@CHI
                    - generic [ref=e48]: 7:30PM
                - listitem [ref=e49]:
                  - button "ATL@TOR 7:30PM" [ref=e50] [cursor=pointer]:
                    - text: ATL@TOR
                    - generic [ref=e51]: 7:30PM
                - listitem [ref=e52]:
                  - button "CON@PHX 10:00PM" [ref=e53] [cursor=pointer]:
                    - text: CON@PHX
                    - generic [ref=e54]: 10:00PM
                - listitem [ref=e55]:
                  - button "PDX@MIN Sat 8PM" [ref=e56] [cursor=pointer]:
                    - text: PDX@MIN
                    - generic [ref=e57]: Sat 8PM
                - listitem [ref=e58]:
                  - button "WAS@GSV Sat 8PM" [ref=e59] [cursor=pointer]:
                    - text: WAS@GSV
                    - generic [ref=e60]: Sat 8PM
              - generic [ref=e61]:
                - generic [ref=e62]:
                  - generic [ref=e65]:
                    - img [ref=e67]
                    - textbox "Search player or team" [ref=e69]
                  - button "Change card style from grid" [ref=e71]
                - list [ref=e73]:
                  - listitem [ref=e74]:
                    - button "Points" [ref=e75]
                  - listitem [ref=e76]:
                    - button "Rebounds" [ref=e77]
                  - listitem [ref=e78]:
                    - button "Assists" [ref=e79]
                  - listitem [ref=e80]:
                    - button "Triple Double" [ref=e81]
                  - listitem [ref=e82]:
                    - button "3PT Made" [ref=e83]
                  - listitem [ref=e84]:
                    - button "Pts + Reb + Ast" [ref=e85]
                  - listitem [ref=e86]:
                    - button "Double Double" [ref=e87]
                  - listitem [ref=e88]:
                    - button "Pts + Reb" [ref=e89]
                  - listitem [ref=e90]:
                    - button "Pts + Ast" [ref=e91]
                  - listitem [ref=e92]:
                    - button "Reb + Ast" [ref=e93]
                  - listitem [ref=e94]:
                    - button "First Point Scorer" [ref=e95]
                  - listitem [ref=e96]:
                    - button "Fantasy Points" [ref=e97]
                  - listitem [ref=e98]:
                    - button "Steals" [ref=e99]
                  - listitem [ref=e100]:
                    - button "Blocks" [ref=e101]
            - generic [ref=e102]:
              - generic [ref=e105]:
                - button "previous slide" [ref=e106] [cursor=pointer]:
                  - img [ref=e107]
                - generic [ref=e110]:
                  - button "Get $20 By referring a friend making a first $10 deposit. lightning-bolt-yellow" [ref=e112] [cursor=pointer]:
                    - generic [ref=e113]:
                      - generic [ref=e115]: Get $20
                      - generic [ref=e116]: By referring a friend making a first $10 deposit.
                    - img "lightning-bolt-yellow" [ref=e117]
                  - 'button "Boosted Picks 🚀 Every Pick Pays: Up to a 35% Boost! lightning-bolt-yellow" [ref=e119] [cursor=pointer]':
                    - generic [ref=e120]:
                      - generic [ref=e122]: Boosted Picks 🚀
                      - generic [ref=e123]: "Every Pick Pays: Up to a 35% Boost!"
                    - img "lightning-bolt-yellow" [ref=e124]
                - button "next slide" [ref=e125] [cursor=pointer]:
                  - img [ref=e126]
              - generic [ref=e131]:
                - generic [ref=e134]:
                  - generic [ref=e137]:
                    - button "Open expert opinion for Aliyah Boston" [ref=e138]:
                      - img [ref=e139]
                    - img "Aliyah Boston" [ref=e142]
                  - generic [ref=e143]:
                    - generic [ref=e144]: Aliyah Boston
                    - button "16.5 Points" [ref=e145]:
                      - generic [ref=e146]:
                        - img [ref=e147]
                        - img [ref=e149]
                      - generic [ref=e151]: "16.5"
                      - generic [ref=e152]: Points
                    - generic [ref=e153]:
                      - generic [ref=e154]: SEA@IND
                      - generic [ref=e155]: 7:30PM
                    - generic [ref=e156]:
                      - button "Select over 16.5 Points for 1.76 times" [ref=e157]:
                        - img [ref=e158]
                        - generic [ref=e160]: 1.76x
                      - button "Select over 16.5 Points for 1.85 times" [ref=e161]:
                        - generic [ref=e162]: 1.85x
                        - img [ref=e163]
                - generic [ref=e167]:
                  - generic [ref=e170]:
                    - button "Open expert opinion for Kelsey Mitchell" [ref=e171]:
                      - img [ref=e172]
                    - img "Kelsey Mitchell" [ref=e175]
                  - generic [ref=e176]:
                    - generic [ref=e177]: K. Mitchell
                    - button "22.5 Points" [ref=e178]:
                      - generic [ref=e179]:
                        - img [ref=e180]
                        - img [ref=e182]
                      - generic [ref=e184]: "22.5"
                      - generic [ref=e185]: Points
                    - generic [ref=e186]:
                      - generic [ref=e187]: SEA@IND
                      - generic [ref=e188]: 7:30PM
                    - generic [ref=e189]:
                      - button "Select over 22.5 Points for 1.8 times" [ref=e190]:
                        - img [ref=e191]
                        - generic [ref=e193]: 1.8x
                      - button "Select over 22.5 Points for 1.82 times" [ref=e194]:
                        - generic [ref=e195]: 1.82x
                        - img [ref=e196]
                - generic [ref=e200]:
                  - generic [ref=e203]:
                    - button "Open expert opinion for Dominique Malonga" [ref=e204]:
                      - img [ref=e205]
                    - img "Dominique Malonga" [ref=e208]
                  - generic [ref=e209]:
                    - generic [ref=e210]: D. Malonga
                    - button "16.5 Points" [ref=e211]:
                      - generic [ref=e212]:
                        - img [ref=e213]
                        - img [ref=e215]
                      - generic [ref=e217]: "16.5"
                      - generic [ref=e218]: Points
                    - generic [ref=e219]:
                      - generic [ref=e220]: SEA@IND
                      - generic [ref=e221]: 7:30PM
                    - generic [ref=e222]:
                      - button "Select over 16.5 Points for 1.88 times" [ref=e223]:
                        - img [ref=e224]
                        - generic [ref=e226]: 1.88x
                      - button "Select over 16.5 Points for 1.72 times" [ref=e227]:
                        - generic [ref=e228]: 1.72x
                        - img [ref=e229]
                - generic [ref=e233]:
                  - generic [ref=e236]:
                    - button "Open expert opinion for Kamilla Cardoso" [ref=e237]:
                      - img [ref=e238]
                    - img "Kamilla Cardoso" [ref=e241]
                  - generic [ref=e242]:
                    - generic [ref=e243]: K. Cardoso
                    - button "14.5 Points" [ref=e244]:
                      - generic [ref=e245]:
                        - img [ref=e246]
                        - img [ref=e248]
                      - generic [ref=e250]: "14.5"
                      - generic [ref=e251]: Points
                    - generic [ref=e252]:
                      - generic [ref=e253]: LAS@CHI
                      - generic [ref=e254]: 7:30PM
                    - generic [ref=e255]:
                      - button "Select over 14.5 Points for 1.81 times" [ref=e256]:
                        - img [ref=e257]
                        - generic [ref=e259]: 1.81x
                      - button "Select over 14.5 Points for 1.75 times" [ref=e260]:
                        - generic [ref=e261]: 1.75x
                        - img [ref=e262]
                - generic [ref=e266]:
                  - generic [ref=e269]:
                    - button "Open expert opinion for Dearica Hamby" [ref=e270]:
                      - img [ref=e271]
                    - img "Dearica Hamby" [ref=e274]
                  - generic [ref=e275]:
                    - generic [ref=e276]: Dearica Hamby
                    - button "15.5 Points" [ref=e277]:
                      - generic [ref=e278]:
                        - img [ref=e279]
                        - img [ref=e281]
                      - generic [ref=e283]: "15.5"
                      - generic [ref=e284]: Points
                    - generic [ref=e285]:
                      - generic [ref=e286]: LAS@CHI
                      - generic [ref=e287]: 7:30PM
                    - generic [ref=e288]:
                      - button "Select over 15.5 Points for 1.81 times" [ref=e289]:
                        - img [ref=e290]
                        - generic [ref=e292]: 1.81x
                      - button "Select over 15.5 Points for 1.8 times" [ref=e293]:
                        - generic [ref=e294]: 1.8x
                        - img [ref=e295]
                - generic [ref=e299]:
                  - generic [ref=e302]:
                    - button "Open expert opinion for Allisha Gray" [ref=e303]:
                      - img [ref=e304]
                    - img "Allisha Gray" [ref=e307]
                  - generic [ref=e308]:
                    - generic [ref=e309]: Allisha Gray
                    - button "19.5 Points" [ref=e310]:
                      - generic [ref=e311]:
                        - img [ref=e312]
                        - img [ref=e314]
                      - generic [ref=e316]: "19.5"
                      - generic [ref=e317]: Points
                    - generic [ref=e318]:
                      - generic [ref=e319]: ATL@TOR
                      - generic [ref=e320]: 7:30PM
                    - generic [ref=e321]:
                      - button "Select over 19.5 Points for 1.78 times" [ref=e322]:
                        - img [ref=e323]
                        - generic [ref=e325]: 1.78x
                      - button "Select over 19.5 Points for 1.83 times" [ref=e326]:
                        - generic [ref=e327]: 1.83x
                        - img [ref=e328]
                - generic [ref=e332]:
                  - generic [ref=e335]:
                    - button "Open expert opinion for Rhyne Howard" [ref=e336]:
                      - img [ref=e337]
                    - img "Rhyne Howard" [ref=e340]
                  - generic [ref=e341]:
                    - generic [ref=e342]: Rhyne Howard
                    - button "19.5 Points" [ref=e343]:
                      - generic [ref=e344]:
                        - img [ref=e345]
                        - img [ref=e347]
                      - generic [ref=e349]: "19.5"
                      - generic [ref=e350]: Points
                    - generic [ref=e351]:
                      - generic [ref=e352]: ATL@TOR
                      - generic [ref=e353]: 7:30PM
                    - generic [ref=e354]:
                      - button "Select over 19.5 Points for 1.74 times" [ref=e355]:
                        - img [ref=e356]
                        - generic [ref=e358]: 1.74x
                      - button "Select over 19.5 Points for 1.88 times" [ref=e359]:
                        - generic [ref=e360]: 1.88x
                        - img [ref=e361]
                - generic [ref=e365]:
                  - generic [ref=e368]:
                    - button "Open expert opinion for Jordin Canada" [ref=e369]:
                      - img [ref=e370]
                    - img "Jordin Canada" [ref=e373]
                  - generic [ref=e374]:
                    - generic [ref=e375]: Jordin Canada
                    - button "11.5 Points" [ref=e376]:
                      - generic [ref=e377]:
                        - img [ref=e378]
                        - img [ref=e380]
                      - generic [ref=e382]: "11.5"
                      - generic [ref=e383]: Points
                    - generic [ref=e384]:
                      - generic [ref=e385]: ATL@TOR
                      - generic [ref=e386]: 7:30PM
                    - generic [ref=e387]:
                      - button "Select over 11.5 Points for 1.84 times" [ref=e388]:
                        - img [ref=e389]
                        - generic [ref=e391]: 1.84x
                      - button "Select over 11.5 Points for 1.77 times" [ref=e392]:
                        - generic [ref=e393]: 1.77x
                        - img [ref=e394]
                - generic [ref=e398]:
                  - generic [ref=e401]:
                    - button "Open expert opinion for Naz Hillmon" [ref=e402]:
                      - img [ref=e403]
                    - img "Naz Hillmon" [ref=e406]
                  - generic [ref=e407]:
                    - generic [ref=e408]: Naz Hillmon
                    - button "9.5 Points" [ref=e409]:
                      - generic [ref=e410]:
                        - img [ref=e411]
                        - img [ref=e413]
                      - generic [ref=e415]: "9.5"
                      - generic [ref=e416]: Points
                    - generic [ref=e417]:
                      - generic [ref=e418]: ATL@TOR
                      - generic [ref=e419]: 7:30PM
                    - generic [ref=e420]:
                      - button "Select over 9.5 Points for 1.76 times" [ref=e421]:
                        - img [ref=e422]
                        - generic [ref=e424]: 1.76x
                      - button "Select over 9.5 Points for 1.87 times" [ref=e425]:
                        - generic [ref=e426]: 1.87x
                        - img [ref=e427]
                - generic [ref=e431]:
                  - generic [ref=e434]:
                    - button "Open expert opinion for Laura Juškaitė" [ref=e435]:
                      - img [ref=e436]
                    - img "Laura Juškaitė" [ref=e439]
                  - generic [ref=e440]:
                    - generic [ref=e441]: L. Juškaitė
                    - button "9.5 Points" [ref=e442]:
                      - generic [ref=e443]:
                        - img [ref=e444]
                        - img [ref=e446]
                      - generic [ref=e448]: "9.5"
                      - generic [ref=e449]: Points
                    - generic [ref=e450]:
                      - generic [ref=e451]: ATL@TOR
                      - generic [ref=e452]: 7:30PM
                    - generic [ref=e453]:
                      - button "Select over 9.5 Points for 1.86 times" [ref=e454]:
                        - img [ref=e455]
                        - generic [ref=e457]: 1.86x
                      - button "Select over 9.5 Points for 1.75 times" [ref=e458]:
                        - generic [ref=e459]: 1.75x
                        - img [ref=e460]
            - generic [ref=e463]:
              - generic [ref=e464]:
                - img [ref=e466]
                - generic [ref=e468]:
                  - generic [ref=e469]: 1000x
                  - generic [ref=e484]: 9 picks (max)
                - button "Continue" [ref=e485] [cursor=pointer]
              - generic [ref=e486]:
                - generic [ref=e487]:
                  - generic [ref=e488]: Your Selection
                  - generic [ref=e489]:
                    - generic [ref=e490]:
                      - generic [ref=e491]:
                        - img [ref=e492]
                        - generic [ref=e494]:
                          - text: D. Rice (0.5 Goals - More - FG)
                          - generic [ref=e495]: 7.6x
                      - img [ref=e497]
                    - generic [ref=e499]:
                      - generic [ref=e500]:
                        - img [ref=e501]
                        - generic [ref=e503]:
                          - text: J. Bellingham (0.5 Goals - More - FG)
                          - generic [ref=e504]: 3.47x
                      - img [ref=e506]
                    - generic [ref=e508]:
                      - generic [ref=e509]:
                        - img [ref=e510]
                        - generic [ref=e512]:
                          - text: J. Stones (0.5 Goals - More - FG)
                          - generic [ref=e513]: 16x
                      - img [ref=e515]
                    - generic [ref=e517]:
                      - generic [ref=e518]:
                        - img [ref=e519]
                        - generic [ref=e521]:
                          - text: J. Caminero (1.5 Hits - Less - FG)
                          - generic [ref=e522]: 1.26x
                      - img [ref=e524]
                    - generic [ref=e526]:
                      - generic [ref=e527]:
                        - img [ref=e528]
                        - generic [ref=e530]:
                          - text: A. Gordon (1.5 Shots - More - FG)
                          - generic [ref=e531]: 1.8x
                      - img [ref=e533]
                    - generic [ref=e535]:
                      - generic [ref=e536]:
                        - img [ref=e537]
                        - generic [ref=e539]:
                          - text: H. Kane (2.5 Shots - More - FG)
                          - generic [ref=e540]: 1.52x
                      - img [ref=e542]
                    - generic [ref=e544]:
                      - generic [ref=e545]:
                        - img [ref=e546]
                        - generic [ref=e548]:
                          - text: B. Saka (1.5 Shots - More - FG)
                          - generic [ref=e549]: 1.8x
                      - img [ref=e551]
                    - generic [ref=e553]:
                      - generic [ref=e554]:
                        - img [ref=e555]
                        - generic [ref=e557]:
                          - text: E. Anderson (0.5 Shots - More - FG)
                          - generic [ref=e558]: 1.56x
                      - img [ref=e560]
                    - generic [ref=e562]:
                      - generic [ref=e563]:
                        - img [ref=e564]
                        - generic [ref=e566]:
                          - text: J. Alvarez (1.5 Shots - More - FG)
                          - generic [ref=e567]: 1.48x
                      - img [ref=e569]
                - generic [ref=e571]:
                  - img [ref=e572]
                  - generic [ref=e574]: Clear All
          - generic [ref=e576]:
            - generic [ref=e578]:
              - link "Download ParlayPlay On The Play Store" [ref=e579] [cursor=pointer]:
                - /url: https://parlayplay.onelink.me/oLJk/fh7u6juo
                - img "Download ParlayPlay On The Play Store" [ref=e580]
              - paragraph [ref=e581]:
                - text: Get the app.
                - text: Better. Faster. Convenient
            - navigation [ref=e582]:
              - link "Privacy" [ref=e583] [cursor=pointer]:
                - /url: /privacy-policy
              - link "Fantasy Terms" [ref=e584] [cursor=pointer]:
                - /url: /terms
              - link "Packs Terms" [ref=e585] [cursor=pointer]:
                - /url: /terms/packs
              - link "Responsible Gaming" [ref=e586] [cursor=pointer]:
                - /url: /responsible-gaming
              - link "Gaming Rules" [ref=e587] [cursor=pointer]:
                - /url: /rules
              - link "FAQ" [ref=e588] [cursor=pointer]:
                - /url: https://intercom.help/parlayplay/en/
            - navigation [ref=e589]:
              - generic [ref=e590]:
                - paragraph [ref=e591]: © ParlayPlay 2026
                - generic [ref=e592]:
                  - link [ref=e593] [cursor=pointer]:
                    - /url: https://www.facebook.com/parlayplay.io
                    - img [ref=e594]
                  - link [ref=e596] [cursor=pointer]:
                    - /url: https://www.instagram.com/parlayplay_?igsh=bHBldWQyMmV2b3Y4
                    - img [ref=e597]
                  - link [ref=e599] [cursor=pointer]:
                    - /url: https://www.twitter.com/parlay_play
                    - img [ref=e600]
                  - link [ref=e602] [cursor=pointer]:
                    - /url: https://discord.com/invite/parlayplay
                    - img [ref=e603]
                - img "18+ icon" [ref=e605]
            - paragraph [ref=e607]
      - contentinfo [ref=e608]:
        - navigation [ref=e609]:
          - list [ref=e610]:
            - listitem [ref=e611]:
              - button "Home" [ref=e612] [cursor=pointer]:
                - generic [ref=e613]:
                  - img [ref=e614]
                  - generic [ref=e615]: Home
            - listitem [ref=e616]:
              - button "Entries 194" [ref=e617] [cursor=pointer]:
                - generic [ref=e618]:
                  - img [ref=e619]
                  - generic [ref=e620]: Entries
                - generic [ref=e621]: "194"
            - listitem [ref=e622]:
              - button "Feed" [ref=e623] [cursor=pointer]:
                - generic [ref=e624]:
                  - img [ref=e625]
                  - generic [ref=e626]: Feed
            - listitem [ref=e627]:
              - button "Rewards" [ref=e628] [cursor=pointer]:
                - generic [ref=e629]:
                  - img [ref=e630]
                  - generic [ref=e631]: Rewards
            - listitem [ref=e632]:
              - button "Packs" [ref=e633] [cursor=pointer]:
                - generic [ref=e634]:
                  - img [ref=e635]
                  - generic [ref=e636]: Packs
    - region "Notifications Alt+T"
  - alert [ref=e637]
  - iframe [ref=e638]:
    
```

# Test source

```ts
  182 |     return leagueButtonsLocator;
  183 |   }
  184 | 
  185 |   async isContinueEnabled(): Promise<boolean> {
  186 |     const button = this.continueBtn;
  187 |     const isPresent = await button.isVisible().catch(() => false);
  188 |     if (!isPresent) return false;
  189 |     const enabled = await button.isEnabled().catch(() => false);
  190 |     return enabled;
  191 |   }
  192 | 
  193 |   async trySelectPick(card: Locator): Promise<boolean> {
  194 |     const buttons = card.getByTestId("grid-button");
  195 |     const lessButton = buttons.first();
  196 |     // Bounded checks: league/stat filter updates run inside useTransition and
  197 |     // the grid is virtualised, so a card captured from listVisiblePlayerIds
  198 |     // can unmount before we act on it. With no actionTimeout configured, an
  199 |     // unbounded isEnabled()/click() on a gone card would hang the test —
  200 |     // treat "card no longer there" as an unpickable card instead.
  201 |     let isEnabled: boolean;
  202 |     try {
  203 |       isEnabled = await lessButton.isEnabled({ timeout: 5000 });
  204 |     } catch {
  205 |       return false;
  206 |     }
  207 | 
  208 |     try {
  209 |       await buttons.nth(isEnabled ? 0 : 1).click({ timeout: 10_000 });
  210 |     } catch {
  211 |       return false;
  212 |     }
  213 | 
  214 |     //warning modal check
  215 |     try {
  216 |       const modal = this.warningModal;
  217 |       if (await modal.isVisible({ timeout: 2000 }).catch(() => false)) {
  218 |         await modal.getByRole("button", { name: "Understood" }).click();
  219 |         return false;
  220 |       }
  221 |     } catch {
  222 |       // log will be added
  223 |     }
  224 |     return true;
  225 |   }
  226 | 
  227 |   async deselectPick(card: Locator): Promise<void> {
  228 |     const buttons = card.getByTestId("grid-button");
  229 |     const count = await buttons.count();
  230 | 
  231 |     for (let i = 0; i < count; i++) {
  232 |       const btn = buttons.nth(i);
  233 |       const classes = (await btn.getAttribute("class")) ?? "";
  234 |       if (classes.includes("bg-playYellow")) {
  235 |         await btn.click(); // Deselects the selected button
  236 |         return;
  237 |       }
  238 |     }
  239 |     throw new Error("No selected button found with bg-yellow class.");
  240 |   }
  241 | 
  242 |   /**
  243 |    * Picks `count` players.
  244 |    *
  245 |    * `excludeIds` skips players that a previous attempt already tried. Retries
  246 |    * (e.g. after "multiple promos cannot be applied") pass the players from the
  247 |    * failed slip so the next attempt selects genuinely new cards instead of
  248 |    * re-picking the same promo-bearing players in the same deterministic order.
  249 |    */
  250 |   async pickPlayers(
  251 |     count: number,
  252 |     statIdx?: number,
  253 |     excludeIds?: Set<string>,
  254 |   ): Promise<string[]> {
  255 |     const leagueButtons = await this.listLeagueButtons();
  256 | 
  257 |     const selected = new Set<string>();
  258 |     let lastPickId: string | null = null;
  259 |     // Caller-provided players to skip for the whole call. Kept separate from
  260 |     // recentlyFailed (which is cleared once a valid combo is found) so retries
  261 |     // never re-pick a player a prior attempt already tried.
  262 |     const excluded = new Set<string>(excludeIds ?? []);
  263 |     const recentlyFailed = new Set<string>();
  264 |     for (const leagueButton of leagueButtons) {
  265 |       const leagueId = (await leagueButton.getAttribute("id")) ?? "";
  266 |       // Skip the Combo (`league-*-combo`) and Promo (`league-Promo`) leagues:
  267 |       // every card in them carries a promo, so picking >1 always trips
  268 |       // "multiple promos cannot be applied" — and since the whole league is
  269 |       // promos, re-picking never escapes it. Regular sport leagues almost
  270 |       // never stack two promos (the exclusion retry handles the rare case).
  271 |       const lid = leagueId.toLowerCase();
  272 |       if (lid.includes("combo") || lid.includes("promo")) continue;
  273 | 
  274 |       await leagueButton.click();
  275 |       await this.waitForPlayersGrid();
  276 | 
  277 |       // Each league resets to its default stat tab on click, so re-pin
  278 |       // the requested stat after navigating into the league.
  279 |       if (statIdx !== undefined) {
  280 |         const statTab = this.statsSelector.locator("li button").nth(statIdx);
  281 |         if (await statTab.isVisible().catch(() => false)) {
> 282 |           await statTab.click();
      |                         ^ Error: locator.click: Target page, context or browser has been closed
  283 |           await this.waitForPlayersGrid();
  284 |         }
  285 |       }
  286 | 
  287 |       if (await this.noPlayerLabel.isVisible().catch(() => false)) {
  288 |         continue;
  289 |       }
  290 | 
  291 |       const playerIds = await this.listVisiblePlayerIds();
  292 |       for (const playerId of playerIds) {
  293 |         if (
  294 |           selected.has(playerId) ||
  295 |           recentlyFailed.has(playerId) ||
  296 |           excluded.has(playerId)
  297 |         )
  298 |           continue;
  299 | 
  300 |         if (await this.trySelectPick(this.playerCardById(playerId))) {
  301 |           selected.add(playerId);
  302 |           lastPickId = playerId;
  303 | 
  304 |           let continueFlag = await this.isContinueEnabled();
  305 |           if (selected.size >= count && continueFlag)
  306 |             return Array.from(selected);
  307 | 
  308 |           // Warning modal continuation
  309 |           while (!continueFlag && selected.size == count && lastPickId) {
  310 |             await this.deselectPick(this.playerCardById(lastPickId));
  311 |             selected.delete(lastPickId);
  312 |             recentlyFailed.add(lastPickId);
  313 | 
  314 |             let replaced = false;
  315 |             for (const nextId of playerIds) {
  316 |               if (
  317 |                 selected.has(nextId) ||
  318 |                 recentlyFailed.has(nextId) ||
  319 |                 excluded.has(nextId)
  320 |               )
  321 |                 continue;
  322 |               if (await this.trySelectPick(this.playerCardById(nextId))) {
  323 |                 selected.add(nextId);
  324 |                 lastPickId = nextId;
  325 |                 replaced = true;
  326 |                 break;
  327 |               }
  328 |             }
  329 |             if (!replaced) {
  330 |               throw new Error(
  331 |                 `Unable to find replacement pick when Continue is disabled (target: ${count})`
  332 |               );
  333 |             }
  334 |             continueFlag = await this.isContinueEnabled();
  335 |           }
  336 | 
  337 |           if (continueFlag && selected.size == count)
  338 |             return Array.from(selected);
  339 |           if (continueFlag) recentlyFailed.clear();
  340 |         }
  341 |       }
  342 |     }
  343 | 
  344 |     if (selected.size < count)
  345 |       throw new Error(`Could not select ${count} valid picks`);
  346 |     return Array.from(selected);
  347 |   }
  348 | 
  349 |   async pickFivePlayers(): Promise<string[]> {
  350 |     return this.pickPlayers(5);
  351 |   }
  352 | 
  353 |   /**
  354 |    * Reads the persisted slip from localStorage and returns the set of player
  355 |    * IDs it currently contains. Source of truth is the storage key the app
  356 |    * writes via `slipPersistence.saveSlip` — see `utils/slipPersistence.ts`.
  357 |    *
  358 |    * Why this over scraping the DOM: card visualisation depends on the offering
  359 |    * having a flagged main/default altLine. When the backend omits those flags
  360 |    * for a player (e.g. Cunningham bb_points), the card boots on a fallback
  361 |    * line that doesn't match the picked one, and the highlight isn't visible
  362 |    * even though the pick is correctly persisted. Reading storage decouples the
  363 |    * persistence assertion from the render path.
  364 |    */
  365 |   async getPersistedPickIds(): Promise<string[]> {
  366 |     return this.page.evaluate(() => {
  367 |       const raw = localStorage.getItem("pp_persistent_slip:v1");
  368 |       if (!raw) return [];
  369 |       try {
  370 |         const parsed = JSON.parse(raw);
  371 |         return Object.keys(parsed.selectedPicks ?? {});
  372 |       } catch {
  373 |         return [];
  374 |       }
  375 |     });
  376 |   }
  377 | 
  378 |   async assertPicksPersist(
  379 |     expectedIds: string[],
  380 |     timeout = 10_000,
  381 |   ): Promise<void> {
  382 |     // Storage IDs are bare player IDs ("1089"); pickPlayers returns the DOM
```