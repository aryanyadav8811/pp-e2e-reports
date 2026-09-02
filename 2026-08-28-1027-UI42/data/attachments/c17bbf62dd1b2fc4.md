# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: packs/opening-iframe.spec.ts >> Pack opening iframe (DFS-2087 / DFS-2169) >> Buy launches the Repackz opening iframe with a close bar
- Location: tests/packs/opening-iframe.spec.ts:25:5

# Error details

```
Test timeout of 300000ms exceeded.
```

```
Error: locator.click: Target page, context or browser has been closed
Call log:
  - waiting for getByRole('button', { name: /^Buy for \$/ }).filter({ visible: true }).first()
    - locator resolved to <button disabled type="button" class="flex-1 rounded-lg bg-playYellow px-6 py-2.5 text-base font-museo text-black hover:brightness-95 transition disabled:opacity-60">Buy for $25</button>
  - attempting click action
    2 × waiting for element to be visible, enabled and stable
      - element is not enabled
    - retrying click action
    - waiting 20ms
    2 × waiting for element to be visible, enabled and stable
      - element is not enabled
    - retrying click action
      - waiting 100ms
    567 × waiting for element to be visible, enabled and stable
        - element is not enabled
      - retrying click action
        - waiting 500ms

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
          - generic [ref=e10]:
            - generic [ref=e12]:
              - generic [ref=e13]: $0.00
              - generic [ref=e14]:
                - img "gift-icon" [ref=e15]
                - text: "38.00"
            - button "Toggle Menu" [ref=e16]:
              - img [ref=e17]
      - main [ref=e19]:
        - generic [ref=e22]:
          - link "Back" [ref=e23] [cursor=pointer]:
            - /url: /packs
            - img [ref=e24]
            - generic [ref=e26]: Back
          - img "Multi-Sport Starter Pack" [ref=e28]
          - heading "Multi-Sport Starter Pack" [level=1] [ref=e29]
          - paragraph [ref=e30]: "Card value: $13.00 – $400.00"
          - paragraph [ref=e31]: Every pack contains one authentic graded card. Keep it or sell it back for 100% Fair Market Value.
          - generic [ref=e32]:
            - button "Odds" [ref=e33]:
              - img [ref=e34]
              - text: Odds
            - button "How it works" [ref=e36]:
              - img [ref=e37]
              - text: How it works
          - generic [ref=e39]:
            - generic [ref=e40]:
              - generic [ref=e41]:
                - generic [ref=e42]:
                  - img [ref=e43]
                  - generic [ref=e45]: Insufficient funds
                - generic [ref=e46]: "Your balance: $0.00"
              - link "Deposit now" [ref=e48] [cursor=pointer]:
                - /url: /payments/deposit
                - button "Deposit now" [ref=e49]
            - button "Buy for $25" [disabled] [ref=e51]
          - region "More packs" [ref=e52]:
            - heading "More Packs" [level=2] [ref=e53]
            - generic [ref=e54]:
              - link "MAX PULL $1,000 Multi-Sport Premier Pack Multi-Sport Premier Pack $50" [ref=e56] [cursor=pointer]:
                - /url: /packs/pack/10
                - generic [ref=e57]: MAX PULL $1,000
                - img "Multi-Sport Premier Pack" [ref=e59]
                - generic [ref=e60]:
                  - heading "Multi-Sport Premier Pack" [level=3] [ref=e61]
                  - paragraph [ref=e62]: $50
              - link "MAX PULL $3,500 Multi-Sport Pro Pack Multi-Sport Pro Pack $100" [ref=e64] [cursor=pointer]:
                - /url: /packs/pack/11
                - generic [ref=e65]: MAX PULL $3,500
                - img "Multi-Sport Pro Pack" [ref=e67]
                - generic [ref=e68]:
                  - heading "Multi-Sport Pro Pack" [level=3] [ref=e69]
                  - paragraph [ref=e70]: $100
              - link "MAX PULL $7,500 Multi-Sport Elite Pack Multi-Sport Elite Pack $250" [ref=e72] [cursor=pointer]:
                - /url: /packs/pack/12
                - generic [ref=e73]: MAX PULL $7,500
                - generic [ref=e74]:
                  - img "Multi-Sport Elite Pack"
                - generic [ref=e75]:
                  - heading "Multi-Sport Elite Pack" [level=3] [ref=e76]
                  - paragraph [ref=e77]: $250
          - region "Potential Hits" [ref=e78]:
            - heading "Potential Hits" [level=2] [ref=e79]
            - generic [ref=e80]:
              - button "2015 UPPER DECK CONNOR McDAVID 201 PSA 10 $2376.00 est. 2015 UPPER DECK CONNOR McDAVID 201 PSA 10" [ref=e81]:
                - generic [ref=e82]:
                  - img "2015 UPPER DECK CONNOR McDAVID 201 PSA 10" [ref=e83]
                  - generic [ref=e84]: $2376.00 est.
                - generic [ref=e85]: 2015 UPPER DECK CONNOR McDAVID 201 PSA 10
              - button "2023 TOPPS CHROME UEFA CLUB COMPETITIONS GOLD GEOMETRIC REFRACTOR LAMINE YAMAL 64 PSA 9 $2250.00 est. 2023 TOPPS CHROME UEFA CLUB COMPETITIONS GOLD GEOMETRIC REFRACTOR LAMINE YAMAL 64 PSA 9" [ref=e86]:
                - generic [ref=e87]:
                  - img "2023 TOPPS CHROME UEFA CLUB COMPETITIONS GOLD GEOMETRIC REFRACTOR LAMINE YAMAL 64 PSA 9" [ref=e88]
                  - generic [ref=e89]: $2250.00 est.
                - generic [ref=e90]: 2023 TOPPS CHROME UEFA CLUB COMPETITIONS GOLD GEOMETRIC REFRACTOR LAMINE YAMAL 64 PSA 9
              - button "2012 PANINI ROOKIE ANTHOLOGY PRIZM PRIZM-GOLD TEEMU SELANNE 1 PSA 10 $1984.50 est. 2012 PANINI ROOKIE ANTHOLOGY PRIZM PRIZM-GOLD TEEMU SELANNE 1 PSA 10" [ref=e91]:
                - generic [ref=e92]:
                  - img "2012 PANINI ROOKIE ANTHOLOGY PRIZM PRIZM-GOLD TEEMU SELANNE 1 PSA 10" [ref=e93]
                  - generic [ref=e94]: $1984.50 est.
                - generic [ref=e95]: 2012 PANINI ROOKIE ANTHOLOGY PRIZM PRIZM-GOLD TEEMU SELANNE 1 PSA 10
              - button "2005 UPPER DECK ALEXANDER OVECHKIN 443 PSA 9 $1405.80 est. 2005 UPPER DECK ALEXANDER OVECHKIN 443 PSA 9" [ref=e96]:
                - generic [ref=e97]:
                  - img "2005 UPPER DECK ALEXANDER OVECHKIN 443 PSA 9" [ref=e98]
                  - generic [ref=e99]: $1405.80 est.
                - generic [ref=e100]: 2005 UPPER DECK ALEXANDER OVECHKIN 443 PSA 9
              - button "2003 NETPRO ELITE 2000 RAFAEL NADAL 19 PSA 10 $899.91 est. 2003 NETPRO ELITE 2000 RAFAEL NADAL 19 PSA 10" [ref=e101]:
                - generic [ref=e102]:
                  - img "2003 NETPRO ELITE 2000 RAFAEL NADAL 19 PSA 10" [ref=e103]
                  - generic [ref=e104]: $899.91 est.
                - generic [ref=e105]: 2003 NETPRO ELITE 2000 RAFAEL NADAL 19 PSA 10
              - button "2025 PANINI DONRUSS DOWNTOWN SAQUON BARKLEY 7 PSA 10 $831.60 est. 2025 PANINI DONRUSS DOWNTOWN SAQUON BARKLEY 7 PSA 10" [ref=e106]:
                - generic [ref=e107]:
                  - img "2025 PANINI DONRUSS DOWNTOWN SAQUON BARKLEY 7 PSA 10" [ref=e108]
                  - generic [ref=e109]: $831.60 est.
                - generic [ref=e110]: 2025 PANINI DONRUSS DOWNTOWN SAQUON BARKLEY 7 PSA 10
              - button "2009 TOPPS UFC ROUND 1 SILVER A.SILVA/C.LEBEN 46 PSA 8 $816.75 est. 2009 TOPPS UFC ROUND 1 SILVER A.SILVA/C.LEBEN 46 PSA 8" [ref=e111]:
                - generic [ref=e112]:
                  - img "2009 TOPPS UFC ROUND 1 SILVER A.SILVA/C.LEBEN 46 PSA 8" [ref=e113]
                  - generic [ref=e114]: $816.75 est.
                - generic [ref=e115]: 2009 TOPPS UFC ROUND 1 SILVER A.SILVA/C.LEBEN 46 PSA 8
              - button "2013 BBM ROOKIE EDITION THEN & NOW THEN & NOW S.OHTANI/M.YOSHIKAWA 90 PSA 10 $792.00 est. 2013 BBM ROOKIE EDITION THEN & NOW THEN & NOW S.OHTANI/M.YOSHIKAWA 90 PSA 10" [ref=e116]:
                - generic [ref=e117]:
                  - img "2013 BBM ROOKIE EDITION THEN & NOW THEN & NOW S.OHTANI/M.YOSHIKAWA 90 PSA 10" [ref=e118]
                  - generic [ref=e119]: $792.00 est.
                - generic [ref=e120]: 2013 BBM ROOKIE EDITION THEN & NOW THEN & NOW S.OHTANI/M.YOSHIKAWA 90 PSA 10
              - button "2023 TOPPS ECCELLENZA FORMULA 1 TRIONFO-RED LANDO NORRIS PSA 10 $792.00 est. 2023 TOPPS ECCELLENZA FORMULA 1 TRIONFO-RED LANDO NORRIS PSA 10" [ref=e121]:
                - generic [ref=e122]:
                  - img "2023 TOPPS ECCELLENZA FORMULA 1 TRIONFO-RED LANDO NORRIS PSA 10" [ref=e123]
                  - generic [ref=e124]: $792.00 est.
                - generic [ref=e125]: 2023 TOPPS ECCELLENZA FORMULA 1 TRIONFO-RED LANDO NORRIS PSA 10
              - button "2024 PANINI PRIZM BLACK BLUE SHIMMER FOTL JALEN BRUNSON 160 PSA 10 $742.50 est. 2024 PANINI PRIZM BLACK BLUE SHIMMER FOTL JALEN BRUNSON 160 PSA 10" [ref=e126]:
                - generic [ref=e127]:
                  - img "2024 PANINI PRIZM BLACK BLUE SHIMMER FOTL JALEN BRUNSON 160 PSA 10" [ref=e128]
                  - generic [ref=e129]: $742.50 est.
                - generic [ref=e130]: 2024 PANINI PRIZM BLACK BLUE SHIMMER FOTL JALEN BRUNSON 160 PSA 10
              - button "2024 PANINI PRIZM CONMEBOL COPA AMERICA SCORERS CLUB SCORERS CLUB-GOLD PRIZM PELE 26 PSA 10 $693.00 est. 2024 PANINI PRIZM CONMEBOL COPA AMERICA SCORERS CLUB SCORERS CLUB-GOLD PRIZM PELE 26 PSA 10" [ref=e131]:
                - generic [ref=e132]:
                  - img "2024 PANINI PRIZM CONMEBOL COPA AMERICA SCORERS CLUB SCORERS CLUB-GOLD PRIZM PELE 26 PSA 10" [ref=e133]
                  - generic [ref=e134]: $693.00 est.
                - generic [ref=e135]: 2024 PANINI PRIZM CONMEBOL COPA AMERICA SCORERS CLUB SCORERS CLUB-GOLD PRIZM PELE 26 PSA 10
              - button "2025 PANINI DONRUSS DOWNTOWN TETAIROA MCMILLAN 15 PSA 10 $668.25 est. 2025 PANINI DONRUSS DOWNTOWN TETAIROA MCMILLAN 15 PSA 10" [ref=e136]:
                - generic [ref=e137]:
                  - img "2025 PANINI DONRUSS DOWNTOWN TETAIROA MCMILLAN 15 PSA 10" [ref=e138]
                  - generic [ref=e139]: $668.25 est.
                - generic [ref=e140]: 2025 PANINI DONRUSS DOWNTOWN TETAIROA MCMILLAN 15 PSA 10
              - button "2025 PANINI DONRUSS DOWNTOWN CEEDEE LAMB 9 PSA 10 $613.80 est. 2025 PANINI DONRUSS DOWNTOWN CEEDEE LAMB 9 PSA 10" [ref=e141]:
                - generic [ref=e142]:
                  - img "2025 PANINI DONRUSS DOWNTOWN CEEDEE LAMB 9 PSA 10" [ref=e143]
                  - generic [ref=e144]: $613.80 est.
                - generic [ref=e145]: 2025 PANINI DONRUSS DOWNTOWN CEEDEE LAMB 9 PSA 10
              - button "2024 PANINI PRIZM CONMEBOL COPA AMERICA BLUE WAVE LIONEL MESSI 1 PSA 10 $603.90 est. 2024 PANINI PRIZM CONMEBOL COPA AMERICA BLUE WAVE LIONEL MESSI 1 PSA 10" [ref=e146]:
                - generic [ref=e147]:
                  - img "2024 PANINI PRIZM CONMEBOL COPA AMERICA BLUE WAVE LIONEL MESSI 1 PSA 10" [ref=e148]
                  - generic [ref=e149]: $603.90 est.
                - generic [ref=e150]: 2024 PANINI PRIZM CONMEBOL COPA AMERICA BLUE WAVE LIONEL MESSI 1 PSA 10
              - button "2023 PANINI PRIZM UFC FEARLESS FEARLESS-GREEN PULSAR ALEX PEREIRA 25 PSA 10 $543.38 est. 2023 PANINI PRIZM UFC FEARLESS FEARLESS-GREEN PULSAR ALEX PEREIRA 25 PSA 10" [ref=e151]:
                - generic [ref=e152]:
                  - img "2023 PANINI PRIZM UFC FEARLESS FEARLESS-GREEN PULSAR ALEX PEREIRA 25 PSA 10" [ref=e153]
                  - generic [ref=e154]: $543.38 est.
                - generic [ref=e155]: 2023 PANINI PRIZM UFC FEARLESS FEARLESS-GREEN PULSAR ALEX PEREIRA 25 PSA 10
              - button "2017 TOPPS FIRE AARON JUDGE 62 PSA 10 $495.00 est. 2017 TOPPS FIRE AARON JUDGE 62 PSA 10" [ref=e156]:
                - generic [ref=e157]:
                  - img "2017 TOPPS FIRE AARON JUDGE 62 PSA 10" [ref=e158]
                  - generic [ref=e159]: $495.00 est.
                - generic [ref=e160]: 2017 TOPPS FIRE AARON JUDGE 62 PSA 10
              - button "2024 PANINI PHOENIX COLOR BLAST MARVIN HARRISON JR. CBMHJ PSA 10 $495.00 est. 2024 PANINI PHOENIX COLOR BLAST MARVIN HARRISON JR. CBMHJ PSA 10" [ref=e161]:
                - generic [ref=e162]:
                  - img "2024 PANINI PHOENIX COLOR BLAST MARVIN HARRISON JR. CBMHJ PSA 10" [ref=e163]
                  - generic [ref=e164]: $495.00 est.
                - generic [ref=e165]: 2024 PANINI PHOENIX COLOR BLAST MARVIN HARRISON JR. CBMHJ PSA 10
              - button "2017 TOPPS CHROME 1987 TOPPS 1987 TOPPS AARON JUDGE 87T8 PSA 10 $445.50 est. 2017 TOPPS CHROME 1987 TOPPS 1987 TOPPS AARON JUDGE 87T8 PSA 10" [ref=e166]:
                - generic [ref=e167]:
                  - img "2017 TOPPS CHROME 1987 TOPPS 1987 TOPPS AARON JUDGE 87T8 PSA 10" [ref=e168]
                  - generic [ref=e169]: $445.50 est.
                - generic [ref=e170]: 2017 TOPPS CHROME 1987 TOPPS 1987 TOPPS AARON JUDGE 87T8 PSA 10
              - button "2024 PANINI SELECT RED SHOCK DRAKE MAYE 113 PSA 10 $361.35 est. 2024 PANINI SELECT RED SHOCK DRAKE MAYE 113 PSA 10" [ref=e171]:
                - generic [ref=e172]:
                  - img "2024 PANINI SELECT RED SHOCK DRAKE MAYE 113 PSA 10" [ref=e173]
                  - generic [ref=e174]: $361.35 est.
                - generic [ref=e175]: 2024 PANINI SELECT RED SHOCK DRAKE MAYE 113 PSA 10
              - button "2025 TOPPS CHROME WWE MARKS OF CHAMPIONS AUTOGRAPHS STEVE AUSTIN SA PSA 10 $360.00 est. 2025 TOPPS CHROME WWE MARKS OF CHAMPIONS AUTOGRAPHS STEVE AUSTIN SA PSA 10" [ref=e176]:
                - generic [ref=e177]:
                  - img "2025 TOPPS CHROME WWE MARKS OF CHAMPIONS AUTOGRAPHS STEVE AUSTIN SA PSA 10" [ref=e178]
                  - generic [ref=e179]: $360.00 est.
                - generic [ref=e180]: 2025 TOPPS CHROME WWE MARKS OF CHAMPIONS AUTOGRAPHS STEVE AUSTIN SA PSA 10
              - button "2021 PANINI PRIZM UFC NEON GREEN PRIZM KHAMZAT CHIMAEV 7 PSA 9 $360.00 est. 2021 PANINI PRIZM UFC NEON GREEN PRIZM KHAMZAT CHIMAEV 7 PSA 9" [ref=e181]:
                - generic [ref=e182]:
                  - img "2021 PANINI PRIZM UFC NEON GREEN PRIZM KHAMZAT CHIMAEV 7 PSA 9" [ref=e183]
                  - generic [ref=e184]: $360.00 est.
                - generic [ref=e185]: 2021 PANINI PRIZM UFC NEON GREEN PRIZM KHAMZAT CHIMAEV 7 PSA 9
              - button "2023 BOWMAN SAPPHIRE EDITION CHROME PROSPECTS CHROME PROSPECTS ROMAN ANTHONY BCP71 PSA 10 $356.40 est. 2023 BOWMAN SAPPHIRE EDITION CHROME PROSPECTS CHROME PROSPECTS ROMAN ANTHONY BCP71 PSA 10" [ref=e186]:
                - generic [ref=e187]:
                  - img "2023 BOWMAN SAPPHIRE EDITION CHROME PROSPECTS CHROME PROSPECTS ROMAN ANTHONY BCP71 PSA 10" [ref=e188]
                  - generic [ref=e189]: $356.40 est.
                - generic [ref=e190]: 2023 BOWMAN SAPPHIRE EDITION CHROME PROSPECTS CHROME PROSPECTS ROMAN ANTHONY BCP71 PSA 10
              - button "2025 TOPPS MIDNIGHT UFC HORIZON SIGNATURES HORIZON SIG-DUSK JON JONES HNS-JJ PSA 7 $331.65 est. 2025 TOPPS MIDNIGHT UFC HORIZON SIGNATURES HORIZON SIG-DUSK JON JONES HNS-JJ PSA 7" [ref=e191]:
                - generic [ref=e192]:
                  - img "2025 TOPPS MIDNIGHT UFC HORIZON SIGNATURES HORIZON SIG-DUSK JON JONES HNS-JJ PSA 7" [ref=e193]
                  - generic [ref=e194]: $331.65 est.
                - generic [ref=e195]: 2025 TOPPS MIDNIGHT UFC HORIZON SIGNATURES HORIZON SIG-DUSK JON JONES HNS-JJ PSA 7
              - button "2022 PANINI PRIZM WORLD CUP QATAR GREEN PRIZM JESPER LINDSTROM 68 PSA 10 $327.69 est. 2022 PANINI PRIZM WORLD CUP QATAR GREEN PRIZM JESPER LINDSTROM 68 PSA 10" [ref=e196]:
                - generic [ref=e197]:
                  - img "2022 PANINI PRIZM WORLD CUP QATAR GREEN PRIZM JESPER LINDSTROM 68 PSA 10" [ref=e198]
                  - generic [ref=e199]: $327.69 est.
                - generic [ref=e200]: 2022 PANINI PRIZM WORLD CUP QATAR GREEN PRIZM JESPER LINDSTROM 68 PSA 10
              - button "2024 UPPER DECK MACKLIN CELEBRINI 451 PSA 8 $324.00 est. 2024 UPPER DECK MACKLIN CELEBRINI 451 PSA 8" [ref=e201]:
                - generic [ref=e202]:
                  - img "2024 UPPER DECK MACKLIN CELEBRINI 451 PSA 8" [ref=e203]
                  - generic [ref=e204]: $324.00 est.
                - generic [ref=e205]: 2024 UPPER DECK MACKLIN CELEBRINI 451 PSA 8
              - button "1985 TOPPS MARIO LEMIEUX 9 PSA 8 $320.66 est. 1985 TOPPS MARIO LEMIEUX 9 PSA 8" [ref=e206]:
                - generic [ref=e207]:
                  - img "1985 TOPPS MARIO LEMIEUX 9 PSA 8" [ref=e208]
                  - generic [ref=e209]: $320.66 est.
                - generic [ref=e210]: 1985 TOPPS MARIO LEMIEUX 9 PSA 8
              - button "2019 TOPPS UFC CHROME FIGHTER AUTOGRAPHS FIGHTER AUTOGRAPH MAYCEE BARBER FAMB PSA 10 $305.65 est. 2019 TOPPS UFC CHROME FIGHTER AUTOGRAPHS FIGHTER AUTOGRAPH MAYCEE BARBER FAMB PSA 10" [ref=e211]:
                - generic [ref=e212]:
                  - img "2019 TOPPS UFC CHROME FIGHTER AUTOGRAPHS FIGHTER AUTOGRAPH MAYCEE BARBER FAMB PSA 10" [ref=e213]
                  - generic [ref=e214]: $305.65 est.
                - generic [ref=e215]: 2019 TOPPS UFC CHROME FIGHTER AUTOGRAPHS FIGHTER AUTOGRAPH MAYCEE BARBER FAMB PSA 10
              - button "2023 TOPPS CHROME FORMULA 1 SPEED DEMONS SPEED DEMONS-RED REFRACTOR NICO HULKENBERG SDNH PSA 10 $302.94 est. 2023 TOPPS CHROME FORMULA 1 SPEED DEMONS SPEED DEMONS-RED REFRACTOR NICO HULKENBERG SDNH PSA 10" [ref=e216]:
                - generic [ref=e217]:
                  - img "2023 TOPPS CHROME FORMULA 1 SPEED DEMONS SPEED DEMONS-RED REFRACTOR NICO HULKENBERG SDNH PSA 10" [ref=e218]
                  - generic [ref=e219]: $302.94 est.
                - generic [ref=e220]: 2023 TOPPS CHROME FORMULA 1 SPEED DEMONS SPEED DEMONS-RED REFRACTOR NICO HULKENBERG SDNH PSA 10
              - button "2021 TOPPS CHROME MLS SAPPHIRE EDITION SAPPHIRE ED-SP-ORANGE PAXTEN AARONSON 72 PSA 10 $302.67 est. 2021 TOPPS CHROME MLS SAPPHIRE EDITION SAPPHIRE ED-SP-ORANGE PAXTEN AARONSON 72 PSA 10" [ref=e221]:
                - generic [ref=e222]:
                  - img "2021 TOPPS CHROME MLS SAPPHIRE EDITION SAPPHIRE ED-SP-ORANGE PAXTEN AARONSON 72 PSA 10" [ref=e223]
                  - generic [ref=e224]: $302.67 est.
                - generic [ref=e225]: 2021 TOPPS CHROME MLS SAPPHIRE EDITION SAPPHIRE ED-SP-ORANGE PAXTEN AARONSON 72 PSA 10
              - button "2020 TOPPS MERLIN CHROME UEFA CHAMPIONS LEAGUE SUPERFRACTOR 1/1 MARCOS ANTONIO 34 PSA 9 $297.99 est. 2020 TOPPS MERLIN CHROME UEFA CHAMPIONS LEAGUE SUPERFRACTOR 1/1 MARCOS ANTONIO 34 PSA 9" [ref=e226]:
                - generic [ref=e227]:
                  - img "2020 TOPPS MERLIN CHROME UEFA CHAMPIONS LEAGUE SUPERFRACTOR 1/1 MARCOS ANTONIO 34 PSA 9" [ref=e228]
                  - generic [ref=e229]: $297.99 est.
                - generic [ref=e230]: 2020 TOPPS MERLIN CHROME UEFA CHAMPIONS LEAGUE SUPERFRACTOR 1/1 MARCOS ANTONIO 34 PSA 9
              - button "2024 S.I. FOR KIDS CHARLIE WOODS 907 PSA 8 $297.00 est. 2024 S.I. FOR KIDS CHARLIE WOODS 907 PSA 8" [ref=e231]:
                - generic [ref=e232]:
                  - img "2024 S.I. FOR KIDS CHARLIE WOODS 907 PSA 8" [ref=e233]
                  - generic [ref=e234]: $297.00 est.
                - generic [ref=e235]: 2024 S.I. FOR KIDS CHARLIE WOODS 907 PSA 8
              - button "2018 PANINI PRIZM LAMAR JACKSON 212 PSA 10 $292.05 est. 2018 PANINI PRIZM LAMAR JACKSON 212 PSA 10" [ref=e236]:
                - generic [ref=e237]:
                  - img "2018 PANINI PRIZM LAMAR JACKSON 212 PSA 10" [ref=e238]
                  - generic [ref=e239]: $292.05 est.
                - generic [ref=e240]: 2018 PANINI PRIZM LAMAR JACKSON 212 PSA 10
              - 'button "2024 PANINI PRIZM WWE THROWBACK SIGNATURES #TSCMP CM PUNK THROWBACK SIG-GREEN PRIZM PSA 10 $287.10 est. 2024 PANINI PRIZM WWE THROWBACK SIGNATURES #TSCMP CM PUNK THROWBACK SIG-GREEN PRIZM PSA 10" [ref=e241]':
                - generic [ref=e242]:
                  - 'img "2024 PANINI PRIZM WWE THROWBACK SIGNATURES #TSCMP CM PUNK THROWBACK SIG-GREEN PRIZM PSA 10" [ref=e243]'
                  - generic [ref=e244]: $287.10 est.
                - generic [ref=e245]: "2024 PANINI PRIZM WWE THROWBACK SIGNATURES #TSCMP CM PUNK THROWBACK SIG-GREEN PRIZM PSA 10"
              - button "2023 UPPER DECK CONNOR BEDARD 451 PSA 9 $282.15 est. 2023 UPPER DECK CONNOR BEDARD 451 PSA 9" [ref=e246]:
                - generic [ref=e247]:
                  - img "2023 UPPER DECK CONNOR BEDARD 451 PSA 9" [ref=e248]
                  - generic [ref=e249]: $282.15 est.
                - generic [ref=e250]: 2023 UPPER DECK CONNOR BEDARD 451 PSA 9
              - button "2020 BOWMAN DRAFT CHROME-SPARKLE REFRACTOR JORDAN WALKER BD57 PSA 10 $277.20 est. 2020 BOWMAN DRAFT CHROME-SPARKLE REFRACTOR JORDAN WALKER BD57 PSA 10" [ref=e251]:
                - generic [ref=e252]:
                  - img "2020 BOWMAN DRAFT CHROME-SPARKLE REFRACTOR JORDAN WALKER BD57 PSA 10" [ref=e253]
                  - generic [ref=e254]: $277.20 est.
                - generic [ref=e255]: 2020 BOWMAN DRAFT CHROME-SPARKLE REFRACTOR JORDAN WALKER BD57 PSA 10
              - button "2003 SP AUTHENTIC GOLF EXTRA LIMITED-AUTOGRAPH DARREN CLARKE 122 PSA 10 $277.16 est. 2003 SP AUTHENTIC GOLF EXTRA LIMITED-AUTOGRAPH DARREN CLARKE 122 PSA 10" [ref=e256]:
                - generic [ref=e257]:
                  - img "2003 SP AUTHENTIC GOLF EXTRA LIMITED-AUTOGRAPH DARREN CLARKE 122 PSA 10" [ref=e258]
                  - generic [ref=e259]: $277.16 est.
                - generic [ref=e260]: 2003 SP AUTHENTIC GOLF EXTRA LIMITED-AUTOGRAPH DARREN CLARKE 122 PSA 10
              - button "2024 TOPPS CHROME UFC SUPERFRACTOR 1/1 ALLAN NASCIMENTO 13 PSA 9 $275.06 est. 2024 TOPPS CHROME UFC SUPERFRACTOR 1/1 ALLAN NASCIMENTO 13 PSA 9" [ref=e261]:
                - generic [ref=e262]:
                  - img "2024 TOPPS CHROME UFC SUPERFRACTOR 1/1 ALLAN NASCIMENTO 13 PSA 9" [ref=e263]
                  - generic [ref=e264]: $275.06 est.
                - generic [ref=e265]: 2024 TOPPS CHROME UFC SUPERFRACTOR 1/1 ALLAN NASCIMENTO 13 PSA 9
              - button "2021 TOPPS CHROME FORMULA 1 SAPPHIRE EDITION SAPPHIRE EDITION-GOLD LEWIS HAMILTON 152 PSA 10 $270.00 est. 2021 TOPPS CHROME FORMULA 1 SAPPHIRE EDITION SAPPHIRE EDITION-GOLD LEWIS HAMILTON 152 PSA 10" [ref=e266]:
                - generic [ref=e267]:
                  - img "2021 TOPPS CHROME FORMULA 1 SAPPHIRE EDITION SAPPHIRE EDITION-GOLD LEWIS HAMILTON 152 PSA 10" [ref=e268]
                  - generic [ref=e269]: $270.00 est.
                - generic [ref=e270]: 2021 TOPPS CHROME FORMULA 1 SAPPHIRE EDITION SAPPHIRE EDITION-GOLD LEWIS HAMILTON 152 PSA 10
              - button "2022 TOPPS CHROME FORMULA 1 SAPPHIRE EDITION SSP-AQUA OSCAR PIASTRI 199 PSA 10 $270.00 est. 2022 TOPPS CHROME FORMULA 1 SAPPHIRE EDITION SSP-AQUA OSCAR PIASTRI 199 PSA 10" [ref=e271]:
                - generic [ref=e272]:
                  - img "2022 TOPPS CHROME FORMULA 1 SAPPHIRE EDITION SSP-AQUA OSCAR PIASTRI 199 PSA 10" [ref=e273]
                  - generic [ref=e274]: $270.00 est.
                - generic [ref=e275]: 2022 TOPPS CHROME FORMULA 1 SAPPHIRE EDITION SSP-AQUA OSCAR PIASTRI 199 PSA 10
              - button "1999 MERLIN SERIE A ANDRIY SHEVCHENKO 49 PSA 9 $269.10 est. 1999 MERLIN SERIE A ANDRIY SHEVCHENKO 49 PSA 9" [ref=e276]:
                - generic [ref=e277]:
                  - img "1999 MERLIN SERIE A ANDRIY SHEVCHENKO 49 PSA 9" [ref=e278]
                  - generic [ref=e279]: $269.10 est.
                - generic [ref=e280]: 1999 MERLIN SERIE A ANDRIY SHEVCHENKO 49 PSA 9
              - button "2005 TOPPS AARON RODGERS 431 PSA 10 $268.46 est. 2005 TOPPS AARON RODGERS 431 PSA 10" [ref=e281]:
                - generic [ref=e282]:
                  - img "2005 TOPPS AARON RODGERS 431 PSA 10" [ref=e283]
                  - generic [ref=e284]: $268.46 est.
                - generic [ref=e285]: 2005 TOPPS AARON RODGERS 431 PSA 10
              - button "2020 TOPPS CHROME FORMULA 1 REFRACTOR MAX VERSTAPPEN 171 PSA 10 $262.35 est. 2020 TOPPS CHROME FORMULA 1 REFRACTOR MAX VERSTAPPEN 171 PSA 10" [ref=e286]:
                - generic [ref=e287]:
                  - img "2020 TOPPS CHROME FORMULA 1 REFRACTOR MAX VERSTAPPEN 171 PSA 10" [ref=e288]
                  - generic [ref=e289]: $262.35 est.
                - generic [ref=e290]: 2020 TOPPS CHROME FORMULA 1 REFRACTOR MAX VERSTAPPEN 171 PSA 10
              - button "2008 UPPER DECK STARQUEST COPPER KOBE BRYANT SQ-5 PSA 10 $258.45 est. 2008 UPPER DECK STARQUEST COPPER KOBE BRYANT SQ-5 PSA 10" [ref=e291]:
                - generic [ref=e292]:
                  - img "2008 UPPER DECK STARQUEST COPPER KOBE BRYANT SQ-5 PSA 10" [ref=e293]
                  - generic [ref=e294]: $258.45 est.
                - generic [ref=e295]: 2008 UPPER DECK STARQUEST COPPER KOBE BRYANT SQ-5 PSA 10
              - button "2024 PANINI OBSIDIAN MOLTEN FOTL JOSH ALLEN 19 PSA 9 $257.40 est. 2024 PANINI OBSIDIAN MOLTEN FOTL JOSH ALLEN 19 PSA 9" [ref=e296]:
                - generic [ref=e297]:
                  - img "2024 PANINI OBSIDIAN MOLTEN FOTL JOSH ALLEN 19 PSA 9" [ref=e298]
                  - generic [ref=e299]: $257.40 est.
                - generic [ref=e300]: 2024 PANINI OBSIDIAN MOLTEN FOTL JOSH ALLEN 19 PSA 9
              - button "2024 UPPER DECK SP AUTHENTIC AUTOGRAPH MATT REMPE 109 PSA 10 $257.40 est. 2024 UPPER DECK SP AUTHENTIC AUTOGRAPH MATT REMPE 109 PSA 10" [ref=e301]:
                - generic [ref=e302]:
                  - img "2024 UPPER DECK SP AUTHENTIC AUTOGRAPH MATT REMPE 109 PSA 10" [ref=e303]
                  - generic [ref=e304]: $257.40 est.
                - generic [ref=e305]: 2024 UPPER DECK SP AUTHENTIC AUTOGRAPH MATT REMPE 109 PSA 10
              - button "2022 PANINI SELECT SERIE A GREEN NICOLO FAGIOLI 49 PSA 10 $257.40 est. 2022 PANINI SELECT SERIE A GREEN NICOLO FAGIOLI 49 PSA 10" [ref=e306]:
                - generic [ref=e307]:
                  - img "2022 PANINI SELECT SERIE A GREEN NICOLO FAGIOLI 49 PSA 10" [ref=e308]
                  - generic [ref=e309]: $257.40 est.
                - generic [ref=e310]: 2022 PANINI SELECT SERIE A GREEN NICOLO FAGIOLI 49 PSA 10
              - button "2025 TOPPS UEFA CLUB COMPETITIONS TOPPS SUPERSTAR AUTOGRAPH RELICS SSTAR AUTO RELICS-GOLD ETHAN NWANERI EN PSA 10 $254.41 est. 2025 TOPPS UEFA CLUB COMPETITIONS TOPPS SUPERSTAR AUTOGRAPH RELICS SSTAR AUTO RELICS-GOLD ETHAN NWANERI EN PSA 10" [ref=e311]:
                - generic [ref=e312]:
                  - img "2025 TOPPS UEFA CLUB COMPETITIONS TOPPS SUPERSTAR AUTOGRAPH RELICS SSTAR AUTO RELICS-GOLD ETHAN NWANERI EN PSA 10" [ref=e313]
                  - generic [ref=e314]: $254.41 est.
                - generic [ref=e315]: 2025 TOPPS UEFA CLUB COMPETITIONS TOPPS SUPERSTAR AUTOGRAPH RELICS SSTAR AUTO RELICS-GOLD ETHAN NWANERI EN PSA 10
              - button "2024 PANINI PRIZM PREMIER LEAGUE CHERRY BLOSSOM CHOICE WILLIAM SALIBA 20 PSA 10 $254.04 est. 2024 PANINI PRIZM PREMIER LEAGUE CHERRY BLOSSOM CHOICE WILLIAM SALIBA 20 PSA 10" [ref=e316]:
                - generic [ref=e317]:
                  - img "2024 PANINI PRIZM PREMIER LEAGUE CHERRY BLOSSOM CHOICE WILLIAM SALIBA 20 PSA 10" [ref=e318]
                  - generic [ref=e319]: $254.04 est.
                - generic [ref=e320]: 2024 PANINI PRIZM PREMIER LEAGUE CHERRY BLOSSOM CHOICE WILLIAM SALIBA 20 PSA 10
              - button "2025 TOPPS NOW FORMULA 1 ORANGE FOIL MCLAREN F1 TEAM 54 PSA 10 $251.81 est. 2025 TOPPS NOW FORMULA 1 ORANGE FOIL MCLAREN F1 TEAM 54 PSA 10" [ref=e321]:
                - generic [ref=e322]:
                  - img "2025 TOPPS NOW FORMULA 1 ORANGE FOIL MCLAREN F1 TEAM 54 PSA 10" [ref=e323]
                  - generic [ref=e324]: $251.81 est.
                - generic [ref=e325]: 2025 TOPPS NOW FORMULA 1 ORANGE FOIL MCLAREN F1 TEAM 54 PSA 10
              - button "2025 TOPPS CHROME WWE AUTOGRAPH-RED REFRACTOR ANGELO DAWKINS 63 PSA 10 $250.47 est. 2025 TOPPS CHROME WWE AUTOGRAPH-RED REFRACTOR ANGELO DAWKINS 63 PSA 10" [ref=e326]:
                - generic [ref=e327]:
                  - img "2025 TOPPS CHROME WWE AUTOGRAPH-RED REFRACTOR ANGELO DAWKINS 63 PSA 10" [ref=e328]
                  - generic [ref=e329]: $250.47 est.
                - generic [ref=e330]: 2025 TOPPS CHROME WWE AUTOGRAPH-RED REFRACTOR ANGELO DAWKINS 63 PSA 10
    - generic:
      - region "Notifications Alt+T"
  - alert [ref=e331]: ParlayPlay | Fun Fantasy Sports
  - iframe [ref=e332]:
    
```

# Test source

```ts
  192 |       .filter({ hasText: "Confirm Shipping" })
  193 |       .first();
  194 |   }
  195 | 
  196 |   // Final CTA on the Delivery Information checkout → charges shipping+handling
  197 |   // (Django /shipping-debit).
  198 |   get submitShippingButton(): Locator {
  199 |     return this.packFrame
  200 |       .locator("button")
  201 |       .filter({ hasText: /^Submit$/ })
  202 |       .first();
  203 |   }
  204 | 
  205 |   // Terminal state: the "Shipping" tab of the provider's My Packs section.
  206 |   get shippingTab(): Locator {
  207 |     return this.packFrame.getByRole("tab").filter({ hasText: "Shipping" });
  208 |   }
  209 | 
  210 |   // A delivery entry under the Shipping tab. Layout varies by Repackz build
  211 |   // (desktop: an "Open delivery #<n>" button; mobile: a card tile) — the stable
  212 |   // signal in both is the "<n> item" count.
  213 |   get deliveryRows(): Locator {
  214 |     return this.packFrame.getByText(/\d+\s+items?/);
  215 |   }
  216 | 
  217 |   constructor(page: Page) {
  218 |     super(page);
  219 |   }
  220 | 
  221 |   /** Current header (nav) cash balance in dollars, e.g. "$234.15" → 234.15. */
  222 |   async headerBalanceUsd(): Promise<number> {
  223 |     const label = await this.page
  224 |       .getByRole("banner")
  225 |       .getByText(/^\$[\d,]+\.\d{2}$/)
  226 |       .first()
  227 |       .textContent();
  228 |     const match = (label ?? "").match(/\$([\d,]+\.\d{2})/);
  229 |     return match ? Number(match[1].replace(/,/g, "")) : NaN;
  230 |   }
  231 | 
  232 |   /** Detail-page pack name (the <h1>). */
  233 |   get detailHeading(): Locator {
  234 |     return this.page
  235 |       .getByRole("heading", { level: 1 })
  236 |       .filter({ visible: true })
  237 |       .first();
  238 |   }
  239 | 
  240 |   async openLobby(): Promise<void> {
  241 |     await this.open("/packs");
  242 |     await this.openAPackHeading.waitFor({ state: "visible", timeout: 30_000 });
  243 |   }
  244 | 
  245 |   /** Open the first visible pack tile; returns its /packs/pack/<id> href. */
  246 |   async openFirstPack(): Promise<string> {
  247 |     const first = this.packTiles.first();
  248 |     await first.waitFor({ state: "visible", timeout: 30_000 });
  249 |     const href = (await first.getAttribute("href")) ?? "";
  250 |     await first.click();
  251 |     await this.page.waitForURL("**/packs/pack/**");
  252 |     await this.buyButton.waitFor({ state: "visible", timeout: 30_000 });
  253 |     return href;
  254 |   }
  255 | 
  256 |   /**
  257 |    * Open the CHEAPEST catalog pack and land on its detail page. Keeps the
  258 |    * money-flow spend (and the balance the account needs) as low as possible —
  259 |    * the first catalog tile can be a $100 pack that a drained staging balance
  260 |    * can't afford. Reads the price off each tile's text and clicks the min.
  261 |    */
  262 |   async openCheapestPack(): Promise<void> {
  263 |     const tiles = this.packTiles;
  264 |     await tiles.first().waitFor({ state: "visible", timeout: 30_000 });
  265 |     const count = await tiles.count();
  266 |     let bestIdx = 0;
  267 |     let bestPrice = Infinity;
  268 |     for (let i = 0; i < count; i++) {
  269 |       const text = (await tiles.nth(i).textContent()) ?? "";
  270 |       const match = text.match(/\$([\d,]+(?:\.\d+)?)/);
  271 |       const price = match ? Number(match[1].replace(/,/g, "")) : Infinity;
  272 |       if (price < bestPrice) {
  273 |         bestPrice = price;
  274 |         bestIdx = i;
  275 |       }
  276 |     }
  277 |     await tiles.nth(bestIdx).click();
  278 |     await this.page.waitForURL("**/packs/pack/**");
  279 |     await this.buyButton.waitFor({ state: "visible", timeout: 30_000 });
  280 |   }
  281 | 
  282 |   /** The dollar amount currently on the Buy CTA (e.g. "Buy for $50" → 50). */
  283 |   async buyPriceUsd(): Promise<number> {
  284 |     const label = (await this.buyButton.textContent()) ?? "";
  285 |     const match = label.match(/\$([\d,]+(?:\.\d+)?)/);
  286 |     return match ? Number(match[1].replace(/,/g, "")) : NaN;
  287 |   }
  288 | 
  289 |   /** Click Buy and wait for the Repackz iframe to mount. Does NOT open/charge —
  290 |    *  the money-moving "RIP" button lives inside the (provider-owned) iframe. */
  291 |   async buyAndAwaitIframe(): Promise<void> {
> 292 |     await this.buyButton.click();
      |                          ^ Error: locator.click: Target page, context or browser has been closed
  293 |     await this.openPackIframe.waitFor({ state: "visible", timeout: 45_000 });
  294 |   }
  295 | 
  296 |   /**
  297 |    * Click Buy and report whether the Repackz iframe actually mounted. Returns
  298 |    * false when `POST /packs/sessions/` fails upstream — Repackz staging
  299 |    * intermittently 502s on session creation, which leaves the buy CTA in place
  300 |    * and never opens the iframe. The provider-flow specs `test.skip` on false so
  301 |    * a provider outage reads as skipped, not a spurious failure.
  302 |    */
  303 |   async buyAndTryAwaitIframe(timeoutMs = 30_000): Promise<boolean> {
  304 |     await this.buyButton.click();
  305 |     return this.openPackIframe
  306 |       .waitFor({ state: "visible", timeout: timeoutMs })
  307 |       .then(() => true)
  308 |       .catch(() => false);
  309 |   }
  310 | 
  311 |   // ── Transaction history (/transactions) ─────────────────────────────────
  312 |   // Pack money movements land here as balance-log rows: "Pack Purchase",
  313 |   // "Pack Sell-Back", "Pack Shipping", "Card Shipped", "Pack Refund" — newest
  314 |   // first, each with a signed amount and a "View pack details" link.
  315 |   readonly transactionLogHeading = this.byText("Transaction Log");
  316 | 
  317 |   // The type <select> — the one offering a "Packs" option (the other is the
  318 |   // month picker).
  319 |   get transactionTypeFilter(): Locator {
  320 |     return this.page
  321 |       .getByRole("combobox")
  322 |       .filter({
  323 |         has: this.page.getByRole("option", { name: "Packs", exact: true }),
  324 |       })
  325 |       .first();
  326 |   }
  327 | 
  328 |   // One row per transaction (bgSecondary pill). Newest first.
  329 |   get transactionRows(): Locator {
  330 |     return this.page
  331 |       .locator("div.bg-bgSecondary.rounded-full")
  332 |       .filter({ visible: true });
  333 |   }
  334 | 
  335 |   async openTransactions(): Promise<void> {
  336 |     await this.open("/transactions");
  337 |     await this.transactionLogHeading.waitFor({
  338 |       state: "visible",
  339 |       timeout: 30_000,
  340 |     });
  341 |   }
  342 | 
  343 |   async filterTransactionsToPacks(): Promise<void> {
  344 |     await this.transactionTypeFilter.selectOption({ label: "Packs" });
  345 |   }
  346 | 
  347 |   /** A transaction row carrying both an action label and (optionally) an
  348 |    *  amount — e.g. row("Pack Purchase", "- $50.00"). */
  349 |   transactionRow(actionLabel: string, amount?: string): Locator {
  350 |     let row = this.transactionRows.filter({ hasText: actionLabel });
  351 |     if (amount) row = row.filter({ hasText: amount });
  352 |     return row.first();
  353 |   }
  354 | }
  355 | 
```