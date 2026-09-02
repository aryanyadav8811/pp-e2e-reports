# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: entries/entry-card-redesign.spec.ts >> My Entries card redesign — cancel flow >> Freshly placed entry is cancellable with a live countdown, and confirming Cancel Entry removes it from Active and History (refund + hard delete)
- Location: tests/entries/entry-card-redesign.spec.ts:250:5

# Error details

```
Error: Could not place contest after 5 attempts (last error: Unable to find replacement pick when Continue is disabled (target: 3)) — every attempted stat tab ran out of selectable cards; the environment's offering is likely too thin for this pick count

expect(received).toBe(expected) // Object.is equality

Expected: true
Received: false
```

# Page snapshot

```yaml
- generic [ref=f8e1]:
  - generic [ref=f8e2]:
    - generic [ref=f8e3]:
      - banner [ref=f8e4]:
        - navigation [ref=f8e5]:
          - link [ref=f8e6] [cursor=pointer]:
            - /url: /
            - img "Parlay Play Logo" [ref=f8e8]
          - generic [ref=f8e9]:
            - list [ref=f8e10]:
              - listitem [ref=f8e11]:
                - link "Home" [ref=f8e12] [cursor=pointer]:
                  - /url: /
              - listitem [ref=f8e15]:
                - link "Packs" [ref=f8e16] [cursor=pointer]:
                  - /url: /packs
              - listitem [ref=f8e19]:
                - link "Feed" [ref=f8e20] [cursor=pointer]:
                  - /url: /challenges/feed
              - listitem [ref=f8e23]:
                - link "Rewards 6" [ref=f8e24] [cursor=pointer]:
                  - /url: /rewards
                  - generic [ref=f8e25]:
                    - generic [ref=f8e26]: Rewards
                    - generic [ref=f8e27]: "6"
              - listitem [ref=f8e28]:
                - link "Track Picks 55" [ref=f8e29] [cursor=pointer]:
                  - /url: /challenges/pending
                  - generic [ref=f8e30]:
                    - generic [ref=f8e31]: Track Picks
                    - generic [ref=f8e32]: "55"
            - button "Claim your $100 Deposit Match" [ref=f8e33] [cursor=pointer]
            - generic [ref=f8e34]:
              - generic [ref=f8e36]:
                - generic [ref=f8e37]: $208.92
                - generic [ref=f8e38]:
                  - img "gift-icon" [ref=f8e39]
                  - text: "5.00"
              - button "Toggle Menu" [ref=f8e40]
      - main [ref=f8e43]:
        - generic [ref=f8e45]:
          - generic [ref=f8e49]:
            - button "previous slide" [ref=f8e50] [cursor=pointer]
            - generic [ref=f8e54]:
              - generic [ref=f8e56]:
                - generic [ref=f8e57]:
                  - generic [ref=f8e58]: Receive a referral Bonus!
                  - generic [ref=f8e59]: $20
                - generic [ref=f8e60]:
                  - text: Refer a Friendwhen they make their first deposit
                  - button "Invite Now" [ref=f8e62] [cursor=pointer]
              - generic [ref=f8e64]:
                - generic [ref=f8e65]:
                  - text: $100
                  - img "black lightning bol" [ref=f8e66]
                - generic [ref=f8e67]: =
                - generic [ref=f8e69]:
                  - text: $200
                  - img "black lightning bol" [ref=f8e70]
                - generic [ref=f8e71]:
                  - text: We match your 1st depositWe match your first deposit up to $100.
                  - button "Deposit Now" [ref=f8e73] [cursor=pointer]
            - button "next slide" [ref=f8e74] [cursor=pointer]
          - generic [ref=f8e78]:
            - generic [ref=f8e80]:
              - textbox "Search player or team" [ref=f8e84]
              - generic [ref=f8e85]:
                - button "All" [ref=f8e86] [cursor=pointer]
                - button "MLB" [ref=f8e87] [cursor=pointer]
                - button "SerieA" [ref=f8e88] [cursor=pointer]
                - button "EPL" [ref=f8e89] [cursor=pointer]
                - button "WNBA" [ref=f8e90] [cursor=pointer]
                - button "WNBA-Combos" [ref=f8e91] [cursor=pointer]
                - button "WNBA Q1" [ref=f8e92] [cursor=pointer]
                - button "WNBA H1" [ref=f8e93] [cursor=pointer]
                - button "MLS" [ref=f8e94] [cursor=pointer]
                - button "NFLSZN" [ref=f8e95] [cursor=pointer]
                - button "LaLiga" [ref=f8e96] [cursor=pointer]
                - button "UFC" [ref=f8e97] [cursor=pointer]
                - button "Bundes" [ref=f8e98] [cursor=pointer]
              - button [ref=f8e100] [cursor=pointer]:
                - img "right chevron sign" [ref=f8e101]
                - text: Filter
            - generic [ref=f8e102]:
              - generic [ref=f8e105]:
                - generic [ref=f8e108]:
                  - generic [ref=f8e109]:
                    - img "Ian Seymour" [ref=f8e111]
                    - generic [ref=f8e112]:
                      - generic [ref=f8e113]: Ian Seymour
                      - generic [ref=f8e114]: SP - TB
                      - generic [ref=f8e115]: TB @ DET 6:40 PM
                    - button "Open expert opinion for Ian Seymour" [ref=f8e118]
                  - generic [ref=f8e123]:
                    - generic [ref=f8e124]:
                      - generic [ref=f8e125]:
                        - generic [ref=f8e126]: Less
                        - generic [ref=f8e130]: Strikeouts (K)
                        - generic [ref=f8e131]: More
                      - generic [ref=f8e135]:
                        - generic [ref=f8e136]:
                          - button "Select over 3.5 Strikeouts (K) for 0 times" [disabled] [ref=f8e137]
                          - generic [ref=f8e138]: 3.5 Strikeouts (K)
                          - button "Select over 3.5 Strikeouts (K) for 1.06 times" [ref=f8e139]: 1.06x
                        - generic [ref=f8e140]:
                          - button "Select over 4.5 Strikeouts (K) for 0 times" [disabled] [ref=f8e141]
                          - generic [ref=f8e142]: 4.5 Strikeouts (K)
                          - button "Select over 4.5 Strikeouts (K) for 1.27 times" [ref=f8e143]: 1.27x
                        - generic [ref=f8e144]:
                          - button "Select over 5.5 Strikeouts (K) for 1.86 times" [ref=f8e145]: 1.86x
                          - generic [ref=f8e146]: 5.5 Strikeouts (K)
                          - button "Select over 5.5 Strikeouts (K) for 1.78 times" [ref=f8e147]: 1.78x
                        - generic [ref=f8e148]:
                          - button "Select over 6.5 Strikeouts (K) for 0 times" [disabled] [ref=f8e149]
                          - generic [ref=f8e150]: 6.5 Strikeouts (K)
                          - button "Select over 6.5 Strikeouts (K) for 2.59 times" [ref=f8e151]: 2.59x
                        - generic [ref=f8e152]:
                          - button "Select over 7.5 Strikeouts (K) for 0 times" [disabled] [ref=f8e153]
                          - generic [ref=f8e154]: 7.5 Strikeouts (K)
                          - button "Select over 7.5 Strikeouts (K) for 3.91 times" [ref=f8e155]: 3.91x
                        - button "Show more Strikeouts (K) lines (7)" [ref=f8e156]
                    - generic [ref=f8e159]:
                      - generic [ref=f8e160]:
                        - generic [ref=f8e161]: Less
                        - generic [ref=f8e165]: Hits Allowed
                        - generic [ref=f8e166]: More
                      - generic [ref=f8e171]:
                        - button "Select over 4.5 Hits Allowed for 1.78 times" [ref=f8e172]: 1.78x
                        - generic [ref=f8e173]: 4.5 Hits Allowed
                        - button "Select over 4.5 Hits Allowed for 1.78 times" [ref=f8e174]: 1.78x
                  - button "Show More Stats" [ref=f8e176]
                - generic [ref=f8e181]:
                  - generic [ref=f8e182]:
                    - img "Junior Caminero" [ref=f8e184]
                    - generic [ref=f8e185]:
                      - generic [ref=f8e186]: J. Caminero
                      - generic [ref=f8e187]: 3B - TB
                      - generic [ref=f8e188]: TB @ DET 6:40 PM
                    - button "Open expert opinion for Junior Caminero" [ref=f8e191]
                  - generic [ref=f8e196]:
                    - generic [ref=f8e197]:
                      - generic [ref=f8e198]:
                        - generic [ref=f8e199]: Less
                        - generic [ref=f8e203]: Hits
                        - generic [ref=f8e204]: More
                      - generic [ref=f8e208]:
                        - generic [ref=f8e209]:
                          - button "Select over 0.5 Hits for 2.61 times" [active] [ref=f8e210]: 2.61x
                          - generic [ref=f8e211]: 0.5 Hits
                          - button "Select over 0.5 Hits for 1.28 times" [ref=f8e212]: 1.28x
                        - generic [ref=f8e213]:
                          - button "Select over 1.5 Hits for 0 times" [disabled] [ref=f8e214]
                          - generic [ref=f8e215]: 1.5 Hits
                          - button "Select over 1.5 Hits for 2.87 times" [ref=f8e216]: 2.87x
                        - generic [ref=f8e217]:
                          - button "Select over 2.5 Hits for 0 times" [disabled] [ref=f8e218]
                          - generic [ref=f8e219]: 2.5 Hits
                          - button "Select over 2.5 Hits for 7.79 times" [ref=f8e220]: 7.79x
                        - generic [ref=f8e221]:
                          - button "Select over 3.5 Hits for 0 times" [disabled] [ref=f8e222]
                          - generic [ref=f8e223]: 3.5 Hits
                          - button "Select over 3.5 Hits for 26.8 times" [ref=f8e224]: 26.8x
                    - generic [ref=f8e225]:
                      - generic [ref=f8e226]:
                        - generic [ref=f8e227]: Less
                        - generic [ref=f8e231]: Hits + Runs + RBIs
                        - generic [ref=f8e232]: More
                      - generic [ref=f8e236]:
                        - generic [ref=f8e237]:
                          - button "Select over 0.5 Hits + Runs + RBIs for 0 times" [disabled] [ref=f8e238]
                          - generic [ref=f8e239]: 0.5 H+R+R
                          - button "Select over 0.5 Hits + Runs + RBIs for 1.21 times" [ref=f8e240]: 1.21x
                        - generic [ref=f8e241]:
                          - button "Select over 1.5 Hits + Runs + RBIs for 1.89 times" [ref=f8e242]: 1.89x
                          - generic [ref=f8e243]: 1.5 H+R+R
                          - button "Select over 1.5 Hits + Runs + RBIs for 1.64 times" [ref=f8e244]: 1.64x
                        - generic [ref=f8e245]:
                          - button "Select over 2.5 Hits + Runs + RBIs for 0 times" [disabled] [ref=f8e246]
                          - generic [ref=f8e247]: 2.5 H+R+R
                          - button "Select over 2.5 Hits + Runs + RBIs for 2.35 times" [ref=f8e248]: 2.35x
                        - generic [ref=f8e249]:
                          - button "Select over 3.5 Hits + Runs + RBIs for 0 times" [disabled] [ref=f8e250]
                          - generic [ref=f8e251]: 3.5 H+R+R
                          - button "Select over 3.5 Hits + Runs + RBIs for 3.2 times" [ref=f8e252]: 3.2x
                        - generic [ref=f8e253]:
                          - button "Select over 4.5 Hits + Runs + RBIs for 0 times" [disabled] [ref=f8e254]
                          - generic [ref=f8e255]: 4.5 H+R+R
                          - button "Select over 4.5 Hits + Runs + RBIs for 4.52 times" [ref=f8e256]: 4.52x
                    - generic [ref=f8e257]:
                      - generic [ref=f8e258]:
                        - generic [ref=f8e259]: Less
                        - generic [ref=f8e263]: Singles
                        - generic [ref=f8e264]: More
                      - generic [ref=f8e268]:
                        - generic [ref=f8e269]:
                          - button "Select over 0.5 Singles for 1.72 times" [ref=f8e270]: 1.72x
                          - generic [ref=f8e271]: 0.5 Singles
                          - button "Select over 0.5 Singles for 1.78 times" [ref=f8e272]: 1.78x
                        - generic [ref=f8e273]:
                          - button "Select over 1.5 Singles for 0 times" [disabled] [ref=f8e274]
                          - generic [ref=f8e275]: 1.5 Singles
                          - button "Select over 1.5 Singles for 5.31 times" [ref=f8e276]: 5.31x
                    - generic [ref=f8e277]:
                      - generic [ref=f8e278]:
                        - generic [ref=f8e279]: Less
                        - generic [ref=f8e283]: Doubles
                        - generic [ref=f8e284]: More
                      - generic [ref=f8e289]:
                        - button "Select over 0.5 Doubles for 1.07 times" [ref=f8e290]: 1.07x
                        - generic [ref=f8e291]: 0.5 Doubles
                        - button "Select over 0.5 Doubles for 4.14 times" [ref=f8e292]: 4.14x
                    - generic [ref=f8e293]:
                      - generic [ref=f8e294]:
                        - generic [ref=f8e295]: Less
                        - generic [ref=f8e299]: Triples
                        - generic [ref=f8e300]: More
                      - generic [ref=f8e305]:
                        - button "Select over 0.5 Triples for 0 times" [disabled] [ref=f8e306]
                        - generic [ref=f8e307]: 0.5 Triples
                        - button "Select over 0.5 Triples for 35.5 times" [ref=f8e308]: 35.5x
                    - generic [ref=f8e309]:
                      - generic [ref=f8e310]:
                        - generic [ref=f8e311]: Less
                        - generic [ref=f8e315]: Runs
                        - generic [ref=f8e316]: More
                      - generic [ref=f8e320]:
                        - generic [ref=f8e321]:
                          - button "Select over 0.5 Runs for 1.58 times" [ref=f8e322]: 1.58x
                          - generic [ref=f8e323]: 0.5 Runs
                          - button "Select over 0.5 Runs for 1.91 times" [ref=f8e324]: 1.91x
                        - generic [ref=f8e325]:
                          - button "Select over 1.5 Runs for 0 times" [disabled] [ref=f8e326]
                          - generic [ref=f8e327]: 1.5 Runs
                          - button "Select over 1.5 Runs for 5.9 times" [ref=f8e328]: 5.9x
                    - generic [ref=f8e329]:
                      - generic [ref=f8e330]:
                        - generic [ref=f8e331]: Less
                        - generic [ref=f8e335]: RBIs
                        - generic [ref=f8e336]: More
                      - generic [ref=f8e340]:
                        - generic [ref=f8e341]:
                          - button "Select over 0.5 RBIs for 1.35 times" [ref=f8e342]: 1.35x
                          - generic [ref=f8e343]: 0.5 RBIs
                          - button "Select over 0.5 RBIs for 2.28 times" [ref=f8e344]: 2.28x
                        - generic [ref=f8e345]:
                          - button "Select over 1.5 RBIs for 0 times" [disabled] [ref=f8e346]
                          - generic [ref=f8e347]: 1.5 RBIs
                          - button "Select over 1.5 RBIs for 4.22 times" [ref=f8e348]: 4.22x
                        - generic [ref=f8e349]:
                          - button "Select over 2.5 RBIs for 0 times" [disabled] [ref=f8e350]
                          - generic [ref=f8e351]: 2.5 RBIs
                          - button "Select over 2.5 RBIs for 7.79 times" [ref=f8e352]: 7.79x
                    - generic [ref=f8e353]:
                      - generic [ref=f8e354]:
                        - generic [ref=f8e355]: Less
                        - generic [ref=f8e359]: Homeruns
                        - generic [ref=f8e360]: More
                      - generic [ref=f8e364]:
                        - generic [ref=f8e365]:
                          - button "Select over 0.5 Homeruns for 0 times" [disabled] [ref=f8e366]
                          - generic [ref=f8e367]: 0.5 Homeruns
                          - button "Select over 0.5 Homeruns for 4.06 times" [ref=f8e368]: 4.06x
                        - generic [ref=f8e369]:
                          - button "Select over 1.5 Homeruns for 0 times" [disabled] [ref=f8e370]
                          - generic [ref=f8e371]: 1.5 Homeruns
                          - button "Select over 1.5 Homeruns for 22.89 times" [ref=f8e372]: 22.89x
                    - generic [ref=f8e373]:
                      - generic [ref=f8e374]:
                        - generic [ref=f8e375]: Less
                        - generic [ref=f8e379]: Total Bases
                        - generic [ref=f8e380]: More
                      - generic [ref=f8e384]:
                        - generic [ref=f8e385]:
                          - button "Select over 1.5 Total Bases for 1.59 times" [ref=f8e386]: 1.59x
                          - generic [ref=f8e387]: 1.5 Total Bases
                          - button "Select over 1.5 Total Bases for 1.96 times" [ref=f8e388]: 1.96x
                        - generic [ref=f8e389]:
                          - button "Select over 2.5 Total Bases for 0 times" [disabled] [ref=f8e390]
                          - generic [ref=f8e391]: 2.5 Total Bases
                          - button "Select over 2.5 Total Bases for 2.76 times" [ref=f8e392]: 2.76x
                        - generic [ref=f8e393]:
                          - button "Select over 3.5 Total Bases for 0 times" [disabled] [ref=f8e394]
                          - generic [ref=f8e395]: 3.5 Total Bases
                          - button "Select over 3.5 Total Bases for 3.36 times" [ref=f8e396]: 3.36x
                        - generic [ref=f8e397]:
                          - button "Select over 4.5 Total Bases for 0 times" [disabled] [ref=f8e398]
                          - generic [ref=f8e399]: 4.5 Total Bases
                          - button "Select over 4.5 Total Bases for 5.5 times" [ref=f8e400]: 5.5x
                        - generic [ref=f8e401]:
                          - button "Select over 5.5 Total Bases for 0 times" [disabled] [ref=f8e402]
                          - generic [ref=f8e403]: 5.5 Total Bases
                          - button "Select over 5.5 Total Bases for 7.6 times" [ref=f8e404]: 7.6x
                    - generic [ref=f8e405]:
                      - generic [ref=f8e406]:
                        - generic [ref=f8e407]: Less
                        - generic [ref=f8e411]: Strikeouts
                        - generic [ref=f8e412]: More
                      - generic [ref=f8e416]:
                        - generic [ref=f8e417]:
                          - button "Select over 0.5 Strikeouts for 0 times" [disabled] [ref=f8e418]
                          - generic [ref=f8e419]: 0.5 Strikeouts
                          - button "Select over 0.5 Strikeouts for 1.28 times" [ref=f8e420]: 1.28x
                        - generic [ref=f8e421]:
                          - button "Select over 1.5 Strikeouts for 0 times" [disabled] [ref=f8e422]
                          - generic [ref=f8e423]: 1.5 Strikeouts
                          - button "Select over 1.5 Strikeouts for 2.96 times" [ref=f8e424]: 2.96x
                        - generic [ref=f8e425]:
                          - button "Select over 2.5 Strikeouts for 0 times" [disabled] [ref=f8e426]
                          - generic [ref=f8e427]: 2.5 Strikeouts
                          - button "Select over 2.5 Strikeouts for 7.84 times" [ref=f8e428]: 7.84x
                    - generic [ref=f8e429]:
                      - generic [ref=f8e430]:
                        - generic [ref=f8e431]: Less
                        - generic [ref=f8e435]: Fantasy Points
                        - generic [ref=f8e436]: More
                      - generic [ref=f8e441]:
                        - button "Select over 6.5 Fantasy Points for 1.78 times" [ref=f8e442]: 1.78x
                        - generic [ref=f8e443]: 6.5 Fantasy Points
                        - button "Select over 6.5 Fantasy Points for 1.78 times" [ref=f8e444]: 1.78x
                  - button "Show More Stats" [ref=f8e446]
                - generic [ref=f8e451]:
                  - generic [ref=f8e452]:
                    - img "Yandy Diaz" [ref=f8e454]
                    - generic [ref=f8e455]:
                      - generic [ref=f8e456]: Yandy Diaz
                      - generic [ref=f8e457]: DH - TB
                      - generic [ref=f8e458]: TB @ DET 6:40 PM
                    - button "Open expert opinion for Yandy Diaz" [ref=f8e461]
                  - generic [ref=f8e466]:
                    - generic [ref=f8e467]:
                      - generic [ref=f8e468]:
                        - generic [ref=f8e469]: Less
                        - generic [ref=f8e473]: Hits
                        - generic [ref=f8e474]: More
                      - generic [ref=f8e478]:
                        - generic [ref=f8e479]:
                          - button "Select over 0.5 Hits for 0 times" [disabled] [ref=f8e480]
                          - generic [ref=f8e481]: 0.5 Hits
                          - button "Select over 0.5 Hits for 1.25 times" [ref=f8e482]: 1.25x
                        - generic [ref=f8e483]:
                          - button "Select over 1.5 Hits for 1.28 times" [ref=f8e484]: 1.28x
                          - generic [ref=f8e485]: 1.5 Hits
                          - button "Select over 1.5 Hits for 2.65 times" [ref=f8e486]: 2.65x
                        - generic [ref=f8e487]:
                          - button "Select over 2.5 Hits for 0 times" [disabled] [ref=f8e488]
                          - generic [ref=f8e489]: 2.5 Hits
                          - button "Select over 2.5 Hits for 6.78 times" [ref=f8e490]: 6.78x
                        - generic [ref=f8e491]:
                          - button "Select over 3.5 Hits for 0 times" [disabled] [ref=f8e492]
                          - generic [ref=f8e493]: 3.5 Hits
                          - button "Select over 3.5 Hits for 23.8 times" [ref=f8e494]: 23.8x
                    - generic [ref=f8e495]:
                      - generic [ref=f8e496]:
                        - generic [ref=f8e497]: Less
                        - generic [ref=f8e501]: Hits + Runs + RBIs
                        - generic [ref=f8e502]: More
                      - generic [ref=f8e506]:
                        - generic [ref=f8e507]:
                          - button "Select over 0.5 Hits + Runs + RBIs for 0 times" [disabled] [ref=f8e508]
                          - generic [ref=f8e509]: 0.5 H+R+R
                          - button "Select over 0.5 Hits + Runs + RBIs for 1.15 times" [ref=f8e510]: 1.15x
                        - generic [ref=f8e511]:
                          - button "Select over 1.5 Hits + Runs + RBIs for 1.96 times" [ref=f8e512]: 1.96x
                          - generic [ref=f8e513]: 1.5 H+R+R
                          - button "Select over 1.5 Hits + Runs + RBIs for 1.6 times" [ref=f8e514]: 1.6x
                        - generic [ref=f8e515]:
                          - button "Select over 2.5 Hits + Runs + RBIs for 0 times" [disabled] [ref=f8e516]
                          - generic [ref=f8e517]: 2.5 H+R+R
                          - button "Select over 2.5 Hits + Runs + RBIs for 2.46 times" [ref=f8e518]: 2.46x
                        - generic [ref=f8e519]:
                          - button "Select over 3.5 Hits + Runs + RBIs for 0 times" [disabled] [ref=f8e520]
                          - generic [ref=f8e521]: 3.5 H+R+R
                          - button "Select over 3.5 Hits + Runs + RBIs for 3.65 times" [ref=f8e522]: 3.65x
                        - generic [ref=f8e523]:
                          - button "Select over 4.5 Hits + Runs + RBIs for 0 times" [disabled] [ref=f8e524]
                          - generic [ref=f8e525]: 4.5 H+R+R
                          - button "Select over 4.5 Hits + Runs + RBIs for 5.51 times" [ref=f8e526]: 5.51x
                    - generic [ref=f8e527]:
                      - generic [ref=f8e528]:
                        - generic [ref=f8e529]: Less
                        - generic [ref=f8e533]: Singles
                        - generic [ref=f8e534]: More
                      - generic [ref=f8e538]:
                        - generic [ref=f8e539]:
                          - button "Select over 0.5 Singles for 2.1 times" [ref=f8e540]: 2.1x
                          - generic [ref=f8e541]: 0.5 Singles
                          - button "Select over 0.5 Singles for 1.5 times" [ref=f8e542]: 1.5x
                        - generic [ref=f8e543]:
                          - button "Select over 1.5 Singles for 0 times" [disabled] [ref=f8e544]
                          - generic [ref=f8e545]: 1.5 Singles
                          - button "Select over 1.5 Singles for 3.93 times" [ref=f8e546]: 3.93x
                    - generic [ref=f8e547]:
                      - generic [ref=f8e548]:
                        - generic [ref=f8e549]: Less
                        - generic [ref=f8e553]: Doubles
                        - generic [ref=f8e554]: More
                      - generic [ref=f8e559]:
                        - button "Select over 0.5 Doubles for 1.07 times" [ref=f8e560]: 1.07x
                        - generic [ref=f8e561]: 0.5 Doubles
                        - button "Select over 0.5 Doubles for 4.06 times" [ref=f8e562]: 4.06x
                    - generic [ref=f8e563]:
                      - generic [ref=f8e564]:
                        - generic [ref=f8e565]: Less
                        - generic [ref=f8e569]: Triples
                        - generic [ref=f8e570]: More
                      - generic [ref=f8e575]:
                        - button "Select over 0.5 Triples for 0 times" [disabled] [ref=f8e576]
                        - generic [ref=f8e577]: 0.5 Triples
                        - button "Select over 0.5 Triples for 40.9 times" [ref=f8e578]: 40.9x
                    - generic [ref=f8e579]:
                      - generic [ref=f8e580]:
                        - generic [ref=f8e581]: Less
                        - generic [ref=f8e585]: Runs
                        - generic [ref=f8e586]: More
                      - generic [ref=f8e590]:
                        - generic [ref=f8e591]:
                          - button "Select over 0.5 Runs for 1.68 times" [ref=f8e592]: 1.68x
                          - generic [ref=f8e593]: 0.5 Runs
                          - button "Select over 0.5 Runs for 1.84 times" [ref=f8e594]: 1.84x
                        - generic [ref=f8e595]:
                          - button "Select over 1.5 Runs for 0 times" [disabled] [ref=f8e596]
                          - generic [ref=f8e597]: 1.5 Runs
                          - button "Select over 1.5 Runs for 5.28 times" [ref=f8e598]: 5.28x
                    - generic [ref=f8e599]:
                      - generic [ref=f8e600]:
                        - generic [ref=f8e601]: Less
                        - generic [ref=f8e605]: RBIs
                        - generic [ref=f8e606]: More
                      - generic [ref=f8e610]:
                        - generic [ref=f8e611]:
                          - button "Select over 0.5 RBIs for 1.23 times" [ref=f8e612]: 1.23x
                          - generic [ref=f8e613]: 0.5 RBIs
                          - button "Select over 0.5 RBIs for 2.84 times" [ref=f8e614]: 2.84x
                        - generic [ref=f8e615]:
                          - button "Select over 1.5 RBIs for 0 times" [disabled] [ref=f8e616]
                          - generic [ref=f8e617]: 1.5 RBIs
                          - button "Select over 1.5 RBIs for 6.2 times" [ref=f8e618]: 6.2x
                    - generic [ref=f8e619]:
                      - generic [ref=f8e620]:
                        - generic [ref=f8e621]: Less
                        - generic [ref=f8e625]: Homeruns
                        - generic [ref=f8e626]: More
                      - generic [ref=f8e630]:
                        - generic [ref=f8e631]:
                          - button "Select over 0.5 Homeruns for 0 times" [disabled] [ref=f8e632]
                          - generic [ref=f8e633]: 0.5 Homeruns
                          - button "Select over 0.5 Homeruns for 6.54 times" [ref=f8e634]: 6.54x
                        - generic [ref=f8e635]:
                          - button "Select over 1.5 Homeruns for 0 times" [disabled] [ref=f8e636]
                          - generic [ref=f8e637]: 1.5 Homeruns
                          - button "Select over 1.5 Homeruns for 61 times" [ref=f8e638]: 61x
                    - generic [ref=f8e639]:
                      - generic [ref=f8e640]:
                        - generic [ref=f8e641]: Less
                        - generic [ref=f8e645]: Total Bases
                        - generic [ref=f8e646]: More
                      - generic [ref=f8e650]:
                        - generic [ref=f8e651]:
                          - button "Select over 1.5 Total Bases for 1.53 times" [ref=f8e652]: 1.53x
                          - generic [ref=f8e653]: 1.5 Total Bases
                          - button "Select over 1.5 Total Bases for 2.03 times" [ref=f8e654]: 2.03x
                        - generic [ref=f8e655]:
                          - button "Select over 2.5 Total Bases for 0 times" [disabled] [ref=f8e656]
                          - generic [ref=f8e657]: 2.5 Total Bases
                          - button "Select over 2.5 Total Bases for 3.29 times" [ref=f8e658]: 3.29x
                        - generic [ref=f8e659]:
                          - button "Select over 3.5 Total Bases for 0 times" [disabled] [ref=f8e660]
                          - generic [ref=f8e661]: 3.5 Total Bases
                          - button "Select over 3.5 Total Bases for 4.8 times" [ref=f8e662]: 4.8x
                        - generic [ref=f8e663]:
                          - button "Select over 4.5 Total Bases for 0 times" [disabled] [ref=f8e664]
                          - generic [ref=f8e665]: 4.5 Total Bases
                          - button "Select over 4.5 Total Bases for 7.48 times" [ref=f8e666]: 7.48x
                    - generic [ref=f8e667]:
                      - generic [ref=f8e668]:
                        - generic [ref=f8e669]: Less
                        - generic [ref=f8e673]: Strikeouts
                        - generic [ref=f8e674]: More
                      - generic [ref=f8e678]:
                        - generic [ref=f8e679]:
                          - button "Select over 0.5 Strikeouts for 0 times" [disabled] [ref=f8e680]
                          - generic [ref=f8e681]: 0.5 Strikeouts
                          - button "Select over 0.5 Strikeouts for 1.57 times" [ref=f8e682]: 1.57x
                        - generic [ref=f8e683]:
                          - button "Select over 1.5 Strikeouts for 0 times" [disabled] [ref=f8e684]
                          - generic [ref=f8e685]: 1.5 Strikeouts
                          - button "Select over 1.5 Strikeouts for 4.34 times" [ref=f8e686]: 4.34x
                    - generic [ref=f8e687]:
                      - generic [ref=f8e688]:
                        - generic [ref=f8e689]: Less
                        - generic [ref=f8e693]: Fantasy Points
                        - generic [ref=f8e694]: More
                      - generic [ref=f8e699]:
                        - button "Select over 7.5 Fantasy Points for 1.78 times" [ref=f8e700]: 1.78x
                        - generic [ref=f8e701]: 7.5 Fantasy Points
                        - button "Select over 7.5 Fantasy Points for 1.78 times" [ref=f8e702]: 1.78x
                  - button "Show More Stats" [ref=f8e704]
                - generic [ref=f8e709]:
                  - generic [ref=f8e710]:
                    - img "Richie Palacios" [ref=f8e712]
                    - generic [ref=f8e713]:
                      - generic [ref=f8e714]: R. Palacios
                      - generic [ref=f8e715]: SS - TB
                      - generic [ref=f8e716]: TB @ DET 6:40 PM
                    - button "Open expert opinion for Richie Palacios" [ref=f8e719]
                  - generic [ref=f8e724]:
                    - generic [ref=f8e725]:
                      - generic [ref=f8e726]:
                        - generic [ref=f8e727]: Less
                        - generic [ref=f8e731]: Hits
                        - generic [ref=f8e732]: More
                      - generic [ref=f8e736]:
                        - generic [ref=f8e737]:
                          - button "Select over 0.5 Hits for 1.93 times" [ref=f8e738]: 1.93x
                          - generic [ref=f8e739]: 0.5 Hits
                          - button "Select over 0.5 Hits for 1.7 times" [ref=f8e740]: 1.7x
                        - generic [ref=f8e741]:
                          - button "Select over 1.5 Hits for 0 times" [disabled] [ref=f8e742]
                          - generic [ref=f8e743]: 1.5 Hits
                          - button "Select over 1.5 Hits for 4.48 times" [ref=f8e744]: 4.48x
                        - generic [ref=f8e745]:
                          - button "Select over 2.5 Hits for 0 times" [disabled] [ref=f8e746]
                          - generic [ref=f8e747]: 2.5 Hits
                          - button "Select over 2.5 Hits for 14.2 times" [ref=f8e748]: 14.2x
                    - generic [ref=f8e749]:
                      - generic [ref=f8e750]:
                        - generic [ref=f8e751]: Less
                        - generic [ref=f8e755]: Hits + Runs + RBIs
                        - generic [ref=f8e756]: More
                      - generic [ref=f8e760]:
                        - generic [ref=f8e761]:
                          - button "Select over 0.5 Hits + Runs + RBIs for 2.26 times" [ref=f8e762]: 2.26x
                          - generic [ref=f8e763]: 0.5 H+R+R
                          - button "Select over 0.5 Hits + Runs + RBIs for 1.46 times" [ref=f8e764]: 1.46x
                        - generic [ref=f8e765]:
                          - button "Select over 1.5 Hits + Runs + RBIs for 0 times" [disabled] [ref=f8e766]
                          - generic [ref=f8e767]: 1.5 H+R+R
                          - button "Select over 1.5 Hits + Runs + RBIs for 2.3 times" [ref=f8e768]: 2.3x
                        - generic [ref=f8e769]:
                          - button "Select over 2.5 Hits + Runs + RBIs for 0 times" [disabled] [ref=f8e770]
                          - generic [ref=f8e771]: 2.5 H+R+R
                          - button "Select over 2.5 Hits + Runs + RBIs for 3.52 times" [ref=f8e772]: 3.52x
                        - generic [ref=f8e773]:
                          - button "Select over 3.5 Hits + Runs + RBIs for 0 times" [disabled] [ref=f8e774]
                          - generic [ref=f8e775]: 3.5 H+R+R
                          - button "Select over 3.5 Hits + Runs + RBIs for 5.63 times" [ref=f8e776]: 5.63x
                        - generic [ref=f8e777]:
                          - button "Select over 4.5 Hits + Runs + RBIs for 0 times" [disabled] [ref=f8e778]
                          - generic [ref=f8e779]: 4.5 H+R+R
                          - button "Select over 4.5 Hits + Runs + RBIs for 8.2 times" [ref=f8e780]: 8.2x
                    - generic [ref=f8e781]:
                      - generic [ref=f8e782]:
                        - generic [ref=f8e783]: Less
                        - generic [ref=f8e787]: Singles
                        - generic [ref=f8e788]: More
                      - generic [ref=f8e792]:
                        - generic [ref=f8e793]:
                          - button "Select over 0.5 Singles for 1.53 times" [ref=f8e794]: 1.53x
                          - generic [ref=f8e795]: 0.5 Singles
                          - button "Select over 0.5 Singles for 2.12 times" [ref=f8e796]: 2.12x
                        - generic [ref=f8e797]:
                          - button "Select over 1.5 Singles for 0 times" [disabled] [ref=f8e798]
                          - generic [ref=f8e799]: 1.5 Singles
                          - button "Select over 1.5 Singles for 6.09 times" [ref=f8e800]: 6.09x
                    - generic [ref=f8e801]:
                      - generic [ref=f8e802]:
                        - generic [ref=f8e803]: Less
                        - generic [ref=f8e807]: Doubles
                        - generic [ref=f8e808]: More
                      - generic [ref=f8e813]:
                        - button "Select over 0.5 Doubles for 0 times" [disabled] [ref=f8e814]
                        - generic [ref=f8e815]: 0.5 Doubles
                        - button "Select over 0.5 Doubles for 5.1 times" [ref=f8e816]: 5.1x
                    - generic [ref=f8e817]:
                      - generic [ref=f8e818]:
                        - generic [ref=f8e819]: Less
                        - generic [ref=f8e823]: Triples
                        - generic [ref=f8e824]: More
                      - generic [ref=f8e829]:
                        - button "Select over 0.5 Triples for 0 times" [disabled] [ref=f8e830]
                        - generic [ref=f8e831]: 0.5 Triples
                        - button "Select over 0.5 Triples for 18.1 times" [ref=f8e832]: 18.1x
                    - generic [ref=f8e833]:
                      - generic [ref=f8e834]:
                        - generic [ref=f8e835]: Less
                        - generic [ref=f8e839]: Runs
                        - generic [ref=f8e840]: More
                      - generic [ref=f8e844]:
                        - generic [ref=f8e845]:
                          - button "Select over 0.5 Runs for 1.27 times" [ref=f8e846]: 1.27x
                          - generic [ref=f8e847]: 0.5 Runs
                          - button "Select over 0.5 Runs for 2.68 times" [ref=f8e848]: 2.68x
                        - generic [ref=f8e849]:
                          - button "Select over 1.5 Runs for 0 times" [disabled] [ref=f8e850]
                          - generic [ref=f8e851]: 1.5 Runs
                          - button "Select over 1.5 Runs for 10.59 times" [ref=f8e852]: 10.59x
                    - generic [ref=f8e853]:
                      - generic [ref=f8e854]:
                        - generic [ref=f8e855]: Less
                        - generic [ref=f8e859]: RBIs
                        - generic [ref=f8e860]: More
                      - generic [ref=f8e864]:
                        - generic [ref=f8e865]:
                          - button "Select over 0.5 RBIs for 1.13 times" [ref=f8e866]: 1.13x
                          - generic [ref=f8e867]: 0.5 RBIs
                          - button "Select over 0.5 RBIs for 3.24 times" [ref=f8e868]: 3.24x
                        - generic [ref=f8e869]:
                          - button "Select over 1.5 RBIs for 0 times" [disabled] [ref=f8e870]
                          - generic [ref=f8e871]: 1.5 RBIs
                          - button "Select over 1.5 RBIs for 7.28 times" [ref=f8e872]: 7.28x
                    - generic [ref=f8e873]:
                      - generic [ref=f8e874]:
                        - generic [ref=f8e875]: Less
                        - generic [ref=f8e879]: Homeruns
                        - generic [ref=f8e880]: More
                      - generic [ref=f8e884]:
                        - generic [ref=f8e885]:
                          - button "Select over 0.5 Homeruns for 0 times" [disabled] [ref=f8e886]
                          - generic [ref=f8e887]: 0.5 Homeruns
                          - button "Select over 0.5 Homeruns for 8.8 times" [ref=f8e888]: 8.8x
                        - generic [ref=f8e889]:
                          - button "Select over 1.5 Homeruns for 0 times" [disabled] [ref=f8e890]
                          - generic [ref=f8e891]: 1.5 Homeruns
                          - button "Select over 1.5 Homeruns for 240.98 times" [ref=f8e892]: 240.98x
                    - generic [ref=f8e893]:
                      - generic [ref=f8e894]:
                        - generic [ref=f8e895]: Less
                        - generic [ref=f8e899]: Total Bases
                        - generic [ref=f8e900]: More
                      - generic [ref=f8e904]:
                        - generic [ref=f8e905]:
                          - button "Select over 1.5 Total Bases for 0 times" [disabled] [ref=f8e906]
                          - generic [ref=f8e907]: 1.5 Total Bases
                          - button "Select over 1.5 Total Bases for 2.94 times" [ref=f8e908]: 2.94x
                        - generic [ref=f8e909]:
                          - button "Select over 2.5 Total Bases for 0 times" [disabled] [ref=f8e910]
                          - generic [ref=f8e911]: 2.5 Total Bases
                          - button "Select over 2.5 Total Bases for 5.27 times" [ref=f8e912]: 5.27x
                        - generic [ref=f8e913]:
                          - button "Select over 3.5 Total Bases for 0 times" [disabled] [ref=f8e914]
                          - generic [ref=f8e915]: 3.5 Total Bases
                          - button "Select over 3.5 Total Bases for 7.42 times" [ref=f8e916]: 7.42x
                        - generic [ref=f8e917]:
                          - button "Select over 4.5 Total Bases for 0 times" [disabled] [ref=f8e918]
                          - generic [ref=f8e919]: 4.5 Total Bases
                          - button "Select over 4.5 Total Bases for 17.18 times" [ref=f8e920]: 17.18x
                    - generic [ref=f8e921]:
                      - generic [ref=f8e922]:
                        - generic [ref=f8e923]: Less
                        - generic [ref=f8e927]: Strikeouts
                        - generic [ref=f8e928]: More
                      - generic [ref=f8e932]:
                        - generic [ref=f8e933]:
                          - button "Select over 0.5 Strikeouts for 0 times" [disabled] [ref=f8e934]
                          - generic [ref=f8e935]: 0.5 Strikeouts
                          - button "Select over 0.5 Strikeouts for 1.78 times" [ref=f8e936]: 1.78x
                        - generic [ref=f8e937]:
                          - button "Select over 1.5 Strikeouts for 0 times" [disabled] [ref=f8e938]
                          - generic [ref=f8e939]: 1.5 Strikeouts
                          - button "Select over 1.5 Strikeouts for 5.5 times" [ref=f8e940]: 5.5x
                    - generic [ref=f8e941]:
                      - generic [ref=f8e942]:
                        - generic [ref=f8e943]: Less
                        - generic [ref=f8e947]: Fantasy Points
                        - generic [ref=f8e948]: More
                      - generic [ref=f8e953]:
                        - button "Select over 3.5 Fantasy Points for 1.78 times" [ref=f8e954]: 1.78x
                        - generic [ref=f8e955]: 3.5 Fantasy Points
                        - button "Select over 3.5 Fantasy Points for 1.78 times" [ref=f8e956]: 1.78x
                  - button "Show More Stats" [ref=f8e958]
              - generic [ref=f8e2059]:
                - generic [ref=f8e2061]:
                  - generic [ref=f8e2062]: 2.86x
                  - generic [ref=f8e2063]:
                    - button "+ 5% Boost 🚀" [ref=f8e2068]
                    - generic [ref=f8e2079]: "Add 3rd Pick: 5% Boost"
                - generic [ref=f8e2082]:
                  - generic [ref=f8e2084]:
                    - generic [ref=f8e2085]:
                      - generic [ref=f8e2086]: "1"
                      - button [ref=f8e2090]
                      - generic [ref=f8e2094]: Real Betis Balompié - Natan Bernardo de Souza
                      - generic [ref=f8e2095]: Today 3:00 PM vs VAL
                      - generic [ref=f8e2096]:
                        - button "Less 0.5 Shots" [disabled] [ref=f8e2098]:
                          - generic [ref=f8e2099]: Less
                          - generic [ref=f8e2100]: "0.5"
                          - generic [ref=f8e2101]: Shots
                        - button "2.38 x More 0.5 Shots" [ref=f8e2103]:
                          - generic [ref=f8e2104]: 2.38 x
                          - generic [ref=f8e2106]: More
                          - generic [ref=f8e2107]: "0.5"
                          - generic [ref=f8e2108]: Shots
                    - img "Natan Bernardo de Souza" [ref=f8e2115]
                  - generic [ref=f8e2117]:
                    - generic [ref=f8e2118]:
                      - generic [ref=f8e2119]: "2"
                      - button [ref=f8e2123]
                      - generic [ref=f8e2127]: Valencia CF - Hugo Duro
                      - generic [ref=f8e2128]: Today 3:00 PM vs BET
                      - generic [ref=f8e2129]:
                        - button "Less 1.5 Shots" [disabled] [ref=f8e2131]:
                          - generic [ref=f8e2132]: Less
                          - generic [ref=f8e2133]: "1.5"
                          - generic [ref=f8e2134]: Shots
                        - button "1.2 x More 1.5 Shots" [ref=f8e2136]:
                          - generic [ref=f8e2137]: 1.2 x
                          - generic [ref=f8e2139]: More
                          - generic [ref=f8e2140]: "1.5"
                          - generic [ref=f8e2141]: Shots
                    - img "Hugo Duro" [ref=f8e2148]
                  - generic [ref=f8e2149]:
                    - generic [ref=f8e2150]:
                      - generic [ref=f8e2152]:
                        - radio "$25"
                        - generic [ref=f8e2153] [cursor=pointer]: $25
                        - radio "$75"
                        - generic [ref=f8e2154] [cursor=pointer]: $75
                        - radio "$300" [disabled]
                        - generic: $300
                      - generic [ref=f8e2156]:
                        - generic [ref=f8e2157]: $
                        - spinbutton [ref=f8e2161]: "3"
                      - button "5" [ref=f8e2162] [cursor=pointer]
                    - generic [ref=f8e2166]:
                      - generic [ref=f8e2167]:
                        - generic [ref=f8e2168]:
                          - button "Insured" [ref=f8e2169]
                          - button "All In" [ref=f8e2170]
                        - generic [ref=f8e2171]: 2.86x
                      - generic [ref=f8e2174]:
                        - generic [ref=f8e2175]:
                          - paragraph [ref=f8e2176]: Perfect line-up
                          - paragraph [ref=f8e2177]: $8.58
                        - generic [ref=f8e2179]:
                          - paragraph [ref=f8e2180]: Or 1st place in group
                          - generic [ref=f8e2181]: $1 + $8.58
                    - button "Place" [ref=f8e2185] [cursor=pointer]
          - generic [ref=f8e2190]:
            - generic [ref=f8e2191]:
              - link [ref=f8e2192] [cursor=pointer]:
                - /url: /
                - img "Parlay Play Logo" [ref=f8e2194]
              - generic [ref=f8e2195]:
                - generic [ref=f8e2196]: Improve your experience. Download our app.
                - generic [ref=f8e2197]:
                  - link [ref=f8e2198] [cursor=pointer]:
                    - /url: https://parlayplay.onelink.me/oLJk/gnqpwjha
                    - img "Apple Store" [ref=f8e2199]
                  - link [ref=f8e2200] [cursor=pointer]:
                    - /url: https://parlayplay.onelink.me/oLJk/fh7u6juo
                    - img "Google Play Store" [ref=f8e2201]
            - generic [ref=f8e2202]:
              - link "Privacy" [ref=f8e2203] [cursor=pointer]:
                - /url: /privacy-policy
              - link "Fantasy Terms" [ref=f8e2204] [cursor=pointer]:
                - /url: /terms
              - link "Packs Terms" [ref=f8e2205] [cursor=pointer]:
                - /url: /terms/packs
              - link "Responsible Gaming" [ref=f8e2206] [cursor=pointer]:
                - /url: /responsible-gaming
              - link "Gaming Rules" [ref=f8e2207] [cursor=pointer]:
                - /url: /rules
              - link "FAQ" [ref=f8e2208] [cursor=pointer]:
                - /url: https://intercom.help/parlayplay/en/
              - link "Contact Us" [ref=f8e2209] [cursor=pointer]:
                - /url: /
              - paragraph [ref=f8e2210]: © ParlayPlay 2026 - All Rights Reserved
            - list [ref=f8e2211]:
              - listitem [ref=f8e2212]:
                - generic [ref=f8e2213]:
                  - log [ref=f8e2215]
                  - generic [ref=f8e2217]:
                    - generic [ref=f8e2218]: 🇺🇸English
                    - combobox "Select language" [ref=f8e2219]
              - listitem [ref=f8e2225]:
                - img "18+-icon" [ref=f8e2226]
              - listitem [ref=f8e2227]:
                - link "ParlayPlay on Twitter" [ref=f8e2228] [cursor=pointer]:
                  - /url: https://twitter.com/parlay_play?lang=en
              - listitem [ref=f8e2231]:
                - link "ParlayPlay on Facebook" [ref=f8e2232] [cursor=pointer]:
                  - /url: https://www.facebook.com/ParlayPlay.io/
              - listitem [ref=f8e2235]:
                - link "ParlayPlay on Instagram" [ref=f8e2236] [cursor=pointer]:
                  - /url: https://www.instagram.com/parlayplay_?igsh=bHBldWQyMmV2b3Y4
              - listitem [ref=f8e2239]:
                - link "ParlayPlay on Discord" [ref=f8e2240] [cursor=pointer]:
                  - /url: https://discord.com/invite/parlayplay
            - link [ref=f8e2244] [cursor=pointer]:
              - /url: https://sportsdata.io/
              - img "Powered by SportsDataIO" [ref=f8e2245]
    - generic:
      - region "Notifications Alt+T"
  - alert [ref=f8e2246]
  - iframe [ref=f8e2247]:
    
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
      |       ^ Error: Could not place contest after 5 attempts (last error: Unable to find replacement pick when Continue is disabled (target: 3)) — every attempted stat tab ran out of selectable cards; the environment's offering is likely too thin for this pick count
  185 | 
  186 |     return { pickIds };
  187 | }
  188 | 
```