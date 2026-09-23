# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: navigation/shell.spec.ts >> Shell - system pages >> ?coupon and ?btag are stored as the referral cookies
- Location: tests/navigation/shell.spec.ts:80:3

# Error details

```
Error: ParlayPlayReferralCode is written from ?coupon

expect(received).toBe(expected) // Object.is equality

Expected: "E2ECOUPON"
Received: undefined

Call Log:
- Timeout 15000ms exceeded while waiting on the predicate
```

# Page snapshot

```yaml
- generic [active] [ref=e1]:
  - generic [ref=e2]:
    - generic [ref=e3]:
      - banner [ref=e4]:
        - navigation [ref=e5]:
          - link "Parlay Play Logo" [ref=e6] [cursor=pointer]:
            - /url: /
            - img "Parlay Play Logo" [ref=e8]
          - generic [ref=e9]:
            - list [ref=e10]:
              - listitem [ref=e11]:
                - link "Home" [ref=e12] [cursor=pointer]:
                  - /url: /
                  - generic [ref=e14]: Home
              - listitem [ref=e15]:
                - button "Free2Play" [ref=e16] [cursor=pointer]
              - listitem [ref=e17]:
                - button "Feed" [ref=e18] [cursor=pointer]
              - listitem [ref=e19]:
                - button "Rewards" [ref=e20] [cursor=pointer]
              - listitem [ref=e21]:
                - button "Track Picks" [ref=e22] [cursor=pointer]
            - button "Join Now" [ref=e23] [cursor=pointer]
            - button "Login" [ref=e24] [cursor=pointer]
      - main [ref=e25]:
        - generic [ref=e27]:
          - generic [ref=e31]:
            - button "previous slide" [ref=e32] [cursor=pointer]:
              - img [ref=e33]
            - generic [ref=e36]:
              - generic [ref=e38]:
                - img "white lightning bol" [ref=e39]
                - generic [ref=e40]: Join Now!
                - generic [ref=e41]:
                  - text: $5
                  - generic [ref=e42]: Free Entry
                - img "treasureBox" [ref=e43]
                - generic [ref=e44]:
                  - text: Join Now and receive a $5 Free Entry. No deposit required!
                  - button "Join Now!" [ref=e46] [cursor=pointer]
              - generic [ref=e48]:
                - generic [ref=e49]:
                  - text: $100
                  - img "black lightning bol" [ref=e50]
                - generic [ref=e52]: =
                - generic [ref=e53]:
                  - text: $200
                  - img "black lightning bol" [ref=e54]
                - generic [ref=e55]:
                  - text: We match your 1st deposit
                  - text: We match your first deposit up to $100.
                  - button "Deposit Now" [ref=e57] [cursor=pointer]
            - button "next slide" [ref=e58] [cursor=pointer]:
              - img [ref=e59]
          - generic [ref=e62]:
            - generic [ref=e64]:
              - generic [ref=e67]:
                - generic:
                  - img
                - textbox "Search player or team" [ref=e68]
              - generic [ref=e69]:
                - button "All" [ref=e70] [cursor=pointer]
                - button "MLB" [ref=e71] [cursor=pointer]
                - button "NHL" [ref=e72] [cursor=pointer]
                - button "CSGO" [ref=e73] [cursor=pointer]
                - button "WNBA" [ref=e74] [cursor=pointer]
                - button "WNBA H1" [ref=e75] [cursor=pointer]
                - button "WNBA Q1" [ref=e76] [cursor=pointer]
                - button "MLS" [ref=e77] [cursor=pointer]
                - button "UFC" [ref=e78] [cursor=pointer]
              - button "right chevron sign Filter" [ref=e80] [cursor=pointer]:
                - img "right chevron sign" [ref=e81]
                - text: Filter
            - generic [ref=e82]:
              - generic [ref=e85]:
                - generic [ref=e88]:
                  - generic [ref=e89]:
                    - img "James Wood" [ref=e91]
                    - generic [ref=e92]:
                      - generic [ref=e93]: James Wood
                      - generic [ref=e94]: OF - WSH
                      - generic [ref=e97]: WSH @ DET 1:10 PM
                    - button "Open expert opinion for James Wood" [ref=e98]:
                      - img [ref=e99]
                  - generic [ref=e103]:
                    - generic [ref=e104]:
                      - generic [ref=e105]:
                        - generic [ref=e107] [cursor=pointer]:
                          - text: Less
                          - img [ref=e108]
                        - generic [ref=e110]: Hits
                        - generic [ref=e112] [cursor=pointer]:
                          - text: More
                          - img [ref=e113]
                      - generic [ref=e115]:
                        - generic [ref=e116]:
                          - button "Select over 0.5 Hits for 2.29 times" [ref=e117]: 2.29x
                          - generic [ref=e118]: 0.5 Hits
                          - button "Select over 0.5 Hits for 1.46 times" [ref=e119]: 1.46x
                        - generic [ref=e120]:
                          - button "Select over 1.5 Hits for 0 times" [disabled] [ref=e121]
                          - generic [ref=e122]: 1.5 Hits
                          - button "Select over 1.5 Hits for 3.39 times" [ref=e123]: 3.39x
                        - generic [ref=e124]:
                          - button "Select over 2.5 Hits for 0 times" [disabled] [ref=e125]
                          - generic [ref=e126]: 2.5 Hits
                          - button "Select over 2.5 Hits for 9.04 times" [ref=e127]: 9.04x
                    - generic [ref=e128]:
                      - generic [ref=e129]:
                        - generic [ref=e131] [cursor=pointer]:
                          - text: Less
                          - img [ref=e132]
                        - generic [ref=e134]: Hits + Runs + RBIs
                        - generic [ref=e136] [cursor=pointer]:
                          - text: More
                          - img [ref=e137]
                      - generic [ref=e139]:
                        - generic [ref=e140]:
                          - button "Select over 0.5 Hits + Runs + RBIs for 0 times" [disabled] [ref=e141]
                          - generic [ref=e142]: 0.5 H+R+R
                          - button "Select over 0.5 Hits + Runs + RBIs for 1.28 times" [ref=e143]: 1.28x
                        - generic [ref=e144]:
                          - button "Select over 1.5 Hits + Runs + RBIs for 1.68 times" [ref=e145]: 1.68x
                          - generic [ref=e146]: 1.5 H+R+R
                          - button "Select over 1.5 Hits + Runs + RBIs for 1.94 times" [ref=e147]: 1.94x
                        - generic [ref=e148]:
                          - button "Select over 2.5 Hits + Runs + RBIs for 0 times" [disabled] [ref=e149]
                          - generic [ref=e150]: 2.5 H+R+R
                          - button "Select over 2.5 Hits + Runs + RBIs for 2.71 times" [ref=e151]: 2.71x
                        - generic [ref=e152]:
                          - button "Select over 3.5 Hits + Runs + RBIs for 0 times" [disabled] [ref=e153]
                          - generic [ref=e154]: 3.5 H+R+R
                          - button "Select over 3.5 Hits + Runs + RBIs for 4.28 times" [ref=e155]: 4.28x
                        - generic [ref=e156]:
                          - button "Select over 4.5 Hits + Runs + RBIs for 0 times" [disabled] [ref=e157]
                          - generic [ref=e158]: 4.5 H+R+R
                          - button "Select over 4.5 Hits + Runs + RBIs for 6.24 times" [ref=e159]: 6.24x
                    - generic [ref=e160]:
                      - generic [ref=e161]:
                        - generic [ref=e163] [cursor=pointer]:
                          - text: Less
                          - img [ref=e164]
                        - generic [ref=e166]: Singles
                        - generic [ref=e168] [cursor=pointer]:
                          - text: More
                          - img [ref=e169]
                      - generic [ref=e171]:
                        - generic [ref=e172]:
                          - button "Select over 0.5 Singles for 1.65 times" [ref=e173]: 1.65x
                          - generic [ref=e174]: 0.5 Singles
                          - button "Select over 0.5 Singles for 1.94 times" [ref=e175]: 1.94x
                        - generic [ref=e176]:
                          - button "Select over 1.5 Singles for 0 times" [disabled] [ref=e177]
                          - generic [ref=e178]: 1.5 Singles
                          - button "Select over 1.5 Singles for 5.94 times" [ref=e179]: 5.94x
                    - generic [ref=e180]:
                      - generic [ref=e181]:
                        - generic [ref=e183] [cursor=pointer]:
                          - text: Less
                          - img [ref=e184]
                        - generic [ref=e186]: Doubles
                        - generic [ref=e188] [cursor=pointer]:
                          - text: More
                          - img [ref=e189]
                      - generic [ref=e192]:
                        - button "Select over 0.5 Doubles for 1.07 times" [ref=e193]: 1.07x
                        - generic [ref=e194]: 0.5 Doubles
                        - button "Select over 0.5 Doubles for 4.07 times" [ref=e195]: 4.07x
                    - generic [ref=e196]:
                      - generic [ref=e197]:
                        - generic [ref=e199] [cursor=pointer]:
                          - text: Less
                          - img [ref=e200]
                        - generic [ref=e202]: Triples
                        - generic [ref=e204] [cursor=pointer]:
                          - text: More
                          - img [ref=e205]
                      - generic [ref=e208]:
                        - button "Select over 0.5 Triples for 0 times" [disabled] [ref=e209]
                        - generic [ref=e210]: 0.5 Triples
                        - button "Select over 0.5 Triples for 18.4 times" [ref=e211]: 18.4x
                    - generic [ref=e212]:
                      - generic [ref=e213]:
                        - generic [ref=e215] [cursor=pointer]:
                          - text: Less
                          - img [ref=e216]
                        - generic [ref=e218]: Runs
                        - generic [ref=e220] [cursor=pointer]:
                          - text: More
                          - img [ref=e221]
                      - generic [ref=e223]:
                        - generic [ref=e224]:
                          - button "Select over 0.5 Runs for 1.5 times" [ref=e225]: 1.5x
                          - generic [ref=e226]: 0.5 Runs
                          - button "Select over 0.5 Runs for 2.15 times" [ref=e227]: 2.15x
                        - generic [ref=e228]:
                          - button "Select over 1.5 Runs for 0 times" [disabled] [ref=e229]
                          - generic [ref=e230]: 1.5 Runs
                          - button "Select over 1.5 Runs for 6.03 times" [ref=e231]: 6.03x
                    - generic [ref=e232]:
                      - generic [ref=e233]:
                        - generic [ref=e235] [cursor=pointer]:
                          - text: Less
                          - img [ref=e236]
                        - generic [ref=e238]: RBIs
                        - generic [ref=e240] [cursor=pointer]:
                          - text: More
                          - img [ref=e241]
                      - generic [ref=e243]:
                        - generic [ref=e244]:
                          - button "Select over 0.5 RBIs for 1.22 times" [ref=e245]: 1.22x
                          - generic [ref=e246]: 0.5 RBIs
                          - button "Select over 0.5 RBIs for 2.91 times" [ref=e247]: 2.91x
                        - generic [ref=e248]:
                          - button "Select over 1.5 RBIs for 0 times" [disabled] [ref=e249]
                          - generic [ref=e250]: 1.5 RBIs
                          - button "Select over 1.5 RBIs for 6.09 times" [ref=e251]: 6.09x
                    - generic [ref=e252]:
                      - generic [ref=e253]:
                        - generic [ref=e255] [cursor=pointer]:
                          - text: Less
                          - img [ref=e256]
                        - generic [ref=e258]: Homeruns
                        - generic [ref=e260] [cursor=pointer]:
                          - text: More
                          - img [ref=e261]
                      - generic [ref=e263]:
                        - generic [ref=e264]:
                          - button "Select over 0.5 Homeruns for 0 times" [disabled] [ref=e265]
                          - generic [ref=e266]: 0.5 Homeruns
                          - button "Select over 0.5 Homeruns for 5.36 times" [ref=e267]: 5.36x
                        - generic [ref=e268]:
                          - button "Select over 1.5 Homeruns for 0 times" [disabled] [ref=e269]
                          - generic [ref=e270]: 1.5 Homeruns
                          - button "Select over 1.5 Homeruns for 37 times" [ref=e271]: 37x
                    - generic [ref=e272]:
                      - generic [ref=e273]:
                        - generic [ref=e275] [cursor=pointer]:
                          - text: Less
                          - img [ref=e276]
                        - generic [ref=e278]: Total Bases
                        - generic [ref=e280] [cursor=pointer]:
                          - text: More
                          - img [ref=e281]
                      - generic [ref=e283]:
                        - generic [ref=e284]:
                          - button "Select over 1.5 Total Bases for 0 times" [disabled] [ref=e285]
                          - generic [ref=e286]: 1.5 Total Bases
                          - button "Select over 1.5 Total Bases for 2.36 times" [ref=e287]: 2.36x
                        - generic [ref=e288]:
                          - button "Select over 2.5 Total Bases for 0 times" [disabled] [ref=e289]
                          - generic [ref=e290]: 2.5 Total Bases
                          - button "Select over 2.5 Total Bases for 3.46 times" [ref=e291]: 3.46x
                        - generic [ref=e292]:
                          - button "Select over 3.5 Total Bases for 0 times" [disabled] [ref=e293]
                          - generic [ref=e294]: 3.5 Total Bases
                          - button "Select over 3.5 Total Bases for 4.29 times" [ref=e295]: 4.29x
                        - generic [ref=e296]:
                          - button "Select over 4.5 Total Bases for 0 times" [disabled] [ref=e297]
                          - generic [ref=e298]: 4.5 Total Bases
                          - button "Select over 4.5 Total Bases for 6.84 times" [ref=e299]: 6.84x
                    - generic [ref=e300]:
                      - generic [ref=e301]:
                        - generic [ref=e303] [cursor=pointer]:
                          - text: Less
                          - img [ref=e304]
                        - generic [ref=e306]: Strikeouts
                        - generic [ref=e308] [cursor=pointer]:
                          - text: More
                          - img [ref=e309]
                      - generic [ref=e311]:
                        - generic [ref=e312]:
                          - button "Select over 0.5 Strikeouts for 0 times" [disabled] [ref=e313]
                          - generic [ref=e314]: 0.5 Strikeouts
                          - button "Select over 0.5 Strikeouts for 1.08 times" [ref=e315]: 1.08x
                        - generic [ref=e316]:
                          - button "Select over 1.5 Strikeouts for 0 times" [disabled] [ref=e317]
                          - generic [ref=e318]: 1.5 Strikeouts
                          - button "Select over 1.5 Strikeouts for 2.07 times" [ref=e319]: 2.07x
                        - generic [ref=e320]:
                          - button "Select over 2.5 Strikeouts for 0 times" [disabled] [ref=e321]
                          - generic [ref=e322]: 2.5 Strikeouts
                          - button "Select over 2.5 Strikeouts for 5.09 times" [ref=e323]: 5.09x
                    - generic [ref=e324]:
                      - generic [ref=e325]:
                        - generic [ref=e327] [cursor=pointer]:
                          - text: Less
                          - img [ref=e328]
                        - generic [ref=e330]: Fantasy Points
                        - generic [ref=e332] [cursor=pointer]:
                          - text: More
                          - img [ref=e333]
                      - generic [ref=e336]:
                        - button "Select over 6.5 Fantasy Points for 1.78 times" [ref=e337]: 1.78x
                        - generic [ref=e338]: 6.5 Fantasy Points
                        - button "Select over 6.5 Fantasy Points for 1.78 times" [ref=e339]: 1.78x
                  - button "Show More Stats" [ref=e341]:
                    - img [ref=e342]
                - generic [ref=e346]:
                  - generic [ref=e347]:
                    - img "Andres Chaparro" [ref=e349]
                    - generic [ref=e350]:
                      - generic [ref=e351]: A. Chaparro
                      - generic [ref=e352]: 3B - WSH
                      - generic [ref=e355]: WSH @ DET 1:10 PM
                    - button "Open expert opinion for Andres Chaparro" [ref=e356]:
                      - img [ref=e357]
                  - generic [ref=e361]:
                    - generic [ref=e362]:
                      - generic [ref=e363]:
                        - generic [ref=e365] [cursor=pointer]:
                          - text: Less
                          - img [ref=e366]
                        - generic [ref=e368]: Hits
                        - generic [ref=e370] [cursor=pointer]:
                          - text: More
                          - img [ref=e371]
                      - generic [ref=e373]:
                        - generic [ref=e374]:
                          - button "Select over 0.5 Hits for 2.04 times" [ref=e375]: 2.04x
                          - generic [ref=e376]: 0.5 Hits
                          - button "Select over 0.5 Hits for 1.57 times" [ref=e377]: 1.57x
                        - generic [ref=e378]:
                          - button "Select over 1.5 Hits for 0 times" [disabled] [ref=e379]
                          - generic [ref=e380]: 1.5 Hits
                          - button "Select over 1.5 Hits for 4.11 times" [ref=e381]: 4.11x
                        - generic [ref=e382]:
                          - button "Select over 2.5 Hits for 0 times" [disabled] [ref=e383]
                          - generic [ref=e384]: 2.5 Hits
                          - button "Select over 2.5 Hits for 11.92 times" [ref=e385]: 11.92x
                    - generic [ref=e386]:
                      - generic [ref=e387]:
                        - generic [ref=e389] [cursor=pointer]:
                          - text: Less
                          - img [ref=e390]
                        - generic [ref=e392]: Hits + Runs + RBIs
                        - generic [ref=e394] [cursor=pointer]:
                          - text: More
                          - img [ref=e395]
                      - generic [ref=e397]:
                        - generic [ref=e398]:
                          - button "Select over 0.5 Hits + Runs + RBIs for 0 times" [disabled] [ref=e399]
                          - generic [ref=e400]: 0.5 H+R+R
                          - button "Select over 0.5 Hits + Runs + RBIs for 1.35 times" [ref=e401]: 1.35x
                        - generic [ref=e402]:
                          - button "Select over 1.5 Hits + Runs + RBIs for 1.5 times" [ref=e403]: 1.5x
                          - generic [ref=e404]: 1.5 H+R+R
                          - button "Select over 1.5 Hits + Runs + RBIs for 2.18 times" [ref=e405]: 2.18x
                        - generic [ref=e406]:
                          - button "Select over 2.5 Hits + Runs + RBIs for 0 times" [disabled] [ref=e407]
                          - generic [ref=e408]: 2.5 H+R+R
                          - button "Select over 2.5 Hits + Runs + RBIs for 3.19 times" [ref=e409]: 3.19x
                        - generic [ref=e410]:
                          - button "Select over 3.5 Hits + Runs + RBIs for 0 times" [disabled] [ref=e411]
                          - generic [ref=e412]: 3.5 H+R+R
                          - button "Select over 3.5 Hits + Runs + RBIs for 4.74 times" [ref=e413]: 4.74x
                        - generic [ref=e414]:
                          - button "Select over 4.5 Hits + Runs + RBIs for 0 times" [disabled] [ref=e415]
                          - generic [ref=e416]: 4.5 H+R+R
                          - button "Select over 4.5 Hits + Runs + RBIs for 7.18 times" [ref=e417]: 7.18x
                    - generic [ref=e418]:
                      - generic [ref=e419]:
                        - generic [ref=e421] [cursor=pointer]:
                          - text: Less
                          - img [ref=e422]
                        - generic [ref=e424]: Singles
                        - generic [ref=e426] [cursor=pointer]:
                          - text: More
                          - img [ref=e427]
                      - generic [ref=e429]:
                        - generic [ref=e430]:
                          - button "Select over 0.5 Singles for 1.52 times" [ref=e431]: 1.52x
                          - generic [ref=e432]: 0.5 Singles
                          - button "Select over 0.5 Singles for 2.09 times" [ref=e433]: 2.09x
                        - generic [ref=e434]:
                          - button "Select over 1.5 Singles for 0 times" [disabled] [ref=e435]
                          - generic [ref=e436]: 1.5 Singles
                          - button "Select over 1.5 Singles for 6.16 times" [ref=e437]: 6.16x
                    - generic [ref=e438]:
                      - generic [ref=e439]:
                        - generic [ref=e441] [cursor=pointer]:
                          - text: Less
                          - img [ref=e442]
                        - generic [ref=e444]: Doubles
                        - generic [ref=e446] [cursor=pointer]:
                          - text: More
                          - img [ref=e447]
                      - generic [ref=e450]:
                        - button "Select over 0.5 Doubles for 0 times" [disabled] [ref=e451]
                        - generic [ref=e452]: 0.5 Doubles
                        - button "Select over 0.5 Doubles for 4.67 times" [ref=e453]: 4.67x
                    - generic [ref=e454]:
                      - generic [ref=e455]:
                        - generic [ref=e457] [cursor=pointer]:
                          - text: Less
                          - img [ref=e458]
                        - generic [ref=e460]: Triples
                        - generic [ref=e462] [cursor=pointer]:
                          - text: More
                          - img [ref=e463]
                      - generic [ref=e466]:
                        - button "Select over 0.5 Triples for 0 times" [disabled] [ref=e467]
                        - generic [ref=e468]: 0.5 Triples
                        - button "Select over 0.5 Triples for 24.4 times" [ref=e469]: 24.4x
                    - generic [ref=e470]:
                      - generic [ref=e471]:
                        - generic [ref=e473] [cursor=pointer]:
                          - text: Less
                          - img [ref=e474]
                        - generic [ref=e476]: Runs
                        - generic [ref=e478] [cursor=pointer]:
                          - text: More
                          - img [ref=e479]
                      - generic [ref=e481]:
                        - generic [ref=e482]:
                          - button "Select over 0.5 Runs for 1.3 times" [ref=e483]: 1.3x
                          - generic [ref=e484]: 0.5 Runs
                          - button "Select over 0.5 Runs for 2.54 times" [ref=e485]: 2.54x
                        - generic [ref=e486]:
                          - button "Select over 1.5 Runs for 0 times" [disabled] [ref=e487]
                          - generic [ref=e488]: 1.5 Runs
                          - button "Select over 1.5 Runs for 7.84 times" [ref=e489]: 7.84x
                    - generic [ref=e490]:
                      - generic [ref=e491]:
                        - generic [ref=e493] [cursor=pointer]:
                          - text: Less
                          - img [ref=e494]
                        - generic [ref=e496]: RBIs
                        - generic [ref=e498] [cursor=pointer]:
                          - text: More
                          - img [ref=e499]
                      - generic [ref=e501]:
                        - generic [ref=e502]:
                          - button "Select over 0.5 RBIs for 1.2 times" [ref=e503]: 1.2x
                          - generic [ref=e504]: 0.5 RBIs
                          - button "Select over 0.5 RBIs for 3.05 times" [ref=e505]: 3.05x
                        - generic [ref=e506]:
                          - button "Select over 1.5 RBIs for 0 times" [disabled] [ref=e507]
                          - generic [ref=e508]: 1.5 RBIs
                          - button "Select over 1.5 RBIs for 6.09 times" [ref=e509]: 6.09x
                    - generic [ref=e510]:
                      - generic [ref=e511]:
                        - generic [ref=e513] [cursor=pointer]:
                          - text: Less
                          - img [ref=e514]
                        - generic [ref=e516]: Homeruns
                        - generic [ref=e518] [cursor=pointer]:
                          - text: More
                          - img [ref=e519]
                      - generic [ref=e521]:
                        - generic [ref=e522]:
                          - button "Select over 0.5 Homeruns for 0 times" [disabled] [ref=e523]
                          - generic [ref=e524]: 0.5 Homeruns
                          - button "Select over 0.5 Homeruns for 6.01 times" [ref=e525]: 6.01x
                        - generic [ref=e526]:
                          - button "Select over 1.5 Homeruns for 0 times" [disabled] [ref=e527]
                          - generic [ref=e528]: 1.5 Homeruns
                          - button "Select over 1.5 Homeruns for 45.4 times" [ref=e529]: 45.4x
                    - generic [ref=e530]:
                      - generic [ref=e531]:
                        - generic [ref=e533] [cursor=pointer]:
                          - text: Less
                          - img [ref=e534]
                        - generic [ref=e536]: Total Bases
                        - generic [ref=e538] [cursor=pointer]:
                          - text: More
                          - img [ref=e539]
                      - generic [ref=e541]:
                        - generic [ref=e542]:
                          - button "Select over 1.5 Total Bases for 0 times" [disabled] [ref=e543]
                          - generic [ref=e544]: 1.5 Total Bases
                          - button "Select over 1.5 Total Bases for 2.72 times" [ref=e545]: 2.72x
                        - generic [ref=e546]:
                          - button "Select over 2.5 Total Bases for 0 times" [disabled] [ref=e547]
                          - generic [ref=e548]: 2.5 Total Bases
                          - button "Select over 2.5 Total Bases for 4.15 times" [ref=e549]: 4.15x
                        - generic [ref=e550]:
                          - button "Select over 3.5 Total Bases for 0 times" [disabled] [ref=e551]
                          - generic [ref=e552]: 3.5 Total Bases
                          - button "Select over 3.5 Total Bases for 4.99 times" [ref=e553]: 4.99x
                        - generic [ref=e554]:
                          - button "Select over 4.5 Total Bases for 0 times" [disabled] [ref=e555]
                          - generic [ref=e556]: 4.5 Total Bases
                          - button "Select over 4.5 Total Bases for 7.72 times" [ref=e557]: 7.72x
                    - generic [ref=e558]:
                      - generic [ref=e559]:
                        - generic [ref=e561] [cursor=pointer]:
                          - text: Less
                          - img [ref=e562]
                        - generic [ref=e564]: Strikeouts
                        - generic [ref=e566] [cursor=pointer]:
                          - text: More
                          - img [ref=e567]
                      - generic [ref=e569]:
                        - generic [ref=e570]:
                          - button "Select over 0.5 Strikeouts for 0 times" [disabled] [ref=e571]
                          - generic [ref=e572]: 0.5 Strikeouts
                          - button "Select over 0.5 Strikeouts for 1.32 times" [ref=e573]: 1.32x
                        - generic [ref=e574]:
                          - button "Select over 1.5 Strikeouts for 0 times" [disabled] [ref=e575]
                          - generic [ref=e576]: 1.5 Strikeouts
                          - button "Select over 1.5 Strikeouts for 3.22 times" [ref=e577]: 3.22x
                    - generic [ref=e578]:
                      - generic [ref=e579]:
                        - generic [ref=e581] [cursor=pointer]:
                          - text: Less
                          - img [ref=e582]
                        - generic [ref=e584]: Fantasy Points
                        - generic [ref=e586] [cursor=pointer]:
                          - text: More
                          - img [ref=e587]
                      - generic [ref=e590]:
                        - button "Select over 4.5 Fantasy Points for 1.78 times" [ref=e591]: 1.78x
                        - generic [ref=e592]: 4.5 Fantasy Points
                        - button "Select over 4.5 Fantasy Points for 1.78 times" [ref=e593]: 1.78x
                  - button "Show More Stats" [ref=e595]:
                    - img [ref=e596]
              - generic [ref=e1831]:
                - generic [ref=e1834]: Please select your 1st pick
                - generic [ref=e1837]:
                  - img "arrow" [ref=e1838]
                  - heading "Let's Start!" [level=2] [ref=e1839]
                  - generic [ref=e1840]:
                    - text: Pick at least two players
                    - text: from different teams to play
          - generic [ref=e1843]:
            - generic [ref=e1844]:
              - link "Parlay Play Logo" [ref=e1845] [cursor=pointer]:
                - /url: /
                - img "Parlay Play Logo" [ref=e1847]
              - generic [ref=e1848]:
                - generic [ref=e1849]: Improve your experience. Download our app.
                - generic [ref=e1850]:
                  - link "Apple Store" [ref=e1851] [cursor=pointer]:
                    - /url: https://parlayplay.onelink.me/oLJk/gnqpwjha
                    - img "Apple Store" [ref=e1852]
                  - link "Google Play Store" [ref=e1853] [cursor=pointer]:
                    - /url: https://parlayplay.onelink.me/oLJk/fh7u6juo
                    - img "Google Play Store" [ref=e1854]
            - generic [ref=e1855]:
              - link "Privacy" [ref=e1856] [cursor=pointer]:
                - /url: /privacy-policy
              - link "Fantasy Terms" [ref=e1857] [cursor=pointer]:
                - /url: /terms
              - link "Packs Terms" [ref=e1858] [cursor=pointer]:
                - /url: /terms/packs
              - link "Responsible Gaming" [ref=e1859] [cursor=pointer]:
                - /url: /responsible-gaming
              - link "Gaming Rules" [ref=e1860] [cursor=pointer]:
                - /url: /rules
              - link "FAQ" [ref=e1861] [cursor=pointer]:
                - /url: https://intercom.help/parlayplay/en/
              - link "Contact Us" [ref=e1862] [cursor=pointer]:
                - /url: /
              - paragraph [ref=e1863]: © ParlayPlay 2026 - All Rights Reserved
            - list [ref=e1864]:
              - listitem [ref=e1865]:
                - generic [ref=e1866]:
                  - log [ref=e1868]
                  - generic [ref=e1869]:
                    - generic [ref=e1870]:
                      - generic [ref=e1871]: 🇺🇸English
                      - combobox "Select language" [ref=e1872]
                    - img [ref=e1876]
              - listitem [ref=e1878]:
                - img "18+-icon" [ref=e1879]
              - listitem [ref=e1880]:
                - link "ParlayPlay on Twitter" [ref=e1881] [cursor=pointer]:
                  - /url: https://twitter.com/parlay_play?lang=en
                  - img [ref=e1882]
              - listitem [ref=e1884]:
                - link "ParlayPlay on Facebook" [ref=e1885] [cursor=pointer]:
                  - /url: https://www.facebook.com/ParlayPlay.io/
                  - img [ref=e1886]
              - listitem [ref=e1888]:
                - link "ParlayPlay on Instagram" [ref=e1889] [cursor=pointer]:
                  - /url: https://www.instagram.com/parlayplay_?igsh=bHBldWQyMmV2b3Y4
                  - img [ref=e1890]
              - listitem [ref=e1892]:
                - link "ParlayPlay on Discord" [ref=e1893] [cursor=pointer]:
                  - /url: https://discord.com/invite/parlayplay
                  - img [ref=e1894]
    - generic:
      - region "Notifications Alt+T"
  - alert [ref=e1896]
```

# Test source

```ts
  1   | /**
  2   |  * Anonymous shell: the mobile bottom-nav tabs that need an account send a
  3   |  * logged-out visitor to the free-signup login page, an unknown route renders
  4   |  * the 404 page, /_offline renders the PWA offline page, and ?coupon / ?btag on
  5   |  * any URL are captured into the referral cookies. Every test runs in a fresh
  6   |  * anonymous context. Desktop's logged-out top nav and header carousel live in
  7   |  * shell-desktop.spec.ts.
  8   |  */
  9   | import { test, expect } from '../../fixtures/test.extend';
  10  | import { AuthPage } from '@pages/auth.page';
  11  | import { HomePage } from '@pages/home.page';
  12  | import { NotFoundPage } from '@pages/notFound.page';
  13  | import { OfflinePage } from '@pages/offline.page';
  14  | import { isDesktopProject } from '@utils/project';
  15  | 
  16  | const REFERRAL_COOKIE = 'ParlayPlayReferralCode';
  17  | const BTAG_COOKIE = 'ParlayPlayBtag';
  18  | 
  19  | const daysUntil = (expiresSec: number): number => (expiresSec - Date.now() / 1000) / 86_400;
  20  | 
  21  | test.describe('Shell - logged-out bottom nav', { tag: ['@navigation', '@prod'] }, () => {
  22  |   test.describe.configure({ mode: 'parallel' });
  23  | 
  24  |   test.beforeEach(async ({ page }) => {
  25  |     test.skip(isDesktopProject(), 'Desktop renders a top nav instead — see shell-desktop.spec.ts');
  26  |     await page.goto('/');
  27  |     await new HomePage(page).waitForFeedReady();
  28  |   });
  29  | 
  30  |   // A logged-out visitor always gets all five tabs: the Feed and Packs kill
  31  |   // switches need a user payload to hide anything.
  32  |   for (const label of ['Entries', 'Feed', 'Rewards', 'Packs']) {
  33  |     test(`${label} tab sends a logged-out visitor to the free-signup login page`, async ({
  34  |       page,
  35  |     }) => {
  36  |       const homePage = new HomePage(page);
  37  |       const authPage = new AuthPage(page);
  38  | 
  39  |       await homePage.bottomNav.getByRole('button', { name: label, exact: true }).click();
  40  |       await page.waitForURL(/\/account\/login\?showFreeSignup=true$/);
  41  |       await authPage.assertOnLoginPage();
  42  |       await expect(
  43  |         authPage.freeSignupBanner,
  44  |         'free-signup banner renders under the login form',
  45  |       ).toBeVisible();
  46  |     });
  47  |   }
  48  | });
  49  | 
  50  | test.describe('Shell - system pages', { tag: ['@navigation', '@prod'] }, () => {
  51  |   test.describe.configure({ mode: 'parallel' });
  52  | 
  53  |   test('Unknown route renders the 404 page', async ({ page }) => {
  54  |     const notFound = new NotFoundPage(page);
  55  |     const response = await page.goto('/this-route-does-not-exist');
  56  | 
  57  |     expect(response?.status(), 'unknown route answers with HTTP 404').toBe(404);
  58  |     await expect(notFound.heading).toHaveText('404 - Page Not Found');
  59  |     await expect(page).toHaveTitle(/Page Not Found/);
  60  |   });
  61  | 
  62  |   test('/_offline renders the offline page and Reload reloads it', async ({ page }) => {
  63  |     const offline = new OfflinePage(page);
  64  |     await page.goto('/_offline');
  65  | 
  66  |     await test.step('Offline copy and Reload CTA are shown', async () => {
  67  |       await expect(offline.heading).toHaveText('Offline!');
  68  |       await expect(offline.message).toBeVisible();
  69  |       await expect(offline.reloadBtn).toBeVisible();
  70  |     });
  71  | 
  72  |     await test.step('Reload re-requests the page', async () => {
  73  |       const reloaded = page.waitForEvent('load');
  74  |       await offline.reloadBtn.click();
  75  |       await reloaded;
  76  |       await expect(offline.heading).toHaveText('Offline!');
  77  |     });
  78  |   });
  79  | 
  80  |   test('?coupon and ?btag are stored as the referral cookies', async ({ page }) => {
  81  |     await page.goto('/?coupon=E2ECOUPON&btag=E2EBTAG');
  82  | 
  83  |     const cookie = async (name: string) =>
  84  |       (await page.context().cookies()).find((c) => c.name === name);
  85  | 
> 86  |     await expect
      |     ^ Error: ParlayPlayReferralCode is written from ?coupon
  87  |       .poll(async () => (await cookie(REFERRAL_COOKIE))?.value, {
  88  |         message: `${REFERRAL_COOKIE} is written from ?coupon`,
  89  |       })
  90  |       .toBe('E2ECOUPON');
  91  |     await expect
  92  |       .poll(async () => (await cookie(BTAG_COOKIE))?.value, {
  93  |         message: `${BTAG_COOKIE} is written from ?btag`,
  94  |       })
  95  |       .toBe('E2EBTAG');
  96  | 
  97  |     const referral = (await cookie(REFERRAL_COOKIE))!;
  98  |     const btag = (await cookie(BTAG_COOKIE))!;
  99  |     expect(daysUntil(referral.expires), 'referral cookie lives 7 days').toBeCloseTo(7, 1);
  100 |     expect(daysUntil(btag.expires), 'btag cookie lives 31 days').toBeCloseTo(31, 1);
  101 |   });
  102 | });
  103 | 
```