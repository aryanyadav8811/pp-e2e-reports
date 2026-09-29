# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: navigation/footer-nav.spec.ts >> Bottom nav - tab routing and active indicator >> Fifth tab (Free2Play or Packs) routes and takes the indicator
- Location: tests/navigation/footer-nav.spec.ts:55:5

# Error details

```
TimeoutError: locator.click: Timeout 15000ms exceeded.
Call log:
  - waiting for getByRole('button', { name: 'Toggle Menu' }).filter({ visible: true }).first()
    - locator resolved to <button class="w-8 p-1" aria-label="Toggle Menu">…</button>
  - attempting click action
    - waiting for element to be visible, enabled and stable
    - element is visible, enabled and stable
    - scrolling into view if needed
    - done scrolling

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
              - generic [ref=e13]: $679.77
              - generic [ref=e14]:
                - img "gift-icon" [ref=e15]
                - text: "9.00"
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
                - button "2006 POKEMON EX TRAINER KIT 2 MINUN HALF DECK TRNR. KIT 2-MINUN HALF DK. FIRE ENERGY 11 PSA 9 $21.78 est." [ref=e44]:
                  - generic [ref=e45]:
                    - generic [ref=e46]: 2006 POKEMON EX TRAINER KIT 2 MINUN HALF DECK TRNR. KIT 2-MINUN HALF DK. FIRE ENERGY 11 PSA 9
                    - generic [ref=e47]: $21.78 est.
                - button "2025 POKEMON PLAY! POKEMON PRIZE PACK POKEMON PRIZE PACK-HOLO AREA ZERO UNDERDEPTHS 131 PSA 9 $21.78 est." [ref=e48]:
                  - generic [ref=e49]:
                    - generic [ref=e50]: 2025 POKEMON PLAY! POKEMON PRIZE PACK POKEMON PRIZE PACK-HOLO AREA ZERO UNDERDEPTHS 131 PSA 9
                    - generic [ref=e51]: $21.78 est.
                - button "2024 POKEMON SVP EN-SV BLACK STAR PROMO SHROUDED FABLE ETB PECHARUNT 129 PSA 9 $20.79 est." [ref=e52]:
                  - generic [ref=e53]:
                    - generic [ref=e54]: 2024 POKEMON SVP EN-SV BLACK STAR PROMO SHROUDED FABLE ETB PECHARUNT 129 PSA 9
                    - generic [ref=e55]: $20.79 est.
                - button "2023 BOWMAN MEGA BOX CHROME CHROME MATT MERVIS 74 PSA 10 $24.75 est." [ref=e56]:
                  - generic [ref=e57]:
                    - generic [ref=e58]: 2023 BOWMAN MEGA BOX CHROME CHROME MATT MERVIS 74 PSA 10
                    - generic [ref=e59]: $24.75 est.
                - button "2021 POKEMON SWSH BLACK STAR PROMO SHNG.FATES ELITE TRNR.BOX FA/EEVEE VMAX 087 PSA 9 $21.78 est." [ref=e60]:
                  - generic [ref=e61]:
                    - generic [ref=e62]: 2021 POKEMON SWSH BLACK STAR PROMO SHNG.FATES ELITE TRNR.BOX FA/EEVEE VMAX 087 PSA 9
                    - generic [ref=e63]: $21.78 est.
                - button "2004 POKEMON EX FIRE RED & LEAF GREEN FIRE RED & LEAF GREEN EXP.ALL-REVERSE FOIL 91 PSA 5 $10.80 est." [ref=e64]:
                  - generic [ref=e65]:
                    - generic [ref=e66]: 2004 POKEMON EX FIRE RED & LEAF GREEN FIRE RED & LEAF GREEN EXP.ALL-REVERSE FOIL 91 PSA 5
                    - generic [ref=e67]: $10.80 est.
                - button "2021 POKEMON CELEBRATIONS CLASSIC COLLECTION CLASS.COLL-GYM CHALLENGE ROCKET'S ZAPDOS-HOLO 15 PSA 8 $19.08 est." [ref=e68]:
                  - generic [ref=e69]:
                    - generic [ref=e70]: 2021 POKEMON CELEBRATIONS CLASSIC COLLECTION CLASS.COLL-GYM CHALLENGE ROCKET'S ZAPDOS-HOLO 15 PSA 8
                    - generic [ref=e71]: $19.08 est.
                - button "2016 POKEMON XY EVOLUTIONS EVOLUTIONS-PRERELEASE GYARADOS-HOLO 34 PSA 8 $0.79 est." [ref=e72]:
                  - generic [ref=e73]:
                    - generic [ref=e74]: 2016 POKEMON XY EVOLUTIONS EVOLUTIONS-PRERELEASE GYARADOS-HOLO 34 PSA 8
                    - generic [ref=e75]: $0.79 est.
                - button "2016 POKEMON XY EVOLUTIONS EVOLUTIONS-PRERELEASE GYARADOS-HOLO 34 PSA 8 $0.55 est." [ref=e76]:
                  - generic [ref=e77]:
                    - generic [ref=e78]: 2016 POKEMON XY EVOLUTIONS EVOLUTIONS-PRERELEASE GYARADOS-HOLO 34 PSA 8
                    - generic [ref=e79]: $0.55 est.
                - button "2025 POKEMON PRE EN-PRISMATIC EVOLUTIONS POKE BALL REVERSE HOLO ESPEON 033 PSA 9 $21.78 est." [ref=e80]:
                  - generic [ref=e81]:
                    - generic [ref=e82]: 2025 POKEMON PRE EN-PRISMATIC EVOLUTIONS POKE BALL REVERSE HOLO ESPEON 033 PSA 9
                    - generic [ref=e83]: $21.78 est.
                - button "2015 POKEMON XY BREAKTHROUGH BREAKTHROUGH GALLADE-HOLO 84 PSA 9 $21.78 est." [ref=e84]:
                  - generic [ref=e85]:
                    - generic [ref=e86]: 2015 POKEMON XY BREAKTHROUGH BREAKTHROUGH GALLADE-HOLO 84 PSA 9
                    - generic [ref=e87]: $21.78 est.
                - button "2022 POKEMON SWORD & SHIELD SILVER TEMPEST SILVER TEMPEST FA/WORKER 195 PSA 8 $16.83 est." [ref=e88]:
                  - generic [ref=e89]:
                    - generic [ref=e90]: 2022 POKEMON SWORD & SHIELD SILVER TEMPEST SILVER TEMPEST FA/WORKER 195 PSA 8
                    - generic [ref=e91]: $16.83 est.
                - button "2023 POKEMON OBF EN-OBSIDIAN FLAMES TADBULB 076 PSA 9 $18.81 est." [ref=e92]:
                  - generic [ref=e93]:
                    - generic [ref=e94]: 2023 POKEMON OBF EN-OBSIDIAN FLAMES TADBULB 076 PSA 9
                    - generic [ref=e95]: $18.81 est.
                - button "2016 POKEMON XY EVOLUTIONS EVOLUTIONS-PRERELEASE GYARADOS-HOLO 34 PSA 8 $1.34 est." [ref=e96]:
                  - generic [ref=e97]:
                    - generic [ref=e98]: 2016 POKEMON XY EVOLUTIONS EVOLUTIONS-PRERELEASE GYARADOS-HOLO 34 PSA 8
                    - generic [ref=e99]: $1.34 est.
                - button "2016 POKEMON XY EVOLUTIONS EVOLUTIONS-PRERELEASE GYARADOS-HOLO 34 PSA 8 $0.87 est." [ref=e100]:
                  - generic [ref=e101]:
                    - generic [ref=e102]: 2016 POKEMON XY EVOLUTIONS EVOLUTIONS-PRERELEASE GYARADOS-HOLO 34 PSA 8
                    - generic [ref=e103]: $0.87 est.
                - button "2015 POKEMON JAPANESE LEGENDARY SHINE COLLECTION LEGENDARY SHINE COLL. HIPPOPOTAS 013 PSA 8 $20.79 est." [ref=e104]:
                  - generic [ref=e105]:
                    - generic [ref=e106]: 2015 POKEMON JAPANESE LEGENDARY SHINE COLLECTION LEGENDARY SHINE COLL. HIPPOPOTAS 013 PSA 8
                    - generic [ref=e107]: $20.79 est.
                - button "1999 TOPPS POKEMON TV WEEPINBELL 70 PSA 9 $15.84 est." [ref=e108]:
                  - generic [ref=e109]:
                    - generic [ref=e110]: 1999 TOPPS POKEMON TV WEEPINBELL 70 PSA 9
                    - generic [ref=e111]: $15.84 est.
                - button "2016 POKEMON XY EVOLUTIONS EVOLUTIONS-PRERELEASE GYARADOS-HOLO 34 PSA 8 $0.49 est." [ref=e112]:
                  - generic [ref=e113]:
                    - generic [ref=e114]: 2016 POKEMON XY EVOLUTIONS EVOLUTIONS-PRERELEASE GYARADOS-HOLO 34 PSA 8
                    - generic [ref=e115]: $0.49 est.
                - button "2022 POKEMON SWORD u0026 SHIELD BRILLIANT STARS BRILLIANT STARS PROBOPASS-REV.FOIL 099 PSA 8 $18.08 est." [ref=e116]:
                  - generic [ref=e117]:
                    - generic [ref=e118]: 2022 POKEMON SWORD u0026 SHIELD BRILLIANT STARS BRILLIANT STARS PROBOPASS-REV.FOIL 099 PSA 8
                    - generic [ref=e119]: $18.08 est.
                - 'button "2024 PANINI DONRUSS OPTIC #180 JAXON SMITH-NJIGBA PURPLE STARS PSA 9 $9.00 est." [ref=e120]':
                  - generic [ref=e121]:
                    - generic [ref=e122]: "2024 PANINI DONRUSS OPTIC #180 JAXON SMITH-NJIGBA PURPLE STARS PSA 9"
                    - generic [ref=e123]: $9.00 est.
                - button "2006 POKEMON EX TRAINER KIT 2 MINUN HALF DECK TRNR. KIT 2-MINUN HALF DK. FIRE ENERGY 11 PSA 9 $21.78 est." [ref=e124]:
                  - generic [ref=e125]:
                    - generic [ref=e126]: 2006 POKEMON EX TRAINER KIT 2 MINUN HALF DECK TRNR. KIT 2-MINUN HALF DK. FIRE ENERGY 11 PSA 9
                    - generic [ref=e127]: $21.78 est.
                - button "2025 POKEMON PLAY! POKEMON PRIZE PACK POKEMON PRIZE PACK-HOLO AREA ZERO UNDERDEPTHS 131 PSA 9 $21.78 est." [ref=e128]:
                  - generic [ref=e129]:
                    - generic [ref=e130]: 2025 POKEMON PLAY! POKEMON PRIZE PACK POKEMON PRIZE PACK-HOLO AREA ZERO UNDERDEPTHS 131 PSA 9
                    - generic [ref=e131]: $21.78 est.
                - button "2024 POKEMON SVP EN-SV BLACK STAR PROMO SHROUDED FABLE ETB PECHARUNT 129 PSA 9 $20.79 est." [ref=e132]:
                  - generic [ref=e133]:
                    - generic [ref=e134]: 2024 POKEMON SVP EN-SV BLACK STAR PROMO SHROUDED FABLE ETB PECHARUNT 129 PSA 9
                    - generic [ref=e135]: $20.79 est.
                - button "2023 BOWMAN MEGA BOX CHROME CHROME MATT MERVIS 74 PSA 10 $24.75 est." [ref=e136]:
                  - generic [ref=e137]:
                    - generic [ref=e138]: 2023 BOWMAN MEGA BOX CHROME CHROME MATT MERVIS 74 PSA 10
                    - generic [ref=e139]: $24.75 est.
                - button "2021 POKEMON SWSH BLACK STAR PROMO SHNG.FATES ELITE TRNR.BOX FA/EEVEE VMAX 087 PSA 9 $21.78 est." [ref=e140]:
                  - generic [ref=e141]:
                    - generic [ref=e142]: 2021 POKEMON SWSH BLACK STAR PROMO SHNG.FATES ELITE TRNR.BOX FA/EEVEE VMAX 087 PSA 9
                    - generic [ref=e143]: $21.78 est.
                - button "2004 POKEMON EX FIRE RED & LEAF GREEN FIRE RED & LEAF GREEN EXP.ALL-REVERSE FOIL 91 PSA 5 $10.80 est." [ref=e144]:
                  - generic [ref=e145]:
                    - generic [ref=e146]: 2004 POKEMON EX FIRE RED & LEAF GREEN FIRE RED & LEAF GREEN EXP.ALL-REVERSE FOIL 91 PSA 5
                    - generic [ref=e147]: $10.80 est.
                - button "2021 POKEMON CELEBRATIONS CLASSIC COLLECTION CLASS.COLL-GYM CHALLENGE ROCKET'S ZAPDOS-HOLO 15 PSA 8 $19.08 est." [ref=e148]:
                  - generic [ref=e149]:
                    - generic [ref=e150]: 2021 POKEMON CELEBRATIONS CLASSIC COLLECTION CLASS.COLL-GYM CHALLENGE ROCKET'S ZAPDOS-HOLO 15 PSA 8
                    - generic [ref=e151]: $19.08 est.
                - button "2016 POKEMON XY EVOLUTIONS EVOLUTIONS-PRERELEASE GYARADOS-HOLO 34 PSA 8 $0.79 est." [ref=e152]:
                  - generic [ref=e153]:
                    - generic [ref=e154]: 2016 POKEMON XY EVOLUTIONS EVOLUTIONS-PRERELEASE GYARADOS-HOLO 34 PSA 8
                    - generic [ref=e155]: $0.79 est.
                - button "2016 POKEMON XY EVOLUTIONS EVOLUTIONS-PRERELEASE GYARADOS-HOLO 34 PSA 8 $0.55 est." [ref=e156]:
                  - generic [ref=e157]:
                    - generic [ref=e158]: 2016 POKEMON XY EVOLUTIONS EVOLUTIONS-PRERELEASE GYARADOS-HOLO 34 PSA 8
                    - generic [ref=e159]: $0.55 est.
                - button "2025 POKEMON PRE EN-PRISMATIC EVOLUTIONS POKE BALL REVERSE HOLO ESPEON 033 PSA 9 $21.78 est." [ref=e160]:
                  - generic [ref=e161]:
                    - generic [ref=e162]: 2025 POKEMON PRE EN-PRISMATIC EVOLUTIONS POKE BALL REVERSE HOLO ESPEON 033 PSA 9
                    - generic [ref=e163]: $21.78 est.
                - button "2015 POKEMON XY BREAKTHROUGH BREAKTHROUGH GALLADE-HOLO 84 PSA 9 $21.78 est." [ref=e164]:
                  - generic [ref=e165]:
                    - generic [ref=e166]: 2015 POKEMON XY BREAKTHROUGH BREAKTHROUGH GALLADE-HOLO 84 PSA 9
                    - generic [ref=e167]: $21.78 est.
                - button "2022 POKEMON SWORD & SHIELD SILVER TEMPEST SILVER TEMPEST FA/WORKER 195 PSA 8 $16.83 est." [ref=e168]:
                  - generic [ref=e169]:
                    - generic [ref=e170]: 2022 POKEMON SWORD & SHIELD SILVER TEMPEST SILVER TEMPEST FA/WORKER 195 PSA 8
                    - generic [ref=e171]: $16.83 est.
                - button "2023 POKEMON OBF EN-OBSIDIAN FLAMES TADBULB 076 PSA 9 $18.81 est." [ref=e172]:
                  - generic [ref=e173]:
                    - generic [ref=e174]: 2023 POKEMON OBF EN-OBSIDIAN FLAMES TADBULB 076 PSA 9
                    - generic [ref=e175]: $18.81 est.
                - button "2016 POKEMON XY EVOLUTIONS EVOLUTIONS-PRERELEASE GYARADOS-HOLO 34 PSA 8 $1.34 est." [ref=e176]:
                  - generic [ref=e177]:
                    - generic [ref=e178]: 2016 POKEMON XY EVOLUTIONS EVOLUTIONS-PRERELEASE GYARADOS-HOLO 34 PSA 8
                    - generic [ref=e179]: $1.34 est.
                - button "2016 POKEMON XY EVOLUTIONS EVOLUTIONS-PRERELEASE GYARADOS-HOLO 34 PSA 8 $0.87 est." [ref=e180]:
                  - generic [ref=e181]:
                    - generic [ref=e182]: 2016 POKEMON XY EVOLUTIONS EVOLUTIONS-PRERELEASE GYARADOS-HOLO 34 PSA 8
                    - generic [ref=e183]: $0.87 est.
                - button "2015 POKEMON JAPANESE LEGENDARY SHINE COLLECTION LEGENDARY SHINE COLL. HIPPOPOTAS 013 PSA 8 $20.79 est." [ref=e184]:
                  - generic [ref=e185]:
                    - generic [ref=e186]: 2015 POKEMON JAPANESE LEGENDARY SHINE COLLECTION LEGENDARY SHINE COLL. HIPPOPOTAS 013 PSA 8
                    - generic [ref=e187]: $20.79 est.
                - button "1999 TOPPS POKEMON TV WEEPINBELL 70 PSA 9 $15.84 est." [ref=e188]:
                  - generic [ref=e189]:
                    - generic [ref=e190]: 1999 TOPPS POKEMON TV WEEPINBELL 70 PSA 9
                    - generic [ref=e191]: $15.84 est.
                - button "2016 POKEMON XY EVOLUTIONS EVOLUTIONS-PRERELEASE GYARADOS-HOLO 34 PSA 8 $0.49 est." [ref=e192]:
                  - generic [ref=e193]:
                    - generic [ref=e194]: 2016 POKEMON XY EVOLUTIONS EVOLUTIONS-PRERELEASE GYARADOS-HOLO 34 PSA 8
                    - generic [ref=e195]: $0.49 est.
                - button "2022 POKEMON SWORD u0026 SHIELD BRILLIANT STARS BRILLIANT STARS PROBOPASS-REV.FOIL 099 PSA 8 $18.08 est." [ref=e196]:
                  - generic [ref=e197]:
                    - generic [ref=e198]: 2022 POKEMON SWORD u0026 SHIELD BRILLIANT STARS BRILLIANT STARS PROBOPASS-REV.FOIL 099 PSA 8
                    - generic [ref=e199]: $18.08 est.
                - 'button "2024 PANINI DONRUSS OPTIC #180 JAXON SMITH-NJIGBA PURPLE STARS PSA 9 $9.00 est." [ref=e200]':
                  - generic [ref=e201]:
                    - generic [ref=e202]: "2024 PANINI DONRUSS OPTIC #180 JAXON SMITH-NJIGBA PURPLE STARS PSA 9"
                    - generic [ref=e203]: $9.00 est.
            - generic [ref=e204]:
              - heading "Open a Pack" [level=1] [ref=e205]
              - generic [ref=e207]:
                - link "All" [ref=e208]:
                  - /url: /packs/6
                - link "Pokémon" [ref=e209]:
                  - /url: /packs/2
                - link "Football" [ref=e210]:
                  - /url: /packs/4
                - link "Multi-Sport" [ref=e211]:
                  - /url: /packs/7
                - link "Comics" [ref=e212]:
                  - /url: /packs/8
              - generic [ref=e213]:
                - generic [ref=e214]:
                  - heading "Multi-Sport Packages" [level=2] [ref=e215]
                  - link "See all" [ref=e216]:
                    - /url: /packs/1
                    - text: See all
                    - img [ref=e217]
                - generic [ref=e220]:
                  - link "MAX PULL $500 Multi-Sport Starter Pack Multi-Sport Starter Pack $25" [ref=e222]:
                    - /url: /packs/pack/9
                    - generic [ref=e223]: MAX PULL $500
                    - img "Multi-Sport Starter Pack" [ref=e225]
                    - generic [ref=e226]:
                      - heading "Multi-Sport Starter Pack" [level=3] [ref=e227]
                      - paragraph [ref=e228]: $25
                  - link "MAX PULL $1,000 Multi-Sport Premier Pack Multi-Sport Premier Pack $50" [ref=e230]:
                    - /url: /packs/pack/10
                    - generic [ref=e231]: MAX PULL $1,000
                    - img "Multi-Sport Premier Pack" [ref=e233]
                    - generic [ref=e234]:
                      - heading "Multi-Sport Premier Pack" [level=3] [ref=e235]
                      - paragraph [ref=e236]: $50
                  - link "MAX PULL $2,000 Multi-Sport Pro Pack Multi-Sport Pro Pack $100" [ref=e238]:
                    - /url: /packs/pack/11
                    - generic [ref=e239]: MAX PULL $2,000
                    - generic [ref=e240]:
                      - img "Multi-Sport Pro Pack"
                    - generic [ref=e241]:
                      - heading "Multi-Sport Pro Pack" [level=3] [ref=e242]
                      - paragraph [ref=e243]: $100
                  - link "MAX PULL $5,000 Multi-Sport Elite Pack Multi-Sport Elite Pack $250" [ref=e245]:
                    - /url: /packs/pack/12
                    - generic [ref=e246]: MAX PULL $5,000
                    - generic [ref=e247]:
                      - img "Multi-Sport Elite Pack"
                    - generic [ref=e248]:
                      - heading "Multi-Sport Elite Pack" [level=3] [ref=e249]
                      - paragraph [ref=e250]: $250
              - generic [ref=e251]:
                - generic [ref=e252]:
                  - heading "Pokémon Packages" [level=2] [ref=e253]
                  - link "See all" [ref=e254]:
                    - /url: /packs/9
                    - text: See all
                    - img [ref=e255]
                - generic [ref=e258]:
                  - link "MAX PULL $500 Pokémon Starter Pack Pokémon Starter Pack $25" [ref=e260]:
                    - /url: /packs/pack/5
                    - generic [ref=e261]: MAX PULL $500
                    - img "Pokémon Starter Pack" [ref=e263]
                    - generic [ref=e264]:
                      - heading "Pokémon Starter Pack" [level=3] [ref=e265]
                      - paragraph [ref=e266]: $25
                  - link "MAX PULL $1,000 Pokémon Premier Pack Pokémon Premier Pack $50" [ref=e268]:
                    - /url: /packs/pack/6
                    - generic [ref=e269]: MAX PULL $1,000
                    - img "Pokémon Premier Pack" [ref=e271]
                    - generic [ref=e272]:
                      - heading "Pokémon Premier Pack" [level=3] [ref=e273]
                      - paragraph [ref=e274]: $50
                  - link "MAX PULL $2,000 Pokémon Pro Pack Pokémon Pro Pack $100" [ref=e276]:
                    - /url: /packs/pack/7
                    - generic [ref=e277]: MAX PULL $2,000
                    - generic [ref=e278]:
                      - img "Pokémon Pro Pack"
                    - generic [ref=e279]:
                      - heading "Pokémon Pro Pack" [level=3] [ref=e280]
                      - paragraph [ref=e281]: $100
                  - link "MAX PULL $5,000 Pokémon Elite Pack Pokémon Elite Pack $250" [ref=e283]:
                    - /url: /packs/pack/8
                    - generic [ref=e284]: MAX PULL $5,000
                    - generic [ref=e285]:
                      - img "Pokémon Elite Pack"
                    - generic [ref=e286]:
                      - heading "Pokémon Elite Pack" [level=3] [ref=e287]
                      - paragraph [ref=e288]: $250
          - generic [ref=e290]:
            - generic [ref=e292]:
              - link "Download ParlayPlay On The App Store" [ref=e293]:
                - /url: https://parlayplay.onelink.me/oLJk/gnqpwjha
                - img "Download ParlayPlay On The App Store" [ref=e294]
              - paragraph [ref=e295]:
                - text: Get the app.
                - text: Better. Faster. Convenient
            - navigation [ref=e296]:
              - link "Privacy" [ref=e297]:
                - /url: /privacy-policy
              - link "Fantasy Terms" [ref=e298]:
                - /url: /terms
              - link "Packs Terms" [ref=e299]:
                - /url: /terms/packs
              - link "Responsible Gaming" [ref=e300]:
                - /url: /responsible-gaming
              - link "Gaming Rules" [ref=e301]:
                - /url: /rules
              - link "FAQ" [ref=e302]:
                - /url: https://intercom.help/parlayplay/en/
            - navigation [ref=e303]:
              - generic [ref=e304]:
                - paragraph [ref=e305]: © ParlayPlay 2026
                - generic [ref=e306]:
                  - link "ParlayPlay on Facebook" [ref=e307]:
                    - /url: https://www.facebook.com/parlayplay.io
                    - img [ref=e308]
                  - link "ParlayPlay on Instagram" [ref=e310]:
                    - /url: https://www.instagram.com/parlayplay_?igsh=bHBldWQyMmV2b3Y4
                    - img [ref=e311]
                  - link "ParlayPlay on Twitter" [ref=e313]:
                    - /url: https://www.twitter.com/parlay_play
                    - img [ref=e314]
                  - link "ParlayPlay on Discord" [ref=e316]:
                    - /url: https://discord.com/invite/parlayplay
                    - img [ref=e317]
                - img "18+ icon" [ref=e319]
            - paragraph [ref=e321]
      - contentinfo [ref=e322]:
        - navigation [ref=e323]:
          - list [ref=e324]:
            - listitem [ref=e325]:
              - button "Home" [ref=e326] [cursor=pointer]:
                - generic [ref=e327]:
                  - img [ref=e328]
                  - generic [ref=e329]: Home
            - listitem [ref=e330]:
              - button "Entries 146" [ref=e331] [cursor=pointer]:
                - generic [ref=e332]:
                  - img [ref=e333]
                  - generic [ref=e334]: Entries
                - generic [ref=e335]: "146"
            - listitem [ref=e336]:
              - button "Feed" [ref=e337] [cursor=pointer]:
                - generic [ref=e338]:
                  - img [ref=e339]
                  - generic [ref=e340]: Feed
            - listitem [ref=e341]:
              - button "Rewards 10" [ref=e342] [cursor=pointer]:
                - generic [ref=e343]:
                  - img [ref=e344]
                  - generic [ref=e345]: Rewards
                - generic [ref=e346]: "10"
            - listitem [ref=e347]:
              - button "Packs" [active] [ref=e348] [cursor=pointer]:
                - generic [ref=e349]:
                  - img [ref=e350]
                  - generic [ref=e351]: Packs
    - generic:
      - region "Notifications Alt+T"
  - alert [ref=e352]: ParlayPlay | Fun Fantasy Sports - Packs
```

# Test source

```ts
  406 |   async pickFivePlayers(): Promise<string[]> {
  407 |     return this.pickPlayers(5);
  408 |   }
  409 | 
  410 |   /**
  411 |    * Reads picks from the slip the app persists via `slipPersistence.saveSlip`
  412 |    * rather than the DOM: when the backend omits a player's main/default
  413 |    * altLine flag the card boots on a fallback line and the highlight isn't
  414 |    * visible even though the pick is persisted.
  415 |    */
  416 |   async getPersistedPickIds(): Promise<string[]> {
  417 |     return this.page.evaluate(() => {
  418 |       const raw = localStorage.getItem('pp_persistent_slip:v1');
  419 |       if (!raw) return [];
  420 |       try {
  421 |         const parsed = JSON.parse(raw);
  422 |         return Object.keys(parsed.selectedPicks ?? {});
  423 |       } catch {
  424 |         return [];
  425 |       }
  426 |     });
  427 |   }
  428 | 
  429 |   async assertPicksPersist(expectedIds: string[], timeout = 10_000): Promise<void> {
  430 |     // Storage holds bare ids ("1089"); pickPlayers returns "player-1089".
  431 |     const normalise = (id: string) => id.replace(/^player-/, '');
  432 |     const expected = new Set(expectedIds.map(normalise));
  433 | 
  434 |     // Auto-save is debounced ~1s and the post-reload restore writes back
  435 |     // asynchronously, so poll.
  436 |     await expect
  437 |       .poll(
  438 |         async () => {
  439 |           const ids = await this.getPersistedPickIds();
  440 |           return Array.from(new Set(ids.map(normalise))).sort();
  441 |         },
  442 |         {
  443 |           timeout,
  444 |           message: `Expected persisted picks ${JSON.stringify(
  445 |             Array.from(expected).sort(),
  446 |           )} in localStorage`,
  447 |         },
  448 |       )
  449 |       .toEqual(Array.from(expected).sort());
  450 |   }
  451 | 
  452 |   async waitForSlipPersisted(expectedPickCount: number, timeout = 5_000): Promise<void> {
  453 |     await expect
  454 |       .poll(
  455 |         async () =>
  456 |           this.page.evaluate(() => {
  457 |             const raw = localStorage.getItem('pp_persistent_slip:v1');
  458 |             if (!raw) return 0;
  459 |             try {
  460 |               return JSON.parse(raw).nrOfPicks ?? 0;
  461 |             } catch {
  462 |               return 0;
  463 |             }
  464 |           }),
  465 |         {
  466 |           timeout,
  467 |           message: `Slip with ${expectedPickCount} picks was never written to localStorage`,
  468 |         },
  469 |       )
  470 |       .toBe(expectedPickCount);
  471 |   }
  472 | 
  473 |   async enterFinalContestPage() {
  474 |     // Desktop already shows the submission form — no Continue hop.
  475 |     if (await this.placePickBtn.isVisible().catch(() => false)) return;
  476 |     await this.continueBtn.click();
  477 |   }
  478 | 
  479 |   async clearSlip(): Promise<void> {
  480 |     await this.page.evaluate(() => localStorage.removeItem('pp_persistent_slip:v1'));
  481 |     await this.page.goto('/');
  482 |     await this.waitForFeedReady();
  483 |   }
  484 | 
  485 |   async selectStatByIndex(idx: number): Promise<void> {
  486 |     const tab = this.statsSelector.locator('li button').nth(idx);
  487 |     await expect(tab).toBeVisible();
  488 |     await tab.click();
  489 |     await this.waitForFeedReady();
  490 |   }
  491 | 
  492 |   async enterEntriesPage() {
  493 |     await this.entriesTab.click();
  494 |   }
  495 | 
  496 |   async enterHomePage(): Promise<void> {
  497 |     await this.homeTab.click();
  498 |     await this.waitForFeedReady();
  499 |     await expect(this.leagueSelector).toBeVisible();
  500 |   }
  501 | 
  502 |   async enterMenu() {
  503 |     // Specs can land here before the header mounts; bounded so a hung locator
  504 |     // fails fast instead of absorbing the 10-min test timeout.
  505 |     await this.toggleMenu.waitFor({ state: 'visible', timeout: 15_000 });
> 506 |     await this.toggleMenu.click({ timeout: 15_000 });
      |                           ^ TimeoutError: locator.click: Timeout 15000ms exceeded.
  507 |   }
  508 | 
  509 |   async assertHomePage() {
  510 |     await expect(this.leagueSelector).toBeVisible();
  511 |   }
  512 | 
  513 |   async enterRewarsdsPage() {
  514 |     await this.rewardsTab.click();
  515 |   }
  516 | 
  517 |   // Every tab label span carries `border-playYellow`; the active one adds
  518 |   // `border-b-2`, so assert on that class.
  519 |   navIndicator(label: string): Locator {
  520 |     return this.bottomNav.getByRole('button', { name: label }).locator('span.border-playYellow');
  521 |   }
  522 | 
  523 |   async enterFeedPage() {
  524 |     await this.feedTab.click();
  525 |   }
  526 | 
  527 |   // When Packs occupies the fifth footer slot (see packsTab), Free2Play moves
  528 |   // into the burger menu — exactly one of the two placements exists.
  529 |   async enterFree2PlayPage() {
  530 |     if (await this.free2PlayTab.isVisible().catch(() => false)) {
  531 |       await this.free2PlayTab.click();
  532 |       return;
  533 |     }
  534 |     await this.enterMenu();
  535 |     await this.visible(this.page.getByRole('link', { name: 'Free2Play', exact: true })).click();
  536 |   }
  537 | 
  538 |   // `onSearch` is debounced, so callers assert on the resulting grid/empty
  539 |   // state rather than a fixed wait.
  540 |   async searchPlayers(term: string): Promise<void> {
  541 |     await expect(this.searchInput).toBeVisible();
  542 |     await this.searchInput.fill(term);
  543 |   }
  544 | 
  545 |   async clearSearch(): Promise<void> {
  546 |     await this.searchClearBtn.click();
  547 |   }
  548 | 
  549 |   async fullGameLeagueCount() {
  550 |     return await this.fgleagueTabs.count();
  551 |   }
  552 | 
  553 |   async statsTabCount() {
  554 |     return await this.statsTabs.count();
  555 |   }
  556 | }
  557 | 
```