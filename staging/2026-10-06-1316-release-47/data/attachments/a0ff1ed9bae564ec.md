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
- generic [ref=e1]:
  - generic [ref=e2]:
    - generic [ref=e3]:
      - banner [ref=e4]:
        - navigation [ref=e5]:
          - link "Parlay Play Logo" [ref=e6] [cursor=pointer]:
            - /url: /
            - img "Parlay Play Logo" [ref=e8]
          - generic [ref=e10]:
            - generic [ref=e13]: $500.00
            - button "Toggle Menu" [ref=e14]:
              - img [ref=e15]
      - main [ref=e17]:
        - generic [ref=e22]:
          - generic [ref=e23]:
            - generic [ref=e24]:
              - list [ref=e26]:
                - button "MLB" [ref=e27] [cursor=pointer]
                - button "NHL" [ref=e28] [cursor=pointer]
                - button "SerieA" [ref=e29] [cursor=pointer]
                - button "EPL" [ref=e30] [cursor=pointer]
                - button "LaLiga" [ref=e31] [cursor=pointer]
                - button "UFC" [ref=e32] [cursor=pointer]
              - list [ref=e34]:
                - listitem [ref=e35]:
                  - button "ALL" [ref=e36] [cursor=pointer]:
                    - generic [ref=e37]: ALL
                - listitem [ref=e38]:
                  - button "NSH@TOR 7:00PM" [ref=e39] [cursor=pointer]:
                    - text: NSH@TOR
                    - generic [ref=e40]: 7:00PM
                - listitem [ref=e41]:
                  - button "UTA@NJD 7:00PM" [ref=e42] [cursor=pointer]:
                    - text: UTA@NJD
                    - generic [ref=e43]: 7:00PM
                - listitem [ref=e44]:
                  - button "CAR@MTL 7:00PM" [ref=e45] [cursor=pointer]:
                    - text: CAR@MTL
                    - generic [ref=e46]: 7:00PM
                - listitem [ref=e47]:
                  - button "OTT@DET 7:00PM" [ref=e48] [cursor=pointer]:
                    - text: OTT@DET
                    - generic [ref=e49]: 7:00PM
                - listitem [ref=e50]:
                  - button "MIN@BUF 7:00PM" [ref=e51] [cursor=pointer]:
                    - text: MIN@BUF
                    - generic [ref=e52]: 7:00PM
                - listitem [ref=e53]:
                  - button "NYI@NYR 7:30PM" [ref=e54] [cursor=pointer]:
                    - text: NYI@NYR
                    - generic [ref=e55]: 7:30PM
                - listitem [ref=e56]:
                  - button "VGK@SEA 9:40PM" [ref=e57] [cursor=pointer]:
                    - text: VGK@SEA
                    - generic [ref=e58]: 9:40PM
                - listitem [ref=e59]:
                  - button "FLO@LAK 10:00PM" [ref=e60] [cursor=pointer]:
                    - text: FLO@LAK
                    - generic [ref=e61]: 10:00PM
                - listitem [ref=e62]:
                  - button "PIT@WSH Wed 7PM" [ref=e63] [cursor=pointer]:
                    - text: PIT@WSH
                    - generic [ref=e64]: Wed 7PM
                - listitem [ref=e65]:
                  - button "COL@WPJ Wed 7PM" [ref=e66] [cursor=pointer]:
                    - text: COL@WPJ
                    - generic [ref=e67]: Wed 7PM
              - generic [ref=e68]:
                - generic [ref=e69]:
                  - generic [ref=e72]:
                    - generic:
                      - img
                    - textbox "Search player or team" [ref=e73]
                  - button "Change card style from grid" [ref=e75]
                - list [ref=e77]:
                  - listitem [ref=e78]:
                    - button "Shots on Target" [ref=e79]
                  - listitem [ref=e80]:
                    - button "Goals" [ref=e81]
                  - listitem [ref=e82]:
                    - button "Saves" [ref=e83]
                  - listitem [ref=e84]:
                    - button "Points" [ref=e85]
                  - listitem [ref=e86]:
                    - button "Assists" [ref=e87]
                  - listitem [ref=e88]:
                    - button "Time on Ice (M)" [ref=e89]
                  - listitem [ref=e90]:
                    - button "Faceoffs Won" [ref=e91]
                  - listitem [ref=e92]:
                    - button "Hits" [ref=e93]
                  - listitem [ref=e94]:
                    - button "Blocked Shots" [ref=e95]
                  - listitem [ref=e96]:
                    - button "Fantasy Points" [ref=e97]
            - generic [ref=e98]:
              - generic [ref=e103]:
                - generic [ref=e106] [cursor=pointer]:
                  - generic [ref=e107]:
                    - generic [ref=e108]:
                      - generic [ref=e109]: 100%
                      - generic [ref=e110]: Deposit Match
                    - generic [ref=e111]: New User Promotion
                  - button "Deposit" [ref=e113]
                - generic [ref=e117] [cursor=pointer]:
                  - generic [ref=e118]: Pull real graded cards worth up to $10,000
                  - generic [ref=e119]: Sell or ship instantly
                  - button "Rip a pack" [ref=e120]:
                    - generic [ref=e121]:
                      - img [ref=e122]
                      - text: Rip a pack
                - generic [ref=e127] [cursor=pointer]:
                  - generic [ref=e128]:
                    - generic [ref=e129]: Refer a friend, get a $20 Free Entry
                    - generic [ref=e130]: Referral bonus
                  - button "Refer" [ref=e131]
                - generic [ref=e134] [cursor=pointer]:
                  - generic [ref=e135]:
                    - generic [ref=e136]:
                      - img [ref=e137]
                      - generic [ref=e141]: Boosted Picks
                    - generic [ref=e142]: "Every Pick Pays: Up to a 35% Boost!"
                  - button "Details" [ref=e144]
              - generic [ref=e148]:
                - generic [ref=e151]:
                  - generic [ref=e154]:
                    - button "Open expert opinion for Clayton Keller" [ref=e155]:
                      - img [ref=e156]
                    - img "Clayton Keller" [ref=e159]
                  - generic [ref=e160]:
                    - generic [ref=e161]: C. Keller
                    - button "2.5 SHO" [ref=e162]:
                      - generic [ref=e163]:
                        - img [ref=e164]
                        - img [ref=e166]
                      - generic [ref=e168]: "2.5"
                      - generic [ref=e169]: SHO
                    - generic [ref=e170]:
                      - generic [ref=e171]: UTA@NJD
                      - generic [ref=e172]: 7:00PM
                    - generic [ref=e173]:
                      - button "Select over 2.5 Shots on Target for 1.61 times" [ref=e174]:
                        - img [ref=e175]
                        - img [ref=e179]
                        - generic [ref=e181]: 1.61x
                      - button "Select over 2.5 Shots on Target for 2 times" [ref=e182]:
                        - generic [ref=e183]: 2x
                        - img [ref=e184]
                - generic [ref=e188]:
                  - generic [ref=e191]:
                    - button "Open expert opinion for Nick Schmaltz" [ref=e192]:
                      - img [ref=e193]
                    - img "Nick Schmaltz" [ref=e196]
                  - generic [ref=e197]:
                    - generic [ref=e198]: Nick Schmaltz
                    - button "2.5 SHO" [ref=e199]:
                      - generic [ref=e200]:
                        - img [ref=e201]
                        - img [ref=e203]
                      - generic [ref=e205]: "2.5"
                      - generic [ref=e206]: SHO
                    - generic [ref=e207]:
                      - generic [ref=e208]: UTA@NJD
                      - generic [ref=e209]: 7:00PM
                    - generic [ref=e210]:
                      - button "Select over 2.5 Shots on Target for 1.48 times" [ref=e211]:
                        - img [ref=e212]
                        - img [ref=e216]
                        - generic [ref=e218]: 1.48x
                      - button "Select over 2.5 Shots on Target for 2.24 times" [ref=e219]:
                        - generic [ref=e220]: 2.24x
                        - img [ref=e221]
                - generic [ref=e225]:
                  - generic [ref=e228]:
                    - button "Open expert opinion for Mikhail Sergachev" [ref=e229]:
                      - img [ref=e230]
                    - img "Mikhail Sergachev" [ref=e233]
                  - generic [ref=e234]:
                    - generic [ref=e235]: M. Sergachev
                    - button "1.5 SHO" [ref=e236]:
                      - generic [ref=e237]:
                        - img [ref=e238]
                        - img [ref=e240]
                      - generic [ref=e242]: "1.5"
                      - generic [ref=e243]: SHO
                    - generic [ref=e244]:
                      - generic [ref=e245]: UTA@NJD
                      - generic [ref=e246]: 7:00PM
                    - generic [ref=e247]:
                      - button "Select over 1.5 Shots on Target for 2.1 times" [ref=e248]:
                        - img [ref=e249]
                        - img [ref=e253]
                        - generic [ref=e255]: 2.1x
                      - button "Select over 1.5 Shots on Target for 1.5 times" [ref=e256]:
                        - generic [ref=e257]: 1.5x
                        - img [ref=e258]
                - generic [ref=e262]:
                  - generic [ref=e265]:
                    - button "Open expert opinion for Cole Caufield" [ref=e266]:
                      - img [ref=e267]
                    - img "Cole Caufield" [ref=e270]
                  - generic [ref=e271]:
                    - generic [ref=e272]: Cole Caufield
                    - button "2.5 SHO" [ref=e273]:
                      - generic [ref=e274]:
                        - img [ref=e275]
                        - img [ref=e277]
                      - generic [ref=e279]: "2.5"
                      - generic [ref=e280]: SHO
                    - generic [ref=e281]:
                      - generic [ref=e282]: CAR@MTL
                      - generic [ref=e283]: 7:00PM
                    - generic [ref=e284]:
                      - button "Select over 2.5 Shots on Target for 2.08 times" [active] [ref=e285]:
                        - img [ref=e286]
                        - img [ref=e290]
                        - generic [ref=e292]: 2.08x
                      - button "Select over 2.5 Shots on Target for 1.54 times" [ref=e293]:
                        - generic [ref=e294]: 1.54x
                        - img [ref=e295]
                - generic [ref=e299]:
                  - generic [ref=e302]:
                    - button "Open expert opinion for Ivan Demidov" [ref=e303]:
                      - img [ref=e304]
                    - img "Ivan Demidov" [ref=e307]
                  - generic [ref=e308]:
                    - generic [ref=e309]: Ivan Demidov
                    - button "1.5 SHO" [ref=e310]:
                      - generic [ref=e311]:
                        - img [ref=e312]
                        - img [ref=e314]
                      - generic [ref=e316]: "1.5"
                      - generic [ref=e317]: SHO
                    - generic [ref=e318]:
                      - generic [ref=e319]: CAR@MTL
                      - generic [ref=e320]: 7:00PM
                    - generic [ref=e321]:
                      - button "Select over 1.5 Shots on Target for 0 times" [disabled] [ref=e322]
                      - button "Select over 1.5 Shots on Target for 1.72 times" [ref=e324]:
                        - generic [ref=e325]: 1.72x
                        - img [ref=e326]
                - generic [ref=e330]:
                  - generic [ref=e333]:
                    - button "Open expert opinion for Juraj Slafkovsky" [ref=e334]:
                      - img [ref=e335]
                    - img "Juraj Slafkovsky" [ref=e338]
                  - generic [ref=e339]:
                    - generic [ref=e340]: J. Slafkovsky
                    - button "1.5 SHO" [ref=e341]:
                      - generic [ref=e342]:
                        - img [ref=e343]
                        - img [ref=e345]
                      - generic [ref=e347]: "1.5"
                      - generic [ref=e348]: SHO
                    - generic [ref=e349]:
                      - generic [ref=e350]: CAR@MTL
                      - generic [ref=e351]: 7:00PM
                    - generic [ref=e352]:
                      - button "Select over 1.5 Shots on Target for 2.26 times" [ref=e353]:
                        - img [ref=e354]
                        - generic [ref=e356]: 2.26x
                      - button "Select over 1.5 Shots on Target for 1.47 times" [ref=e357]:
                        - generic [ref=e358]: 1.47x
                        - img [ref=e359]
                - generic [ref=e363]:
                  - generic [ref=e366]:
                    - button "Open expert opinion for Nick Suzuki" [ref=e367]:
                      - img [ref=e368]
                    - img "Nick Suzuki" [ref=e371]
                  - generic [ref=e372]:
                    - generic [ref=e373]: Nick Suzuki
                    - button "1.5 SHO" [ref=e374]:
                      - generic [ref=e375]:
                        - img [ref=e376]
                        - img [ref=e378]
                      - generic [ref=e380]: "1.5"
                      - generic [ref=e381]: SHO
                    - generic [ref=e382]:
                      - generic [ref=e383]: CAR@MTL
                      - generic [ref=e384]: 7:00PM
                    - generic [ref=e385]:
                      - button "Select over 1.5 Shots on Target for 2.3 times" [ref=e386]:
                        - img [ref=e387]
                        - generic [ref=e389]: 2.3x
                      - button "Select over 1.5 Shots on Target for 1.45 times" [ref=e390]:
                        - generic [ref=e391]: 1.45x
                        - img [ref=e392]
                - generic [ref=e396]:
                  - generic [ref=e399]:
                    - button "Open expert opinion for Lane Hutson" [ref=e400]:
                      - img [ref=e401]
                    - img "Lane Hutson" [ref=e404]
                  - generic [ref=e405]:
                    - generic [ref=e406]: Lane Hutson
                    - button "1.5 SHO" [ref=e407]:
                      - generic [ref=e408]:
                        - img [ref=e409]
                        - img [ref=e411]
                      - generic [ref=e413]: "1.5"
                      - generic [ref=e414]: SHO
                    - generic [ref=e415]:
                      - generic [ref=e416]: CAR@MTL
                      - generic [ref=e417]: 7:00PM
                    - generic [ref=e418]:
                      - button "Select over 1.5 Shots on Target for 0 times" [disabled] [ref=e419]
                      - button "Select over 1.5 Shots on Target for 1.77 times" [ref=e421]:
                        - generic [ref=e422]: 1.77x
                        - img [ref=e423]
                - generic [ref=e427]:
                  - generic [ref=e430]:
                    - button "Open expert opinion for Sebastian Aho" [ref=e431]:
                      - img [ref=e432]
                    - img "Sebastian Aho" [ref=e435]
                  - generic [ref=e436]:
                    - generic [ref=e437]: Sebastian Aho
                    - button "2.5 SHO" [ref=e438]:
                      - generic [ref=e439]:
                        - img [ref=e440]
                        - img [ref=e442]
                      - generic [ref=e444]: "2.5"
                      - generic [ref=e445]: SHO
                    - generic [ref=e446]:
                      - generic [ref=e447]: CAR@MTL
                      - generic [ref=e448]: 7:00PM
                    - generic [ref=e449]:
                      - button "Select over 2.5 Shots on Target for 1.92 times" [ref=e450]:
                        - img [ref=e451]
                        - generic [ref=e453]: 1.92x
                      - button "Select over 2.5 Shots on Target for 1.71 times" [ref=e454]:
                        - generic [ref=e455]: 1.71x
                        - img [ref=e456]
                - generic [ref=e460]:
                  - generic [ref=e463]:
                    - button "Open expert opinion for Jackson Blake" [ref=e464]:
                      - img [ref=e465]
                    - img "Jackson Blake" [ref=e468]
                  - generic [ref=e469]:
                    - generic [ref=e470]: Jackson Blake
                    - button "2.5 SHO" [ref=e471]:
                      - generic [ref=e472]:
                        - img [ref=e473]
                        - img [ref=e475]
                      - generic [ref=e477]: "2.5"
                      - generic [ref=e478]: SHO
                    - generic [ref=e479]:
                      - generic [ref=e480]: CAR@MTL
                      - generic [ref=e481]: 7:00PM
                    - generic [ref=e482]:
                      - button "Select over 2.5 Shots on Target for 1.68 times" [ref=e483]:
                        - img [ref=e484]
                        - generic [ref=e486]: 1.68x
                      - button "Select over 2.5 Shots on Target for 1.94 times" [ref=e487]:
                        - generic [ref=e488]: 1.94x
                        - img [ref=e489]
                - generic [ref=e493]:
                  - generic [ref=e496]:
                    - button "Open expert opinion for Nikolaj Ehlers" [ref=e497]:
                      - img [ref=e498]
                    - img "Nikolaj Ehlers" [ref=e501]
                  - generic [ref=e502]:
                    - generic [ref=e503]: N. Ehlers
                    - button "2.5 SHO" [ref=e504]:
                      - generic [ref=e505]:
                        - img [ref=e506]
                        - img [ref=e508]
                      - generic [ref=e510]: "2.5"
                      - generic [ref=e511]: SHO
                    - generic [ref=e512]:
                      - generic [ref=e513]: CAR@MTL
                      - generic [ref=e514]: 7:00PM
                    - generic [ref=e515]:
                      - button "Select over 2.5 Shots on Target for 1.82 times" [ref=e516]:
                        - img [ref=e517]
                        - generic [ref=e519]: 1.82x
                      - button "Select over 2.5 Shots on Target for 1.78 times" [ref=e520]:
                        - generic [ref=e521]: 1.78x
                        - img [ref=e522]
                - generic [ref=e526]:
                  - generic [ref=e529]:
                    - button "Open expert opinion for Logan Stankoven" [ref=e530]:
                      - img [ref=e531]
                    - img "Logan Stankoven" [ref=e534]
                  - generic [ref=e535]:
                    - generic [ref=e536]: L. Stankoven
                    - button "2.5 SHO" [ref=e537]:
                      - generic [ref=e538]:
                        - img [ref=e539]
                        - img [ref=e541]
                      - generic [ref=e543]: "2.5"
                      - generic [ref=e544]: SHO
                    - generic [ref=e545]:
                      - generic [ref=e546]: CAR@MTL
                      - generic [ref=e547]: 7:00PM
                    - generic [ref=e548]:
                      - button "Select over 2.5 Shots on Target for 1.56 times" [ref=e549]:
                        - img [ref=e550]
                        - generic [ref=e552]: 1.56x
                      - button "Select over 2.5 Shots on Target for 2.2 times" [ref=e553]:
                        - generic [ref=e554]: 2.2x
                        - img [ref=e555]
            - generic [ref=e558]:
              - generic [ref=e559]:
                - img [ref=e561]
                - generic [ref=e563]:
                  - generic [ref=e565]:
                    - generic [ref=e566]: 34.9x
                    - generic [ref=e567]: 47.11x
                  - generic [ref=e568]:
                    - button "Max Boost 🚀" [ref=e579]:
                      - generic [ref=e580]: Max Boost 🚀
                    - generic [ref=e585]: 9 picks (max)
                - button "Continue" [ref=e586] [cursor=pointer]
              - generic [ref=e587]:
                - generic [ref=e588]:
                  - generic [ref=e589]: Your Selection
                  - generic [ref=e590]:
                    - generic [ref=e591]:
                      - generic [ref=e592]:
                        - img [ref=e593]
                        - generic [ref=e595]:
                          - text: N. Pivetta (4.5 SO (K) - Less - FG)
                          - generic [ref=e596]: 1.5x
                      - img [ref=e598]
                    - generic [ref=e600]:
                      - generic [ref=e601]:
                        - img [ref=e602]
                        - generic [ref=e604]:
                          - text: A. Matthews (3.5 SHO - Less - FG)
                          - generic [ref=e605]: 1.81x
                      - img [ref=e607]
                    - generic [ref=e609]:
                      - generic [ref=e610]:
                        - img [ref=e611]
                        - generic [ref=e613]:
                          - text: W. Nylander (2.5 SHO - Less - FG)
                          - generic [ref=e614]: 1.93x
                      - img [ref=e616]
                    - generic [ref=e618]:
                      - generic [ref=e619]:
                        - img [ref=e620]
                        - generic [ref=e622]:
                          - text: J. Tavares (2.5 SHO - Less - FG)
                          - generic [ref=e623]: 1.52x
                      - img [ref=e625]
                    - generic [ref=e627]:
                      - generic [ref=e628]:
                        - img [ref=e629]
                        - generic [ref=e631]:
                          - text: D. Guenther (2.5 SHO - Less - FG)
                          - generic [ref=e632]: 1.9x
                      - img [ref=e634]
                    - generic [ref=e636]:
                      - generic [ref=e637]:
                        - img [ref=e638]
                        - generic [ref=e640]:
                          - text: C. Keller (2.5 SHO - Less - FG)
                          - generic [ref=e641]: 1.61x
                      - img [ref=e643]
                    - generic [ref=e645]:
                      - generic [ref=e646]:
                        - img [ref=e647]
                        - generic [ref=e649]:
                          - text: N. Schmaltz (2.5 SHO - Less - FG)
                          - generic [ref=e650]: 1.48x
                      - img [ref=e652]
                    - generic [ref=e654]:
                      - generic [ref=e655]:
                        - img [ref=e656]
                        - generic [ref=e658]:
                          - text: M. Sergachev (1.5 SHO - Less - FG)
                          - generic [ref=e659]: 2.1x
                      - img [ref=e661]
                    - generic [ref=e663]:
                      - generic [ref=e664]:
                        - img [ref=e665]
                        - generic [ref=e667]:
                          - text: C. Caufield (2.5 SHO - Less - FG)
                          - generic [ref=e668]: 2.08x
                      - img [ref=e670]
                - generic [ref=e672]:
                  - img [ref=e673]
                  - generic [ref=e675]: Clear All
          - generic [ref=e677]:
            - generic [ref=e679]:
              - link "Download ParlayPlay On The Play Store" [ref=e680] [cursor=pointer]:
                - /url: https://parlayplay.onelink.me/oLJk/fh7u6juo
                - img "Download ParlayPlay On The Play Store" [ref=e681]
              - paragraph [ref=e682]:
                - text: Get the app.
                - text: Better. Faster. Convenient
            - navigation [ref=e683]:
              - link "Privacy" [ref=e684] [cursor=pointer]:
                - /url: /privacy-policy
              - link "Fantasy Terms" [ref=e685] [cursor=pointer]:
                - /url: /terms
              - link "Packs Terms" [ref=e686] [cursor=pointer]:
                - /url: /terms/packs
              - link "Responsible Gaming" [ref=e687] [cursor=pointer]:
                - /url: /responsible-gaming
              - link "Gaming Rules" [ref=e688] [cursor=pointer]:
                - /url: /rules
              - link "FAQ" [ref=e689] [cursor=pointer]:
                - /url: https://intercom.help/parlayplay/en/
            - navigation [ref=e690]:
              - generic [ref=e691]:
                - paragraph [ref=e692]: © ParlayPlay 2026
                - generic [ref=e693]:
                  - link "ParlayPlay on Facebook" [ref=e694] [cursor=pointer]:
                    - /url: https://www.facebook.com/parlayplay.io
                    - img [ref=e695]
                  - link "ParlayPlay on Instagram" [ref=e697] [cursor=pointer]:
                    - /url: https://www.instagram.com/parlayplay_?igsh=bHBldWQyMmV2b3Y4
                    - img [ref=e698]
                  - link "ParlayPlay on Twitter" [ref=e700] [cursor=pointer]:
                    - /url: https://www.twitter.com/parlay_play
                    - img [ref=e701]
                  - link "ParlayPlay on Discord" [ref=e703] [cursor=pointer]:
                    - /url: https://discord.com/invite/parlayplay
                    - img [ref=e704]
                - img "18+ icon" [ref=e706]
            - paragraph [ref=e708]
      - contentinfo [ref=e709]:
        - navigation [ref=e710]:
          - list [ref=e711]:
            - listitem [ref=e712]:
              - button "Home" [ref=e713] [cursor=pointer]:
                - generic [ref=e714]:
                  - img [ref=e715]
                  - generic [ref=e716]: Home
            - listitem [ref=e717]:
              - button "Entries" [ref=e718] [cursor=pointer]:
                - generic [ref=e719]:
                  - img [ref=e720]
                  - generic [ref=e721]: Entries
            - listitem [ref=e722]:
              - button "Feed" [ref=e723] [cursor=pointer]:
                - generic [ref=e724]:
                  - img [ref=e725]
                  - generic [ref=e726]: Feed
            - listitem [ref=e727]:
              - button "Rewards 1" [ref=e728] [cursor=pointer]:
                - generic [ref=e729]:
                  - img [ref=e730]
                  - generic [ref=e731]: Rewards
                - generic [ref=e732]: "1"
            - listitem [ref=e733]:
              - button "Packs" [ref=e734] [cursor=pointer]:
                - generic [ref=e735]:
                  - img [ref=e736]
                  - generic [ref=e737]: Packs
    - generic:
      - region "Notifications Alt+T"
  - alert [ref=e738]
  - iframe [ref=e739]:
    
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