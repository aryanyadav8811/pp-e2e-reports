# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: contests/user-enter-contest.spec.ts >> User Enter Contest >> Five player contest Submission @smoke
- Location: tests/contests/user-enter-contest.spec.ts:18:5

# Error details

```
Error: Could not place contest after 5 attempts (last error: 400 Entering this contest will cause you to exceed your daily contest limit.)

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
          - link "Parlay Play LogoParlay Play text" [ref=e6] [cursor=pointer]:
            - /url: /
            - generic [ref=e7]:
              - img "Parlay Play Logo" [ref=e8]
              - img "Parlay Play text" [ref=e9]
          - generic [ref=e11]:
            - generic [ref=e13]:
              - generic [ref=e14]: $1234.12
              - generic [ref=e15]:
                - img "gift-icon" [ref=e16]
                - text: "33.00"
            - button "Toggle Menu" [ref=e17]:
              - img [ref=e18]
      - main [ref=e20]:
        - generic [ref=e21]:
          - generic [ref=e23]:
            - generic [ref=e24]:
              - generic [ref=e25]:
                - list [ref=e27]:
                  - button "NBA" [ref=e28] [cursor=pointer]
                  - button "NBA-Combos" [ref=e29] [cursor=pointer]
                  - button "NBA Q1" [ref=e30] [cursor=pointer]
                  - button "NBA H1" [ref=e31] [cursor=pointer]
                  - button "MLB" [ref=e32] [cursor=pointer]
                  - button "MLB-Combos" [ref=e33] [cursor=pointer]
                  - button "NHL" [ref=e34] [cursor=pointer]
                  - button "EPL" [ref=e35] [cursor=pointer]
                  - button "CSGO" [ref=e36] [cursor=pointer]
                  - button "LoL" [ref=e37] [cursor=pointer]
                  - button "Valorant" [ref=e38] [cursor=pointer]
                  - button "Dota2" [ref=e39] [cursor=pointer]
                  - button "UFC" [ref=e40] [cursor=pointer]
                - list [ref=e42]:
                  - listitem [ref=e43]:
                    - button "ALL" [ref=e44] [cursor=pointer]:
                      - generic [ref=e45]: ALL
                  - listitem [ref=e46]:
                    - button "SAS@MIN 9:40PM" [ref=e47] [cursor=pointer]:
                      - text: SAS@MIN
                      - generic [ref=e48]: 9:40PM
                  - listitem [ref=e49]:
                    - button "DET@CLE 7:10PM" [ref=e50] [cursor=pointer]:
                      - text: DET@CLE
                      - generic [ref=e51]: 7:10PM
                - generic [ref=e52]:
                  - generic [ref=e53]:
                    - generic [ref=e56]:
                      - img [ref=e58]
                      - textbox "Search player or team" [ref=e60]
                    - button "Change card style from grid" [ref=e62]
                  - list [ref=e64]:
                    - listitem [ref=e65]:
                      - button "Points" [ref=e66]
                    - listitem [ref=e67]:
                      - button "Rebounds" [ref=e68]
                    - listitem [ref=e69]:
                      - button "Assists" [ref=e70]
                    - listitem [ref=e71]:
                      - button "Triple Double" [ref=e72]
                    - listitem [ref=e73]:
                      - button "3PT Made" [ref=e74]
                    - listitem [ref=e75]:
                      - button "Pts + Reb + Ast" [ref=e76]
                    - listitem [ref=e77]:
                      - button "Double Double" [ref=e78]
                    - listitem [ref=e79]:
                      - button "Pts + Reb" [ref=e80]
                    - listitem [ref=e81]:
                      - button "Pts + Ast" [ref=e82]
                    - listitem [ref=e83]:
                      - button "Reb + Ast" [ref=e84]
                    - listitem [ref=e85]:
                      - button "Stl + Blk" [ref=e86]
                    - listitem [ref=e87]:
                      - button "3PT Attempted" [ref=e88]
                    - listitem [ref=e89]:
                      - button "FT Made" [ref=e90]
                    - listitem [ref=e91]:
                      - button "FG Made" [ref=e92]
                    - listitem [ref=e93]:
                      - button "FG Attempted" [ref=e94]
                    - listitem [ref=e95]:
                      - button "Blocks" [ref=e96]
                    - listitem [ref=e97]:
                      - button "Steals" [ref=e98]
                    - listitem [ref=e99]:
                      - button "Fantasy Points" [ref=e100]
                    - listitem [ref=e101]:
                      - button "Turnovers" [ref=e102]
              - generic [ref=e103]:
                - generic [ref=e107]:
                  - button "previous slide / item" [ref=e108] [cursor=pointer]:
                    - img [ref=e109]
                  - list [ref=e112]:
                    - listitem [ref=e113]:
                      - generic [ref=e115] [cursor=pointer]:
                        - img "huddle-bg-small"
                        - generic [ref=e116]:
                          - generic [ref=e117]:
                            - generic [ref=e118]: Pistons
                            - generic [ref=e121]: VS
                            - generic [ref=e122]: Magic
                          - generic [ref=e123]: Huddle
                          - generic [ref=e124]:
                            - generic [ref=e125]:
                              - generic [ref=e126]:
                                - text: Win
                                - generic [ref=e127]: $1000
                              - generic [ref=e128]: + many more prizes
                            - button "Enter" [ref=e130]
                    - listitem [ref=e131]:
                      - 'button "Boosted Picks 🚀 Every Pick Pays: Up to a 35% Boost! lightning-bolt-yellow" [ref=e132] [cursor=pointer]':
                        - generic [ref=e133]:
                          - generic [ref=e135]: Boosted Picks 🚀
                          - generic [ref=e136]: "Every Pick Pays: Up to a 35% Boost!"
                        - img "lightning-bolt-yellow"
                    - listitem [ref=e137]:
                      - button "Get $20 By referring a friend making a first $10 deposit. lightning-bolt-yellow" [ref=e138] [cursor=pointer]:
                        - generic [ref=e139]:
                          - generic [ref=e141]: Get $20
                          - generic [ref=e142]: By referring a friend making a first $10 deposit.
                        - img "lightning-bolt-yellow"
                    - listitem [ref=e143]:
                      - generic [ref=e145] [cursor=pointer]:
                        - img "huddle-bg-small"
                        - generic [ref=e146]:
                          - generic [ref=e147]:
                            - generic [ref=e148]: Pistons
                            - generic [ref=e151]: VS
                            - generic [ref=e152]: Magic
                          - generic [ref=e153]: Huddle
                          - generic [ref=e154]:
                            - generic [ref=e155]:
                              - generic [ref=e156]:
                                - text: Win
                                - generic [ref=e157]: $1000
                              - generic [ref=e158]: + many more prizes
                            - button "Enter" [ref=e160]
                    - listitem [ref=e161]:
                      - 'button "Boosted Picks 🚀 Every Pick Pays: Up to a 35% Boost! lightning-bolt-yellow" [ref=e162] [cursor=pointer]':
                        - generic [ref=e163]:
                          - generic [ref=e165]: Boosted Picks 🚀
                          - generic [ref=e166]: "Every Pick Pays: Up to a 35% Boost!"
                        - img "lightning-bolt-yellow"
                  - button "next slide / item" [ref=e167] [cursor=pointer]:
                    - img [ref=e168]
                - generic [ref=e170]:
                  - generic [ref=e173]:
                    - generic [ref=e176]:
                      - button "Open expert opinion for James Harden" [ref=e177]:
                        - img [ref=e178]
                      - img "James Harden" [ref=e181]
                    - generic [ref=e182]:
                      - generic [ref=e183]: James Harden
                      - button "0.5 TD" [ref=e184]:
                        - generic [ref=e185]:
                          - img [ref=e186]
                          - img [ref=e188]
                        - generic [ref=e190]: "0.5"
                        - generic [ref=e191]: TD
                      - generic [ref=e192]:
                        - generic [ref=e193]: DET@CLE
                        - generic [ref=e194]: 7:10PM
                      - generic [ref=e195]:
                        - button "Select over 0.5 Triple Double for 0 times" [disabled] [ref=e196]
                        - button "Select over 0.5 Triple Double for 38.2 times" [ref=e198]:
                          - img [ref=e201]
                          - generic [ref=e203]: 38.2x
                          - img [ref=e204]
                  - generic [ref=e208]:
                    - generic [ref=e211]:
                      - button "Open expert opinion for Donovan Mitchell" [ref=e212]:
                        - img [ref=e213]
                      - img "Donovan Mitchell" [ref=e216]
                    - generic [ref=e217]:
                      - generic [ref=e218]: D. Mitchell
                      - button "0.5 TD" [ref=e219]:
                        - generic [ref=e220]:
                          - img [ref=e221]
                          - img [ref=e223]
                        - generic [ref=e225]: "0.5"
                        - generic [ref=e226]: TD
                      - generic [ref=e227]:
                        - generic [ref=e228]: DET@CLE
                        - generic [ref=e229]: 7:10PM
                      - generic [ref=e230]:
                        - button "Select over 0.5 Triple Double for 0 times" [disabled] [ref=e231]
                        - button "Select over 0.5 Triple Double for 56.2 times" [ref=e233]:
                          - img [ref=e236]
                          - generic [ref=e238]: 56.2x
                          - img [ref=e239]
                  - generic [ref=e243]:
                    - generic [ref=e246]:
                      - button "Open expert opinion for Evan Mobley" [ref=e247]:
                        - img [ref=e248]
                      - img "Evan Mobley" [ref=e251]
                    - generic [ref=e252]:
                      - generic [ref=e253]: Evan Mobley
                      - button "0.5 TD" [ref=e254]:
                        - generic [ref=e255]:
                          - img [ref=e256]
                          - img [ref=e258]
                        - generic [ref=e260]: "0.5"
                        - generic [ref=e261]: TD
                      - generic [ref=e262]:
                        - generic [ref=e263]: DET@CLE
                        - generic [ref=e264]: 7:10PM
                      - generic [ref=e265]:
                        - button "Select over 0.5 Triple Double for 0 times" [disabled] [ref=e266]
                        - button "Select over 0.5 Triple Double for 32.8 times" [ref=e268]:
                          - img [ref=e271]
                          - generic [ref=e273]: 32.8x
                          - img [ref=e274]
                  - generic [ref=e278]:
                    - generic [ref=e281]:
                      - button "Open expert opinion for Cade Cunningham" [ref=e282]:
                        - img [ref=e283]
                      - img "Cade Cunningham" [ref=e286]
                    - generic [ref=e287]:
                      - generic [ref=e288]: C. Cunningham
                      - button "0.5 TD" [ref=e289]:
                        - generic [ref=e290]:
                          - img [ref=e291]
                          - img [ref=e293]
                        - generic [ref=e295]: "0.5"
                        - generic [ref=e296]: TD
                      - generic [ref=e297]:
                        - generic [ref=e298]: DET@CLE
                        - generic [ref=e299]: 7:10PM
                      - generic [ref=e300]:
                        - button "Select over 0.5 Triple Double for 0 times" [disabled] [ref=e301]
                        - button "Select over 0.5 Triple Double for 11.08 times" [ref=e303]:
                          - img [ref=e306]
                          - generic [ref=e308]: 11.08x
                          - img [ref=e309]
                  - generic [ref=e313]:
                    - generic [ref=e316]:
                      - button "Open expert opinion for Ausar Thompson" [ref=e317]:
                        - img [ref=e318]
                      - img "Ausar Thompson" [ref=e321]
                    - generic [ref=e322]:
                      - generic [ref=e323]: A. Thompson
                      - button "0.5 TD" [ref=e324]:
                        - generic [ref=e325]:
                          - img [ref=e326]
                          - img [ref=e328]
                        - generic [ref=e330]: "0.5"
                        - generic [ref=e331]: TD
                      - generic [ref=e332]:
                        - generic [ref=e333]: DET@CLE
                        - generic [ref=e334]: 7:10PM
                      - generic [ref=e335]:
                        - button "Select over 0.5 Triple Double for 0 times" [disabled] [ref=e336]
                        - button "Select over 0.5 Triple Double for 55 times" [ref=e338]:
                          - img [ref=e341]
                          - generic [ref=e343]: 55x
                          - img [ref=e344]
                  - generic [ref=e348]:
                    - generic [ref=e351]:
                      - button "Open expert opinion for Stephon Castle" [ref=e352]:
                        - img [ref=e353]
                      - img "Stephon Castle" [ref=e356]
                    - generic [ref=e357]:
                      - generic [ref=e358]: S. Castle
                      - button "0.5 TD" [ref=e359]:
                        - generic [ref=e360]:
                          - img [ref=e361]
                          - img [ref=e363]
                        - generic [ref=e365]: "0.5"
                        - generic [ref=e366]: TD
                      - generic [ref=e367]:
                        - generic [ref=e368]: SAS@MIN
                        - generic [ref=e369]: 9:40PM
                      - generic [ref=e370]:
                        - button "Select over 0.5 Triple Double for 0 times" [disabled] [ref=e371]
                        - button "Select over 0.5 Triple Double for 25 times" [ref=e373]:
                          - generic [ref=e374]: 25x
                          - img [ref=e375]
                  - generic [ref=e379]:
                    - generic [ref=e382]:
                      - button "Open expert opinion for Victor Wembanyama" [ref=e383]:
                        - img [ref=e384]
                      - img "Victor Wembanyama" [ref=e387]
                    - generic [ref=e388]:
                      - generic [ref=e389]: V. Wembanyama
                      - button "0.5 TD" [ref=e390]:
                        - generic [ref=e391]:
                          - img [ref=e392]
                          - img [ref=e394]
                        - generic [ref=e396]: "0.5"
                        - generic [ref=e397]: TD
                      - generic [ref=e398]:
                        - generic [ref=e399]: SAS@MIN
                        - generic [ref=e400]: 9:40PM
                      - generic [ref=e401]:
                        - button "Select over 0.5 Triple Double for 0 times" [disabled] [ref=e402]
                        - button "Select over 0.5 Triple Double for 31.9 times" [ref=e404]:
                          - generic [ref=e405]: 31.9x
                          - img [ref=e406]
                  - generic [ref=e410]:
                    - generic [ref=e413]:
                      - button "Open expert opinion for Anthony Edwards" [ref=e414]:
                        - img [ref=e415]
                      - img "Anthony Edwards" [ref=e418]
                    - generic [ref=e419]:
                      - generic [ref=e420]: A. Edwards
                      - button "0.5 TD" [ref=e421]:
                        - generic [ref=e422]:
                          - img [ref=e423]
                          - img [ref=e425]
                        - generic [ref=e427]: "0.5"
                        - generic [ref=e428]: TD
                      - generic [ref=e429]:
                        - generic [ref=e430]: SAS@MIN
                        - generic [ref=e431]: 9:40PM
                      - generic [ref=e432]:
                        - button "Select over 0.5 Triple Double for 0 times" [disabled] [ref=e433]
                        - button "Select over 0.5 Triple Double for 42.4 times" [ref=e435]:
                          - generic [ref=e436]: 42.4x
                          - img [ref=e437]
                  - generic [ref=e441]:
                    - generic [ref=e444]:
                      - button "Open expert opinion for Julius Randle" [ref=e445]:
                        - img [ref=e446]
                      - img "Julius Randle" [ref=e449]
                    - generic [ref=e450]:
                      - generic [ref=e451]: Julius Randle
                      - button "0.5 TD" [ref=e452]:
                        - generic [ref=e453]:
                          - img [ref=e454]
                          - img [ref=e456]
                        - generic [ref=e458]: "0.5"
                        - generic [ref=e459]: TD
                      - generic [ref=e460]:
                        - generic [ref=e461]: SAS@MIN
                        - generic [ref=e462]: 9:40PM
                      - generic [ref=e463]:
                        - button "Select over 0.5 Triple Double for 0 times" [disabled] [ref=e464]
                        - button "Select over 0.5 Triple Double for 34.6 times" [ref=e466]:
                          - generic [ref=e467]: 34.6x
                          - img [ref=e468]
              - generic [ref=e471]:
                - generic [ref=e472]:
                  - img [ref=e474]
                  - generic [ref=e476]:
                    - generic [ref=e477]: 1000.00x
                    - generic [ref=e492]: 5 picks
                  - button "Continue" [ref=e493] [cursor=pointer]
                - generic [ref=e494]:
                  - generic [ref=e495]:
                    - generic [ref=e496]: Your Selection
                    - generic [ref=e497]:
                      - generic [ref=e498]:
                        - generic [ref=e499]:
                          - img [ref=e500]
                          - generic [ref=e502]:
                            - text: J. Harden (0.5 Triple Double - More - FG)
                            - generic [ref=e503]: 38.2x
                        - img [ref=e505]
                      - generic [ref=e507]:
                        - generic [ref=e508]:
                          - img [ref=e509]
                          - generic [ref=e511]:
                            - text: D. Mitchell (0.5 Triple Double - More - FG)
                            - generic [ref=e512]: 56.2x
                        - img [ref=e514]
                      - generic [ref=e516]:
                        - generic [ref=e517]:
                          - img [ref=e518]
                          - generic [ref=e520]:
                            - text: E. Mobley (0.5 Triple Double - More - FG)
                            - generic [ref=e521]: 32.8x
                        - img [ref=e523]
                      - generic [ref=e525]:
                        - generic [ref=e526]:
                          - img [ref=e527]
                          - generic [ref=e529]:
                            - text: C. Cunningham (0.5 Triple Double - More - FG)
                            - generic [ref=e530]: 11.08x
                        - img [ref=e532]
                      - generic [ref=e534]:
                        - generic [ref=e535]:
                          - img [ref=e536]
                          - generic [ref=e538]:
                            - text: A. Thompson (0.5 Triple Double - More - FG)
                            - generic [ref=e539]: 55x
                        - img [ref=e541]
                  - generic [ref=e543]:
                    - img [ref=e544]
                    - generic [ref=e546]: Clear All
              - generic [ref=e548]:
                - generic [ref=e549]:
                  - button [ref=e550]:
                    - img [ref=e551]
                  - generic [ref=e553]: Make Your More/Less Picks
                - generic [ref=e554]:
                  - generic [ref=e556]:
                    - img "James Harden" [ref=e558]
                    - generic [ref=e559]:
                      - paragraph [ref=e560]: James Harden
                      - paragraph [ref=e561]:
                        - generic [ref=e562]: CLE
                        - text: "- DET"
                      - paragraph [ref=e563]: Today 7:10 PM
                    - generic [ref=e564]:
                      - paragraph [ref=e565]:
                        - text: "0.5"
                        - generic [ref=e566]: TD
                      - generic [ref=e567]:
                        - button "Less" [disabled] [ref=e568]:
                          - generic [ref=e569]: Less
                        - button "More 38.2 x" [ref=e570]:
                          - generic [ref=e571]: More
                          - generic [ref=e572]: 38.2 x
                    - button [ref=e573]:
                      - img [ref=e574]
                  - generic [ref=e578]:
                    - img "Donovan Mitchell" [ref=e580]
                    - generic [ref=e581]:
                      - paragraph [ref=e582]: Donovan Mitchell
                      - paragraph [ref=e583]:
                        - generic [ref=e584]: CLE
                        - text: "- DET"
                      - paragraph [ref=e585]: Today 7:10 PM
                    - generic [ref=e586]:
                      - paragraph [ref=e587]:
                        - text: "0.5"
                        - generic [ref=e588]: TD
                      - generic [ref=e589]:
                        - button "Less" [disabled] [ref=e590]:
                          - generic [ref=e591]: Less
                        - button "More 56.2 x" [ref=e592]:
                          - generic [ref=e593]: More
                          - generic [ref=e594]: 56.2 x
                    - button [ref=e595]:
                      - img [ref=e596]
                  - generic [ref=e600]:
                    - img "Evan Mobley" [ref=e602]
                    - generic [ref=e603]:
                      - paragraph [ref=e604]: Evan Mobley
                      - paragraph [ref=e605]:
                        - generic [ref=e606]: CLE
                        - text: "- DET"
                      - paragraph [ref=e607]: Today 7:10 PM
                    - generic [ref=e608]:
                      - paragraph [ref=e609]:
                        - text: "0.5"
                        - generic [ref=e610]: TD
                      - generic [ref=e611]:
                        - button "Less" [disabled] [ref=e612]:
                          - generic [ref=e613]: Less
                        - button "More 32.8 x" [ref=e614]:
                          - generic [ref=e615]: More
                          - generic [ref=e616]: 32.8 x
                    - button [ref=e617]:
                      - img [ref=e618]
                  - generic [ref=e622]:
                    - img "Cade Cunningham" [ref=e624]
                    - generic [ref=e625]:
                      - paragraph [ref=e626]: Cade Cunningham
                      - paragraph [ref=e627]:
                        - generic [ref=e628]: DET
                        - text: "- CLE"
                      - paragraph [ref=e629]: Today 7:10 PM
                    - generic [ref=e630]:
                      - paragraph [ref=e631]:
                        - text: "0.5"
                        - generic [ref=e632]: TD
                      - generic [ref=e633]:
                        - button "Less" [disabled] [ref=e634]:
                          - generic [ref=e635]: Less
                        - button "More 11.08 x" [ref=e636]:
                          - generic [ref=e637]: More
                          - generic [ref=e638]: 11.08 x
                    - button [ref=e639]:
                      - img [ref=e640]
                  - generic [ref=e644]:
                    - img "Ausar Thompson" [ref=e646]
                    - generic [ref=e647]:
                      - paragraph [ref=e648]: Ausar Thompson
                      - paragraph [ref=e649]:
                        - generic [ref=e650]: DET
                        - text: "- CLE"
                      - paragraph [ref=e651]: Today 7:10 PM
                    - generic [ref=e652]:
                      - paragraph [ref=e653]:
                        - text: "0.5"
                        - generic [ref=e654]: TD
                      - generic [ref=e655]:
                        - button "Less" [disabled] [ref=e656]:
                          - generic [ref=e657]: Less
                        - button "More 55 x" [ref=e658]:
                          - generic [ref=e659]: More
                          - generic [ref=e660]: 55 x
                    - button [ref=e661]:
                      - img [ref=e662]
                  - button "+ Add Player" [ref=e666] [cursor=pointer]
                - generic [ref=e668]:
                  - generic [ref=e669]:
                    - generic [ref=e671]:
                      - radio
                      - generic [ref=e672] [cursor=pointer]: $25
                      - radio
                      - generic [ref=e673] [cursor=pointer]: $75
                      - radio
                      - generic [ref=e674] [cursor=pointer]: $300
                    - generic [ref=e676]:
                      - generic [ref=e677]: $
                      - spinbutton [ref=e681]: "3"
                    - button "17" [ref=e682] [cursor=pointer]:
                      - img [ref=e683]
                      - generic [ref=e685]: "17"
                  - generic [ref=e686]:
                    - generic [ref=e687]:
                      - generic [ref=e688]:
                        - button [ref=e689]:
                          - img [ref=e690]
                        - button "All In" [ref=e692]
                      - generic [ref=e694]: 1000x
                    - generic [ref=e696]:
                      - generic [ref=e697]:
                        - paragraph [ref=e698]: Perfect line-up
                        - paragraph [ref=e699]: $3,000
                      - generic [ref=e701]:
                        - paragraph [ref=e702]: Or 1st place in group
                        - generic [ref=e703]: $5 + $3,000
                  - button "Place" [ref=e707] [cursor=pointer]:
                    - text: Place
                    - img [ref=e708]
            - generic [ref=e711]:
              - generic [ref=e713]:
                - link "Download ParlayPlay On The Play Store" [ref=e714] [cursor=pointer]:
                  - /url: https://parlayplay.onelink.me/oLJk/fh7u6juo
                  - img "Download ParlayPlay On The Play Store" [ref=e715]
                - paragraph [ref=e716]:
                  - text: Get the app.
                  - text: Better. Faster. Convenient
              - navigation [ref=e717]:
                - link "Privacy" [ref=e718] [cursor=pointer]:
                  - /url: /privacy-policy
                - link "Terms" [ref=e719] [cursor=pointer]:
                  - /url: /terms
                - link "Responsible Gaming" [ref=e720] [cursor=pointer]:
                  - /url: /responsible-gaming
                - link "Gaming Rules" [ref=e721] [cursor=pointer]:
                  - /url: /rules
                - link "FAQ" [ref=e722] [cursor=pointer]:
                  - /url: https://intercom.help/parlayplay/en/
              - navigation [ref=e723]:
                - generic [ref=e724]:
                  - paragraph [ref=e725]: © ParlayPlay 2026
                  - generic [ref=e726]:
                    - link [ref=e727] [cursor=pointer]:
                      - /url: https://www.facebook.com/parlayplay.io
                      - img [ref=e728]
                    - link [ref=e730] [cursor=pointer]:
                      - /url: https://www.instagram.com/parlayplay_?igsh=bHBldWQyMmV2b3Y4
                      - img [ref=e731]
                    - link [ref=e733] [cursor=pointer]:
                      - /url: https://www.twitter.com/parlay_play
                      - img [ref=e734]
                    - link [ref=e736] [cursor=pointer]:
                      - /url: https://discord.com/invite/parlayplay
                      - img [ref=e737]
                  - img "Under 18 Logo" [ref=e739]
          - generic [ref=e741]:
            - button [ref=e742]
            - dialog "User Limit Exceeded" [ref=e744]:
              - generic [ref=e745]:
                - generic [ref=e746]:
                  - img [ref=e748]
                  - button [active] [ref=e750]:
                    - img [ref=e751]
                - heading "User Limit Exceeded" [level=1] [ref=e753]
                - heading "Daily Amount Limit" [level=1] [ref=e754]
                - generic [ref=e755]:
                  - paragraph [ref=e756]: Placing this contest will cause you to exceed your Daily Amount Limit
                  - generic [ref=e757]:
                    - paragraph [ref=e758]:
                      - strong [ref=e759]: "Current limit:"
                      - text: $5
                    - paragraph [ref=e760]:
                      - strong [ref=e761]: "Can reset to:"
                      - text: $5,000
                  - paragraph [ref=e762]: Click the button below to change your limits or to reset them back to the defaults.
                  - generic [ref=e763]:
                    - button "Go to Settings" [ref=e764] [cursor=pointer]
                    - button "Reset Limits" [ref=e765] [cursor=pointer]
    - region "Notifications Alt+T"
  - alert [ref=e766]
  - iframe [ref=e767]:
    
```

# Test source

```ts
  2   | import type { ContestPage } from '../pages/contest.page';
  3   | import type { HomePage } from '../pages/home.page';
  4   | 
  5   | export interface PlaceContestWithRetryOptions {
  6   |     homePage: HomePage;
  7   |     contestPage: ContestPage;
  8   |     pickCount: number;
  9   |     entryAmount: number;
  10  |     /**
  11  |      * Max attempts before giving up. Falls back to the `CONTEST_RETRY_ATTEMPTS`
  12  |      * env var so each environment (local/dev/staging) can tune how many stat
  13  |      * rotations to try before failing. Defaults to 3.
  14  |      */
  15  |     maxAttempts?: number;
  16  |     /**
  17  |      * Submission step. Runs after picks are selected and the entry amount is set.
  18  |      * Return `{ success: false, error }` to trigger a retry on a different stat tab.
  19  |      * Defaults to `contestPage.submitAndAwaitResult()`.
  20  |      */
  21  |     submit?: () => Promise<{ success: boolean; error: string | null }>;
  22  | }
  23  | 
  24  | function resolveMaxAttempts(explicit?: number): number {
  25  |     if (explicit !== undefined) return explicit;
  26  |     const raw = process.env.CONTEST_RETRY_ATTEMPTS;
  27  |     if (!raw) return 5;
  28  |     const parsed = parseInt(raw, 10);
  29  |     return Number.isFinite(parsed) && parsed > 0 ? parsed : 5;
  30  | }
  31  | 
  32  | function isThrottleError(err: string | null): boolean {
  33  |     return /\b429\b|throttled|too many requests/i.test(err ?? "");
  34  | }
  35  | 
  36  | // DRF emits "Expected available in N second(s)". Parse that and wait at least
  37  | // that long, capped to keep a single throttle from eating the whole suite.
  38  | function throttleBackoffMs(err: string | null): number {
  39  |     const match = (err ?? "").match(/in\s+(\d+)\s+second/i);
  40  |     const seconds = match ? parseInt(match[1], 10) : 0;
  41  |     const buffered = Math.max(seconds, 10) + 3;
  42  |     return Math.min(buffered, 30) * 1000;
  43  | }
  44  | 
  45  | export interface PlaceContestWithRetryResult {
  46  |     /** Picks from the successful attempt. */
  47  |     pickIds: string[];
  48  | }
  49  | 
  50  | /**
  51  |  * Picks N players, advances to the contest page, and submits — retrying on
  52  |  * a different stat tab when a user limit (or other submission error) trips.
  53  |  *
  54  |  * Used by both the contest-submission specs and the slip-sharing flow, since
  55  |  * any user can hit a per-stat limit on the first try.
  56  |  */
  57  | export async function placeContestWithRetry(
  58  |     opts: PlaceContestWithRetryOptions,
  59  | ): Promise<PlaceContestWithRetryResult> {
  60  |     const { homePage, contestPage, pickCount, entryAmount } = opts;
  61  |     const maxAttempts = resolveMaxAttempts(opts.maxAttempts);
  62  |     const submit = opts.submit ?? (() => contestPage.submitAndAwaitResult());
  63  | 
  64  |     let pickIds: string[] = [];
  65  |     let placed = false;
  66  |     let lastError: string | null = null;
  67  |     let statIdx = 0;
  68  | 
  69  |     for (let attempt = 1; attempt <= maxAttempts && !placed; attempt++) {
  70  |         if (attempt > 1) {
  71  |             // Always reset back to home — pickPlayers below needs the grid.
  72  |             // But only rotate the stat tab on a per-stat user limit. On a 429,
  73  |             // the picks were fine; rotating wastes stat tabs (we can run out
  74  |             // before the throttle window even closes), so we sleep instead.
  75  |             await homePage.clearSlip();
  76  |             if (isThrottleError(lastError)) {
  77  |                 await new Promise((r) => setTimeout(r, throttleBackoffMs(lastError)));
  78  |             } else {
  79  |                 statIdx++;
  80  |             }
  81  |         }
  82  |         await homePage.waitForPlayersGrid();
  83  |         pickIds = await homePage.pickPlayers(
  84  |             pickCount,
  85  |             attempt > 1 ? statIdx : undefined,
  86  |         );
  87  |         await homePage.enterFinalContestPage();
  88  |         await contestPage.verifyPage();
  89  |         await contestPage.setEntryAmountIfEditable(entryAmount);
  90  | 
  91  |         const result = await submit();
  92  |         if (!result.success) {
  93  |             lastError = result.error;
  94  |             continue;
  95  |         }
  96  |         placed = true;
  97  |     }
  98  | 
  99  |     expect(
  100 |         placed,
  101 |         `Could not place contest after ${maxAttempts} attempts (last error: ${lastError})`,
> 102 |     ).toBe(true);
      |       ^ Error: Could not place contest after 5 attempts (last error: 400 Entering this contest will cause you to exceed your daily contest limit.)
  103 | 
  104 |     return { pickIds };
  105 | }
  106 | 
```