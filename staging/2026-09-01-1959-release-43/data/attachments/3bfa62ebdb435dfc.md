# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: modals/userlimits.spec.ts >> User limit modal >> Verify user limit modal
- Location: tests/modals/userlimits.spec.ts:48:3

# Error details

```
Error: expect(locator).toBeVisible() failed

Locator: locator('[data-testid="cross-game-card-wrapper"]').filter({ visible: true }).first().locator('div[id^="player-"]').filter({ visible: true }).first().or(getByTestId('no-player-found').filter({ visible: true }).first()).first()
Expected: visible
Timeout: 15000ms
Error: element(s) not found

Call log:
  - Expect "toBeVisible" with timeout 15000ms
  - waiting for locator('[data-testid="cross-game-card-wrapper"]').filter({ visible: true }).first().locator('div[id^="player-"]').filter({ visible: true }).first().or(getByTestId('no-player-found').filter({ visible: true }).first()).first()

```

# Page snapshot

```yaml
- generic [ref=e1]:
  - generic [ref=e2]:
    - generic [ref=e3]:
      - banner [ref=e4]:
        - navigation [ref=e5]:
          - link "Parlay Play Logo" [active] [ref=e6] [cursor=pointer]:
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
                - link "Rewards 52" [ref=e24] [cursor=pointer]:
                  - /url: /rewards
                  - generic [ref=e25]:
                    - generic [ref=e26]: Rewards
                    - generic [ref=e27]: "52"
              - listitem [ref=e28]:
                - link "Track Picks 32" [ref=e29] [cursor=pointer]:
                  - /url: /challenges/pending
                  - generic [ref=e30]:
                    - generic [ref=e31]: Track Picks
                    - generic [ref=e32]: "32"
            - button "Claim your $100 Deposit Match" [ref=e33] [cursor=pointer]
            - generic [ref=e34]:
              - generic [ref=e36]:
                - generic [ref=e37]: $942.00
                - generic [ref=e38]:
                  - img "gift-icon" [ref=e39]
                  - text: "51.00"
              - button "Toggle Menu" [ref=e40]:
                - img [ref=e41]
      - main [ref=e43]:
        - generic [ref=e45]:
          - generic [ref=e49]:
            - button "previous slide" [ref=e50] [cursor=pointer]:
              - img [ref=e51]
            - generic [ref=e54]:
              - generic [ref=e56]:
                - generic [ref=e57]:
                  - generic [ref=e58]: Receive a referral Bonus!
                  - generic [ref=e59]: $20
                - generic [ref=e60]:
                  - text: Refer a Friend
                  - text: when they make their first deposit
                  - button "Invite Now" [ref=e62] [cursor=pointer]
              - generic [ref=e64]:
                - generic [ref=e65]:
                  - text: $100
                  - img "black lightning bol" [ref=e66]
                - generic [ref=e68]: =
                - generic [ref=e69]:
                  - text: $200
                  - img "black lightning bol" [ref=e70]
                - generic [ref=e71]:
                  - text: We match your 1st deposit
                  - text: We match your first deposit up to $100.
                  - button "Deposit Now" [ref=e73] [cursor=pointer]
            - button "next slide" [ref=e74] [cursor=pointer]:
              - img [ref=e75]
          - generic [ref=e78]:
            - generic [ref=e80]:
              - generic [ref=e83]:
                - generic:
                  - img
                - textbox "Search player or team" [ref=e84]
              - generic [ref=e85]:
                - button "All" [ref=e86] [cursor=pointer]
                - button "MLB" [ref=e87] [cursor=pointer]
                - button "MLB-Combos" [ref=e88] [cursor=pointer]
                - button "EPL" [ref=e89] [cursor=pointer]
                - button "MLS" [ref=e90] [cursor=pointer]
                - button "NFLSZN" [ref=e91] [cursor=pointer]
                - button "LaLiga" [ref=e92] [cursor=pointer]
                - button "UFC" [ref=e93] [cursor=pointer]
              - button "right chevron sign Filter" [ref=e95] [cursor=pointer]:
                - img "right chevron sign" [ref=e96]
                - text: Filter
            - generic [ref=e97]:
              - generic [ref=e100]:
                - generic [ref=e103]:
                  - generic [ref=e104]:
                    - img "Randy Vasquez" [ref=e106]
                    - generic [ref=e107]:
                      - generic [ref=e108]: Randy Vasquez
                      - generic [ref=e109]: SP - SD
                      - generic [ref=e112]: SD @ CIN 6:40 PM
                    - button "Open expert opinion for Randy Vasquez" [ref=e113]:
                      - img [ref=e114]
                  - generic [ref=e118]:
                    - generic [ref=e119]:
                      - generic [ref=e120]:
                        - generic [ref=e122] [cursor=pointer]:
                          - text: Less
                          - img [ref=e123]
                        - generic [ref=e125]: Strikeouts (K)
                        - generic [ref=e127] [cursor=pointer]:
                          - text: More
                          - img [ref=e128]
                      - generic [ref=e130]:
                        - generic [ref=e131]:
                          - button "Select over 1.5 Strikeouts (K) for 0 times" [disabled] [ref=e132]
                          - generic [ref=e133]: 1.5 Strikeouts (K)
                          - button "Select over 1.5 Strikeouts (K) for 1.06 times" [ref=e134]: 1.06x
                        - generic [ref=e135]:
                          - button "Select over 2.5 Strikeouts (K) for 0 times" [disabled] [ref=e136]
                          - generic [ref=e137]: 2.5 Strikeouts (K)
                          - button "Select over 2.5 Strikeouts (K) for 1.3 times" [ref=e138]: 1.3x
                        - generic [ref=e139]:
                          - button "Select over 3.5 Strikeouts (K) for 1.62 times" [ref=e140]: 1.62x
                          - generic [ref=e141]: 3.5 Strikeouts (K)
                          - button "Select over 3.5 Strikeouts (K) for 2.04 times" [ref=e142]: 2.04x
                        - generic [ref=e143]:
                          - button "Select over 4.5 Strikeouts (K) for 0 times" [disabled] [ref=e144]
                          - generic [ref=e145]: 4.5 Strikeouts (K)
                          - button "Select over 4.5 Strikeouts (K) for 3.18 times" [ref=e146]: 3.18x
                        - generic [ref=e147]:
                          - button "Select over 5.5 Strikeouts (K) for 0 times" [disabled] [ref=e148]
                          - generic [ref=e149]: 5.5 Strikeouts (K)
                          - button "Select over 5.5 Strikeouts (K) for 5.54 times" [ref=e150]: 5.54x
                        - button "Show more Strikeouts (K) lines (6)" [ref=e151]:
                          - img [ref=e152]
                          - text: Show more Strikeouts (K) lines (6)
                    - generic [ref=e154]:
                      - generic [ref=e155]:
                        - generic [ref=e157] [cursor=pointer]:
                          - text: Less
                          - img [ref=e158]
                        - generic [ref=e160]: Hits Allowed
                        - generic [ref=e162] [cursor=pointer]:
                          - text: More
                          - img [ref=e163]
                      - generic [ref=e165]:
                        - generic [ref=e166]:
                          - button "Select over 2.5 Hits Allowed for 4.38 times" [ref=e167]: 4.38x
                          - generic [ref=e168]: 2.5 Hits Allowed
                          - button "Select over 2.5 Hits Allowed for 0 times" [disabled] [ref=e169]
                        - generic [ref=e170]:
                          - button "Select over 3.5 Hits Allowed for 2.69 times" [ref=e171]: 2.69x
                          - generic [ref=e172]: 3.5 Hits Allowed
                          - button "Select over 3.5 Hits Allowed for 0 times" [disabled] [ref=e173]
                        - generic [ref=e174]:
                          - button "Select over 4.5 Hits Allowed for 1.89 times" [ref=e175]: 1.89x
                          - generic [ref=e176]: 4.5 Hits Allowed
                          - button "Select over 4.5 Hits Allowed for 1.71 times" [ref=e177]: 1.71x
                        - generic [ref=e178]:
                          - button "Select over 5.5 Hits Allowed for 1.32 times" [ref=e179]: 1.32x
                          - generic [ref=e180]: 5.5 Hits Allowed
                          - button "Select over 5.5 Hits Allowed for 0 times" [disabled] [ref=e181]
                        - generic [ref=e182]:
                          - button "Select over 6.5 Hits Allowed for 1.08 times" [ref=e183]: 1.08x
                          - generic [ref=e184]: 6.5 Hits Allowed
                          - button "Select over 6.5 Hits Allowed for 0 times" [disabled] [ref=e185]
                        - button "Show more Hits Allowed lines (6)" [ref=e186]:
                          - img [ref=e187]
                          - text: Show more Hits Allowed lines (6)
                    - generic [ref=e189]:
                      - generic [ref=e190]:
                        - generic [ref=e192] [cursor=pointer]:
                          - text: Less
                          - img [ref=e193]
                        - generic [ref=e195]: Pitching Outs
                        - generic [ref=e197] [cursor=pointer]:
                          - text: More
                          - img [ref=e198]
                      - generic [ref=e201]:
                        - button "Select over 14.5 Pitching Outs for 1.68 times" [ref=e202]: 1.68x
                        - generic [ref=e203]: 14.5 Pitching Outs
                        - button "Select over 14.5 Pitching Outs for 1.93 times" [ref=e204]: 1.93x
                    - generic [ref=e205]:
                      - generic [ref=e206]:
                        - generic [ref=e208] [cursor=pointer]:
                          - text: Less
                          - img [ref=e209]
                        - generic [ref=e211]: Earned Runs
                        - generic [ref=e213] [cursor=pointer]:
                          - text: More
                          - img [ref=e214]
                      - generic [ref=e216]:
                        - generic [ref=e217]:
                          - button "Select over 1.5 Earned Runs for 2.41 times" [ref=e218]: 2.41x
                          - generic [ref=e219]: 1.5 Earned Runs
                          - button "Select over 1.5 Earned Runs for 0 times" [disabled] [ref=e220]
                        - generic [ref=e221]:
                          - button "Select over 2.5 Earned Runs for 1.58 times" [ref=e222]: 1.58x
                          - generic [ref=e223]: 2.5 Earned Runs
                          - button "Select over 2.5 Earned Runs for 2.03 times" [ref=e224]: 2.03x
                        - generic [ref=e225]:
                          - button "Select over 3.5 Earned Runs for 1.22 times" [ref=e226]: 1.22x
                          - generic [ref=e227]: 3.5 Earned Runs
                          - button "Select over 3.5 Earned Runs for 0 times" [disabled] [ref=e228]
                    - generic [ref=e229]:
                      - generic [ref=e230]:
                        - generic [ref=e232] [cursor=pointer]:
                          - text: Less
                          - img [ref=e233]
                        - generic [ref=e235]: Fantasy Points
                        - generic [ref=e237] [cursor=pointer]:
                          - text: More
                          - img [ref=e238]
                      - generic [ref=e241]:
                        - button "Select over 18.5 Fantasy Points for 1.78 times" [ref=e242]: 1.78x
                        - generic [ref=e243]: 18.5 Fantasy Points
                        - button "Select over 18.5 Fantasy Points for 1.78 times" [ref=e244]: 1.78x
                  - button "Show More Stats" [ref=e246]:
                    - img [ref=e247]
                - generic [ref=e251]:
                  - generic [ref=e252]:
                    - img "Fernando Tatis Jr." [ref=e254]
                    - generic [ref=e255]:
                      - generic [ref=e256]: F. Tatis Jr.
                      - generic [ref=e257]: RF - SD
                      - generic [ref=e260]: SD @ CIN 6:40 PM
                    - button "Open expert opinion for Fernando Tatis Jr." [ref=e261]:
                      - img [ref=e262]
                  - generic [ref=e266]:
                    - generic [ref=e267]:
                      - generic [ref=e268]:
                        - generic [ref=e270] [cursor=pointer]:
                          - text: Less
                          - img [ref=e271]
                        - generic [ref=e273]: Hits
                        - generic [ref=e275] [cursor=pointer]:
                          - text: More
                          - img [ref=e276]
                      - generic [ref=e278]:
                        - generic [ref=e279]:
                          - button "Select over 0.5 Hits for 0 times" [disabled] [ref=e280]
                          - generic [ref=e281]: 0.5 Hits
                          - button "Select over 0.5 Hits for 1.16 times" [ref=e282]: 1.16x
                        - generic [ref=e283]:
                          - button "Select over 1.5 Hits for 1.35 times" [ref=e284]: 1.35x
                          - generic [ref=e285]: 1.5 Hits
                          - button "Select over 1.5 Hits for 2.26 times" [ref=e286]: 2.26x
                        - generic [ref=e287]:
                          - button "Select over 2.5 Hits for 0 times" [disabled] [ref=e288]
                          - generic [ref=e289]: 2.5 Hits
                          - button "Select over 2.5 Hits for 5.46 times" [ref=e290]: 5.46x
                        - generic [ref=e291]:
                          - button "Select over 3.5 Hits for 0 times" [disabled] [ref=e292]
                          - generic [ref=e293]: 3.5 Hits
                          - button "Select over 3.5 Hits for 16.59 times" [ref=e294]: 16.59x
                    - generic [ref=e295]:
                      - generic [ref=e296]:
                        - generic [ref=e298] [cursor=pointer]:
                          - text: Less
                          - img [ref=e299]
                        - generic [ref=e301]: Hits + Runs + RBIs
                        - generic [ref=e303] [cursor=pointer]:
                          - text: More
                          - img [ref=e304]
                      - generic [ref=e306]:
                        - generic [ref=e307]:
                          - button "Select over 0.5 Hits + Runs + RBIs for 0 times" [disabled] [ref=e308]
                          - generic [ref=e309]: 0.5 H+R+R
                          - button "Select over 0.5 Hits + Runs + RBIs for 1.08 times" [ref=e310]: 1.08x
                        - generic [ref=e311]:
                          - button "Select over 1.5 Hits + Runs + RBIs for 0 times" [disabled] [ref=e312]
                          - generic [ref=e313]: 1.5 H+R+R
                          - button "Select over 1.5 Hits + Runs + RBIs for 1.37 times" [ref=e314]: 1.37x
                        - generic [ref=e315]:
                          - button "Select over 2.5 Hits + Runs + RBIs for 1.68 times" [ref=e316]: 1.68x
                          - generic [ref=e317]: 2.5 H+R+R
                          - button "Select over 2.5 Hits + Runs + RBIs for 1.85 times" [ref=e318]: 1.85x
                        - generic [ref=e319]:
                          - button "Select over 3.5 Hits + Runs + RBIs for 0 times" [disabled] [ref=e320]
                          - generic [ref=e321]: 3.5 H+R+R
                          - button "Select over 3.5 Hits + Runs + RBIs for 2.58 times" [ref=e322]: 2.58x
                        - generic [ref=e323]:
                          - button "Select over 4.5 Hits + Runs + RBIs for 0 times" [disabled] [ref=e324]
                          - generic [ref=e325]: 4.5 H+R+R
                          - button "Select over 4.5 Hits + Runs + RBIs for 3.76 times" [ref=e326]: 3.76x
                    - generic [ref=e327]:
                      - generic [ref=e328]:
                        - generic [ref=e330] [cursor=pointer]:
                          - text: Less
                          - img [ref=e331]
                        - generic [ref=e333]: Singles
                        - generic [ref=e335] [cursor=pointer]:
                          - text: More
                          - img [ref=e336]
                      - generic [ref=e338]:
                        - generic [ref=e339]:
                          - button "Select over 0.5 Singles for 1.88 times" [ref=e340]: 1.88x
                          - generic [ref=e341]: 0.5 Singles
                          - button "Select over 0.5 Singles for 1.62 times" [ref=e342]: 1.62x
                        - generic [ref=e343]:
                          - button "Select over 1.5 Singles for 0 times" [disabled] [ref=e344]
                          - generic [ref=e345]: 1.5 Singles
                          - button "Select over 1.5 Singles for 4.39 times" [ref=e346]: 4.39x
                    - generic [ref=e347]:
                      - generic [ref=e348]:
                        - generic [ref=e350] [cursor=pointer]:
                          - text: Less
                          - img [ref=e351]
                        - generic [ref=e353]: Doubles
                        - generic [ref=e355] [cursor=pointer]:
                          - text: More
                          - img [ref=e356]
                      - generic [ref=e359]:
                        - button "Select over 0.5 Doubles for 1.12 times" [ref=e360]: 1.12x
                        - generic [ref=e361]: 0.5 Doubles
                        - button "Select over 0.5 Doubles for 3.4 times" [ref=e362]: 3.4x
                    - generic [ref=e363]:
                      - generic [ref=e364]:
                        - generic [ref=e366] [cursor=pointer]:
                          - text: Less
                          - img [ref=e367]
                        - generic [ref=e369]: Triples
                        - generic [ref=e371] [cursor=pointer]:
                          - text: More
                          - img [ref=e372]
                      - generic [ref=e375]:
                        - button "Select over 0.5 Triples for 0 times" [disabled] [ref=e376]
                        - generic [ref=e377]: 0.5 Triples
                        - button "Select over 0.5 Triples for 20.8 times" [ref=e378]: 20.8x
                    - generic [ref=e379]:
                      - generic [ref=e380]:
                        - generic [ref=e382] [cursor=pointer]:
                          - text: Less
                          - img [ref=e383]
                        - generic [ref=e385]: Runs
                        - generic [ref=e387] [cursor=pointer]:
                          - text: More
                          - img [ref=e388]
                      - generic [ref=e390]:
                        - generic [ref=e391]:
                          - button "Select over 0.5 Runs for 2 times" [ref=e392]: 2x
                          - generic [ref=e393]: 0.5 Runs
                          - button "Select over 0.5 Runs for 1.51 times" [ref=e394]: 1.51x
                        - generic [ref=e395]:
                          - button "Select over 1.5 Runs for 0 times" [disabled] [ref=e396]
                          - generic [ref=e397]: 1.5 Runs
                          - button "Select over 1.5 Runs for 3.92 times" [ref=e398]: 3.92x
                        - generic [ref=e399]:
                          - button "Select over 2.5 Runs for 0 times" [disabled] [ref=e400]
                          - generic [ref=e401]: 2.5 Runs
                          - button "Select over 2.5 Runs for 11.18 times" [ref=e402]: 11.18x
                    - generic [ref=e403]:
                      - generic [ref=e404]:
                        - generic [ref=e406] [cursor=pointer]:
                          - text: Less
                          - img [ref=e407]
                        - generic [ref=e409]: RBIs
                        - generic [ref=e411] [cursor=pointer]:
                          - text: More
                          - img [ref=e412]
                      - generic [ref=e414]:
                        - generic [ref=e415]:
                          - button "Select over 0.5 RBIs for 1.49 times" [ref=e416]: 1.49x
                          - generic [ref=e417]: 0.5 RBIs
                          - button "Select over 0.5 RBIs for 2.1 times" [ref=e418]: 2.1x
                        - generic [ref=e419]:
                          - button "Select over 1.5 RBIs for 0 times" [disabled] [ref=e420]
                          - generic [ref=e421]: 1.5 RBIs
                          - button "Select over 1.5 RBIs for 4.22 times" [ref=e422]: 4.22x
                        - generic [ref=e423]:
                          - button "Select over 2.5 RBIs for 0 times" [disabled] [ref=e424]
                          - generic [ref=e425]: 2.5 RBIs
                          - button "Select over 2.5 RBIs for 7.68 times" [ref=e426]: 7.68x
                        - generic [ref=e427]:
                          - button "Select over 3.5 RBIs for 0 times" [disabled] [ref=e428]
                          - generic [ref=e429]: 3.5 RBIs
                          - button "Select over 3.5 RBIs for 17.18 times" [ref=e430]: 17.18x
                    - generic [ref=e431]:
                      - generic [ref=e432]:
                        - generic [ref=e434] [cursor=pointer]:
                          - text: Less
                          - img [ref=e435]
                        - generic [ref=e437]: Homeruns
                        - generic [ref=e439] [cursor=pointer]:
                          - text: More
                          - img [ref=e440]
                      - generic [ref=e442]:
                        - generic [ref=e443]:
                          - button "Select over 0.5 Homeruns for 0 times" [disabled] [ref=e444]
                          - generic [ref=e445]: 0.5 Homeruns
                          - button "Select over 0.5 Homeruns for 3.07 times" [ref=e446]: 3.07x
                        - generic [ref=e447]:
                          - button "Select over 1.5 Homeruns for 0 times" [disabled] [ref=e448]
                          - generic [ref=e449]: 1.5 Homeruns
                          - button "Select over 1.5 Homeruns for 13.58 times" [ref=e450]: 13.58x
                        - generic [ref=e451]:
                          - button "Select over 2.5 Homeruns for 0 times" [disabled] [ref=e452]
                          - generic [ref=e453]: 2.5 Homeruns
                          - button "Select over 2.5 Homeruns for 60.97 times" [ref=e454]: 60.97x
                    - generic [ref=e455]:
                      - generic [ref=e456]:
                        - generic [ref=e458] [cursor=pointer]:
                          - text: Less
                          - img [ref=e459]
                        - generic [ref=e461]: Total Bases
                        - generic [ref=e463] [cursor=pointer]:
                          - text: More
                          - img [ref=e464]
                      - generic [ref=e466]:
                        - generic [ref=e467]:
                          - button "Select over 1.5 Total Bases for 1.91 times" [ref=e468]: 1.91x
                          - generic [ref=e469]: 1.5 Total Bases
                          - button "Select over 1.5 Total Bases for 1.59 times" [ref=e470]: 1.59x
                        - generic [ref=e471]:
                          - button "Select over 2.5 Total Bases for 0 times" [disabled] [ref=e472]
                          - generic [ref=e473]: 2.5 Total Bases
                          - button "Select over 2.5 Total Bases for 2.16 times" [ref=e474]: 2.16x
                        - generic [ref=e475]:
                          - button "Select over 3.5 Total Bases for 0 times" [disabled] [ref=e476]
                          - generic [ref=e477]: 3.5 Total Bases
                          - button "Select over 3.5 Total Bases for 2.56 times" [ref=e478]: 2.56x
                        - generic [ref=e479]:
                          - button "Select over 4.5 Total Bases for 0 times" [disabled] [ref=e480]
                          - generic [ref=e481]: 4.5 Total Bases
                          - button "Select over 4.5 Total Bases for 3.88 times" [ref=e482]: 3.88x
                        - generic [ref=e483]:
                          - button "Select over 5.5 Total Bases for 0 times" [disabled] [ref=e484]
                          - generic [ref=e485]: 5.5 Total Bases
                          - button "Select over 5.5 Total Bases for 6.16 times" [ref=e486]: 6.16x
                        - button "Show more Total Bases lines (6)" [ref=e487]:
                          - img [ref=e488]
                          - text: Show more Total Bases lines (6)
                    - generic [ref=e490]:
                      - generic [ref=e491]:
                        - generic [ref=e493] [cursor=pointer]:
                          - text: Less
                          - img [ref=e494]
                        - generic [ref=e496]: Strikeouts
                        - generic [ref=e498] [cursor=pointer]:
                          - text: More
                          - img [ref=e499]
                      - generic [ref=e501]:
                        - generic [ref=e502]:
                          - button "Select over 0.5 Strikeouts for 0 times" [disabled] [ref=e503]
                          - generic [ref=e504]: 0.5 Strikeouts
                          - button "Select over 0.5 Strikeouts for 1.31 times" [ref=e505]: 1.31x
                        - generic [ref=e506]:
                          - button "Select over 1.5 Strikeouts for 0 times" [disabled] [ref=e507]
                          - generic [ref=e508]: 1.5 Strikeouts
                          - button "Select over 1.5 Strikeouts for 3.2 times" [ref=e509]: 3.2x
                    - generic [ref=e510]:
                      - generic [ref=e511]:
                        - generic [ref=e513] [cursor=pointer]:
                          - text: Less
                          - img [ref=e514]
                        - generic [ref=e516]: Fantasy Points
                        - generic [ref=e518] [cursor=pointer]:
                          - text: More
                          - img [ref=e519]
                      - generic [ref=e522]:
                        - button "Select over 7.5 Fantasy Points for 1.78 times" [ref=e523]: 1.78x
                        - generic [ref=e524]: 7.5 Fantasy Points
                        - button "Select over 7.5 Fantasy Points for 1.78 times" [ref=e525]: 1.78x
                  - button "Show More Stats" [ref=e527]:
                    - img [ref=e528]
              - generic [ref=e1754]:
                - generic [ref=e1757]: Please select your 1st pick
                - generic [ref=e1760]:
                  - img "arrow" [ref=e1761]
                  - heading "Let's Start!" [level=2] [ref=e1762]
                  - generic [ref=e1763]:
                    - text: Pick at least two players
                    - text: from different teams to play
          - generic [ref=e1766]:
            - generic [ref=e1767]:
              - link "Parlay Play Logo" [ref=e1768] [cursor=pointer]:
                - /url: /
                - img "Parlay Play Logo" [ref=e1770]
              - generic [ref=e1771]:
                - generic [ref=e1772]: Improve your experience. Download our app.
                - generic [ref=e1773]:
                  - link "Apple Store" [ref=e1774] [cursor=pointer]:
                    - /url: https://parlayplay.onelink.me/oLJk/gnqpwjha
                    - img "Apple Store" [ref=e1775]
                  - link "Google Play Store" [ref=e1776] [cursor=pointer]:
                    - /url: https://parlayplay.onelink.me/oLJk/fh7u6juo
                    - img "Google Play Store" [ref=e1777]
            - generic [ref=e1778]:
              - link "Privacy" [ref=e1779] [cursor=pointer]:
                - /url: /privacy-policy
              - link "Fantasy Terms" [ref=e1780] [cursor=pointer]:
                - /url: /terms
              - link "Packs Terms" [ref=e1781] [cursor=pointer]:
                - /url: /terms/packs
              - link "Responsible Gaming" [ref=e1782] [cursor=pointer]:
                - /url: /responsible-gaming
              - link "Gaming Rules" [ref=e1783] [cursor=pointer]:
                - /url: /rules
              - link "FAQ" [ref=e1784] [cursor=pointer]:
                - /url: https://intercom.help/parlayplay/en/
              - link "Contact Us" [ref=e1785] [cursor=pointer]:
                - /url: /
              - paragraph [ref=e1786]: © ParlayPlay 2026 - All Rights Reserved
            - list [ref=e1787]:
              - listitem [ref=e1788]:
                - generic [ref=e1789]:
                  - log [ref=e1791]
                  - generic [ref=e1792]:
                    - generic [ref=e1793]:
                      - generic [ref=e1794]: 🇺🇸English
                      - combobox "Select language" [ref=e1795]
                    - img [ref=e1799]
              - listitem [ref=e1801]:
                - img "18+-icon" [ref=e1802]
              - listitem [ref=e1803]:
                - link "ParlayPlay on Twitter" [ref=e1804] [cursor=pointer]:
                  - /url: https://twitter.com/parlay_play?lang=en
                  - img [ref=e1805]
              - listitem [ref=e1807]:
                - link "ParlayPlay on Facebook" [ref=e1808] [cursor=pointer]:
                  - /url: https://www.facebook.com/ParlayPlay.io/
                  - img [ref=e1809]
              - listitem [ref=e1811]:
                - link "ParlayPlay on Instagram" [ref=e1812] [cursor=pointer]:
                  - /url: https://www.instagram.com/parlayplay_?igsh=bHBldWQyMmV2b3Y4
                  - img [ref=e1813]
              - listitem [ref=e1815]:
                - link "ParlayPlay on Discord" [ref=e1816] [cursor=pointer]:
                  - /url: https://discord.com/invite/parlayplay
                  - img [ref=e1817]
    - generic:
      - region "Notifications Alt+T"
  - alert [ref=e1819]: ParlayPlay | Fun Fantasy Sports
  - iframe [ref=e1820]:
    
  - button "Open Intercom Messenger" [ref=e1821] [cursor=pointer]:
    - img [ref=e1823]
    - generic:
      - img
```

# Test source

```ts
  113 |   readonly toggleMenu = this.byRole("button", { name: "Toggle Menu" });
  114 |   // DFS-2467: button on mobile, link (with an optional badge-count suffix in
  115 |   // the accessible name) on desktop.
  116 |   readonly rewardsTab = this.visible(
  117 |     this.page
  118 |       .getByRole("button", { name: "Rewards" })
  119 |       .or(this.page.getByRole("link", { name: /^Rewards\b/ }))
  120 |   );
  121 |   // DFS-2467: anchor on the pill ids, not the mobile-only `league-selector`
  122 |   // testid container — desktop's pills wrapper has none, so the anchored form
  123 |   // resolved the *hidden* mobile copy on Desktop and every click then waited
  124 |   // on an element that never becomes visible (2-minute hang).
  125 |   readonly fgleagueTabs = this.page
  126 |     .locator(
  127 |       'button[id^="league-"]:not([id*="combo"]):not([id*="H1"]):not([id*="Q1"])'
  128 |     )
  129 |     .filter({ visible: true });
  130 |   // DFS-2467: desktop has no Continue hop — the persistent pick-slip panel
  131 |   // (screens/Crossgame/PickSlip.tsx) renders the submission form inline, and
  132 |   // its `#place-pick` button carries the same "slip is valid" semantics that
  133 |   // the mobile Continue button does.
  134 |   readonly placePickBtn = this.locator("#place-pick");
  135 |   // "The slip is playable" CTA on either breakpoint: mobile's Continue button
  136 |   // or desktop's inline #place-pick. Specs assert on this rather than on
  137 |   // `continueBtn` so they hold on both projects.
  138 |   readonly slipReadyCta = this.continueBtn.or(this.placePickBtn).first();
  139 |   readonly statsContainer = this.page.locator(
  140 |     "div.flex.flex-col.items-center >> ul.flex.flex-row"
  141 |   );
  142 | 
  143 |   readonly statsTabs = this.statsContainer.locator(":scope > li > button");
  144 | 
  145 |   constructor(page: Page) {
  146 |     super(page);
  147 |   }
  148 | 
  149 |   nthPlayerOnDefault(index: number): Locator {
  150 |     return this.playerCardsVisible.nth(index);
  151 |   }
  152 | 
  153 |   /**
  154 |    * Card locator anchored on its stable `id="player-<id>"`. The virtualised
  155 |    * grid unmounts/remounts cards as it scrolls, so index-based handles
  156 |    * (`nth(i)`) silently re-resolve to a different card mid-flow — an
  157 |    * id-anchored locator always points at the same player (or at nothing once
  158 |    * it scrolls out of the mount window).
  159 |    */
  160 |   playerCardById(playerId: string): Locator {
  161 |     return this.visible(this.page.locator(`div[id="${playerId}"]`));
  162 |   }
  163 | 
  164 |   /** Ids of the currently mounted player cards, in DOM order. */
  165 |   async listVisiblePlayerIds(): Promise<string[]> {
  166 |     await this.waitForPlayersGrid();
  167 |     await expect(this.playerCardsVisible.first()).toBeVisible();
  168 |     return (
  169 |       await this.playerCardsVisible.evaluateAll((els) => els.map((el) => el.id))
  170 |     ).filter(Boolean);
  171 |   }
  172 | 
  173 |   playerStatButton(id: string): Locator {
  174 |     return this.visible(
  175 |       this.page.locator(id).locator('button:has([data-testid="stat-value"])')
  176 |     );
  177 |   }
  178 | 
  179 |   /**
  180 |    * DFS-2467: the more/less pick buttons carry `grid-button` in the mobile
  181 |    * card (components/CrossGameCardAlt/Mobile/row.tsx) but
  182 |    * `stat-selection-button` in the desktop card (CrossGameCardAlt/row.tsx).
  183 |    * A card locator only ever resolves inside one tree, so the union is safe
  184 |    * on both breakpoints.
  185 |    */
  186 |   pickButtons(card: Locator): Locator {
  187 |     return card
  188 |       .getByTestId("grid-button")
  189 |       .or(card.getByTestId("stat-selection-button"));
  190 |   }
  191 | 
  192 |   moreLessDefaultPlayerButtons(index: number): Locator {
  193 |     return this.pickButtons(this.nthPlayerOnDefault(index));
  194 |   }
  195 | 
  196 |   async openTermsPageUsingNonAuth(
  197 |     button: "Sign Up" | "Join Now"
  198 |   ): Promise<void> {
  199 |     if (button == "Sign Up") {
  200 |       await this.signupButton.click();
  201 |     } else if (button == "Join Now") {
  202 |       await this.joinNowButton.click();
  203 |     }
  204 |   }
  205 | 
  206 |   async waitForPlayersGrid(): Promise<void> {
  207 |     // DFS-2467: the mobile tree nests the grid as the wrapper's 2nd child,
  208 |     // but the desktop tree's wrapper has a different inner shape — anchor on
  209 |     // the outcome (a mounted card, or the empty-state label for leagues with
  210 |     // no offerings) instead of the wrapper's structure.
  211 |     await expect(
  212 |       this.playerCardsVisible.first().or(this.noPlayerFoundVisible).first()
> 213 |     ).toBeVisible();
      |       ^ Error: expect(locator).toBeVisible() failed
  214 |   }
  215 | 
  216 |   async waitForFeedReady(timeout = 30_000): Promise<void> {
  217 |     await Promise.race([
  218 |       this.crossGameCardWrapper.waitFor({ state: "visible", timeout }),
  219 |       this.noPlayerFoundVisible.waitFor({ state: "visible", timeout }),
  220 |     ]);
  221 |   }
  222 | 
  223 |   async isEmptyState(): Promise<boolean> {
  224 |     return this.noPlayerFoundVisible.isVisible().catch(() => false);
  225 |   }
  226 | 
  227 |   async getPlayerCardCount(): Promise<number> {
  228 |     await this.waitForPlayersGrid();
  229 |     const cards = this.playerCardsVisible;
  230 |     await expect(cards.first()).toBeVisible();
  231 |     return await cards.count();
  232 |   }
  233 | 
  234 |   async listPlayersCard(): Promise<Locator[]> {
  235 |     await this.waitForPlayersGrid();
  236 |     const cards = this.playerCardsVisible;
  237 |     await expect(cards.first()).toBeVisible();
  238 |     const count = await cards.count();
  239 |     const result: Locator[] = [];
  240 |     for (let i = 0; i < count; i++) {
  241 |       result.push(cards.nth(i));
  242 |     }
  243 |     return result;
  244 |   }
  245 | 
  246 |   async getLeagueCount(): Promise<number> {
  247 |     return await this.leagueButtons.count();
  248 |   }
  249 | 
  250 |   /**
  251 |    * WebKit occasionally leaves a player-card image overlapping the league
  252 |    * pill row after a submit → return-to-home cycle, and an unbounded click
  253 |    * then retries against the intercepting <img> until the whole test times
  254 |    * out (observed: 240s hang on Mobile Safari). Bound the normal click,
  255 |    * retry after scrolling back to the top (which restores the row's hit
  256 |    * area), and only then fall back to a forced click.
  257 |    */
  258 |   async clickLeagueTab(btn: Locator): Promise<void> {
  259 |     try {
  260 |       await btn.click({ timeout: 10_000 });
  261 |       return;
  262 |     } catch {
  263 |       /* intercepted — try to restore the layout */
  264 |     }
  265 |     await this.page.evaluate(() => window.scrollTo(0, 0));
  266 |     try {
  267 |       await btn.click({ timeout: 10_000 });
  268 |       return;
  269 |     } catch {
  270 |       /* still intercepted — last resort below */
  271 |     }
  272 |     await btn.click({ force: true, timeout: 10_000 });
  273 |   }
  274 | 
  275 |   async listLeagueButtons(): Promise<Locator[]> {
  276 |     const n = await this.leagueButtons.count();
  277 |     const leagueButtonsLocator: Locator[] = [];
  278 |     for (let i = 0; i < n; i++) {
  279 |       leagueButtonsLocator.push(this.leagueButtons.nth(i));
  280 |     }
  281 |     return leagueButtonsLocator;
  282 |   }
  283 | 
  284 |   /**
  285 |    * "Is the current slip valid?" oracle used by pickPlayers. Mobile: the
  286 |    * Continue button. Desktop (DFS-2467): there is no Continue — the persistent
  287 |    * panel mounts the submission form (with `#place-pick`) once the slip is
  288 |    * playable and shows the "Let's Start" onboarding box otherwise. Without
  289 |    * this branch every desktop pick read as "Continue disabled" and the
  290 |    * deselect/replace loop threw "Unable to find replacement pick".
  291 |    */
  292 |   async isContinueEnabled(): Promise<boolean> {
  293 |     if (await this.continueBtn.isVisible().catch(() => false)) {
  294 |       return this.continueBtn.isEnabled().catch(() => false);
  295 |     }
  296 |     if (await this.placePickBtn.isVisible().catch(() => false)) {
  297 |       // Payout/metadata loading briefly disables place-pick right after a
  298 |       // pick lands — give that a moment before reading the slip as invalid.
  299 |       return expect(this.placePickBtn)
  300 |         .toBeEnabled({ timeout: 3_000 })
  301 |         .then(
  302 |           () => true,
  303 |           () => false
  304 |         );
  305 |     }
  306 |     return false;
  307 |   }
  308 | 
  309 |   async trySelectPick(card: Locator): Promise<boolean> {
  310 |     const buttons = this.pickButtons(card);
  311 |     const lessButton = buttons.first();
  312 |     // Bounded checks: league/stat filter updates run inside useTransition and
  313 |     // the grid is virtualised, so a card captured from listVisiblePlayerIds
```