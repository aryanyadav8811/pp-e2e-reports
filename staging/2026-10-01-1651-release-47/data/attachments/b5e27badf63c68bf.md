# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: theme/dark-mode.spec.ts >> Theme - dark mode >> Toggle visibility matches the staff gate for the logged-in user
- Location: tests/theme/dark-mode.spec.ts:131:3

# Error details

```
Error: theme toggle rendered=false but user isStaff=true

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
                - link "Packs" [ref=e16] [cursor=pointer]:
                  - /url: /packs
                  - generic [ref=e18]: Packs
              - listitem [ref=e19]:
                - link "Feed" [ref=e20] [cursor=pointer]:
                  - /url: /challenges/feed
                  - generic [ref=e22]: Feed
              - listitem [ref=e23]:
                - link "Rewards 1" [ref=e24] [cursor=pointer]:
                  - /url: /rewards
                  - generic [ref=e25]:
                    - generic [ref=e26]: Rewards
                    - generic [ref=e27]: "1"
              - listitem [ref=e28]:
                - link "Track Picks" [ref=e29] [cursor=pointer]:
                  - /url: /challenges/pending
                  - generic [ref=e31]: Track Picks
            - button "Claim your $100 Deposit Match" [ref=e32] [cursor=pointer]
            - generic [ref=e33]:
              - generic [ref=e36]: $500.00
              - button "Toggle Menu" [ref=e37]:
                - img [ref=e38]
      - main [ref=e40]:
        - generic [ref=e42]:
          - generic [ref=e46]:
            - button "previous slide" [ref=e47] [cursor=pointer]:
              - img [ref=e48]
            - generic [ref=e51]:
              - generic [ref=e53]:
                - generic [ref=e54]:
                  - generic [ref=e55]: Receive a referral Bonus!
                  - generic [ref=e56]: $20
                - generic [ref=e57]:
                  - text: Refer a Friend
                  - text: when they make their first deposit
                  - button "Invite Now" [ref=e59] [cursor=pointer]
              - generic [ref=e61]:
                - generic [ref=e62]:
                  - text: $100
                  - img "black lightning bol" [ref=e63]
                - generic [ref=e65]: =
                - generic [ref=e66]:
                  - text: $200
                  - img "black lightning bol" [ref=e67]
                - generic [ref=e68]:
                  - text: We match your 1st deposit
                  - text: We match your first deposit up to $100.
                  - button "Deposit Now" [ref=e70] [cursor=pointer]
            - button "next slide" [ref=e71] [cursor=pointer]:
              - img [ref=e72]
          - generic [ref=e75]:
            - generic [ref=e77]:
              - generic [ref=e80]:
                - generic:
                  - img
                - textbox "Search player or team" [ref=e81]
              - generic [ref=e82]:
                - button "All" [ref=e83] [cursor=pointer]
                - button "MLB" [ref=e84] [cursor=pointer]
                - button "NHL" [ref=e85] [cursor=pointer]
                - button "CSGO" [ref=e86] [cursor=pointer]
                - button "UFC" [ref=e87] [cursor=pointer]
              - button "right chevron sign Filter" [ref=e89] [cursor=pointer]:
                - img "right chevron sign" [ref=e90]
                - text: Filter
            - generic [ref=e91]:
              - generic [ref=e94]:
                - generic [ref=e97]:
                  - generic [ref=e98]:
                    - img "Matt Olson" [ref=e100]
                    - generic [ref=e101]:
                      - generic [ref=e102]: Matt Olson
                      - generic [ref=e103]: 1B - ATL
                      - generic [ref=e106]: PHI @ ATL 8:00 PM
                    - button "Open expert opinion for Matt Olson" [ref=e107]:
                      - img [ref=e108]
                  - generic [ref=e112]:
                    - generic [ref=e113]:
                      - generic [ref=e114]:
                        - generic [ref=e116] [cursor=pointer]:
                          - text: Less
                          - img [ref=e117]
                        - generic [ref=e119]: Hits
                        - generic [ref=e121] [cursor=pointer]:
                          - text: More
                          - img [ref=e122]
                      - generic [ref=e124]:
                        - generic [ref=e125]:
                          - button "Select over 0.5 Hits for 2.34 times" [ref=e126]: 2.34x
                          - generic [ref=e127]: 0.5 Hits
                          - button "Select over 0.5 Hits for 1.46 times" [ref=e128]: 1.46x
                        - generic [ref=e129]:
                          - button "Select over 1.5 Hits for 0 times" [disabled] [ref=e130]
                          - generic [ref=e131]: 1.5 Hits
                          - button "Select over 1.5 Hits for 3.6 times" [ref=e132]: 3.6x
                        - generic [ref=e133]:
                          - button "Select over 2.5 Hits for 0 times" [disabled] [ref=e134]
                          - generic [ref=e135]: 2.5 Hits
                          - button "Select over 2.5 Hits for 11.3 times" [ref=e136]: 11.3x
                        - generic [ref=e137]:
                          - button "Select over 3.5 Hits for 0 times" [disabled] [ref=e138]
                          - generic [ref=e139]: 3.5 Hits
                          - button "Select over 3.5 Hits for 75.97 times" [ref=e140]: 75.97x
                    - generic [ref=e141]:
                      - generic [ref=e142]:
                        - generic [ref=e144] [cursor=pointer]:
                          - text: Less
                          - img [ref=e145]
                        - generic [ref=e147]: Hits + Runs + RBIs
                        - generic [ref=e149] [cursor=pointer]:
                          - text: More
                          - img [ref=e150]
                      - generic [ref=e152]:
                        - generic [ref=e153]:
                          - button "Select over 0.5 Hits + Runs + RBIs for 0 times" [disabled] [ref=e154]
                          - generic [ref=e155]: 0.5 H+R+R
                          - button "Select over 0.5 Hits + Runs + RBIs for 1.3 times" [ref=e156]: 1.3x
                        - generic [ref=e157]:
                          - button "Select over 1.5 Hits + Runs + RBIs for 1.71 times" [ref=e158]: 1.71x
                          - generic [ref=e159]: 1.5 H+R+R
                          - button "Select over 1.5 Hits + Runs + RBIs for 1.93 times" [ref=e160]: 1.93x
                        - generic [ref=e161]:
                          - button "Select over 2.5 Hits + Runs + RBIs for 0 times" [disabled] [ref=e162]
                          - generic [ref=e163]: 2.5 H+R+R
                          - button "Select over 2.5 Hits + Runs + RBIs for 2.71 times" [ref=e164]: 2.71x
                        - generic [ref=e165]:
                          - button "Select over 3.5 Hits + Runs + RBIs for 0 times" [disabled] [ref=e166]
                          - generic [ref=e167]: 3.5 H+R+R
                          - button "Select over 3.5 Hits + Runs + RBIs for 3.96 times" [ref=e168]: 3.96x
                        - generic [ref=e169]:
                          - button "Select over 4.5 Hits + Runs + RBIs for 0 times" [disabled] [ref=e170]
                          - generic [ref=e171]: 4.5 H+R+R
                          - button "Select over 4.5 Hits + Runs + RBIs for 5.86 times" [ref=e172]: 5.86x
                    - generic [ref=e173]:
                      - generic [ref=e174]:
                        - generic [ref=e176] [cursor=pointer]:
                          - text: Less
                          - img [ref=e177]
                        - generic [ref=e179]: Singles
                        - generic [ref=e181] [cursor=pointer]:
                          - text: More
                          - img [ref=e182]
                      - generic [ref=e184]:
                        - generic [ref=e185]:
                          - button "Select over 0.5 Singles for 1.56 times" [ref=e186]: 1.56x
                          - generic [ref=e187]: 0.5 Singles
                          - button "Select over 0.5 Singles for 2.11 times" [ref=e188]: 2.11x
                        - generic [ref=e189]:
                          - button "Select over 1.5 Singles for 0 times" [disabled] [ref=e190]
                          - generic [ref=e191]: 1.5 Singles
                          - button "Select over 1.5 Singles for 6.03 times" [ref=e192]: 6.03x
                    - generic [ref=e193]:
                      - generic [ref=e194]:
                        - generic [ref=e196] [cursor=pointer]:
                          - text: Less
                          - img [ref=e197]
                        - generic [ref=e199]: Doubles
                        - generic [ref=e201] [cursor=pointer]:
                          - text: More
                          - img [ref=e202]
                      - generic [ref=e205]:
                        - button "Select over 0.5 Doubles for 1.06 times" [ref=e206]: 1.06x
                        - generic [ref=e207]: 0.5 Doubles
                        - button "Select over 0.5 Doubles for 4.46 times" [ref=e208]: 4.46x
                    - generic [ref=e209]:
                      - generic [ref=e210]:
                        - generic [ref=e212] [cursor=pointer]:
                          - text: Less
                          - img [ref=e213]
                        - generic [ref=e215]: Triples
                        - generic [ref=e217] [cursor=pointer]:
                          - text: More
                          - img [ref=e218]
                      - generic [ref=e221]:
                        - button "Select over 0.5 Triples for 0 times" [disabled] [ref=e222]
                        - generic [ref=e223]: 0.5 Triples
                        - button "Select over 0.5 Triples for 37 times" [ref=e224]: 37x
                    - generic [ref=e225]:
                      - generic [ref=e226]:
                        - generic [ref=e228] [cursor=pointer]:
                          - text: Less
                          - img [ref=e229]
                        - generic [ref=e231]: Runs
                        - generic [ref=e233] [cursor=pointer]:
                          - text: More
                          - img [ref=e234]
                      - generic [ref=e236]:
                        - generic [ref=e237]:
                          - button "Select over 0.5 Runs for 1.5 times" [ref=e238]: 1.5x
                          - generic [ref=e239]: 0.5 Runs
                          - button "Select over 0.5 Runs for 2.18 times" [ref=e240]: 2.18x
                        - generic [ref=e241]:
                          - button "Select over 1.5 Runs for 0 times" [disabled] [ref=e242]
                          - generic [ref=e243]: 1.5 Runs
                          - button "Select over 1.5 Runs for 7.3 times" [ref=e244]: 7.3x
                    - generic [ref=e245]:
                      - generic [ref=e246]:
                        - generic [ref=e248] [cursor=pointer]:
                          - text: Less
                          - img [ref=e249]
                        - generic [ref=e251]: RBIs
                        - generic [ref=e253] [cursor=pointer]:
                          - text: More
                          - img [ref=e254]
                      - generic [ref=e256]:
                        - generic [ref=e257]:
                          - button "Select over 0.5 RBIs for 1.27 times" [ref=e258]: 1.27x
                          - generic [ref=e259]: 0.5 RBIs
                          - button "Select over 0.5 RBIs for 2.66 times" [ref=e260]: 2.66x
                        - generic [ref=e261]:
                          - button "Select over 1.5 RBIs for 0 times" [disabled] [ref=e262]
                          - generic [ref=e263]: 1.5 RBIs
                          - button "Select over 1.5 RBIs for 4.86 times" [ref=e264]: 4.86x
                    - generic [ref=e265]:
                      - generic [ref=e266]:
                        - generic [ref=e268] [cursor=pointer]:
                          - text: Less
                          - img [ref=e269]
                        - generic [ref=e271]: Homeruns
                        - generic [ref=e273] [cursor=pointer]:
                          - text: More
                          - img [ref=e274]
                      - generic [ref=e276]:
                        - generic [ref=e277]:
                          - button "Select over 0.5 Homeruns for 0 times" [disabled] [ref=e278]
                          - generic [ref=e279]: 0.5 Homeruns
                          - button "Select over 0.5 Homeruns for 4.09 times" [ref=e280]: 4.09x
                        - generic [ref=e281]:
                          - button "Select over 1.5 Homeruns for 0 times" [disabled] [ref=e282]
                          - generic [ref=e283]: 1.5 Homeruns
                          - button "Select over 1.5 Homeruns for 23.8 times" [ref=e284]: 23.8x
                    - generic [ref=e285]:
                      - generic [ref=e286]:
                        - generic [ref=e288] [cursor=pointer]:
                          - text: Less
                          - img [ref=e289]
                        - generic [ref=e291]: Total Bases
                        - generic [ref=e293] [cursor=pointer]:
                          - text: More
                          - img [ref=e294]
                      - generic [ref=e296]:
                        - generic [ref=e297]:
                          - button "Select over 1.5 Total Bases for 1.47 times" [ref=e298]: 1.47x
                          - generic [ref=e299]: 1.5 Total Bases
                          - button "Select over 1.5 Total Bases for 2.2 times" [ref=e300]: 2.2x
                        - generic [ref=e301]:
                          - button "Select over 2.5 Total Bases for 0 times" [disabled] [ref=e302]
                          - generic [ref=e303]: 2.5 Total Bases
                          - button "Select over 2.5 Total Bases for 2.98 times" [ref=e304]: 2.98x
                        - generic [ref=e305]:
                          - button "Select over 3.5 Total Bases for 0 times" [disabled] [ref=e306]
                          - generic [ref=e307]: 3.5 Total Bases
                          - button "Select over 3.5 Total Bases for 3.58 times" [ref=e308]: 3.58x
                        - generic [ref=e309]:
                          - button "Select over 4.5 Total Bases for 0 times" [disabled] [ref=e310]
                          - generic [ref=e311]: 4.5 Total Bases
                          - button "Select over 4.5 Total Bases for 6.2 times" [ref=e312]: 6.2x
                    - generic [ref=e313]:
                      - generic [ref=e314]:
                        - generic [ref=e316] [cursor=pointer]:
                          - text: Less
                          - img [ref=e317]
                        - generic [ref=e319]: Strikeouts
                        - generic [ref=e321] [cursor=pointer]:
                          - text: More
                          - img [ref=e322]
                      - generic [ref=e324]:
                        - generic [ref=e325]:
                          - button "Select over 0.5 Strikeouts for 0 times" [disabled] [ref=e326]
                          - generic [ref=e327]: 0.5 Strikeouts
                          - button "Select over 0.5 Strikeouts for 1.25 times" [ref=e328]: 1.25x
                        - generic [ref=e329]:
                          - button "Select over 1.5 Strikeouts for 0 times" [disabled] [ref=e330]
                          - generic [ref=e331]: 1.5 Strikeouts
                          - button "Select over 1.5 Strikeouts for 2.8 times" [ref=e332]: 2.8x
                        - generic [ref=e333]:
                          - button "Select over 2.5 Strikeouts for 0 times" [disabled] [ref=e334]
                          - generic [ref=e335]: 2.5 Strikeouts
                          - button "Select over 2.5 Strikeouts for 7.32 times" [ref=e336]: 7.32x
                    - generic [ref=e337]:
                      - generic [ref=e338]:
                        - generic [ref=e340] [cursor=pointer]:
                          - text: Less
                          - img [ref=e341]
                        - generic [ref=e343]: Fantasy Points
                        - generic [ref=e345] [cursor=pointer]:
                          - text: More
                          - img [ref=e346]
                      - generic [ref=e349]:
                        - button "Select over 5 Fantasy Points for 1.78 times" [ref=e350]: 1.78x
                        - generic [ref=e351]: 5 Fantasy Points
                        - button "Select over 5 Fantasy Points for 1.78 times" [ref=e352]: 1.78x
                  - button "Show More Stats" [ref=e354]:
                    - img [ref=e355]
                - generic [ref=e359]:
                  - generic [ref=e360]:
                    - img "Ozzie Albies" [ref=e362]
                    - generic [ref=e363]:
                      - generic [ref=e364]: Ozzie Albies
                      - generic [ref=e365]: 2B - ATL
                      - generic [ref=e368]: PHI @ ATL 8:00 PM
                    - button "Open expert opinion for Ozzie Albies" [ref=e369]:
                      - img [ref=e370]
                  - generic [ref=e374]:
                    - generic [ref=e375]:
                      - generic [ref=e376]:
                        - generic [ref=e378] [cursor=pointer]:
                          - text: Less
                          - img [ref=e379]
                        - generic [ref=e381]: Hits
                        - generic [ref=e383] [cursor=pointer]:
                          - text: More
                          - img [ref=e384]
                      - generic [ref=e386]:
                        - generic [ref=e387]:
                          - button "Select over 0.5 Hits for 2.18 times" [ref=e388]: 2.18x
                          - generic [ref=e389]: 0.5 Hits
                          - button "Select over 0.5 Hits for 1.51 times" [ref=e390]: 1.51x
                        - generic [ref=e391]:
                          - button "Select over 1.5 Hits for 0 times" [disabled] [ref=e392]
                          - generic [ref=e393]: 1.5 Hits
                          - button "Select over 1.5 Hits for 3.86 times" [ref=e394]: 3.86x
                        - generic [ref=e395]:
                          - button "Select over 2.5 Hits for 0 times" [disabled] [ref=e396]
                          - generic [ref=e397]: 2.5 Hits
                          - button "Select over 2.5 Hits for 12.69 times" [ref=e398]: 12.69x
                        - generic [ref=e399]:
                          - button "Select over 3.5 Hits for 0 times" [disabled] [ref=e400]
                          - generic [ref=e401]: 3.5 Hits
                          - button "Select over 3.5 Hits for 90.98 times" [ref=e402]: 90.98x
                    - generic [ref=e403]:
                      - generic [ref=e404]:
                        - generic [ref=e406] [cursor=pointer]:
                          - text: Less
                          - img [ref=e407]
                        - generic [ref=e409]: Hits + Runs + RBIs
                        - generic [ref=e411] [cursor=pointer]:
                          - text: More
                          - img [ref=e412]
                      - generic [ref=e414]:
                        - generic [ref=e415]:
                          - button "Select over 0.5 Hits + Runs + RBIs for 0 times" [disabled] [ref=e416]
                          - generic [ref=e417]: 0.5 H+R+R
                          - button "Select over 0.5 Hits + Runs + RBIs for 1.34 times" [ref=e418]: 1.34x
                        - generic [ref=e419]:
                          - button "Select over 1.5 Hits + Runs + RBIs for 1.53 times" [ref=e420]: 1.53x
                          - generic [ref=e421]: 1.5 H+R+R
                          - button "Select over 1.5 Hits + Runs + RBIs for 2.16 times" [ref=e422]: 2.16x
                        - generic [ref=e423]:
                          - button "Select over 2.5 Hits + Runs + RBIs for 0 times" [disabled] [ref=e424]
                          - generic [ref=e425]: 2.5 H+R+R
                          - button "Select over 2.5 Hits + Runs + RBIs for 3.12 times" [ref=e426]: 3.12x
                        - generic [ref=e427]:
                          - button "Select over 3.5 Hits + Runs + RBIs for 0 times" [disabled] [ref=e428]
                          - generic [ref=e429]: 3.5 H+R+R
                          - button "Select over 3.5 Hits + Runs + RBIs for 4.97 times" [ref=e430]: 4.97x
                        - generic [ref=e431]:
                          - button "Select over 4.5 Hits + Runs + RBIs for 0 times" [disabled] [ref=e432]
                          - generic [ref=e433]: 4.5 H+R+R
                          - button "Select over 4.5 Hits + Runs + RBIs for 7.73 times" [ref=e434]: 7.73x
                    - generic [ref=e435]:
                      - generic [ref=e436]:
                        - generic [ref=e438] [cursor=pointer]:
                          - text: Less
                          - img [ref=e439]
                        - generic [ref=e441]: Singles
                        - generic [ref=e443] [cursor=pointer]:
                          - text: More
                          - img [ref=e444]
                      - generic [ref=e446]:
                        - generic [ref=e447]:
                          - button "Select over 0.5 Singles for 1.57 times" [ref=e448]: 1.57x
                          - generic [ref=e449]: 0.5 Singles
                          - button "Select over 0.5 Singles for 2.02 times" [ref=e450]: 2.02x
                        - generic [ref=e451]:
                          - button "Select over 1.5 Singles for 0 times" [disabled] [ref=e452]
                          - generic [ref=e453]: 1.5 Singles
                          - button "Select over 1.5 Singles for 6.01 times" [ref=e454]: 6.01x
                    - generic [ref=e455]:
                      - generic [ref=e456]:
                        - generic [ref=e458] [cursor=pointer]:
                          - text: Less
                          - img [ref=e459]
                        - generic [ref=e461]: Doubles
                        - generic [ref=e463] [cursor=pointer]:
                          - text: More
                          - img [ref=e464]
                      - generic [ref=e467]:
                        - button "Select over 0.5 Doubles for 1.06 times" [ref=e468]: 1.06x
                        - generic [ref=e469]: 0.5 Doubles
                        - button "Select over 0.5 Doubles for 4.41 times" [ref=e470]: 4.41x
                    - generic [ref=e471]:
                      - generic [ref=e472]:
                        - generic [ref=e474] [cursor=pointer]:
                          - text: Less
                          - img [ref=e475]
                        - generic [ref=e477]: Triples
                        - generic [ref=e479] [cursor=pointer]:
                          - text: More
                          - img [ref=e480]
                      - generic [ref=e483]:
                        - button "Select over 0.5 Triples for 0 times" [disabled] [ref=e484]
                        - generic [ref=e485]: 0.5 Triples
                        - button "Select over 0.5 Triples for 27.4 times" [ref=e486]: 27.4x
                    - generic [ref=e487]:
                      - generic [ref=e488]:
                        - generic [ref=e490] [cursor=pointer]:
                          - text: Less
                          - img [ref=e491]
                        - generic [ref=e493]: Runs
                        - generic [ref=e495] [cursor=pointer]:
                          - text: More
                          - img [ref=e496]
                      - generic [ref=e498]:
                        - generic [ref=e499]:
                          - button "Select over 0.5 Runs for 1.28 times" [ref=e500]: 1.28x
                          - generic [ref=e501]: 0.5 Runs
                          - button "Select over 0.5 Runs for 2.68 times" [ref=e502]: 2.68x
                        - generic [ref=e503]:
                          - button "Select over 1.5 Runs for 0 times" [disabled] [ref=e504]
                          - generic [ref=e505]: 1.5 Runs
                          - button "Select over 1.5 Runs for 10.58 times" [ref=e506]: 10.58x
                    - generic [ref=e507]:
                      - generic [ref=e508]:
                        - generic [ref=e510] [cursor=pointer]:
                          - text: Less
                          - img [ref=e511]
                        - generic [ref=e513]: RBIs
                        - generic [ref=e515] [cursor=pointer]:
                          - text: More
                          - img [ref=e516]
                      - generic [ref=e518]:
                        - generic [ref=e519]:
                          - button "Select over 0.5 RBIs for 1.2 times" [ref=e520]: 1.2x
                          - generic [ref=e521]: 0.5 RBIs
                          - button "Select over 0.5 RBIs for 3.04 times" [ref=e522]: 3.04x
                        - generic [ref=e523]:
                          - button "Select over 1.5 RBIs for 0 times" [disabled] [ref=e524]
                          - generic [ref=e525]: 1.5 RBIs
                          - button "Select over 1.5 RBIs for 6.36 times" [ref=e526]: 6.36x
                    - generic [ref=e527]:
                      - generic [ref=e528]:
                        - generic [ref=e530] [cursor=pointer]:
                          - text: Less
                          - img [ref=e531]
                        - generic [ref=e533]: Homeruns
                        - generic [ref=e535] [cursor=pointer]:
                          - text: More
                          - img [ref=e536]
                      - generic [ref=e538]:
                        - generic [ref=e539]:
                          - button "Select over 0.5 Homeruns for 0 times" [disabled] [ref=e540]
                          - generic [ref=e541]: 0.5 Homeruns
                          - button "Select over 0.5 Homeruns for 6.02 times" [ref=e542]: 6.02x
                        - generic [ref=e543]:
                          - button "Select over 1.5 Homeruns for 0 times" [disabled] [ref=e544]
                          - generic [ref=e545]: 1.5 Homeruns
                          - button "Select over 1.5 Homeruns for 56.79 times" [ref=e546]: 56.79x
                    - generic [ref=e547]:
                      - generic [ref=e548]:
                        - generic [ref=e550] [cursor=pointer]:
                          - text: Less
                          - img [ref=e551]
                        - generic [ref=e553]: Total Bases
                        - generic [ref=e555] [cursor=pointer]:
                          - text: More
                          - img [ref=e556]
                      - generic [ref=e558]:
                        - generic [ref=e559]:
                          - button "Select over 1.5 Total Bases for 0 times" [disabled] [ref=e560]
                          - generic [ref=e561]: 1.5 Total Bases
                          - button "Select over 1.5 Total Bases for 2.53 times" [ref=e562]: 2.53x
                        - generic [ref=e563]:
                          - button "Select over 2.5 Total Bases for 0 times" [disabled] [ref=e564]
                          - generic [ref=e565]: 2.5 Total Bases
                          - button "Select over 2.5 Total Bases for 3.96 times" [ref=e566]: 3.96x
                        - generic [ref=e567]:
                          - button "Select over 3.5 Total Bases for 0 times" [disabled] [ref=e568]
                          - generic [ref=e569]: 3.5 Total Bases
                          - button "Select over 3.5 Total Bases for 5.01 times" [ref=e570]: 5.01x
                        - generic [ref=e571]:
                          - button "Select over 4.5 Total Bases for 0 times" [disabled] [ref=e572]
                          - generic [ref=e573]: 4.5 Total Bases
                          - button "Select over 4.5 Total Bases for 8.37 times" [ref=e574]: 8.37x
                    - generic [ref=e575]:
                      - generic [ref=e576]:
                        - generic [ref=e578] [cursor=pointer]:
                          - text: Less
                          - img [ref=e579]
                        - generic [ref=e581]: Strikeouts
                        - generic [ref=e583] [cursor=pointer]:
                          - text: More
                          - img [ref=e584]
                      - generic [ref=e586]:
                        - generic [ref=e587]:
                          - button "Select over 0.5 Strikeouts for 0 times" [disabled] [ref=e588]
                          - generic [ref=e589]: 0.5 Strikeouts
                          - button "Select over 0.5 Strikeouts for 1.33 times" [ref=e590]: 1.33x
                        - generic [ref=e591]:
                          - button "Select over 1.5 Strikeouts for 0 times" [disabled] [ref=e592]
                          - generic [ref=e593]: 1.5 Strikeouts
                          - button "Select over 1.5 Strikeouts for 3.3 times" [ref=e594]: 3.3x
                    - generic [ref=e595]:
                      - generic [ref=e596]:
                        - generic [ref=e598] [cursor=pointer]:
                          - text: Less
                          - img [ref=e599]
                        - generic [ref=e601]: Fantasy Points
                        - generic [ref=e603] [cursor=pointer]:
                          - text: More
                          - img [ref=e604]
                      - generic [ref=e607]:
                        - button "Select over 4.5 Fantasy Points for 1.78 times" [ref=e608]: 1.78x
                        - generic [ref=e609]: 4.5 Fantasy Points
                        - button "Select over 4.5 Fantasy Points for 1.78 times" [ref=e610]: 1.78x
                  - button "Show More Stats" [ref=e612]:
                    - img [ref=e613]
              - generic [ref=e678]:
                - generic [ref=e681]: Please select your 1st pick
                - generic [ref=e684]:
                  - img "arrow" [ref=e685]
                  - heading "Let's Start!" [level=2] [ref=e686]
                  - generic [ref=e687]:
                    - text: Pick at least two players
                    - text: from different teams to play
          - generic [ref=e690]:
            - generic [ref=e691]:
              - link "Parlay Play Logo" [ref=e692] [cursor=pointer]:
                - /url: /
                - img "Parlay Play Logo" [ref=e694]
              - generic [ref=e695]:
                - generic [ref=e696]: Improve your experience. Download our app.
                - generic [ref=e697]:
                  - link "Apple Store" [ref=e698] [cursor=pointer]:
                    - /url: https://apps.apple.com/us/app/parlayplay-fantasy-sports-game/id1634803703
                    - img "Apple Store" [ref=e699]
                  - link "Google Play Store" [ref=e700] [cursor=pointer]:
                    - /url: https://play.google.com/store/apps/details?id=com.parlayplay.app&hl=en_US
                    - img "Google Play Store" [ref=e701]
            - generic [ref=e702]:
              - link "Privacy" [ref=e703] [cursor=pointer]:
                - /url: /privacy-policy
              - link "Fantasy Terms" [ref=e704] [cursor=pointer]:
                - /url: /terms
              - link "Packs Terms" [ref=e705] [cursor=pointer]:
                - /url: /terms/packs
              - link "Responsible Gaming" [ref=e706] [cursor=pointer]:
                - /url: /responsible-gaming
              - link "Gaming Rules" [ref=e707] [cursor=pointer]:
                - /url: /rules
              - link "FAQ" [ref=e708] [cursor=pointer]:
                - /url: https://intercom.help/parlayplay/en/
              - link "Contact Us" [ref=e709] [cursor=pointer]:
                - /url: /
              - paragraph [ref=e710]: © ParlayPlay 2026 - All Rights Reserved
            - list [ref=e711]:
              - listitem [ref=e712]:
                - generic [ref=e713]:
                  - log [ref=e715]
                  - generic [ref=e716]:
                    - generic [ref=e717]:
                      - generic [ref=e718]: 🇺🇸English
                      - combobox "Select language" [ref=e719]
                    - img [ref=e723]
              - listitem [ref=e725]:
                - img "18+-icon" [ref=e726]
              - listitem [ref=e727]:
                - link "ParlayPlay on Twitter" [ref=e728] [cursor=pointer]:
                  - /url: https://twitter.com/parlay_play?lang=en
                  - img [ref=e729]
              - listitem [ref=e731]:
                - link "ParlayPlay on Facebook" [ref=e732] [cursor=pointer]:
                  - /url: https://www.facebook.com/ParlayPlay.io/
                  - img [ref=e733]
              - listitem [ref=e735]:
                - link "ParlayPlay on Instagram" [ref=e736] [cursor=pointer]:
                  - /url: https://www.instagram.com/parlayplay_?igsh=bHBldWQyMmV2b3Y4
                  - img [ref=e737]
              - listitem [ref=e739]:
                - link "ParlayPlay on Discord" [ref=e740] [cursor=pointer]:
                  - /url: https://discord.com/invite/parlayplay
                  - img [ref=e741]
    - generic:
      - region "Notifications Alt+T"
    - generic [ref=e744]:
      - button [ref=e745]
      - dialog [ref=e747]:
        - generic [ref=e748]:
          - button [active]
          - generic [ref=e752]:
            - generic [ref=e753]:
              - generic [ref=e754]: E
              - generic [ref=e755]:
                - generic [ref=e756]: etoembhohblbsawaplayer
                - generic [ref=e757]: $500.00
              - button "Switch to dark mode" [ref=e758]:
                - img [ref=e759]
            - link "Deposit" [ref=e761] [cursor=pointer]:
              - /url: /payments/deposit
              - button "Deposit" [ref=e762]
            - generic [ref=e763]:
              - generic [ref=e764]:
                - img [ref=e765]
                - text: Account
              - generic [ref=e767]:
                - link "Settings" [ref=e768] [cursor=pointer]:
                  - /url: /account/update
                - link "Transaction History" [ref=e769] [cursor=pointer]:
                  - /url: /transactions
                - link "Withdraw" [ref=e770] [cursor=pointer]:
                  - /url: /payments/withdraw
                - link "My Entries" [ref=e771] [cursor=pointer]:
                  - /url: /challenges/pending
                - link "Taxes" [ref=e772] [cursor=pointer]:
                  - /url: /payments/taxes
                - link "Responsible Play" [ref=e773] [cursor=pointer]:
                  - /url: /account/responsible-play
            - generic [ref=e774]:
              - generic [ref=e775]:
                - img [ref=e776]
                - text: Rewards
              - generic [ref=e778]:
                - link "Promotions" [ref=e779] [cursor=pointer]:
                  - /url: /rewards/promotions
                - link "Partner Rewards" [ref=e780] [cursor=pointer]:
                  - /url: /rewards
                - link "Refer a friend" [ref=e781] [cursor=pointer]:
                  - /url: /account/referrals
                - link "Free2Play" [ref=e782] [cursor=pointer]:
                  - /url: /challenges/mp
            - generic [ref=e783]:
              - generic [ref=e784]:
                - img [ref=e785]
                - text: Support
              - button "Contact" [ref=e788]
            - button "Log Out" [ref=e789]:
              - img [ref=e790]
              - text: Log Out
  - alert [ref=e792]
  - iframe [ref=e793]:
    
```

# Test source

```ts
  56  |       await expect(navbarLogo(page)).toHaveAttribute('src', /darkLogo\.svg/);
  57  |     },
  58  |   );
  59  | 
  60  |   test(
  61  |     'Stored "light" preference boots the app light with the light logo',
  62  |     { tag: '@staff' },
  63  |     async ({ packsPage: page }) => {
  64  |       await seedPreference(page, 'light');
  65  |       await page.goto('/');
  66  | 
  67  |       await expect(navbarLogo(page)).toBeVisible();
  68  |       await expect
  69  |         .poll(() => htmlIsDark(page), { message: 'html should not have the dark class' })
  70  |         .toBe(false);
  71  |       await expect(navbarLogo(page)).toHaveAttribute('src', /lightLogo\.svg/);
  72  |     },
  73  |   );
  74  | 
  75  |   test(
  76  |     'Staff toggle flips the theme, swaps the logo and persists across reload',
  77  |     { tag: '@staff' },
  78  |     async ({ packsPage: page }) => {
  79  |       // Not seedPreference/addInitScript here: init scripts re-run on every
  80  |       // document load and would overwrite the toggled preference on reload,
  81  |       // faking a persistence failure. Set the starting point once in the live page.
  82  |       await page.goto('/');
  83  |       await page.evaluate((key) => localStorage.setItem(key, 'light'), THEME_KEY);
  84  |       await page.reload();
  85  |       await expect(navbarLogo(page)).toBeVisible();
  86  |       await expect
  87  |         .poll(() => htmlIsDark(page), { message: 'html should not have the dark class' })
  88  |         .toBe(false);
  89  | 
  90  |       await test.step('Toggle to dark from the account menu — preference stored as dark', async () => {
  91  |         await openAccountMenu(page);
  92  |         await expect(themeToggle(page)).toBeVisible();
  93  |         await themeToggle(page).click();
  94  |         await expect
  95  |           .poll(() => htmlIsDark(page), { message: 'html should gain the dark class' })
  96  |           .toBe(true);
  97  |         expect(await storedPreference(page)).toBe('dark');
  98  |         await expect(
  99  |           page
  100 |             .getByRole('button', { name: 'Switch to light mode' })
  101 |             .filter({ visible: true })
  102 |             .first(),
  103 |         ).toBeVisible();
  104 |       });
  105 | 
  106 |       await test.step('Dark survives a hard reload with the dark logo', async () => {
  107 |         // The reload also closes the account overlay, so the navbar logo
  108 |         // is assertable again.
  109 |         await page.reload();
  110 |         await expect(navbarLogo(page)).toBeVisible();
  111 |         await expect
  112 |           .poll(() => htmlIsDark(page), { message: 'html should have the dark class' })
  113 |           .toBe(true);
  114 |         await expect(navbarLogo(page)).toHaveAttribute('src', /darkLogo\.svg/);
  115 |       });
  116 | 
  117 |       await test.step('Toggle back to light — light preference stored, light logo after reload', async () => {
  118 |         await openAccountMenu(page);
  119 |         await expect(themeToggle(page)).toBeVisible();
  120 |         await themeToggle(page).click();
  121 |         await expect
  122 |           .poll(() => htmlIsDark(page), { message: 'html should drop the dark class' })
  123 |           .toBe(false);
  124 |         expect(await storedPreference(page)).toBe('light');
  125 |         await page.reload();
  126 |         await expect(navbarLogo(page)).toHaveAttribute('src', /lightLogo\.svg/);
  127 |       });
  128 |     },
  129 |   );
  130 | 
  131 |   test('Toggle visibility matches the staff gate for the logged-in user', async ({
  132 |     loggedInPage: page,
  133 |   }) => {
  134 |     // Contract test rather than a hardcoded expectation: the toggle is
  135 |     // rendered iff the account is staff (ThemeToggle returns null
  136 |     // otherwise), and the primary test user differs per environment.
  137 |     await page.goto('/');
  138 |     await expect(navbarLogo(page)).toBeVisible();
  139 | 
  140 |     const me = await page.evaluate(async () => {
  141 |       const resp = await fetch('/api/v1/user/', {
  142 |         headers: { 'X-Requested-With': 'XMLHttpRequest', 'X-Parlay-Request': '1' },
  143 |         credentials: 'include',
  144 |       });
  145 |       return resp.json();
  146 |     });
  147 | 
  148 |     // The toggle only mounts inside the account menu — open it first.
  149 |     await openAccountMenu(page);
  150 |     const toggleVisible = await themeToggle(page)
  151 |       .isVisible({ timeout: 5_000 })
  152 |       .catch(() => false);
  153 |     expect(
  154 |       toggleVisible,
  155 |       `theme toggle rendered=${toggleVisible} but user isStaff=${me.isStaff}`,
> 156 |     ).toBe(Boolean(me.isStaff));
      |       ^ Error: theme toggle rendered=false but user isStaff=true
  157 |   });
  158 | 
  159 |   test('Login page renders its form in dark mode', { tag: '@prod' }, async ({ page }) => {
  160 |     // Regression for the login/signup dark-mode fixes: the form must be
  161 |     // fully usable with the dark class applied.
  162 |     await seedPreference(page, 'dark');
  163 |     await page.goto('/account/login');
  164 | 
  165 |     await expect
  166 |       .poll(() => htmlIsDark(page), { message: 'html should have the dark class' })
  167 |       .toBe(true);
  168 |     // Desktop renders the login form as a modal over the lobby,
  169 |     // which can leave a second, hidden copy of the fields in the DOM —
  170 |     // filter to the visible one to stay breakpoint-agnostic.
  171 |     await expect(page.locator('#username').filter({ visible: true }).first()).toBeVisible();
  172 |     await expect(page.locator('#password').filter({ visible: true }).first()).toBeVisible();
  173 |     await expect(
  174 |       page.locator('button[type="submit"]', { hasText: 'Login' }).filter({ visible: true }).first(),
  175 |     ).toBeVisible();
  176 |   });
  177 | 
  178 |   test.describe('System preference - no stored choice', () => {
  179 |     test.use({ colorScheme: 'dark' });
  180 | 
  181 |     test('OS dark appearance resolves to dark', { tag: '@staff' }, async ({ packsPage: page }) => {
  182 |       // No seeded preference — ThemeProvider should fall through to the
  183 |       // prefers-color-scheme media query, emulated dark for this test.
  184 |       await page.addInitScript((key) => localStorage.removeItem(key), THEME_KEY);
  185 |       await page.goto('/');
  186 | 
  187 |       await expect(navbarLogo(page)).toBeVisible();
  188 |       await expect
  189 |         .poll(() => htmlIsDark(page), { message: 'html should have the dark class' })
  190 |         .toBe(true);
  191 |       await expect(navbarLogo(page)).toHaveAttribute('src', /darkLogo\.svg/);
  192 |     });
  193 |   });
  194 | });
  195 | 
```