# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: contests/submission-validation.spec.ts >> Contests - Slip validation >> Selection is capped at 9 picks
- Location: tests/contests/submission-validation.spec.ts:167:3

# Error details

```
Error: expect(locator).toBeVisible() failed

Locator: locator('div[role="dialog"]').filter({ hasText: 'Pick Warning' }).filter({ visible: true }).first()
Expected: visible
Timeout: 15000ms
Error: element(s) not found

Call log:
  - Expect "toBeVisible" with timeout 15000ms
  - waiting for locator('div[role="dialog"]').filter({ hasText: 'Pick Warning' }).filter({ visible: true }).first()

```

# Page snapshot

```yaml
- generic [active] [ref=e1]:
  - generic [ref=e2]:
    - generic [ref=e3]:
      - banner [ref=e4]:
        - navigation [ref=e5]:
          - link "Parlay Play Logo" [ref=e6]:
            - /url: /
            - img "Parlay Play Logo" [ref=e8]
          - generic [ref=e10]:
            - generic [ref=e12]:
              - generic [ref=e13]: $479.03
              - generic [ref=e14]:
                - img "gift-icon" [ref=e15]
                - text: "12.00"
            - button "Toggle Menu" [ref=e16]:
              - img [ref=e17]
      - main [ref=e19]:
        - generic [ref=e24]:
          - generic [ref=e25]:
            - generic [ref=e26]:
              - list [ref=e28]:
                - button "MLB" [ref=e29] [cursor=pointer]
                - button "NHL" [ref=e30] [cursor=pointer]
                - button "SerieA" [ref=e31] [cursor=pointer]
                - button "EPL" [ref=e32] [cursor=pointer]
                - button "LaLiga" [ref=e33] [cursor=pointer]
                - button "UFC" [ref=e34] [cursor=pointer]
              - list [ref=e36]:
                - listitem [ref=e37]:
                  - button "ALL" [ref=e38] [cursor=pointer]:
                    - generic [ref=e39]: ALL
                - listitem [ref=e40]:
                  - button "NSH@TOR 7:00PM" [ref=e41] [cursor=pointer]:
                    - text: NSH@TOR
                    - generic [ref=e42]: 7:00PM
                - listitem [ref=e43]:
                  - button "UTA@NJD 7:00PM" [ref=e44] [cursor=pointer]:
                    - text: UTA@NJD
                    - generic [ref=e45]: 7:00PM
                - listitem [ref=e46]:
                  - button "CAR@MTL 7:00PM" [ref=e47] [cursor=pointer]:
                    - text: CAR@MTL
                    - generic [ref=e48]: 7:00PM
                - listitem [ref=e49]:
                  - button "OTT@DET 7:00PM" [ref=e50] [cursor=pointer]:
                    - text: OTT@DET
                    - generic [ref=e51]: 7:00PM
                - listitem [ref=e52]:
                  - button "MIN@BUF 7:00PM" [ref=e53] [cursor=pointer]:
                    - text: MIN@BUF
                    - generic [ref=e54]: 7:00PM
                - listitem [ref=e55]:
                  - button "NYI@NYR 7:30PM" [ref=e56] [cursor=pointer]:
                    - text: NYI@NYR
                    - generic [ref=e57]: 7:30PM
                - listitem [ref=e58]:
                  - button "VGK@SEA 9:40PM" [ref=e59] [cursor=pointer]:
                    - text: VGK@SEA
                    - generic [ref=e60]: 9:40PM
                - listitem [ref=e61]:
                  - button "FLO@LAK 10:00PM" [ref=e62] [cursor=pointer]:
                    - text: FLO@LAK
                    - generic [ref=e63]: 10:00PM
                - listitem [ref=e64]:
                  - button "PIT@WSH Wed 7PM" [ref=e65] [cursor=pointer]:
                    - text: PIT@WSH
                    - generic [ref=e66]: Wed 7PM
                - listitem [ref=e67]:
                  - button "COL@WPJ Wed 7PM" [ref=e68] [cursor=pointer]:
                    - text: COL@WPJ
                    - generic [ref=e69]: Wed 7PM
              - generic [ref=e70]:
                - generic [ref=e71]:
                  - generic [ref=e74]:
                    - generic:
                      - img
                    - textbox "Search player or team" [ref=e75]
                  - button "Change card style from grid" [ref=e77]
                - list [ref=e79]:
                  - listitem [ref=e80]:
                    - button "Shots on Target" [ref=e81]
                  - listitem [ref=e82]:
                    - button "Goals" [ref=e83]
                  - listitem [ref=e84]:
                    - button "Saves" [ref=e85]
                  - listitem [ref=e86]:
                    - button "Points" [ref=e87]
                  - listitem [ref=e88]:
                    - button "Assists" [ref=e89]
                  - listitem [ref=e90]:
                    - button "Time on Ice (M)" [ref=e91]
                  - listitem [ref=e92]:
                    - button "Faceoffs Won" [ref=e93]
                  - listitem [ref=e94]:
                    - button "Hits" [ref=e95]
                  - listitem [ref=e96]:
                    - button "Blocked Shots" [ref=e97]
                  - listitem [ref=e98]:
                    - button "Fantasy Points" [ref=e99]
            - generic [ref=e100]:
              - generic [ref=e105]:
                - generic [ref=e108] [cursor=pointer]:
                  - generic [ref=e109]:
                    - generic [ref=e110]:
                      - generic [ref=e111]: 100%
                      - generic [ref=e112]: Deposit Match
                    - generic [ref=e113]: New User Promotion
                  - button "Deposit" [ref=e115]
                - generic [ref=e119] [cursor=pointer]:
                  - generic [ref=e120]: Pull real graded cards worth up to $10,000
                  - generic [ref=e121]: Sell or ship instantly
                  - button "Rip a pack" [ref=e122]:
                    - generic [ref=e123]:
                      - img [ref=e124]
                      - text: Rip a pack
                - generic [ref=e129] [cursor=pointer]:
                  - generic [ref=e130]:
                    - generic [ref=e131]: Refer a friend, get a $20 Free Entry
                    - generic [ref=e132]: Referral bonus
                  - button "Refer" [ref=e133]
                - generic [ref=e136] [cursor=pointer]:
                  - generic [ref=e137]:
                    - generic [ref=e138]:
                      - img [ref=e139]
                      - generic [ref=e143]: Boosted Picks
                    - generic [ref=e144]: "Every Pick Pays: Up to a 35% Boost!"
                  - button "Details" [ref=e146]
              - generic [ref=e150]:
                - generic [ref=e153]:
                  - generic [ref=e156]:
                    - button "Open expert opinion for John Tavares" [ref=e157]:
                      - img [ref=e158]
                    - img "John Tavares" [ref=e161]
                  - generic [ref=e162]:
                    - generic [ref=e163]: John Tavares
                    - button "2.5 SHO" [ref=e164]:
                      - generic [ref=e165]:
                        - img [ref=e166]
                        - img [ref=e168]
                      - generic [ref=e170]: "2.5"
                      - generic [ref=e171]: SHO
                    - generic [ref=e172]:
                      - generic [ref=e173]: NSH@TOR
                      - generic [ref=e174]: 7:00PM
                    - generic [ref=e175]:
                      - button "Select over 2.5 Shots on Target for 1.52 times" [ref=e176]:
                        - img [ref=e177]
                        - img [ref=e181]
                        - generic [ref=e183]: 1.52x
                      - button "Select over 2.5 Shots on Target for 2.16 times" [ref=e184]:
                        - generic [ref=e185]: 2.16x
                        - img [ref=e186]
                - generic [ref=e190]:
                  - generic [ref=e193]:
                    - button "Open expert opinion for Dylan Guenther" [ref=e194]:
                      - img [ref=e195]
                    - img "Dylan Guenther" [ref=e198]
                  - generic [ref=e199]:
                    - generic [ref=e200]: D. Guenther
                    - button "2.5 SHO" [ref=e201]:
                      - generic [ref=e202]:
                        - img [ref=e203]
                        - img [ref=e205]
                      - generic [ref=e207]: "2.5"
                      - generic [ref=e208]: SHO
                    - generic [ref=e209]:
                      - generic [ref=e210]: UTA@NJD
                      - generic [ref=e211]: 7:00PM
                    - generic [ref=e212]:
                      - button "Select over 2.5 Shots on Target for 1.9 times" [ref=e213]:
                        - img [ref=e214]
                        - img [ref=e218]
                        - generic [ref=e220]: 1.9x
                      - button "Select over 2.5 Shots on Target for 1.7 times" [ref=e221]:
                        - generic [ref=e222]: 1.7x
                        - img [ref=e223]
                - generic [ref=e227]:
                  - generic [ref=e230]:
                    - button "Open expert opinion for Clayton Keller" [ref=e231]:
                      - img [ref=e232]
                    - img "Clayton Keller" [ref=e235]
                  - generic [ref=e236]:
                    - generic [ref=e237]: C. Keller
                    - button "2.5 SHO" [ref=e238]:
                      - generic [ref=e239]:
                        - img [ref=e240]
                        - img [ref=e242]
                      - generic [ref=e244]: "2.5"
                      - generic [ref=e245]: SHO
                    - generic [ref=e246]:
                      - generic [ref=e247]: UTA@NJD
                      - generic [ref=e248]: 7:00PM
                    - generic [ref=e249]:
                      - button "Select over 2.5 Shots on Target for 1.61 times" [ref=e250]:
                        - img [ref=e251]
                        - img [ref=e255]
                        - generic [ref=e257]: 1.61x
                      - button "Select over 2.5 Shots on Target for 2 times" [ref=e258]:
                        - generic [ref=e259]: 2x
                        - img [ref=e260]
                - generic [ref=e264]:
                  - generic [ref=e267]:
                    - button "Open expert opinion for Nick Schmaltz" [ref=e268]:
                      - img [ref=e269]
                    - img "Nick Schmaltz" [ref=e272]
                  - generic [ref=e273]:
                    - generic [ref=e274]: Nick Schmaltz
                    - button "2.5 SHO" [ref=e275]:
                      - generic [ref=e276]:
                        - img [ref=e277]
                        - img [ref=e279]
                      - generic [ref=e281]: "2.5"
                      - generic [ref=e282]: SHO
                    - generic [ref=e283]:
                      - generic [ref=e284]: UTA@NJD
                      - generic [ref=e285]: 7:00PM
                    - generic [ref=e286]:
                      - button "Select over 2.5 Shots on Target for 1.48 times" [ref=e287]:
                        - img [ref=e288]
                        - img [ref=e292]
                        - generic [ref=e294]: 1.48x
                      - button "Select over 2.5 Shots on Target for 2.24 times" [ref=e295]:
                        - generic [ref=e296]: 2.24x
                        - img [ref=e297]
                - generic [ref=e301]:
                  - generic [ref=e304]:
                    - button "Open expert opinion for Mikhail Sergachev" [ref=e305]:
                      - img [ref=e306]
                    - img "Mikhail Sergachev" [ref=e309]
                  - generic [ref=e310]:
                    - generic [ref=e311]: M. Sergachev
                    - button "1.5 SHO" [ref=e312]:
                      - generic [ref=e313]:
                        - img [ref=e314]
                        - img [ref=e316]
                      - generic [ref=e318]: "1.5"
                      - generic [ref=e319]: SHO
                    - generic [ref=e320]:
                      - generic [ref=e321]: UTA@NJD
                      - generic [ref=e322]: 7:00PM
                    - generic [ref=e323]:
                      - button "Select over 1.5 Shots on Target for 2.1 times" [ref=e324]:
                        - img [ref=e325]
                        - img [ref=e329]
                        - generic [ref=e331]: 2.1x
                      - button "Select over 1.5 Shots on Target for 1.5 times" [ref=e332]:
                        - generic [ref=e333]: 1.5x
                        - img [ref=e334]
                - generic [ref=e338]:
                  - generic [ref=e341]:
                    - button "Open expert opinion for Cole Caufield" [ref=e342]:
                      - img [ref=e343]
                    - img "Cole Caufield" [ref=e346]
                  - generic [ref=e347]:
                    - generic [ref=e348]: Cole Caufield
                    - button "2.5 SHO" [ref=e349]:
                      - generic [ref=e350]:
                        - img [ref=e351]
                        - img [ref=e353]
                      - generic [ref=e355]: "2.5"
                      - generic [ref=e356]: SHO
                    - generic [ref=e357]:
                      - generic [ref=e358]: CAR@MTL
                      - generic [ref=e359]: 7:00PM
                    - generic [ref=e360]:
                      - button "Select over 2.5 Shots on Target for 2.08 times" [ref=e361]:
                        - img [ref=e362]
                        - img [ref=e366]
                        - generic [ref=e368]: 2.08x
                      - button "Select over 2.5 Shots on Target for 1.54 times" [ref=e369]:
                        - generic [ref=e370]: 1.54x
                        - img [ref=e371]
                - generic [ref=e375]:
                  - generic [ref=e378]:
                    - button "Open expert opinion for Ivan Demidov" [ref=e379]:
                      - img [ref=e380]
                    - img "Ivan Demidov" [ref=e383]
                  - generic [ref=e384]:
                    - generic [ref=e385]: Ivan Demidov
                    - button "1.5 SHO" [ref=e386]:
                      - generic [ref=e387]:
                        - img [ref=e388]
                        - img [ref=e390]
                      - generic [ref=e392]: "1.5"
                      - generic [ref=e393]: SHO
                    - generic [ref=e394]:
                      - generic [ref=e395]: CAR@MTL
                      - generic [ref=e396]: 7:00PM
                    - generic [ref=e397]:
                      - button "Select over 1.5 Shots on Target for 0 times" [disabled] [ref=e398]
                      - button "Select over 1.5 Shots on Target for 1.72 times" [ref=e400]:
                        - generic [ref=e401]: 1.72x
                        - img [ref=e402]
                - generic [ref=e406]:
                  - generic [ref=e409]:
                    - button "Open expert opinion for Juraj Slafkovsky" [ref=e410]:
                      - img [ref=e411]
                    - img "Juraj Slafkovsky" [ref=e414]
                  - generic [ref=e415]:
                    - generic [ref=e416]: J. Slafkovsky
                    - button "1.5 SHO" [ref=e417]:
                      - generic [ref=e418]:
                        - img [ref=e419]
                        - img [ref=e421]
                      - generic [ref=e423]: "1.5"
                      - generic [ref=e424]: SHO
                    - generic [ref=e425]:
                      - generic [ref=e426]: CAR@MTL
                      - generic [ref=e427]: 7:00PM
                    - generic [ref=e428]:
                      - button "Select over 1.5 Shots on Target for 2.26 times" [ref=e429]:
                        - img [ref=e430]
                        - generic [ref=e432]: 2.26x
                      - button "Select over 1.5 Shots on Target for 1.47 times" [ref=e433]:
                        - generic [ref=e434]: 1.47x
                        - img [ref=e435]
                - generic [ref=e439]:
                  - generic [ref=e442]:
                    - button "Open expert opinion for Nick Suzuki" [ref=e443]:
                      - img [ref=e444]
                    - img "Nick Suzuki" [ref=e447]
                  - generic [ref=e448]:
                    - generic [ref=e449]: Nick Suzuki
                    - button "1.5 SHO" [ref=e450]:
                      - generic [ref=e451]:
                        - img [ref=e452]
                        - img [ref=e454]
                      - generic [ref=e456]: "1.5"
                      - generic [ref=e457]: SHO
                    - generic [ref=e458]:
                      - generic [ref=e459]: CAR@MTL
                      - generic [ref=e460]: 7:00PM
                    - generic [ref=e461]:
                      - button "Select over 1.5 Shots on Target for 2.3 times" [ref=e462]:
                        - img [ref=e463]
                        - generic [ref=e465]: 2.3x
                      - button "Select over 1.5 Shots on Target for 1.45 times" [ref=e466]:
                        - generic [ref=e467]: 1.45x
                        - img [ref=e468]
                - generic [ref=e472]:
                  - generic [ref=e475]:
                    - button "Open expert opinion for Lane Hutson" [ref=e476]:
                      - img [ref=e477]
                    - img "Lane Hutson" [ref=e480]
                  - generic [ref=e481]:
                    - generic [ref=e482]: Lane Hutson
                    - button "1.5 SHO" [ref=e483]:
                      - generic [ref=e484]:
                        - img [ref=e485]
                        - img [ref=e487]
                      - generic [ref=e489]: "1.5"
                      - generic [ref=e490]: SHO
                    - generic [ref=e491]:
                      - generic [ref=e492]: CAR@MTL
                      - generic [ref=e493]: 7:00PM
                    - generic [ref=e494]:
                      - button "Select over 1.5 Shots on Target for 0 times" [disabled] [ref=e495]
                      - button "Select over 1.5 Shots on Target for 1.77 times" [ref=e497]:
                        - generic [ref=e498]: 1.77x
                        - img [ref=e499]
                - generic [ref=e503]:
                  - generic [ref=e506]:
                    - button "Open expert opinion for Sebastian Aho" [ref=e507]:
                      - img [ref=e508]
                    - img "Sebastian Aho" [ref=e511]
                  - generic [ref=e512]:
                    - generic [ref=e513]: Sebastian Aho
                    - button "2.5 SHO" [ref=e514]:
                      - generic [ref=e515]:
                        - img [ref=e516]
                        - img [ref=e518]
                      - generic [ref=e520]: "2.5"
                      - generic [ref=e521]: SHO
                    - generic [ref=e522]:
                      - generic [ref=e523]: CAR@MTL
                      - generic [ref=e524]: 7:00PM
                    - generic [ref=e525]:
                      - button "Select over 2.5 Shots on Target for 1.86 times" [ref=e526]:
                        - img [ref=e527]
                        - generic [ref=e529]: 1.86x
                      - button "Select over 2.5 Shots on Target for 1.76 times" [ref=e530]:
                        - generic [ref=e531]: 1.76x
                        - img [ref=e532]
                - generic [ref=e536]:
                  - generic [ref=e539]:
                    - button "Open expert opinion for Jackson Blake" [ref=e540]:
                      - img [ref=e541]
                    - img "Jackson Blake" [ref=e544]
                  - generic [ref=e545]:
                    - generic [ref=e546]: Jackson Blake
                    - button "2.5 SHO" [ref=e547]:
                      - generic [ref=e548]:
                        - img [ref=e549]
                        - img [ref=e551]
                      - generic [ref=e553]: "2.5"
                      - generic [ref=e554]: SHO
                    - generic [ref=e555]:
                      - generic [ref=e556]: CAR@MTL
                      - generic [ref=e557]: 7:00PM
                    - generic [ref=e558]:
                      - button "Select over 2.5 Shots on Target for 1.68 times" [ref=e559]:
                        - img [ref=e560]
                        - generic [ref=e562]: 1.68x
                      - button "Select over 2.5 Shots on Target for 1.94 times" [ref=e563]:
                        - generic [ref=e564]: 1.94x
                        - img [ref=e565]
            - generic [ref=e568]:
              - generic [ref=e569]:
                - img [ref=e571]
                - generic [ref=e573]:
                  - generic [ref=e575]:
                    - generic [ref=e576]: 49.41x
                    - generic [ref=e577]: 66.7x
                  - generic [ref=e578]:
                    - button "Max Boost 🚀" [ref=e589]:
                      - generic [ref=e590]: Max Boost 🚀
                    - generic [ref=e595]: 9 picks (max)
                - button "Continue" [ref=e596] [cursor=pointer]
              - generic [ref=e597]:
                - generic [ref=e598]:
                  - generic [ref=e599]: Your Selection
                  - generic [ref=e600]:
                    - generic [ref=e601]:
                      - generic [ref=e602]:
                        - img [ref=e603]
                        - generic [ref=e605]:
                          - text: N. Pivetta (3.5 SO (K) - Less - FG)
                          - generic [ref=e606]: 2.13x
                      - img [ref=e608]
                    - generic [ref=e610]:
                      - generic [ref=e611]:
                        - img [ref=e612]
                        - generic [ref=e614]:
                          - text: A. Matthews (3.5 SHO - Less - FG)
                          - generic [ref=e615]: 1.8x
                      - img [ref=e617]
                    - generic [ref=e619]:
                      - generic [ref=e620]:
                        - img [ref=e621]
                        - generic [ref=e623]:
                          - text: W. Nylander (2.5 SHO - Less - FG)
                          - generic [ref=e624]: 1.94x
                      - img [ref=e626]
                    - generic [ref=e628]:
                      - generic [ref=e629]:
                        - img [ref=e630]
                        - generic [ref=e632]:
                          - text: J. Tavares (2.5 SHO - Less - FG)
                          - generic [ref=e633]: 1.52x
                      - img [ref=e635]
                    - generic [ref=e637]:
                      - generic [ref=e638]:
                        - img [ref=e639]
                        - generic [ref=e641]:
                          - text: D. Guenther (2.5 SHO - Less - FG)
                          - generic [ref=e642]: 1.9x
                      - img [ref=e644]
                    - generic [ref=e646]:
                      - generic [ref=e647]:
                        - img [ref=e648]
                        - generic [ref=e650]:
                          - text: C. Keller (2.5 SHO - Less - FG)
                          - generic [ref=e651]: 1.61x
                      - img [ref=e653]
                    - generic [ref=e655]:
                      - generic [ref=e656]:
                        - img [ref=e657]
                        - generic [ref=e659]:
                          - text: N. Schmaltz (2.5 SHO - Less - FG)
                          - generic [ref=e660]: 1.48x
                      - img [ref=e662]
                    - generic [ref=e664]:
                      - generic [ref=e665]:
                        - img [ref=e666]
                        - generic [ref=e668]:
                          - text: M. Sergachev (1.5 SHO - Less - FG)
                          - generic [ref=e669]: 2.1x
                      - img [ref=e671]
                    - generic [ref=e673]:
                      - generic [ref=e674]:
                        - img [ref=e675]
                        - generic [ref=e677]:
                          - text: C. Caufield (2.5 SHO - Less - FG)
                          - generic [ref=e678]: 2.08x
                      - img [ref=e680]
                - generic [ref=e682]:
                  - img [ref=e683]
                  - generic [ref=e685]: Clear All
          - generic [ref=e687]:
            - generic [ref=e689]:
              - link "Download ParlayPlay On The App Store" [ref=e690]:
                - /url: https://parlayplay.onelink.me/oLJk/gnqpwjha
                - img "Download ParlayPlay On The App Store" [ref=e691]
              - paragraph [ref=e692]:
                - text: Get the app.
                - text: Better. Faster. Convenient
            - navigation [ref=e693]:
              - link "Privacy" [ref=e694]:
                - /url: /privacy-policy
              - link "Fantasy Terms" [ref=e695]:
                - /url: /terms
              - link "Packs Terms" [ref=e696]:
                - /url: /terms/packs
              - link "Responsible Gaming" [ref=e697]:
                - /url: /responsible-gaming
              - link "Gaming Rules" [ref=e698]:
                - /url: /rules
              - link "FAQ" [ref=e699]:
                - /url: https://intercom.help/parlayplay/en/
            - navigation [ref=e700]:
              - generic [ref=e701]:
                - paragraph [ref=e702]: © ParlayPlay 2026
                - generic [ref=e703]:
                  - link "ParlayPlay on Facebook" [ref=e704]:
                    - /url: https://www.facebook.com/parlayplay.io
                    - img [ref=e705]
                  - link "ParlayPlay on Instagram" [ref=e707]:
                    - /url: https://www.instagram.com/parlayplay_?igsh=bHBldWQyMmV2b3Y4
                    - img [ref=e708]
                  - link "ParlayPlay on Twitter" [ref=e710]:
                    - /url: https://www.twitter.com/parlay_play
                    - img [ref=e711]
                  - link "ParlayPlay on Discord" [ref=e713]:
                    - /url: https://discord.com/invite/parlayplay
                    - img [ref=e714]
                - img "18+ icon" [ref=e716]
            - paragraph [ref=e718]
      - contentinfo [ref=e719]:
        - navigation [ref=e720]:
          - list [ref=e721]:
            - listitem [ref=e722]:
              - button "Home" [ref=e723] [cursor=pointer]:
                - generic [ref=e724]:
                  - img [ref=e725]
                  - generic [ref=e726]: Home
            - listitem [ref=e727]:
              - button "Entries 142" [ref=e728] [cursor=pointer]:
                - generic [ref=e729]:
                  - img [ref=e730]
                  - generic [ref=e731]: Entries
                - generic [ref=e732]: "142"
            - listitem [ref=e733]:
              - button "Feed" [ref=e734] [cursor=pointer]:
                - generic [ref=e735]:
                  - img [ref=e736]
                  - generic [ref=e737]: Feed
            - listitem [ref=e738]:
              - button "Rewards 12" [ref=e739] [cursor=pointer]:
                - generic [ref=e740]:
                  - img [ref=e741]
                  - generic [ref=e742]: Rewards
                - generic [ref=e743]: "12"
            - listitem [ref=e744]:
              - button "Packs" [ref=e745] [cursor=pointer]:
                - generic [ref=e746]:
                  - img [ref=e747]
                  - generic [ref=e748]: Packs
    - generic:
      - region "Notifications Alt+T"
  - alert [ref=e749]
```

# Test source

```ts
  95  |     await home.clickLeagueTab(tab);
  96  |     await home.waitForPlayersGrid();
  97  | 
  98  |     for (const players of teams) {
  99  |       const picked: string[] = [];
  100 |       for (const entry of players) {
  101 |         const cardId = `player-${entry.player.id}`;
  102 |         await home.searchPlayers(entry.player.fullName);
  103 |         const card = home.playerCardById(cardId);
  104 |         // A searched player still has to carry the active stat tab to render.
  105 |         const mounted = await card.waitFor({ state: 'visible', timeout: 5_000 }).then(
  106 |           () => true,
  107 |           () => false,
  108 |         );
  109 |         if (mounted && (await home.trySelectPick(card))) picked.push(cardId);
  110 |         await home.clearSearch();
  111 |         if (picked.length === 2) return picked;
  112 |       }
  113 |       for (const cardId of picked) await home.deselectPick(home.playerCardById(cardId));
  114 |     }
  115 |   }
  116 |   return [];
  117 | }
  118 | 
  119 | test.describe('Contests - Slip validation', { tag: ['@contests'] }, () => {
  120 |   // Read-only: each test builds its own slip in its own context, so one
  121 |   // failing rule must not skip the others the way a serial group would.
  122 |   test.beforeEach(async ({ loggedInPage }) => {
  123 |     const home = new HomePage(loggedInPage);
  124 |     // Navigate first: clearSlip touches localStorage, which throws on about:blank.
  125 |     await loggedInPage.goto('/');
  126 |     await home.clearSlip();
  127 |   });
  128 | 
  129 |   test('A single pick never unlocks the slip', async ({ loggedInPage: page }) => {
  130 |     const home = new HomePage(page);
  131 | 
  132 |     await test.step('Select one pick', async () => {
  133 |       await selectOnePick(home);
  134 |     });
  135 | 
  136 |     await test.step('Slip asks for a 2nd pick and offers no Continue / Place', async () => {
  137 |       await expect(home.visible(page.getByText('Please select your 2nd pick'))).toBeVisible();
  138 |       await expect(home.slipReadyCta).toBeHidden();
  139 |     });
  140 |   });
  141 | 
  142 |   test('Two picks from the same team keep the slip locked', async ({ loggedInPage: page }) => {
  143 |     test.setTimeout(240_000);
  144 |     const home = new HomePage(page);
  145 | 
  146 |     const offering = await test.step('Reload with the offering payload captured', async () => {
  147 |       const offeringPromise = waitForOffering(page);
  148 |       await page.reload();
  149 |       await home.waitForFeedReady();
  150 |       return offeringPromise;
  151 |     });
  152 | 
  153 |     const picked = await test.step('Select two players from one team', async () => {
  154 |       return pickSameTeamPair(home, offering);
  155 |     });
  156 | 
  157 |     test.skip(picked.length < 2, 'No full-game league offers two selectable players from one team');
  158 | 
  159 |     await test.step('Slip demands a second team and offers no Continue / Place', async () => {
  160 |       await expect(
  161 |         home.visible(page.getByText('Pick players from at least 2 different teams')),
  162 |       ).toBeVisible();
  163 |       await expect(home.slipReadyCta).toBeHidden();
  164 |     });
  165 |   });
  166 | 
  167 |   test(`Selection is capped at ${MAX_PICKS} picks`, async ({ loggedInPage: page }) => {
  168 |     test.setTimeout(300_000);
  169 |     const home = new HomePage(page);
  170 | 
  171 |     const pickIds = await test.step(`Select ${MAX_PICKS} valid picks`, async () => {
  172 |       try {
  173 |         return await home.pickPlayers(MAX_PICKS);
  174 |       } catch (err) {
  175 |         const message = err instanceof Error ? err.message : String(err);
  176 |         test.skip(
  177 |           /could not select/i.test(message),
  178 |           `Offering too thin for ${MAX_PICKS} valid picks: ${message}`,
  179 |         );
  180 |         throw err;
  181 |       }
  182 |     });
  183 | 
  184 |     await test.step(`Pick ${MAX_PICKS + 1} is refused with the Pick Warning modal`, async () => {
  185 |       const selected = new Set(pickIds);
  186 |       const spare = (await home.listVisiblePlayerIds()).find((id) => !selected.has(id));
  187 |       expect(spare, 'no unselected card mounted next to the full slip').toBeDefined();
  188 | 
  189 |       const card = home.playerCardById(spare!);
  190 |       await card.scrollIntoViewIfNeeded();
  191 |       // The mobile slip footer auto-expands at 9 picks and sits over the
  192 |       // grid, so a hit-tested click never lands; dispatch it instead.
  193 |       await home.pickButtons(card).first().dispatchEvent('click');
  194 | 
> 195 |       await expect(home.warningModal).toBeVisible();
      |                                       ^ Error: expect(locator).toBeVisible() failed
  196 |       await expect(home.warningModal).toContainText(
  197 |         `You have already selected ${MAX_PICKS} players`,
  198 |       );
  199 |       await home.warningModal.getByRole('button', { name: 'Understood' }).click();
  200 |       await expect(home.warningModal).toBeHidden();
  201 |     });
  202 | 
  203 |     await test.step(`Slip still holds exactly ${MAX_PICKS} picks`, async () => {
  204 |       await home.assertPicksPersist(pickIds);
  205 |     });
  206 |   });
  207 | 
  208 |   test('Entry amount presets and typed values are clamped to balance, cap and cents', async ({
  209 |     loggedInPage: page,
  210 |   }) => {
  211 |     test.setTimeout(240_000);
  212 |     const home = new HomePage(page);
  213 |     const contest = new ContestPage(page);
  214 |     const payouts = trackPayoutStructure(page);
  215 | 
  216 |     await test.step('Open the submission form with two picks', async () => {
  217 |       await home.pickPlayers(2);
  218 |       await home.enterFinalContestPage();
  219 |       await contest.verifyPage();
  220 |     });
  221 | 
  222 |     const balance = await fetchCashBalance(page);
  223 | 
  224 |     const cap = await test.step('Read the entry cap the backend priced for $1', async () => {
  225 |       await contest.setEntryAmountIfEditable(1);
  226 |       const { maxEntryAmount } = await payouts.pricedFor(1);
  227 |       return maxEntryAmount == null ? Infinity : Number(maxEntryAmount);
  228 |     });
  229 | 
  230 |     await test.step('Preset chips select their amount; chips above balance or cap are disabled', async () => {
  231 |       const amounts = [
  232 |         ...new Set(
  233 |           await contest.presetRadios.evaluateAll((els) =>
  234 |             els.map((el) => Number((el as HTMLInputElement).value)),
  235 |           ),
  236 |         ),
  237 |       ];
  238 |       expect(amounts.length, 'no preset chips rendered').toBeGreaterThan(0);
  239 |       for (const amount of amounts) {
  240 |         if (amount > balance || amount > cap) {
  241 |           await expect(contest.presetRadio(amount), `$${amount} chip`).toBeDisabled();
  242 |           continue;
  243 |         }
  244 |         await contest.presetChip(amount).click();
  245 |         await expect(contest.presetRadio(amount)).toBeChecked();
  246 |         await expect(contest.entryAmountField).toHaveValue(String(amount));
  247 |       }
  248 |     });
  249 | 
  250 |     await test.step('$0 is refused at submit and never reaches the server', async () => {
  251 |       await contest.setEntryAmountIfEditable(0);
  252 |       await contest.entryAmountField.blur();
  253 |       const result = await contest.submitAndAwaitResult(5_000);
  254 |       await expect(contest.toast('Your entry amount must be greater than $0')).toBeVisible();
  255 |       expect(result.kind, `submission must not be sent: ${result.error}`).toBe('timeout');
  256 |     });
  257 | 
  258 |     await test.step('A third decimal is dropped while typing', async () => {
  259 |       await contest.entryAmountField.fill('');
  260 |       await contest.entryAmountField.pressSequentially('0.001');
  261 |       await expect(contest.entryAmountField).toHaveValue('0.00');
  262 |     });
  263 | 
  264 |     await test.step('99999 is pulled down to the cap, then clamped to balance on blur', async () => {
  265 |       await contest.entryAmountField.fill('99999');
  266 |       await contest.entryAmountField.blur();
  267 |       await expect(contest.maxAmountWarning).toBeHidden();
  268 |       await expect(contest.placePickBtn).toBeEnabled();
  269 |       const clamped = Number(await contest.entryAmountField.inputValue());
  270 |       expect(clamped).toBeGreaterThan(0);
  271 |       expect(clamped).toBeLessThan(99999);
  272 |       expect(clamped).toBeLessThanOrEqual(Math.min(cap, balance));
  273 |     });
  274 |   });
  275 | 
  276 |   test('Payout figures match the payout-structure API for All In and Insured', async ({
  277 |     loggedInPage: page,
  278 |   }) => {
  279 |     test.setTimeout(240_000);
  280 |     const home = new HomePage(page);
  281 |     const contest = new ContestPage(page);
  282 |     const payouts = trackPayoutStructure(page);
  283 |     const amount = 5;
  284 | 
  285 |     await test.step('Open the submission form with three picks', async () => {
  286 |       await home.pickPlayers(3);
  287 |       await home.enterFinalContestPage();
  288 |       await contest.verifyPage();
  289 |     });
  290 | 
  291 |     const priced =
  292 |       await test.step(`Set the entry to $${amount} and capture its pricing`, async () => {
  293 |         await contest.setEntryAmountIfEditable(amount);
  294 |         return payouts.pricedFor(amount);
  295 |       });
```