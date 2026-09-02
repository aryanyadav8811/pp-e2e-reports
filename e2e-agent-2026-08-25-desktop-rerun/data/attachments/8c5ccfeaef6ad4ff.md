# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: slipPersistent/slip_persistent.spec.ts >> Slip persistence >> slip persists through hard page reload
- Location: tests/slipPersistent/slip_persistent.spec.ts:80:5

# Error details

```
Error: Unable to find replacement pick when Continue is disabled (target: 3)
```

# Page snapshot

```yaml
- generic [ref=e1]:
  - generic [ref=e2]:
    - generic [ref=e3]:
      - banner [ref=e4]:
        - navigation [ref=e5]:
          - link [ref=e6] [cursor=pointer]:
            - /url: /
            - img "Parlay Play Logo" [ref=e8]
          - generic [ref=e9]:
            - list [ref=e10]:
              - listitem [ref=e11]:
                - link "Home" [ref=e12] [cursor=pointer]:
                  - /url: /
              - listitem [ref=e15]:
                - link "Packs" [ref=e16] [cursor=pointer]:
                  - /url: /packs
              - listitem [ref=e19]:
                - link "Feed" [ref=e20] [cursor=pointer]:
                  - /url: /challenges/feed
              - listitem [ref=e23]:
                - link "Rewards 6" [ref=e24] [cursor=pointer]:
                  - /url: /rewards
                  - generic [ref=e25]:
                    - generic [ref=e26]: Rewards
                    - generic [ref=e27]: "6"
              - listitem [ref=e28]:
                - link "Track Picks 55" [ref=e29] [cursor=pointer]:
                  - /url: /challenges/pending
                  - generic [ref=e30]:
                    - generic [ref=e31]: Track Picks
                    - generic [ref=e32]: "55"
            - button "Claim your $100 Deposit Match" [ref=e33] [cursor=pointer]
            - generic [ref=e34]:
              - generic [ref=e36]:
                - generic [ref=e37]: $208.92
                - generic [ref=e38]:
                  - img "gift-icon" [ref=e39]
                  - text: "5.00"
              - button "Toggle Menu" [ref=e40]
      - main [ref=e43]:
        - generic [ref=e45]:
          - generic [ref=e49]:
            - button "previous slide" [ref=e50] [cursor=pointer]
            - generic [ref=e54]:
              - generic [ref=e56]:
                - generic [ref=e57]:
                  - generic [ref=e58]: Receive a referral Bonus!
                  - generic [ref=e59]: $20
                - generic [ref=e60]:
                  - text: Refer a Friendwhen they make their first deposit
                  - button "Invite Now" [ref=e62] [cursor=pointer]
              - generic [ref=e64]:
                - generic [ref=e65]:
                  - text: $100
                  - img "black lightning bol" [ref=e66]
                - generic [ref=e67]: =
                - generic [ref=e69]:
                  - text: $200
                  - img "black lightning bol" [ref=e70]
                - generic [ref=e71]:
                  - text: We match your 1st depositWe match your first deposit up to $100.
                  - button "Deposit Now" [ref=e73] [cursor=pointer]
            - button "next slide" [ref=e74] [cursor=pointer]
          - generic [ref=e78]:
            - generic [ref=e80]:
              - textbox "Search player or team" [ref=e84]
              - generic [ref=e85]:
                - button "All" [ref=e86] [cursor=pointer]
                - button "MLB" [ref=e87] [cursor=pointer]
                - button "SerieA" [ref=e88] [cursor=pointer]
                - button "EPL" [ref=e89] [cursor=pointer]
                - button "WNBA" [ref=e90] [cursor=pointer]
                - button "WNBA-Combos" [ref=e91] [cursor=pointer]
                - button "WNBA Q1" [ref=e92] [cursor=pointer]
                - button "WNBA H1" [ref=e93] [cursor=pointer]
                - button "MLS" [ref=e94] [cursor=pointer]
                - button "NFLSZN" [ref=e95] [cursor=pointer]
                - button "LaLiga" [ref=e96] [cursor=pointer]
                - button "UFC" [ref=e97] [cursor=pointer]
                - button "Bundes" [ref=e98] [cursor=pointer]
              - button [ref=e100] [cursor=pointer]:
                - img "right chevron sign" [ref=e101]
                - text: Filter
            - generic [ref=e102]:
              - generic [ref=e105]:
                - generic [ref=e108]:
                  - generic [ref=e109]:
                    - img "Ian Seymour" [ref=e111]
                    - generic [ref=e112]:
                      - generic [ref=e113]: Ian Seymour
                      - generic [ref=e114]: SP - TB
                      - generic [ref=e115]: TB @ DET 6:40 PM
                    - button "Open expert opinion for Ian Seymour" [ref=e118]
                  - generic [ref=e123]:
                    - generic [ref=e124]:
                      - generic [ref=e125]:
                        - generic [ref=e126]: Less
                        - generic [ref=e130]: Strikeouts (K)
                        - generic [ref=e131]: More
                      - generic [ref=e135]:
                        - generic [ref=e136]:
                          - button "Select over 3.5 Strikeouts (K) for 0 times" [disabled] [ref=e137]
                          - generic [ref=e138]: 3.5 Strikeouts (K)
                          - button "Select over 3.5 Strikeouts (K) for 1.06 times" [ref=e139]: 1.06x
                        - generic [ref=e140]:
                          - button "Select over 4.5 Strikeouts (K) for 0 times" [disabled] [ref=e141]
                          - generic [ref=e142]: 4.5 Strikeouts (K)
                          - button "Select over 4.5 Strikeouts (K) for 1.27 times" [ref=e143]: 1.27x
                        - generic [ref=e144]:
                          - button "Select over 5.5 Strikeouts (K) for 1.86 times" [ref=e145]: 1.86x
                          - generic [ref=e146]: 5.5 Strikeouts (K)
                          - button "Select over 5.5 Strikeouts (K) for 1.78 times" [ref=e147]: 1.78x
                        - generic [ref=e148]:
                          - button "Select over 6.5 Strikeouts (K) for 0 times" [disabled] [ref=e149]
                          - generic [ref=e150]: 6.5 Strikeouts (K)
                          - button "Select over 6.5 Strikeouts (K) for 2.59 times" [ref=e151]: 2.59x
                        - generic [ref=e152]:
                          - button "Select over 7.5 Strikeouts (K) for 0 times" [disabled] [ref=e153]
                          - generic [ref=e154]: 7.5 Strikeouts (K)
                          - button "Select over 7.5 Strikeouts (K) for 3.91 times" [ref=e155]: 3.91x
                        - button "Show more Strikeouts (K) lines (7)" [ref=e156]
                    - generic [ref=e159]:
                      - generic [ref=e160]:
                        - generic [ref=e161]: Less
                        - generic [ref=e165]: Hits Allowed
                        - generic [ref=e166]: More
                      - generic [ref=e171]:
                        - button "Select over 4.5 Hits Allowed for 1.78 times" [ref=e172]: 1.78x
                        - generic [ref=e173]: 4.5 Hits Allowed
                        - button "Select over 4.5 Hits Allowed for 1.78 times" [ref=e174]: 1.78x
                  - button "Show More Stats" [ref=e176]
                - generic [ref=e181]:
                  - generic [ref=e182]:
                    - img "Junior Caminero" [ref=e184]
                    - generic [ref=e185]:
                      - generic [ref=e186]: J. Caminero
                      - generic [ref=e187]: 3B - TB
                      - generic [ref=e188]: TB @ DET 6:40 PM
                    - button "Open expert opinion for Junior Caminero" [ref=e191]
                  - generic [ref=e196]:
                    - generic [ref=e197]:
                      - generic [ref=e198]:
                        - generic [ref=e199]: Less
                        - generic [ref=e203]: Hits
                        - generic [ref=e204]: More
                      - generic [ref=e208]:
                        - generic [ref=e209]:
                          - button "Select over 0.5 Hits for 2.61 times" [active] [ref=e210]: 2.61x
                          - generic [ref=e211]: 0.5 Hits
                          - button "Select over 0.5 Hits for 1.28 times" [ref=e212]: 1.28x
                        - generic [ref=e213]:
                          - button "Select over 1.5 Hits for 0 times" [disabled] [ref=e214]
                          - generic [ref=e215]: 1.5 Hits
                          - button "Select over 1.5 Hits for 2.87 times" [ref=e216]: 2.87x
                        - generic [ref=e217]:
                          - button "Select over 2.5 Hits for 0 times" [disabled] [ref=e218]
                          - generic [ref=e219]: 2.5 Hits
                          - button "Select over 2.5 Hits for 7.79 times" [ref=e220]: 7.79x
                        - generic [ref=e221]:
                          - button "Select over 3.5 Hits for 0 times" [disabled] [ref=e222]
                          - generic [ref=e223]: 3.5 Hits
                          - button "Select over 3.5 Hits for 26.8 times" [ref=e224]: 26.8x
                    - generic [ref=e225]:
                      - generic [ref=e226]:
                        - generic [ref=e227]: Less
                        - generic [ref=e231]: Hits + Runs + RBIs
                        - generic [ref=e232]: More
                      - generic [ref=e236]:
                        - generic [ref=e237]:
                          - button "Select over 0.5 Hits + Runs + RBIs for 0 times" [disabled] [ref=e238]
                          - generic [ref=e239]: 0.5 H+R+R
                          - button "Select over 0.5 Hits + Runs + RBIs for 1.21 times" [ref=e240]: 1.21x
                        - generic [ref=e241]:
                          - button "Select over 1.5 Hits + Runs + RBIs for 1.89 times" [ref=e242]: 1.89x
                          - generic [ref=e243]: 1.5 H+R+R
                          - button "Select over 1.5 Hits + Runs + RBIs for 1.68 times" [ref=e244]: 1.68x
                        - generic [ref=e245]:
                          - button "Select over 2.5 Hits + Runs + RBIs for 0 times" [disabled] [ref=e246]
                          - generic [ref=e247]: 2.5 H+R+R
                          - button "Select over 2.5 Hits + Runs + RBIs for 2.31 times" [ref=e248]: 2.31x
                        - generic [ref=e249]:
                          - button "Select over 3.5 Hits + Runs + RBIs for 0 times" [disabled] [ref=e250]
                          - generic [ref=e251]: 3.5 H+R+R
                          - button "Select over 3.5 Hits + Runs + RBIs for 3.14 times" [ref=e252]: 3.14x
                        - generic [ref=e253]:
                          - button "Select over 4.5 Hits + Runs + RBIs for 0 times" [disabled] [ref=e254]
                          - generic [ref=e255]: 4.5 H+R+R
                          - button "Select over 4.5 Hits + Runs + RBIs for 4.38 times" [ref=e256]: 4.38x
                    - generic [ref=e257]:
                      - generic [ref=e258]:
                        - generic [ref=e259]: Less
                        - generic [ref=e263]: Singles
                        - generic [ref=e264]: More
                      - generic [ref=e268]:
                        - generic [ref=e269]:
                          - button "Select over 0.5 Singles for 1.72 times" [ref=e270]: 1.72x
                          - generic [ref=e271]: 0.5 Singles
                          - button "Select over 0.5 Singles for 1.8 times" [ref=e272]: 1.8x
                        - generic [ref=e273]:
                          - button "Select over 1.5 Singles for 0 times" [disabled] [ref=e274]
                          - generic [ref=e275]: 1.5 Singles
                          - button "Select over 1.5 Singles for 5.31 times" [ref=e276]: 5.31x
                    - generic [ref=e277]:
                      - generic [ref=e278]:
                        - generic [ref=e279]: Less
                        - generic [ref=e283]: Doubles
                        - generic [ref=e284]: More
                      - generic [ref=e289]:
                        - button "Select over 0.5 Doubles for 1.07 times" [ref=e290]: 1.07x
                        - generic [ref=e291]: 0.5 Doubles
                        - button "Select over 0.5 Doubles for 4.1 times" [ref=e292]: 4.1x
                    - generic [ref=e293]:
                      - generic [ref=e294]:
                        - generic [ref=e295]: Less
                        - generic [ref=e299]: Triples
                        - generic [ref=e300]: More
                      - generic [ref=e305]:
                        - button "Select over 0.5 Triples for 0 times" [disabled] [ref=e306]
                        - generic [ref=e307]: 0.5 Triples
                        - button "Select over 0.5 Triples for 35.5 times" [ref=e308]: 35.5x
                    - generic [ref=e309]:
                      - generic [ref=e310]:
                        - generic [ref=e311]: Less
                        - generic [ref=e315]: Runs
                        - generic [ref=e316]: More
                      - generic [ref=e320]:
                        - generic [ref=e321]:
                          - button "Select over 0.5 Runs for 1.58 times" [ref=e322]: 1.58x
                          - generic [ref=e323]: 0.5 Runs
                          - button "Select over 0.5 Runs for 1.93 times" [ref=e324]: 1.93x
                        - generic [ref=e325]:
                          - button "Select over 1.5 Runs for 0 times" [disabled] [ref=e326]
                          - generic [ref=e327]: 1.5 Runs
                          - button "Select over 1.5 Runs for 5.9 times" [ref=e328]: 5.9x
                    - generic [ref=e329]:
                      - generic [ref=e330]:
                        - generic [ref=e331]: Less
                        - generic [ref=e335]: RBIs
                        - generic [ref=e336]: More
                      - generic [ref=e340]:
                        - generic [ref=e341]:
                          - button "Select over 0.5 RBIs for 1.35 times" [ref=e342]: 1.35x
                          - generic [ref=e343]: 0.5 RBIs
                          - button "Select over 0.5 RBIs for 2.31 times" [ref=e344]: 2.31x
                        - generic [ref=e345]:
                          - button "Select over 1.5 RBIs for 0 times" [disabled] [ref=e346]
                          - generic [ref=e347]: 1.5 RBIs
                          - button "Select over 1.5 RBIs for 4.13 times" [ref=e348]: 4.13x
                        - generic [ref=e349]:
                          - button "Select over 2.5 RBIs for 0 times" [disabled] [ref=e350]
                          - generic [ref=e351]: 2.5 RBIs
                          - button "Select over 2.5 RBIs for 7.79 times" [ref=e352]: 7.79x
                    - generic [ref=e353]:
                      - generic [ref=e354]:
                        - generic [ref=e355]: Less
                        - generic [ref=e359]: Homeruns
                        - generic [ref=e360]: More
                      - generic [ref=e364]:
                        - generic [ref=e365]:
                          - button "Select over 0.5 Homeruns for 0 times" [disabled] [ref=e366]
                          - generic [ref=e367]: 0.5 Homeruns
                          - button "Select over 0.5 Homeruns for 4.06 times" [ref=e368]: 4.06x
                        - generic [ref=e369]:
                          - button "Select over 1.5 Homeruns for 0 times" [disabled] [ref=e370]
                          - generic [ref=e371]: 1.5 Homeruns
                          - button "Select over 1.5 Homeruns for 22.89 times" [ref=e372]: 22.89x
                    - generic [ref=e373]:
                      - generic [ref=e374]:
                        - generic [ref=e375]: Less
                        - generic [ref=e379]: Total Bases
                        - generic [ref=e380]: More
                      - generic [ref=e384]:
                        - generic [ref=e385]:
                          - button "Select over 1.5 Total Bases for 1.59 times" [ref=e386]: 1.59x
                          - generic [ref=e387]: 1.5 Total Bases
                          - button "Select over 1.5 Total Bases for 1.98 times" [ref=e388]: 1.98x
                        - generic [ref=e389]:
                          - button "Select over 2.5 Total Bases for 0 times" [disabled] [ref=e390]
                          - generic [ref=e391]: 2.5 Total Bases
                          - button "Select over 2.5 Total Bases for 2.76 times" [ref=e392]: 2.76x
                        - generic [ref=e393]:
                          - button "Select over 3.5 Total Bases for 0 times" [disabled] [ref=e394]
                          - generic [ref=e395]: 3.5 Total Bases
                          - button "Select over 3.5 Total Bases for 3.4 times" [ref=e396]: 3.4x
                        - generic [ref=e397]:
                          - button "Select over 4.5 Total Bases for 0 times" [disabled] [ref=e398]
                          - generic [ref=e399]: 4.5 Total Bases
                          - button "Select over 4.5 Total Bases for 5.32 times" [ref=e400]: 5.32x
                        - generic [ref=e401]:
                          - button "Select over 5.5 Total Bases for 0 times" [disabled] [ref=e402]
                          - generic [ref=e403]: 5.5 Total Bases
                          - button "Select over 5.5 Total Bases for 7.6 times" [ref=e404]: 7.6x
                    - generic [ref=e405]:
                      - generic [ref=e406]:
                        - generic [ref=e407]: Less
                        - generic [ref=e411]: Strikeouts
                        - generic [ref=e412]: More
                      - generic [ref=e416]:
                        - generic [ref=e417]:
                          - button "Select over 0.5 Strikeouts for 0 times" [disabled] [ref=e418]
                          - generic [ref=e419]: 0.5 Strikeouts
                          - button "Select over 0.5 Strikeouts for 1.28 times" [ref=e420]: 1.28x
                        - generic [ref=e421]:
                          - button "Select over 1.5 Strikeouts for 0 times" [disabled] [ref=e422]
                          - generic [ref=e423]: 1.5 Strikeouts
                          - button "Select over 1.5 Strikeouts for 2.96 times" [ref=e424]: 2.96x
                        - generic [ref=e425]:
                          - button "Select over 2.5 Strikeouts for 0 times" [disabled] [ref=e426]
                          - generic [ref=e427]: 2.5 Strikeouts
                          - button "Select over 2.5 Strikeouts for 7.84 times" [ref=e428]: 7.84x
                    - generic [ref=e429]:
                      - generic [ref=e430]:
                        - generic [ref=e431]: Less
                        - generic [ref=e435]: Fantasy Points
                        - generic [ref=e436]: More
                      - generic [ref=e441]:
                        - button "Select over 6.5 Fantasy Points for 1.78 times" [ref=e442]: 1.78x
                        - generic [ref=e443]: 6.5 Fantasy Points
                        - button "Select over 6.5 Fantasy Points for 1.78 times" [ref=e444]: 1.78x
                  - button "Show More Stats" [ref=e446]
                - generic [ref=e451]:
                  - generic [ref=e452]:
                    - img "Yandy Diaz" [ref=e454]
                    - generic [ref=e455]:
                      - generic [ref=e456]: Yandy Diaz
                      - generic [ref=e457]: DH - TB
                      - generic [ref=e458]: TB @ DET 6:40 PM
                    - button "Open expert opinion for Yandy Diaz" [ref=e461]
                  - generic [ref=e466]:
                    - generic [ref=e467]:
                      - generic [ref=e468]:
                        - generic [ref=e469]: Less
                        - generic [ref=e473]: Hits
                        - generic [ref=e474]: More
                      - generic [ref=e478]:
                        - generic [ref=e479]:
                          - button "Select over 0.5 Hits for 0 times" [disabled] [ref=e480]
                          - generic [ref=e481]: 0.5 Hits
                          - button "Select over 0.5 Hits for 1.24 times" [ref=e482]: 1.24x
                        - generic [ref=e483]:
                          - button "Select over 1.5 Hits for 1.28 times" [ref=e484]: 1.28x
                          - generic [ref=e485]: 1.5 Hits
                          - button "Select over 1.5 Hits for 2.68 times" [ref=e486]: 2.68x
                        - generic [ref=e487]:
                          - button "Select over 2.5 Hits for 0 times" [disabled] [ref=e488]
                          - generic [ref=e489]: 2.5 Hits
                          - button "Select over 2.5 Hits for 6.78 times" [ref=e490]: 6.78x
                        - generic [ref=e491]:
                          - button "Select over 3.5 Hits for 0 times" [disabled] [ref=e492]
                          - generic [ref=e493]: 3.5 Hits
                          - button "Select over 3.5 Hits for 23.8 times" [ref=e494]: 23.8x
                    - generic [ref=e495]:
                      - generic [ref=e496]:
                        - generic [ref=e497]: Less
                        - generic [ref=e501]: Hits + Runs + RBIs
                        - generic [ref=e502]: More
                      - generic [ref=e506]:
                        - generic [ref=e507]:
                          - button "Select over 0.5 Hits + Runs + RBIs for 0 times" [disabled] [ref=e508]
                          - generic [ref=e509]: 0.5 H+R+R
                          - button "Select over 0.5 Hits + Runs + RBIs for 1.12 times" [ref=e510]: 1.12x
                        - generic [ref=e511]:
                          - button "Select over 1.5 Hits + Runs + RBIs for 2 times" [ref=e512]: 2x
                          - generic [ref=e513]: 1.5 H+R+R
                          - button "Select over 1.5 Hits + Runs + RBIs for 1.59 times" [ref=e514]: 1.59x
                        - generic [ref=e515]:
                          - button "Select over 2.5 Hits + Runs + RBIs for 0 times" [disabled] [ref=e516]
                          - generic [ref=e517]: 2.5 H+R+R
                          - button "Select over 2.5 Hits + Runs + RBIs for 2.4 times" [ref=e518]: 2.4x
                        - generic [ref=e519]:
                          - button "Select over 3.5 Hits + Runs + RBIs for 0 times" [disabled] [ref=e520]
                          - generic [ref=e521]: 3.5 H+R+R
                          - button "Select over 3.5 Hits + Runs + RBIs for 3.52 times" [ref=e522]: 3.52x
                        - generic [ref=e523]:
                          - button "Select over 4.5 Hits + Runs + RBIs for 0 times" [disabled] [ref=e524]
                          - generic [ref=e525]: 4.5 H+R+R
                          - button "Select over 4.5 Hits + Runs + RBIs for 5.42 times" [ref=e526]: 5.42x
                    - generic [ref=e527]:
                      - generic [ref=e528]:
                        - generic [ref=e529]: Less
                        - generic [ref=e533]: Singles
                        - generic [ref=e534]: More
                      - generic [ref=e538]:
                        - generic [ref=e539]:
                          - button "Select over 0.5 Singles for 2.1 times" [ref=e540]: 2.1x
                          - generic [ref=e541]: 0.5 Singles
                          - button "Select over 0.5 Singles for 1.49 times" [ref=e542]: 1.49x
                        - generic [ref=e543]:
                          - button "Select over 1.5 Singles for 0 times" [disabled] [ref=e544]
                          - generic [ref=e545]: 1.5 Singles
                          - button "Select over 1.5 Singles for 3.93 times" [ref=e546]: 3.93x
                    - generic [ref=e547]:
                      - generic [ref=e548]:
                        - generic [ref=e549]: Less
                        - generic [ref=e553]: Doubles
                        - generic [ref=e554]: More
                      - generic [ref=e559]:
                        - button "Select over 0.5 Doubles for 1.07 times" [ref=e560]: 1.07x
                        - generic [ref=e561]: 0.5 Doubles
                        - button "Select over 0.5 Doubles for 4.1 times" [ref=e562]: 4.1x
                    - generic [ref=e563]:
                      - generic [ref=e564]:
                        - generic [ref=e565]: Less
                        - generic [ref=e569]: Triples
                        - generic [ref=e570]: More
                      - generic [ref=e575]:
                        - button "Select over 0.5 Triples for 0 times" [disabled] [ref=e576]
                        - generic [ref=e577]: 0.5 Triples
                        - button "Select over 0.5 Triples for 40.9 times" [ref=e578]: 40.9x
                    - generic [ref=e579]:
                      - generic [ref=e580]:
                        - generic [ref=e581]: Less
                        - generic [ref=e585]: Runs
                        - generic [ref=e586]: More
                      - generic [ref=e590]:
                        - generic [ref=e591]:
                          - button "Select over 0.5 Runs for 1.68 times" [ref=e592]: 1.68x
                          - generic [ref=e593]: 0.5 Runs
                          - button "Select over 0.5 Runs for 1.84 times" [ref=e594]: 1.84x
                        - generic [ref=e595]:
                          - button "Select over 1.5 Runs for 0 times" [disabled] [ref=e596]
                          - generic [ref=e597]: 1.5 Runs
                          - button "Select over 1.5 Runs for 5.28 times" [ref=e598]: 5.28x
                    - generic [ref=e599]:
                      - generic [ref=e600]:
                        - generic [ref=e601]: Less
                        - generic [ref=e605]: RBIs
                        - generic [ref=e606]: More
                      - generic [ref=e610]:
                        - generic [ref=e611]:
                          - button "Select over 0.5 RBIs for 1.23 times" [ref=e612]: 1.23x
                          - generic [ref=e613]: 0.5 RBIs
                          - button "Select over 0.5 RBIs for 2.82 times" [ref=e614]: 2.82x
                        - generic [ref=e615]:
                          - button "Select over 1.5 RBIs for 0 times" [disabled] [ref=e616]
                          - generic [ref=e617]: 1.5 RBIs
                          - button "Select over 1.5 RBIs for 6.3 times" [ref=e618]: 6.3x
                    - generic [ref=e619]:
                      - generic [ref=e620]:
                        - generic [ref=e621]: Less
                        - generic [ref=e625]: Homeruns
                        - generic [ref=e626]: More
                      - generic [ref=e630]:
                        - generic [ref=e631]:
                          - button "Select over 0.5 Homeruns for 0 times" [disabled] [ref=e632]
                          - generic [ref=e633]: 0.5 Homeruns
                          - button "Select over 0.5 Homeruns for 6.44 times" [ref=e634]: 6.44x
                        - generic [ref=e635]:
                          - button "Select over 1.5 Homeruns for 0 times" [disabled] [ref=e636]
                          - generic [ref=e637]: 1.5 Homeruns
                          - button "Select over 1.5 Homeruns for 61 times" [ref=e638]: 61x
                    - generic [ref=e639]:
                      - generic [ref=e640]:
                        - generic [ref=e641]: Less
                        - generic [ref=e645]: Total Bases
                        - generic [ref=e646]: More
                      - generic [ref=e650]:
                        - generic [ref=e651]:
                          - button "Select over 1.5 Total Bases for 1.53 times" [ref=e652]: 1.53x
                          - generic [ref=e653]: 1.5 Total Bases
                          - button "Select over 1.5 Total Bases for 2.03 times" [ref=e654]: 2.03x
                        - generic [ref=e655]:
                          - button "Select over 2.5 Total Bases for 0 times" [disabled] [ref=e656]
                          - generic [ref=e657]: 2.5 Total Bases
                          - button "Select over 2.5 Total Bases for 3.25 times" [ref=e658]: 3.25x
                        - generic [ref=e659]:
                          - button "Select over 3.5 Total Bases for 0 times" [disabled] [ref=e660]
                          - generic [ref=e661]: 3.5 Total Bases
                          - button "Select over 3.5 Total Bases for 4.84 times" [ref=e662]: 4.84x
                        - generic [ref=e663]:
                          - button "Select over 4.5 Total Bases for 0 times" [disabled] [ref=e664]
                          - generic [ref=e665]: 4.5 Total Bases
                          - button "Select over 4.5 Total Bases for 7.48 times" [ref=e666]: 7.48x
                    - generic [ref=e667]:
                      - generic [ref=e668]:
                        - generic [ref=e669]: Less
                        - generic [ref=e673]: Strikeouts
                        - generic [ref=e674]: More
                      - generic [ref=e678]:
                        - generic [ref=e679]:
                          - button "Select over 0.5 Strikeouts for 0 times" [disabled] [ref=e680]
                          - generic [ref=e681]: 0.5 Strikeouts
                          - button "Select over 0.5 Strikeouts for 1.57 times" [ref=e682]: 1.57x
                        - generic [ref=e683]:
                          - button "Select over 1.5 Strikeouts for 0 times" [disabled] [ref=e684]
                          - generic [ref=e685]: 1.5 Strikeouts
                          - button "Select over 1.5 Strikeouts for 4.34 times" [ref=e686]: 4.34x
                    - generic [ref=e687]:
                      - generic [ref=e688]:
                        - generic [ref=e689]: Less
                        - generic [ref=e693]: Fantasy Points
                        - generic [ref=e694]: More
                      - generic [ref=e699]:
                        - button "Select over 7.5 Fantasy Points for 1.78 times" [ref=e700]: 1.78x
                        - generic [ref=e701]: 7.5 Fantasy Points
                        - button "Select over 7.5 Fantasy Points for 1.78 times" [ref=e702]: 1.78x
                  - button "Show More Stats" [ref=e704]
                - generic [ref=e709]:
                  - generic [ref=e710]:
                    - img "Richie Palacios" [ref=e712]
                    - generic [ref=e713]:
                      - generic [ref=e714]: R. Palacios
                      - generic [ref=e715]: SS - TB
                      - generic [ref=e716]: TB @ DET 6:40 PM
                    - button "Open expert opinion for Richie Palacios" [ref=e719]
                  - generic [ref=e724]:
                    - generic [ref=e725]:
                      - generic [ref=e726]:
                        - generic [ref=e727]: Less
                        - generic [ref=e731]: Hits
                        - generic [ref=e732]: More
                      - generic [ref=e736]:
                        - generic [ref=e737]:
                          - button "Select over 0.5 Hits for 1.93 times" [ref=e738]: 1.93x
                          - generic [ref=e739]: 0.5 Hits
                          - button "Select over 0.5 Hits for 1.7 times" [ref=e740]: 1.7x
                        - generic [ref=e741]:
                          - button "Select over 1.5 Hits for 0 times" [disabled] [ref=e742]
                          - generic [ref=e743]: 1.5 Hits
                          - button "Select over 1.5 Hits for 4.4 times" [ref=e744]: 4.4x
                        - generic [ref=e745]:
                          - button "Select over 2.5 Hits for 0 times" [disabled] [ref=e746]
                          - generic [ref=e747]: 2.5 Hits
                          - button "Select over 2.5 Hits for 14.2 times" [ref=e748]: 14.2x
                    - generic [ref=e749]:
                      - generic [ref=e750]:
                        - generic [ref=e751]: Less
                        - generic [ref=e755]: Hits + Runs + RBIs
                        - generic [ref=e756]: More
                      - generic [ref=e760]:
                        - generic [ref=e761]:
                          - button "Select over 0.5 Hits + Runs + RBIs for 2.26 times" [ref=e762]: 2.26x
                          - generic [ref=e763]: 0.5 H+R+R
                          - button "Select over 0.5 Hits + Runs + RBIs for 1.41 times" [ref=e764]: 1.41x
                        - generic [ref=e765]:
                          - button "Select over 1.5 Hits + Runs + RBIs for 0 times" [disabled] [ref=e766]
                          - generic [ref=e767]: 1.5 H+R+R
                          - button "Select over 1.5 Hits + Runs + RBIs for 2.25 times" [ref=e768]: 2.25x
                        - generic [ref=e769]:
                          - button "Select over 2.5 Hits + Runs + RBIs for 0 times" [disabled] [ref=e770]
                          - generic [ref=e771]: 2.5 H+R+R
                          - button "Select over 2.5 Hits + Runs + RBIs for 3.52 times" [ref=e772]: 3.52x
                        - generic [ref=e773]:
                          - button "Select over 3.5 Hits + Runs + RBIs for 0 times" [disabled] [ref=e774]
                          - generic [ref=e775]: 3.5 H+R+R
                          - button "Select over 3.5 Hits + Runs + RBIs for 5.63 times" [ref=e776]: 5.63x
                        - generic [ref=e777]:
                          - button "Select over 4.5 Hits + Runs + RBIs for 0 times" [disabled] [ref=e778]
                          - generic [ref=e779]: 4.5 H+R+R
                          - button "Select over 4.5 Hits + Runs + RBIs for 8.2 times" [ref=e780]: 8.2x
                    - generic [ref=e781]:
                      - generic [ref=e782]:
                        - generic [ref=e783]: Less
                        - generic [ref=e787]: Singles
                        - generic [ref=e788]: More
                      - generic [ref=e792]:
                        - generic [ref=e793]:
                          - button "Select over 0.5 Singles for 1.53 times" [ref=e794]: 1.53x
                          - generic [ref=e795]: 0.5 Singles
                          - button "Select over 0.5 Singles for 2.12 times" [ref=e796]: 2.12x
                        - generic [ref=e797]:
                          - button "Select over 1.5 Singles for 0 times" [disabled] [ref=e798]
                          - generic [ref=e799]: 1.5 Singles
                          - button "Select over 1.5 Singles for 6.09 times" [ref=e800]: 6.09x
                    - generic [ref=e801]:
                      - generic [ref=e802]:
                        - generic [ref=e803]: Less
                        - generic [ref=e807]: Doubles
                        - generic [ref=e808]: More
                      - generic [ref=e813]:
                        - button "Select over 0.5 Doubles for 0 times" [disabled] [ref=e814]
                        - generic [ref=e815]: 0.5 Doubles
                        - button "Select over 0.5 Doubles for 5.1 times" [ref=e816]: 5.1x
                    - generic [ref=e817]:
                      - generic [ref=e818]:
                        - generic [ref=e819]: Less
                        - generic [ref=e823]: Triples
                        - generic [ref=e824]: More
                      - generic [ref=e829]:
                        - button "Select over 0.5 Triples for 0 times" [disabled] [ref=e830]
                        - generic [ref=e831]: 0.5 Triples
                        - button "Select over 0.5 Triples for 17.2 times" [ref=e832]: 17.2x
                    - generic [ref=e833]:
                      - generic [ref=e834]:
                        - generic [ref=e835]: Less
                        - generic [ref=e839]: Runs
                        - generic [ref=e840]: More
                      - generic [ref=e844]:
                        - generic [ref=e845]:
                          - button "Select over 0.5 Runs for 1.27 times" [ref=e846]: 1.27x
                          - generic [ref=e847]: 0.5 Runs
                          - button "Select over 0.5 Runs for 2.66 times" [ref=e848]: 2.66x
                        - generic [ref=e849]:
                          - button "Select over 1.5 Runs for 0 times" [disabled] [ref=e850]
                          - generic [ref=e851]: 1.5 Runs
                          - button "Select over 1.5 Runs for 10.59 times" [ref=e852]: 10.59x
                    - generic [ref=e853]:
                      - generic [ref=e854]:
                        - generic [ref=e855]: Less
                        - generic [ref=e859]: RBIs
                        - generic [ref=e860]: More
                      - generic [ref=e864]:
                        - generic [ref=e865]:
                          - button "Select over 0.5 RBIs for 1.13 times" [ref=e866]: 1.13x
                          - generic [ref=e867]: 0.5 RBIs
                          - button "Select over 0.5 RBIs for 3.2 times" [ref=e868]: 3.2x
                        - generic [ref=e869]:
                          - button "Select over 1.5 RBIs for 0 times" [disabled] [ref=e870]
                          - generic [ref=e871]: 1.5 RBIs
                          - button "Select over 1.5 RBIs for 7.38 times" [ref=e872]: 7.38x
                    - generic [ref=e873]:
                      - generic [ref=e874]:
                        - generic [ref=e875]: Less
                        - generic [ref=e879]: Homeruns
                        - generic [ref=e880]: More
                      - generic [ref=e884]:
                        - generic [ref=e885]:
                          - button "Select over 0.5 Homeruns for 0 times" [disabled] [ref=e886]
                          - generic [ref=e887]: 0.5 Homeruns
                          - button "Select over 0.5 Homeruns for 8.8 times" [ref=e888]: 8.8x
                        - generic [ref=e889]:
                          - button "Select over 1.5 Homeruns for 0 times" [disabled] [ref=e890]
                          - generic [ref=e891]: 1.5 Homeruns
                          - button "Select over 1.5 Homeruns for 210.98 times" [ref=e892]: 210.98x
                    - generic [ref=e893]:
                      - generic [ref=e894]:
                        - generic [ref=e895]: Less
                        - generic [ref=e899]: Total Bases
                        - generic [ref=e900]: More
                      - generic [ref=e904]:
                        - generic [ref=e905]:
                          - button "Select over 1.5 Total Bases for 0 times" [disabled] [ref=e906]
                          - generic [ref=e907]: 1.5 Total Bases
                          - button "Select over 1.5 Total Bases for 2.89 times" [ref=e908]: 2.89x
                        - generic [ref=e909]:
                          - button "Select over 2.5 Total Bases for 0 times" [disabled] [ref=e910]
                          - generic [ref=e911]: 2.5 Total Bases
                          - button "Select over 2.5 Total Bases for 5.08 times" [ref=e912]: 5.08x
                        - generic [ref=e913]:
                          - button "Select over 3.5 Total Bases for 0 times" [disabled] [ref=e914]
                          - generic [ref=e915]: 3.5 Total Bases
                          - button "Select over 3.5 Total Bases for 7.42 times" [ref=e916]: 7.42x
                        - generic [ref=e917]:
                          - button "Select over 4.5 Total Bases for 0 times" [disabled] [ref=e918]
                          - generic [ref=e919]: 4.5 Total Bases
                          - button "Select over 4.5 Total Bases for 15.98 times" [ref=e920]: 15.98x
                    - generic [ref=e921]:
                      - generic [ref=e922]:
                        - generic [ref=e923]: Less
                        - generic [ref=e927]: Strikeouts
                        - generic [ref=e928]: More
                      - generic [ref=e932]:
                        - generic [ref=e933]:
                          - button "Select over 0.5 Strikeouts for 0 times" [disabled] [ref=e934]
                          - generic [ref=e935]: 0.5 Strikeouts
                          - button "Select over 0.5 Strikeouts for 1.78 times" [ref=e936]: 1.78x
                        - generic [ref=e937]:
                          - button "Select over 1.5 Strikeouts for 0 times" [disabled] [ref=e938]
                          - generic [ref=e939]: 1.5 Strikeouts
                          - button "Select over 1.5 Strikeouts for 5.5 times" [ref=e940]: 5.5x
                    - generic [ref=e941]:
                      - generic [ref=e942]:
                        - generic [ref=e943]: Less
                        - generic [ref=e947]: Fantasy Points
                        - generic [ref=e948]: More
                      - generic [ref=e953]:
                        - button "Select over 3.5 Fantasy Points for 1.78 times" [ref=e954]: 1.78x
                        - generic [ref=e955]: 3.5 Fantasy Points
                        - button "Select over 3.5 Fantasy Points for 1.78 times" [ref=e956]: 1.78x
                  - button "Show More Stats" [ref=e958]
              - generic [ref=e2059]:
                - generic [ref=e2061]:
                  - generic [ref=e2062]: 2.86x
                  - generic [ref=e2063]:
                    - button "+ 5% Boost 🚀" [ref=e2068]
                    - generic [ref=e2079]: "Add 3rd Pick: 5% Boost"
                - generic [ref=e2082]:
                  - generic [ref=e2084]:
                    - generic [ref=e2085]:
                      - generic [ref=e2086]: "1"
                      - button [ref=e2090]
                      - generic [ref=e2094]: Real Betis Balompié - Natan Bernardo de Souza
                      - generic [ref=e2095]: Today 3:00 PM vs VAL
                      - generic [ref=e2096]:
                        - button "Less 0.5 Shots" [disabled] [ref=e2098]:
                          - generic [ref=e2099]: Less
                          - generic [ref=e2100]: "0.5"
                          - generic [ref=e2101]: Shots
                        - button "2.38 x More 0.5 Shots" [ref=e2103]:
                          - generic [ref=e2104]: 2.38 x
                          - generic [ref=e2106]: More
                          - generic [ref=e2107]: "0.5"
                          - generic [ref=e2108]: Shots
                    - img "Natan Bernardo de Souza" [ref=e2115]
                  - generic [ref=e2117]:
                    - generic [ref=e2118]:
                      - generic [ref=e2119]: "2"
                      - button [ref=e2123]
                      - generic [ref=e2127]: Valencia CF - Hugo Duro
                      - generic [ref=e2128]: Today 3:00 PM vs BET
                      - generic [ref=e2129]:
                        - button "Less 1.5 Shots" [disabled] [ref=e2131]:
                          - generic [ref=e2132]: Less
                          - generic [ref=e2133]: "1.5"
                          - generic [ref=e2134]: Shots
                        - button "1.2 x More 1.5 Shots" [ref=e2136]:
                          - generic [ref=e2137]: 1.2 x
                          - generic [ref=e2139]: More
                          - generic [ref=e2140]: "1.5"
                          - generic [ref=e2141]: Shots
                    - img "Hugo Duro" [ref=e2148]
                  - generic [ref=e2149]:
                    - generic [ref=e2150]:
                      - generic [ref=e2152]:
                        - radio "$25"
                        - generic [ref=e2153] [cursor=pointer]: $25
                        - radio "$75"
                        - generic [ref=e2154] [cursor=pointer]: $75
                        - radio "$300" [disabled]
                        - generic: $300
                      - generic [ref=e2156]:
                        - generic [ref=e2157]: $
                        - spinbutton [ref=e2161]: "3"
                      - button "5" [ref=e2162] [cursor=pointer]
                    - generic [ref=e2166]:
                      - generic [ref=e2167]:
                        - generic [ref=e2168]:
                          - button "Insured" [ref=e2169]
                          - button "All In" [ref=e2170]
                        - generic [ref=e2171]: 2.86x
                      - generic [ref=e2174]:
                        - generic [ref=e2175]:
                          - paragraph [ref=e2176]: Perfect line-up
                          - paragraph [ref=e2177]: $8.58
                        - generic [ref=e2179]:
                          - paragraph [ref=e2180]: Or 1st place in group
                          - generic [ref=e2181]: $1 + $8.58
                    - button "Place" [ref=e2185] [cursor=pointer]
          - generic [ref=e2190]:
            - generic [ref=e2191]:
              - link [ref=e2192] [cursor=pointer]:
                - /url: /
                - img "Parlay Play Logo" [ref=e2194]
              - generic [ref=e2195]:
                - generic [ref=e2196]: Improve your experience. Download our app.
                - generic [ref=e2197]:
                  - link [ref=e2198] [cursor=pointer]:
                    - /url: https://parlayplay.onelink.me/oLJk/gnqpwjha
                    - img "Apple Store" [ref=e2199]
                  - link [ref=e2200] [cursor=pointer]:
                    - /url: https://parlayplay.onelink.me/oLJk/fh7u6juo
                    - img "Google Play Store" [ref=e2201]
            - generic [ref=e2202]:
              - link "Privacy" [ref=e2203] [cursor=pointer]:
                - /url: /privacy-policy
              - link "Fantasy Terms" [ref=e2204] [cursor=pointer]:
                - /url: /terms
              - link "Packs Terms" [ref=e2205] [cursor=pointer]:
                - /url: /terms/packs
              - link "Responsible Gaming" [ref=e2206] [cursor=pointer]:
                - /url: /responsible-gaming
              - link "Gaming Rules" [ref=e2207] [cursor=pointer]:
                - /url: /rules
              - link "FAQ" [ref=e2208] [cursor=pointer]:
                - /url: https://intercom.help/parlayplay/en/
              - link "Contact Us" [ref=e2209] [cursor=pointer]:
                - /url: /
              - paragraph [ref=e2210]: © ParlayPlay 2026 - All Rights Reserved
            - list [ref=e2211]:
              - listitem [ref=e2212]:
                - generic [ref=e2213]:
                  - log [ref=e2215]
                  - generic [ref=e2217]:
                    - generic [ref=e2218]: 🇺🇸English
                    - combobox "Select language" [ref=e2219]
              - listitem [ref=e2225]:
                - img "18+-icon" [ref=e2226]
              - listitem [ref=e2227]:
                - link "ParlayPlay on Twitter" [ref=e2228] [cursor=pointer]:
                  - /url: https://twitter.com/parlay_play?lang=en
              - listitem [ref=e2231]:
                - link "ParlayPlay on Facebook" [ref=e2232] [cursor=pointer]:
                  - /url: https://www.facebook.com/ParlayPlay.io/
              - listitem [ref=e2235]:
                - link "ParlayPlay on Instagram" [ref=e2236] [cursor=pointer]:
                  - /url: https://www.instagram.com/parlayplay_?igsh=bHBldWQyMmV2b3Y4
              - listitem [ref=e2239]:
                - link "ParlayPlay on Discord" [ref=e2240] [cursor=pointer]:
                  - /url: https://discord.com/invite/parlayplay
            - link [ref=e2244] [cursor=pointer]:
              - /url: https://sportsdata.io/
              - img "Powered by SportsDataIO" [ref=e2245]
    - generic:
      - region "Notifications Alt+T"
  - alert [ref=e2246]
  - iframe [ref=e2247]:
    
```

# Test source

```ts
  313 | 
  314 |     for (let i = 0; i < count; i++) {
  315 |       const btn = buttons.nth(i);
  316 |       const classes = (await btn.getAttribute("class")) ?? "";
  317 |       if (classes.includes("bg-playYellow")) {
  318 |         await btn.click(); // Deselects the selected button
  319 |         return;
  320 |       }
  321 |     }
  322 |     throw new Error("No selected button found with bg-yellow class.");
  323 |   }
  324 | 
  325 |   /**
  326 |    * Picks `count` players.
  327 |    *
  328 |    * `excludeIds` skips players that a previous attempt already tried. Retries
  329 |    * (e.g. after "multiple promos cannot be applied") pass the players from the
  330 |    * failed slip so the next attempt selects genuinely new cards instead of
  331 |    * re-picking the same promo-bearing players in the same deterministic order.
  332 |    */
  333 |   async pickPlayers(
  334 |     count: number,
  335 |     statIdx?: number,
  336 |     excludeIds?: Set<string>,
  337 |   ): Promise<string[]> {
  338 |     const leagueButtons = await this.listLeagueButtons();
  339 | 
  340 |     const selected = new Set<string>();
  341 |     let lastPickId: string | null = null;
  342 |     // Caller-provided players to skip for the whole call. Kept separate from
  343 |     // recentlyFailed (which is cleared once a valid combo is found) so retries
  344 |     // never re-pick a player a prior attempt already tried.
  345 |     const excluded = new Set<string>(excludeIds ?? []);
  346 |     const recentlyFailed = new Set<string>();
  347 |     for (const leagueButton of leagueButtons) {
  348 |       const leagueId = (await leagueButton.getAttribute("id")) ?? "";
  349 |       // Skip the Combo (`league-*-combo`) and Promo (`league-Promo`) leagues:
  350 |       // every card in them carries a promo, so picking >1 always trips
  351 |       // "multiple promos cannot be applied" — and since the whole league is
  352 |       // promos, re-picking never escapes it. Regular sport leagues almost
  353 |       // never stack two promos (the exclusion retry handles the rare case).
  354 |       const lid = leagueId.toLowerCase();
  355 |       if (lid.includes("combo") || lid.includes("promo")) continue;
  356 | 
  357 |       await this.clickLeagueTab(leagueButton);
  358 |       await this.waitForPlayersGrid();
  359 | 
  360 |       // Each league resets to its default stat tab on click, so re-pin
  361 |       // the requested stat after navigating into the league.
  362 |       if (statIdx !== undefined) {
  363 |         const statTab = this.statsSelector.locator("li button").nth(statIdx);
  364 |         if (await statTab.isVisible().catch(() => false)) {
  365 |           await statTab.click();
  366 |           await this.waitForPlayersGrid();
  367 |         }
  368 |       }
  369 | 
  370 |       if (await this.noPlayerLabel.isVisible().catch(() => false)) {
  371 |         continue;
  372 |       }
  373 | 
  374 |       const playerIds = await this.listVisiblePlayerIds();
  375 |       for (const playerId of playerIds) {
  376 |         if (
  377 |           selected.has(playerId) ||
  378 |           recentlyFailed.has(playerId) ||
  379 |           excluded.has(playerId)
  380 |         )
  381 |           continue;
  382 | 
  383 |         if (await this.trySelectPick(this.playerCardById(playerId))) {
  384 |           selected.add(playerId);
  385 |           lastPickId = playerId;
  386 | 
  387 |           let continueFlag = await this.isContinueEnabled();
  388 |           if (selected.size >= count && continueFlag)
  389 |             return Array.from(selected);
  390 | 
  391 |           // Warning modal continuation
  392 |           while (!continueFlag && selected.size == count && lastPickId) {
  393 |             await this.deselectPick(this.playerCardById(lastPickId));
  394 |             selected.delete(lastPickId);
  395 |             recentlyFailed.add(lastPickId);
  396 | 
  397 |             let replaced = false;
  398 |             for (const nextId of playerIds) {
  399 |               if (
  400 |                 selected.has(nextId) ||
  401 |                 recentlyFailed.has(nextId) ||
  402 |                 excluded.has(nextId)
  403 |               )
  404 |                 continue;
  405 |               if (await this.trySelectPick(this.playerCardById(nextId))) {
  406 |                 selected.add(nextId);
  407 |                 lastPickId = nextId;
  408 |                 replaced = true;
  409 |                 break;
  410 |               }
  411 |             }
  412 |             if (!replaced) {
> 413 |               throw new Error(
      |                     ^ Error: Unable to find replacement pick when Continue is disabled (target: 3)
  414 |                 `Unable to find replacement pick when Continue is disabled (target: ${count})`
  415 |               );
  416 |             }
  417 |             continueFlag = await this.isContinueEnabled();
  418 |           }
  419 | 
  420 |           if (continueFlag && selected.size == count)
  421 |             return Array.from(selected);
  422 |           if (continueFlag) recentlyFailed.clear();
  423 |         }
  424 |       }
  425 |     }
  426 | 
  427 |     if (selected.size < count)
  428 |       throw new Error(`Could not select ${count} valid picks`);
  429 |     return Array.from(selected);
  430 |   }
  431 | 
  432 |   async pickFivePlayers(): Promise<string[]> {
  433 |     return this.pickPlayers(5);
  434 |   }
  435 | 
  436 |   /**
  437 |    * Reads the persisted slip from localStorage and returns the set of player
  438 |    * IDs it currently contains. Source of truth is the storage key the app
  439 |    * writes via `slipPersistence.saveSlip` — see `utils/slipPersistence.ts`.
  440 |    *
  441 |    * Why this over scraping the DOM: card visualisation depends on the offering
  442 |    * having a flagged main/default altLine. When the backend omits those flags
  443 |    * for a player (e.g. Cunningham bb_points), the card boots on a fallback
  444 |    * line that doesn't match the picked one, and the highlight isn't visible
  445 |    * even though the pick is correctly persisted. Reading storage decouples the
  446 |    * persistence assertion from the render path.
  447 |    */
  448 |   async getPersistedPickIds(): Promise<string[]> {
  449 |     return this.page.evaluate(() => {
  450 |       const raw = localStorage.getItem("pp_persistent_slip:v1");
  451 |       if (!raw) return [];
  452 |       try {
  453 |         const parsed = JSON.parse(raw);
  454 |         return Object.keys(parsed.selectedPicks ?? {});
  455 |       } catch {
  456 |         return [];
  457 |       }
  458 |     });
  459 |   }
  460 | 
  461 |   async assertPicksPersist(
  462 |     expectedIds: string[],
  463 |     timeout = 10_000,
  464 |   ): Promise<void> {
  465 |     // Storage IDs are bare player IDs ("1089"); pickPlayers returns the DOM
  466 |     // attribute form ("player-1089"). Normalise both sides.
  467 |     const normalise = (id: string) => id.replace(/^player-/, "");
  468 |     const expected = new Set(expectedIds.map(normalise));
  469 | 
  470 |     // Auto-save is debounced ~1s and the post-reload restore writes its
  471 |     // reconciled state back asynchronously, so poll rather than read once.
  472 |     await expect
  473 |       .poll(
  474 |         async () => {
  475 |           const ids = await this.getPersistedPickIds();
  476 |           return Array.from(new Set(ids.map(normalise))).sort();
  477 |         },
  478 |         {
  479 |           timeout,
  480 |           message: `Expected persisted picks ${JSON.stringify(
  481 |             Array.from(expected).sort(),
  482 |           )} in localStorage`,
  483 |         },
  484 |       )
  485 |       .toEqual(Array.from(expected).sort());
  486 |   }
  487 | 
  488 |   async waitForSlipPersisted(
  489 |     expectedPickCount: number,
  490 |     timeout = 5_000
  491 |   ): Promise<void> {
  492 |     await expect
  493 |       .poll(
  494 |         async () =>
  495 |           this.page.evaluate(() => {
  496 |             const raw = localStorage.getItem("pp_persistent_slip:v1");
  497 |             if (!raw) return 0;
  498 |             try {
  499 |               return JSON.parse(raw).nrOfPicks ?? 0;
  500 |             } catch {
  501 |               return 0;
  502 |             }
  503 |           }),
  504 |         {
  505 |           timeout,
  506 |           message: `Slip with ${expectedPickCount} picks was never written to localStorage`,
  507 |         }
  508 |       )
  509 |       .toBe(expectedPickCount);
  510 |   }
  511 | 
  512 |   async enterFinalContestPage() {
  513 |     await this.continueBtn.click();
```