# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: navigation/footer-nav.spec.ts >> Bottom nav - tab routing and active indicator >> Fifth tab (Free2Play or Packs) routes and takes the indicator
- Location: tests/navigation/footer-nav.spec.ts:55:5

# Error details

```
Error: expect(locator).toHaveClass(expected) failed

Locator: locator('nav').filter({ has: locator('ul.grid-cols-5') }).filter({ visible: true }).first().getByRole('button', { name: 'Packs' }).locator('span.border-playYellow')
Expected pattern: /border-b-2/
Received string:  "text-xs border-playYellow"
Timeout: 15000ms

Call log:
  - Expect "toHaveClass" with timeout 15000ms
  - waiting for locator('nav').filter({ has: locator('ul.grid-cols-5') }).filter({ visible: true }).first().getByRole('button', { name: 'Packs' }).locator('span.border-playYellow')
    6 × locator resolved to <span class="text-xs border-playYellow">Packs</span>
      - unexpected value "text-xs border-playYellow"

```

# Page snapshot

```yaml
- generic [ref=e1]:
  - generic [ref=e2]:
    - generic [ref=e3]:
      - banner [ref=e4]:
        - navigation [ref=e5]:
          - link "Parlay Play Logo" [ref=e6]:
            - /url: /
            - img "Parlay Play Logo" [ref=e8]
          - generic [ref=e10]:
            - generic [ref=e12]:
              - generic [ref=e13]: $714.00
              - generic [ref=e14]:
                - img "gift-icon" [ref=e15]
                - text: "43.00"
            - button "Toggle Menu" [ref=e16]:
              - img [ref=e17]
      - main [ref=e19]:
        - generic [ref=e22]:
          - generic [ref=e23]:
            - generic [ref=e31] [cursor=pointer]:
              - generic [ref=e32]: Pull real graded cards worth up to $10,000
              - generic [ref=e33]: Sell or ship instantly
              - button "Rip a pack" [ref=e34]:
                - generic [ref=e35]:
                  - img [ref=e36]
                  - text: Rip a pack
            - region "Just Opened" [ref=e39]:
              - heading "Just Opened" [level=2] [ref=e40]
              - generic [ref=e43]:
                - button "2021 POKEMON JAPANESE SWORD & SHIELD VMAX CLIMAX VMAX CLIMAX ELECTRODE 048 PSA 8 $17.82 est." [ref=e44]:
                  - generic [ref=e45]:
                    - generic [ref=e46]: 2021 POKEMON JAPANESE SWORD & SHIELD VMAX CLIMAX VMAX CLIMAX ELECTRODE 048 PSA 8
                    - generic [ref=e47]: $17.82 est.
                - button "2000 POKEMON JAPANESE NEO 2 POLIWAG 60 PSA 9 $31.50 est." [ref=e48]:
                  - generic [ref=e49]:
                    - generic [ref=e50]: 2000 POKEMON JAPANESE NEO 2 POLIWAG 60 PSA 9
                    - generic [ref=e51]: $31.50 est.
                - button "2023 POKEMON JAPANESE SV2a-POKEMON 151 MASTER BALL REVERSE HOLO CLOYSTER 091 PSA 9 $16.83 est." [ref=e52]:
                  - generic [ref=e53]:
                    - generic [ref=e54]: 2023 POKEMON JAPANESE SV2a-POKEMON 151 MASTER BALL REVERSE HOLO CLOYSTER 091 PSA 9
                    - generic [ref=e55]: $16.83 est.
                - button "2025 POKEMON PRE EN-PRISMATIC EVOLUTIONS ULTRA RARE RAIFORT 142 PSA 9 $15.39 est." [ref=e56]:
                  - generic [ref=e57]:
                    - generic [ref=e58]: 2025 POKEMON PRE EN-PRISMATIC EVOLUTIONS ULTRA RARE RAIFORT 142 PSA 9
                    - generic [ref=e59]: $15.39 est.
                - button "2025 POKEMON MEP EN-ME BLACK STAR PROMO ULTRA-PREMIUM COLLECTION ORICORIO ex 024 PSA 9 $30.69 est." [ref=e60]:
                  - generic [ref=e61]:
                    - generic [ref=e62]: 2025 POKEMON MEP EN-ME BLACK STAR PROMO ULTRA-PREMIUM COLLECTION ORICORIO ex 024 PSA 9
                    - generic [ref=e63]: $30.69 est.
                - button "2023 POKEMON PAL EN-PALDEA EVOLVED FORRETRESS ex 005 PSA 10 $43.56 est." [ref=e64]:
                  - generic [ref=e65]:
                    - generic [ref=e66]: 2023 POKEMON PAL EN-PALDEA EVOLVED FORRETRESS ex 005 PSA 10
                    - generic [ref=e67]: $43.56 est.
                - button "2024 POKEMON SSP EN-SURGING SPARKS BLACK KYUREM ex 048 PSA 8 $14.85 est." [ref=e68]:
                  - generic [ref=e69]:
                    - generic [ref=e70]: 2024 POKEMON SSP EN-SURGING SPARKS BLACK KYUREM ex 048 PSA 8
                    - generic [ref=e71]: $14.85 est.
                - button "2025 POKEMON JTG EN-JOURNEY TOGETHER ILLUSTRATION RARE LILLIE'S RIBOMBEE 164 PSA 8 $17.79 est." [ref=e72]:
                  - generic [ref=e73]:
                    - generic [ref=e74]: 2025 POKEMON JTG EN-JOURNEY TOGETHER ILLUSTRATION RARE LILLIE'S RIBOMBEE 164 PSA 8
                    - generic [ref=e75]: $17.79 est.
                - button "2024 POKEMON SFA EN-SHROUDED FABLE CROBAT 029 PSA 9 $17.82 est." [ref=e76]:
                  - generic [ref=e77]:
                    - generic [ref=e78]: 2024 POKEMON SFA EN-SHROUDED FABLE CROBAT 029 PSA 9
                    - generic [ref=e79]: $17.82 est.
                - button "2017 POKEMON JAPANESE THE BEST OF XY THE BEST OF XY AROMATISSE-REV.FOIL 094 PSA 9 $17.82 est." [ref=e80]:
                  - generic [ref=e81]:
                    - generic [ref=e82]: 2017 POKEMON JAPANESE THE BEST OF XY THE BEST OF XY AROMATISSE-REV.FOIL 094 PSA 9
                    - generic [ref=e83]: $17.82 est.
                - button "2021 POKEMON JAPANESE SWORD & SHIELD VMAX CLIMAX VMAX CLIMAX ORBEETLE-HOLO 079 PSA 8 $16.82 est." [ref=e84]:
                  - generic [ref=e85]:
                    - generic [ref=e86]: 2021 POKEMON JAPANESE SWORD & SHIELD VMAX CLIMAX VMAX CLIMAX ORBEETLE-HOLO 079 PSA 8
                    - generic [ref=e87]: $16.82 est.
                - button "2024 POKEMON SVP EN-SV BLACK STAR PROMO SURGING SPARKS ETB MAGNETON 159 PSA 9 $24.75 est." [ref=e88]:
                  - generic [ref=e89]:
                    - generic [ref=e90]: 2024 POKEMON SVP EN-SV BLACK STAR PROMO SURGING SPARKS ETB MAGNETON 159 PSA 9
                    - generic [ref=e91]: $24.75 est.
                - button "2025 POKEMON JTG EN-JOURNEY TOGETHER ULTRA RARE DUDUNSPARCE ex 178 PSA 9 $15.81 est." [ref=e92]:
                  - generic [ref=e93]:
                    - generic [ref=e94]: 2025 POKEMON JTG EN-JOURNEY TOGETHER ULTRA RARE DUDUNSPARCE ex 178 PSA 9
                    - generic [ref=e95]: $15.81 est.
                - button "2025 POKEMON JAPANESE SV11B-BLACK BOLT REVERSE HOLO LAMPENT 016 PSA 9 $17.82 est." [ref=e96]:
                  - generic [ref=e97]:
                    - generic [ref=e98]: 2025 POKEMON JAPANESE SV11B-BLACK BOLT REVERSE HOLO LAMPENT 016 PSA 9
                    - generic [ref=e99]: $17.82 est.
                - button "2004 POKEMON EX FIRE RED & LEAF GREEN FIRE RED & LEAF GREEN EXP.ALL-REVERSE FOIL 91 PSA 5 $10.80 est." [ref=e100]:
                  - generic [ref=e101]:
                    - generic [ref=e102]: 2004 POKEMON EX FIRE RED & LEAF GREEN FIRE RED & LEAF GREEN EXP.ALL-REVERSE FOIL 91 PSA 5
                    - generic [ref=e103]: $10.80 est.
                - button "2025 POKEMON PFL EN-PHANTASMAL FLAMES MEGA GENGAR ex 056 PSA 9 $28.71 est." [ref=e104]:
                  - generic [ref=e105]:
                    - generic [ref=e106]: 2025 POKEMON PFL EN-PHANTASMAL FLAMES MEGA GENGAR ex 056 PSA 9
                    - generic [ref=e107]: $28.71 est.
                - button "2023 POKEMON SVI EN-SCARLET & VIOLET JACQ 250 PSA 9 $17.79 est." [ref=e108]:
                  - generic [ref=e109]:
                    - generic [ref=e110]: 2023 POKEMON SVI EN-SCARLET & VIOLET JACQ 250 PSA 9
                    - generic [ref=e111]: $17.79 est.
                - button "2024 POKEMON SFA EN-SHROUDED FABLE CROBAT 029 PSA 9 $17.82 est." [ref=e112]:
                  - generic [ref=e113]:
                    - generic [ref=e114]: 2024 POKEMON SFA EN-SHROUDED FABLE CROBAT 029 PSA 9
                    - generic [ref=e115]: $17.82 est.
                - button "2023 POKEMON SWSH BLACK STAR PROMO CRZ S/C UNOWN V/LUGIA V UNOWN V 300 PSA 9 $15.84 est." [ref=e116]:
                  - generic [ref=e117]:
                    - generic [ref=e118]: 2023 POKEMON SWSH BLACK STAR PROMO CRZ S/C UNOWN V/LUGIA V UNOWN V 300 PSA 9
                    - generic [ref=e119]: $15.84 est.
                - button "2025 POKEMON JTG EN-JOURNEY TOGETHER ILLUSTRATION RARE MARACTUS 160 PSA 9 $17.78 est." [ref=e120]:
                  - generic [ref=e121]:
                    - generic [ref=e122]: 2025 POKEMON JTG EN-JOURNEY TOGETHER ILLUSTRATION RARE MARACTUS 160 PSA 9
                    - generic [ref=e123]: $17.78 est.
                - button "2021 POKEMON JAPANESE SWORD & SHIELD VMAX CLIMAX VMAX CLIMAX ELECTRODE 048 PSA 8 $17.82 est." [ref=e124]:
                  - generic [ref=e125]:
                    - generic [ref=e126]: 2021 POKEMON JAPANESE SWORD & SHIELD VMAX CLIMAX VMAX CLIMAX ELECTRODE 048 PSA 8
                    - generic [ref=e127]: $17.82 est.
                - button "2000 POKEMON JAPANESE NEO 2 POLIWAG 60 PSA 9 $31.50 est." [ref=e128]:
                  - generic [ref=e129]:
                    - generic [ref=e130]: 2000 POKEMON JAPANESE NEO 2 POLIWAG 60 PSA 9
                    - generic [ref=e131]: $31.50 est.
                - button "2023 POKEMON JAPANESE SV2a-POKEMON 151 MASTER BALL REVERSE HOLO CLOYSTER 091 PSA 9 $16.83 est." [ref=e132]:
                  - generic [ref=e133]:
                    - generic [ref=e134]: 2023 POKEMON JAPANESE SV2a-POKEMON 151 MASTER BALL REVERSE HOLO CLOYSTER 091 PSA 9
                    - generic [ref=e135]: $16.83 est.
                - button "2025 POKEMON PRE EN-PRISMATIC EVOLUTIONS ULTRA RARE RAIFORT 142 PSA 9 $15.39 est." [ref=e136]:
                  - generic [ref=e137]:
                    - generic [ref=e138]: 2025 POKEMON PRE EN-PRISMATIC EVOLUTIONS ULTRA RARE RAIFORT 142 PSA 9
                    - generic [ref=e139]: $15.39 est.
                - button "2025 POKEMON MEP EN-ME BLACK STAR PROMO ULTRA-PREMIUM COLLECTION ORICORIO ex 024 PSA 9 $30.69 est." [ref=e140]:
                  - generic [ref=e141]:
                    - generic [ref=e142]: 2025 POKEMON MEP EN-ME BLACK STAR PROMO ULTRA-PREMIUM COLLECTION ORICORIO ex 024 PSA 9
                    - generic [ref=e143]: $30.69 est.
                - button "2023 POKEMON PAL EN-PALDEA EVOLVED FORRETRESS ex 005 PSA 10 $43.56 est." [ref=e144]:
                  - generic [ref=e145]:
                    - generic [ref=e146]: 2023 POKEMON PAL EN-PALDEA EVOLVED FORRETRESS ex 005 PSA 10
                    - generic [ref=e147]: $43.56 est.
                - button "2024 POKEMON SSP EN-SURGING SPARKS BLACK KYUREM ex 048 PSA 8 $14.85 est." [ref=e148]:
                  - generic [ref=e149]:
                    - generic [ref=e150]: 2024 POKEMON SSP EN-SURGING SPARKS BLACK KYUREM ex 048 PSA 8
                    - generic [ref=e151]: $14.85 est.
                - button "2025 POKEMON JTG EN-JOURNEY TOGETHER ILLUSTRATION RARE LILLIE'S RIBOMBEE 164 PSA 8 $17.79 est." [ref=e152]:
                  - generic [ref=e153]:
                    - generic [ref=e154]: 2025 POKEMON JTG EN-JOURNEY TOGETHER ILLUSTRATION RARE LILLIE'S RIBOMBEE 164 PSA 8
                    - generic [ref=e155]: $17.79 est.
                - button "2024 POKEMON SFA EN-SHROUDED FABLE CROBAT 029 PSA 9 $17.82 est." [ref=e156]:
                  - generic [ref=e157]:
                    - generic [ref=e158]: 2024 POKEMON SFA EN-SHROUDED FABLE CROBAT 029 PSA 9
                    - generic [ref=e159]: $17.82 est.
                - button "2017 POKEMON JAPANESE THE BEST OF XY THE BEST OF XY AROMATISSE-REV.FOIL 094 PSA 9 $17.82 est." [ref=e160]:
                  - generic [ref=e161]:
                    - generic [ref=e162]: 2017 POKEMON JAPANESE THE BEST OF XY THE BEST OF XY AROMATISSE-REV.FOIL 094 PSA 9
                    - generic [ref=e163]: $17.82 est.
                - button "2021 POKEMON JAPANESE SWORD & SHIELD VMAX CLIMAX VMAX CLIMAX ORBEETLE-HOLO 079 PSA 8 $16.82 est." [ref=e164]:
                  - generic [ref=e165]:
                    - generic [ref=e166]: 2021 POKEMON JAPANESE SWORD & SHIELD VMAX CLIMAX VMAX CLIMAX ORBEETLE-HOLO 079 PSA 8
                    - generic [ref=e167]: $16.82 est.
                - button "2024 POKEMON SVP EN-SV BLACK STAR PROMO SURGING SPARKS ETB MAGNETON 159 PSA 9 $24.75 est." [ref=e168]:
                  - generic [ref=e169]:
                    - generic [ref=e170]: 2024 POKEMON SVP EN-SV BLACK STAR PROMO SURGING SPARKS ETB MAGNETON 159 PSA 9
                    - generic [ref=e171]: $24.75 est.
                - button "2025 POKEMON JTG EN-JOURNEY TOGETHER ULTRA RARE DUDUNSPARCE ex 178 PSA 9 $15.81 est." [ref=e172]:
                  - generic [ref=e173]:
                    - generic [ref=e174]: 2025 POKEMON JTG EN-JOURNEY TOGETHER ULTRA RARE DUDUNSPARCE ex 178 PSA 9
                    - generic [ref=e175]: $15.81 est.
                - button "2025 POKEMON JAPANESE SV11B-BLACK BOLT REVERSE HOLO LAMPENT 016 PSA 9 $17.82 est." [ref=e176]:
                  - generic [ref=e177]:
                    - generic [ref=e178]: 2025 POKEMON JAPANESE SV11B-BLACK BOLT REVERSE HOLO LAMPENT 016 PSA 9
                    - generic [ref=e179]: $17.82 est.
                - button "2004 POKEMON EX FIRE RED & LEAF GREEN FIRE RED & LEAF GREEN EXP.ALL-REVERSE FOIL 91 PSA 5 $10.80 est." [ref=e180]:
                  - generic [ref=e181]:
                    - generic [ref=e182]: 2004 POKEMON EX FIRE RED & LEAF GREEN FIRE RED & LEAF GREEN EXP.ALL-REVERSE FOIL 91 PSA 5
                    - generic [ref=e183]: $10.80 est.
                - button "2025 POKEMON PFL EN-PHANTASMAL FLAMES MEGA GENGAR ex 056 PSA 9 $28.71 est." [ref=e184]:
                  - generic [ref=e185]:
                    - generic [ref=e186]: 2025 POKEMON PFL EN-PHANTASMAL FLAMES MEGA GENGAR ex 056 PSA 9
                    - generic [ref=e187]: $28.71 est.
                - button "2023 POKEMON SVI EN-SCARLET & VIOLET JACQ 250 PSA 9 $17.79 est." [ref=e188]:
                  - generic [ref=e189]:
                    - generic [ref=e190]: 2023 POKEMON SVI EN-SCARLET & VIOLET JACQ 250 PSA 9
                    - generic [ref=e191]: $17.79 est.
                - button "2024 POKEMON SFA EN-SHROUDED FABLE CROBAT 029 PSA 9 $17.82 est." [ref=e192]:
                  - generic [ref=e193]:
                    - generic [ref=e194]: 2024 POKEMON SFA EN-SHROUDED FABLE CROBAT 029 PSA 9
                    - generic [ref=e195]: $17.82 est.
                - button "2023 POKEMON SWSH BLACK STAR PROMO CRZ S/C UNOWN V/LUGIA V UNOWN V 300 PSA 9 $15.84 est." [ref=e196]:
                  - generic [ref=e197]:
                    - generic [ref=e198]: 2023 POKEMON SWSH BLACK STAR PROMO CRZ S/C UNOWN V/LUGIA V UNOWN V 300 PSA 9
                    - generic [ref=e199]: $15.84 est.
                - button "2025 POKEMON JTG EN-JOURNEY TOGETHER ILLUSTRATION RARE MARACTUS 160 PSA 9 $17.78 est." [ref=e200]:
                  - generic [ref=e201]:
                    - generic [ref=e202]: 2025 POKEMON JTG EN-JOURNEY TOGETHER ILLUSTRATION RARE MARACTUS 160 PSA 9
                    - generic [ref=e203]: $17.78 est.
            - generic [ref=e204]:
              - heading "Open a Pack" [level=1] [ref=e205]
              - generic [ref=e206]:
                - link "All" [ref=e207]:
                  - /url: /packs/6
                - link "Pokémon" [ref=e208]:
                  - /url: /packs/2
                - link "Football" [ref=e209]:
                  - /url: /packs/4
                - link "Multi-Sport" [ref=e210]:
                  - /url: /packs/7
                - link "Comics" [ref=e211]:
                  - /url: /packs/8
              - generic [ref=e212]:
                - generic [ref=e213]:
                  - heading "Multi-Sport Packages" [level=2] [ref=e214]
                  - link "See all" [ref=e215]:
                    - /url: /packs/1
                    - text: See all
                    - img [ref=e216]
                - generic [ref=e219]:
                  - link "MAX PULL $400 Multi-Sport Starter Pack Multi-Sport Starter Pack $25" [ref=e221]:
                    - /url: /packs/pack/9
                    - generic [ref=e222]: MAX PULL $400
                    - img "Multi-Sport Starter Pack" [ref=e224]
                    - generic [ref=e225]:
                      - heading "Multi-Sport Starter Pack" [level=3] [ref=e226]
                      - paragraph [ref=e227]: $25
                  - link "MAX PULL $1,000 Multi-Sport Premier Pack Multi-Sport Premier Pack $50" [ref=e229]:
                    - /url: /packs/pack/10
                    - generic [ref=e230]: MAX PULL $1,000
                    - img "Multi-Sport Premier Pack" [ref=e232]
                    - generic [ref=e233]:
                      - heading "Multi-Sport Premier Pack" [level=3] [ref=e234]
                      - paragraph [ref=e235]: $50
                  - link "MAX PULL $3,500 Multi-Sport Pro Pack Multi-Sport Pro Pack $100" [ref=e237]:
                    - /url: /packs/pack/11
                    - generic [ref=e238]: MAX PULL $3,500
                    - generic [ref=e239]:
                      - img "Multi-Sport Pro Pack"
                    - generic [ref=e240]:
                      - heading "Multi-Sport Pro Pack" [level=3] [ref=e241]
                      - paragraph [ref=e242]: $100
                  - link "MAX PULL $7,500 Multi-Sport Elite Pack Multi-Sport Elite Pack $250" [ref=e244]:
                    - /url: /packs/pack/12
                    - generic [ref=e245]: MAX PULL $7,500
                    - generic [ref=e246]:
                      - img "Multi-Sport Elite Pack"
                    - generic [ref=e247]:
                      - heading "Multi-Sport Elite Pack" [level=3] [ref=e248]
                      - paragraph [ref=e249]: $250
              - generic [ref=e250]:
                - generic [ref=e251]:
                  - heading "Pokémon Packages" [level=2] [ref=e252]
                  - link "See all" [ref=e253]:
                    - /url: /packs/9
                    - text: See all
                    - img [ref=e254]
                - generic [ref=e257]:
                  - link "MAX PULL $400 Pokémon Starter Pack Pokémon Starter Pack $25" [ref=e259]:
                    - /url: /packs/pack/5
                    - generic [ref=e260]: MAX PULL $400
                    - img "Pokémon Starter Pack" [ref=e262]
                    - generic [ref=e263]:
                      - heading "Pokémon Starter Pack" [level=3] [ref=e264]
                      - paragraph [ref=e265]: $25
                  - link "MAX PULL $1,000 Pokémon Premier Pack Pokémon Premier Pack $50" [ref=e267]:
                    - /url: /packs/pack/6
                    - generic [ref=e268]: MAX PULL $1,000
                    - img "Pokémon Premier Pack" [ref=e270]
                    - generic [ref=e271]:
                      - heading "Pokémon Premier Pack" [level=3] [ref=e272]
                      - paragraph [ref=e273]: $50
                  - link "MAX PULL $2,500 Pokémon Pro Pack Pokémon Pro Pack $100" [ref=e275]:
                    - /url: /packs/pack/7
                    - generic [ref=e276]: MAX PULL $2,500
                    - generic [ref=e277]:
                      - img "Pokémon Pro Pack"
                    - generic [ref=e278]:
                      - heading "Pokémon Pro Pack" [level=3] [ref=e279]
                      - paragraph [ref=e280]: $100
                  - link "MAX PULL $4,500 Pokémon Elite Pack Pokémon Elite Pack $250" [ref=e282]:
                    - /url: /packs/pack/8
                    - generic [ref=e283]: MAX PULL $4,500
                    - generic [ref=e284]:
                      - img "Pokémon Elite Pack"
                    - generic [ref=e285]:
                      - heading "Pokémon Elite Pack" [level=3] [ref=e286]
                      - paragraph [ref=e287]: $250
          - generic [ref=e289]:
            - generic [ref=e291]:
              - link "Download ParlayPlay On The App Store" [ref=e292]:
                - /url: https://parlayplay.onelink.me/oLJk/gnqpwjha
                - img "Download ParlayPlay On The App Store" [ref=e293]
              - paragraph [ref=e294]:
                - text: Get the app.
                - text: Better. Faster. Convenient
            - navigation [ref=e295]:
              - link "Privacy" [ref=e296]:
                - /url: /privacy-policy
              - link "Fantasy Terms" [ref=e297]:
                - /url: /terms
              - link "Packs Terms" [ref=e298]:
                - /url: /terms/packs
              - link "Responsible Gaming" [ref=e299]:
                - /url: /responsible-gaming
              - link "Gaming Rules" [ref=e300]:
                - /url: /rules
              - link "FAQ" [ref=e301]:
                - /url: https://intercom.help/parlayplay/en/
            - navigation [ref=e302]:
              - generic [ref=e303]:
                - paragraph [ref=e304]: © ParlayPlay 2026
                - generic [ref=e305]:
                  - link "ParlayPlay on Facebook" [ref=e306]:
                    - /url: https://www.facebook.com/parlayplay.io
                    - img [ref=e307]
                  - link "ParlayPlay on Instagram" [ref=e309]:
                    - /url: https://www.instagram.com/parlayplay_?igsh=bHBldWQyMmV2b3Y4
                    - img [ref=e310]
                  - link "ParlayPlay on Twitter" [ref=e312]:
                    - /url: https://www.twitter.com/parlay_play
                    - img [ref=e313]
                  - link "ParlayPlay on Discord" [ref=e315]:
                    - /url: https://discord.com/invite/parlayplay
                    - img [ref=e316]
                - img "18+ icon" [ref=e318]
            - paragraph [ref=e320]
      - contentinfo [ref=e321]:
        - navigation [ref=e322]:
          - list [ref=e323]:
            - listitem [ref=e324]:
              - button "Home" [ref=e325] [cursor=pointer]:
                - generic [ref=e326]:
                  - img [ref=e327]
                  - generic [ref=e328]: Home
            - listitem [ref=e329]:
              - button "Entries 67" [ref=e330] [cursor=pointer]:
                - generic [ref=e331]:
                  - img [ref=e332]
                  - generic [ref=e333]: Entries
                - generic [ref=e334]: "67"
            - listitem [ref=e335]:
              - button "Feed" [ref=e336] [cursor=pointer]:
                - generic [ref=e337]:
                  - img [ref=e338]
                  - generic [ref=e339]: Feed
            - listitem [ref=e340]:
              - button "Rewards 44" [ref=e341] [cursor=pointer]:
                - generic [ref=e342]:
                  - img [ref=e343]
                  - generic [ref=e344]: Rewards
                - generic [ref=e345]: "44"
            - listitem [ref=e346]:
              - button "Packs" [active] [ref=e347] [cursor=pointer]:
                - generic [ref=e348]:
                  - img [ref=e349]
                  - generic [ref=e350]: Packs
    - generic:
      - region "Notifications Alt+T"
  - alert [ref=e351]: ParlayPlay | Fun Fantasy Sports - Packs
```

# Test source

```ts
  1   | /**
  2   |  * Mobile bottom-nav routing: each tab routes to its destination and only the
  3   |  * current route's tab carries the `border-b-2` underline. The Entries tab's
  4   |  * cross-sub-tab behaviour lives in entries-nav-indicator.spec.ts. The fifth
  5   |  * slot is Packs when the packs kill switch allows it, Free2Play otherwise.
  6   |  */
  7   | import { test, expect } from '../../fixtures/test.extend';
  8   | import { HomePage } from '@pages/home.page';
  9   | 
  10  | test.describe(
  11  |   'Bottom nav - tab routing and active indicator',
  12  |   { tag: ['@navigation', '@prod'] },
  13  |   () => {
  14  |     // Read-only navigation, isolated context per test — safe in parallel.
  15  |     test.describe.configure({ mode: 'parallel' });
  16  | 
  17  |     test.beforeEach(async ({ loggedInPage }) => {
  18  |       const homePage = new HomePage(loggedInPage);
  19  |       await loggedInPage.goto('/');
  20  |       await homePage.waitForFeedReady();
  21  |     });
  22  | 
  23  |     test('Feed tab routes to /challenges/feed and takes the indicator', async ({
  24  |       loggedInPage: page,
  25  |     }) => {
  26  |       const homePage = new HomePage(page);
  27  | 
  28  |       await test.step('Home tab is underlined on landing', async () => {
  29  |         await expect(homePage.navIndicator('Home')).toHaveClass(/border-b-2/);
  30  |         await expect(homePage.navIndicator('Feed')).not.toHaveClass(/border-b-2/);
  31  |       });
  32  | 
  33  |       await test.step('Open Feed — indicator moves to Feed, off Home', async () => {
  34  |         await homePage.enterFeedPage();
  35  |         await page.waitForURL('**/challenges/feed');
  36  |         await expect(homePage.navIndicator('Feed')).toHaveClass(/border-b-2/);
  37  |         await expect(homePage.navIndicator('Home')).not.toHaveClass(/border-b-2/);
  38  |       });
  39  |     });
  40  | 
  41  |     test('Rewards tab routes into /rewards and takes the indicator', async ({
  42  |       loggedInPage: page,
  43  |     }) => {
  44  |       const homePage = new HomePage(page);
  45  | 
  46  |       await test.step('Open Rewards — lands on a /rewards route with Rewards underlined', async () => {
  47  |         await homePage.enterRewarsdsPage();
  48  |         // The tab resolves to /rewards or /rewards/promotions depending on
  49  |         // the partner-reward count, so match the /rewards prefix.
  50  |         await page.waitForURL(/\/rewards(\/|$)/);
  51  |         await expect(homePage.navIndicator('Rewards')).toHaveClass(/border-b-2/);
  52  |       });
  53  |     });
  54  | 
  55  |     test('Fifth tab (Free2Play or Packs) routes and takes the indicator', async ({
  56  |       loggedInPage: page,
  57  |     }) => {
  58  |       const homePage = new HomePage(page);
  59  | 
  60  |       // The fifth slot renders Packs when the user's packs_visibility allows
  61  |       // it and Free2Play otherwise — detect which one this environment mounted.
  62  |       const packsVisible = await homePage.packsTab.isVisible().catch(() => false);
  63  | 
  64  |       if (packsVisible) {
  65  |         await test.step('Open Packs — indicator moves to Packs, off Home', async () => {
  66  |           await homePage.packsTab.click();
  67  |           await page.waitForURL('**/packs**');
> 68  |           await expect(homePage.navIndicator('Packs')).toHaveClass(/border-b-2/);
      |                                                        ^ Error: expect(locator).toHaveClass(expected) failed
  69  |           await expect(homePage.navIndicator('Home')).not.toHaveClass(/border-b-2/);
  70  |         });
  71  | 
  72  |         // With Packs in the footer, Free2Play relocates to the burger menu
  73  |         // (Account Center → Rewards) — no footer tab exists to underline.
  74  |         await test.step('Free2Play routes to /challenges/mp from the burger menu', async () => {
  75  |           await homePage.enterFree2PlayPage();
  76  |           await page.waitForURL('**/challenges/mp');
  77  |         });
  78  |       } else {
  79  |         await test.step('Open Free2Play — indicator moves to Free2Play, off Home', async () => {
  80  |           await homePage.enterFree2PlayPage();
  81  |           await page.waitForURL('**/challenges/mp');
  82  |           await expect(homePage.navIndicator('Free2Play')).toHaveClass(/border-b-2/);
  83  |           await expect(homePage.navIndicator('Home')).not.toHaveClass(/border-b-2/);
  84  |         });
  85  |       }
  86  |     });
  87  | 
  88  |     test(
  89  |       'Only one tab is active at a time and Home restores',
  90  |       { tag: ['@smoke', '@critical'] },
  91  |       async ({ loggedInPage: page }) => {
  92  |         const homePage = new HomePage(page);
  93  | 
  94  |         await test.step('Open Feed — indicator moves to Feed, off Home', async () => {
  95  |           await homePage.enterFeedPage();
  96  |           await page.waitForURL('**/challenges/feed');
  97  |           await expect(homePage.navIndicator('Feed')).toHaveClass(/border-b-2/);
  98  |           await expect(homePage.navIndicator('Home')).not.toHaveClass(/border-b-2/);
  99  |         });
  100 | 
  101 |         await test.step('Return Home — indicator returns to Home, off Feed', async () => {
  102 |           await homePage.enterHomePage();
  103 |           await page.waitForURL(/\/$/);
  104 |           await expect(homePage.navIndicator('Home')).toHaveClass(/border-b-2/);
  105 |           await expect(homePage.navIndicator('Feed')).not.toHaveClass(/border-b-2/);
  106 |         });
  107 |       },
  108 |     );
  109 |   },
  110 | );
  111 | 
```