# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: data-verification/picks-grid.spec.ts >> Data verification - picks grid >> League selector tabs correspond to leagues present in the API
- Location: tests/data-verification/picks-grid.spec.ts:365:3

# Error details

```
Error: league tab "league-NFL-combo" has no players for "NFL" in the API

expect(received).toEqual(expected) // deep equality

- Expected  - 1
+ Received  + 3

- Array []
+ Array [
+   "league tab \"league-NFL-combo\" has no players for \"NFL\" in the API",
+ ]
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
                - link "Packs" [ref=e16] [cursor=pointer]:
                  - /url: /packs
                  - generic [ref=e18]: Packs
              - listitem [ref=e19]:
                - link "Feed" [ref=e20] [cursor=pointer]:
                  - /url: /challenges/feed
                  - generic [ref=e22]: Feed
              - listitem [ref=e23]:
                - link "Rewards 60" [ref=e24] [cursor=pointer]:
                  - /url: /rewards
                  - generic [ref=e25]:
                    - generic [ref=e26]: Rewards
                    - generic [ref=e27]: "60"
              - listitem [ref=e28]:
                - link "Track Picks 107" [ref=e29] [cursor=pointer]:
                  - /url: /challenges/pending
                  - generic [ref=e30]:
                    - generic [ref=e31]: Track Picks
                    - generic [ref=e32]: "107"
            - button "Claim your $100 Deposit Match" [ref=e33] [cursor=pointer]
            - generic [ref=e34]:
              - generic [ref=e36]:
                - generic [ref=e37]: $825.00
                - generic [ref=e38]:
                  - img "gift-icon" [ref=e39]
                  - text: "60.00"
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
                - button "NFL-Combos" [ref=e88] [cursor=pointer]
                - button "SerieA" [ref=e89] [cursor=pointer]
                - button "EPL" [ref=e90] [cursor=pointer]
                - button "MLS" [ref=e91] [cursor=pointer]
                - button "NFLSZN" [ref=e92] [cursor=pointer]
                - button "UFC" [ref=e93] [cursor=pointer]
                - button "Bundes" [ref=e94] [cursor=pointer]
              - button "right chevron sign Filter" [ref=e96] [cursor=pointer]:
                - img "right chevron sign" [ref=e97]
                - text: Filter
            - generic [ref=e98]:
              - generic [ref=e101]:
                - generic [ref=e104]:
                  - generic [ref=e105]:
                    - img "Mookie Betts" [ref=e107]
                    - generic [ref=e108]:
                      - generic [ref=e109]: Mookie Betts
                      - generic [ref=e110]: SS - LAD
                      - generic [ref=e113]: LAD @ MIA 7:10 PM
                    - button "Open expert opinion for Mookie Betts" [ref=e114]:
                      - img [ref=e115]
                  - generic [ref=e119]:
                    - generic [ref=e120]:
                      - generic [ref=e121]:
                        - generic [ref=e123] [cursor=pointer]:
                          - text: Less
                          - img [ref=e124]
                        - generic [ref=e126]: Hits
                        - generic [ref=e128] [cursor=pointer]:
                          - text: More
                          - img [ref=e129]
                      - generic [ref=e132]:
                        - button "Select over 0.5 Hits for 2.74 times" [ref=e133]: 2.74x
                        - generic [ref=e134]: 0.5 Hits
                        - button "Select over 0.5 Hits for 1.28 times" [ref=e135]: 1.28x
                    - generic [ref=e136]:
                      - generic [ref=e137]:
                        - generic [ref=e139] [cursor=pointer]:
                          - text: Less
                          - img [ref=e140]
                        - generic [ref=e142]: Hits + Runs + RBIs
                        - generic [ref=e144] [cursor=pointer]:
                          - text: More
                          - img [ref=e145]
                      - generic [ref=e148]:
                        - button "Select over 1.5 Hits + Runs + RBIs for 1.89 times" [ref=e149]: 1.89x
                        - generic [ref=e150]: 1.5 H+R+R
                        - button "Select over 1.5 Hits + Runs + RBIs for 1.71 times" [ref=e151]: 1.71x
                    - generic [ref=e152]:
                      - generic [ref=e153]:
                        - generic [ref=e155] [cursor=pointer]:
                          - text: Less
                          - img [ref=e156]
                        - generic [ref=e158]: Singles
                        - generic [ref=e160] [cursor=pointer]:
                          - text: More
                          - img [ref=e161]
                      - generic [ref=e164]:
                        - button "Select over 1.5 Singles for 0 times" [disabled] [ref=e165]
                        - generic [ref=e166]: 1.5 Singles
                        - button "Select over 1.5 Singles for 4.28 times" [ref=e167]: 4.28x
                    - generic [ref=e168]:
                      - generic [ref=e169]:
                        - generic [ref=e171] [cursor=pointer]:
                          - text: Less
                          - img [ref=e172]
                        - generic [ref=e174]: Runs
                        - generic [ref=e176] [cursor=pointer]:
                          - text: More
                          - img [ref=e177]
                      - generic [ref=e179]:
                        - generic [ref=e180]:
                          - button "Select over 0.5 Runs for 0 times" [disabled] [ref=e181]
                          - generic [ref=e182]: 0.5 Runs
                          - button "Select over 0.5 Runs for 2.05 times" [ref=e183]: 2.05x
                        - generic [ref=e184]:
                          - button "Select over 1.5 Runs for 0 times" [disabled] [ref=e185]
                          - generic [ref=e186]: 1.5 Runs
                          - button "Select over 1.5 Runs for 6.2 times" [ref=e187]: 6.2x
                    - generic [ref=e188]:
                      - generic [ref=e189]:
                        - generic [ref=e191] [cursor=pointer]:
                          - text: Less
                          - img [ref=e192]
                        - generic [ref=e194]: RBIs
                        - generic [ref=e196] [cursor=pointer]:
                          - text: More
                          - img [ref=e197]
                      - generic [ref=e199]:
                        - generic [ref=e200]:
                          - button "Select over 0.5 RBIs for 1.28 times" [ref=e201]: 1.28x
                          - generic [ref=e202]: 0.5 RBIs
                          - button "Select over 0.5 RBIs for 2.65 times" [ref=e203]: 2.65x
                        - generic [ref=e204]:
                          - button "Select over 1.5 RBIs for 0 times" [disabled] [ref=e205]
                          - generic [ref=e206]: 1.5 RBIs
                          - button "Select over 1.5 RBIs for 5.2 times" [ref=e207]: 5.2x
                  - button "Show More Stats" [ref=e209]:
                    - img [ref=e210]
                - generic [ref=e214]:
                  - generic [ref=e215]:
                    - img "Teoscar Hernandez" [ref=e217]
                    - generic [ref=e218]:
                      - generic [ref=e219]: T. Hernandez
                      - generic [ref=e220]: RF - LAD
                      - generic [ref=e223]: LAD @ MIA 7:10 PM
                    - button "Open expert opinion for Teoscar Hernandez" [ref=e224]:
                      - img [ref=e225]
                  - generic [ref=e229]:
                    - generic [ref=e230]:
                      - generic [ref=e231]:
                        - generic [ref=e233] [cursor=pointer]:
                          - text: Less
                          - img [ref=e234]
                        - generic [ref=e236]: Hits
                        - generic [ref=e238] [cursor=pointer]:
                          - text: More
                          - img [ref=e239]
                      - generic [ref=e241]:
                        - generic [ref=e242]:
                          - button "Select over 0.5 Hits for 0 times" [disabled] [ref=e243]
                          - generic [ref=e244]: 0.5 Hits
                          - button "Select over 0.5 Hits for 1.43 times" [ref=e245]: 1.43x
                        - generic [ref=e246]:
                          - button "Select over 1.5 Hits for 0 times" [disabled] [ref=e247]
                          - generic [ref=e248]: 1.5 Hits
                          - button "Select over 1.5 Hits for 3.31 times" [ref=e249]: 3.31x
                        - generic [ref=e250]:
                          - button "Select over 2.5 Hits for 0 times" [disabled] [ref=e251]
                          - generic [ref=e252]: 2.5 Hits
                          - button "Select over 2.5 Hits for 8.92 times" [ref=e253]: 8.92x
                    - generic [ref=e254]:
                      - generic [ref=e255]:
                        - generic [ref=e257] [cursor=pointer]:
                          - text: Less
                          - img [ref=e258]
                        - generic [ref=e260]: Hits + Runs + RBIs
                        - generic [ref=e262] [cursor=pointer]:
                          - text: More
                          - img [ref=e263]
                      - generic [ref=e265]:
                        - generic [ref=e266]:
                          - button "Select over 0.5 Hits + Runs + RBIs for 0 times" [disabled] [ref=e267]
                          - generic [ref=e268]: 0.5 H+R+R
                          - button "Select over 0.5 Hits + Runs + RBIs for 1.27 times" [ref=e269]: 1.27x
                        - generic [ref=e270]:
                          - button "Select over 2.5 Hits + Runs + RBIs for 0 times" [disabled] [ref=e271]
                          - generic [ref=e272]: 2.5 H+R+R
                          - button "Select over 2.5 Hits + Runs + RBIs for 2.68 times" [ref=e273]: 2.68x
                        - generic [ref=e274]:
                          - button "Select over 3.5 Hits + Runs + RBIs for 0 times" [disabled] [ref=e275]
                          - generic [ref=e276]: 3.5 H+R+R
                          - button "Select over 3.5 Hits + Runs + RBIs for 3.87 times" [ref=e277]: 3.87x
                        - generic [ref=e278]:
                          - button "Select over 4.5 Hits + Runs + RBIs for 0 times" [disabled] [ref=e279]
                          - generic [ref=e280]: 4.5 H+R+R
                          - button "Select over 4.5 Hits + Runs + RBIs for 5.71 times" [ref=e281]: 5.71x
                    - generic [ref=e282]:
                      - generic [ref=e283]:
                        - generic [ref=e285] [cursor=pointer]:
                          - text: Less
                          - img [ref=e286]
                        - generic [ref=e288]: Runs
                        - generic [ref=e290] [cursor=pointer]:
                          - text: More
                          - img [ref=e291]
                      - generic [ref=e293]:
                        - generic [ref=e294]:
                          - button "Select over 0.5 Runs for 0 times" [disabled] [ref=e295]
                          - generic [ref=e296]: 0.5 Runs
                          - button "Select over 0.5 Runs for 2.22 times" [ref=e297]: 2.22x
                        - generic [ref=e298]:
                          - button "Select over 1.5 Runs for 0 times" [disabled] [ref=e299]
                          - generic [ref=e300]: 1.5 Runs
                          - button "Select over 1.5 Runs for 6.66 times" [ref=e301]: 6.66x
                    - generic [ref=e302]:
                      - generic [ref=e303]:
                        - generic [ref=e305] [cursor=pointer]:
                          - text: Less
                          - img [ref=e306]
                        - generic [ref=e308]: RBIs
                        - generic [ref=e310] [cursor=pointer]:
                          - text: More
                          - img [ref=e311]
                      - generic [ref=e313]:
                        - generic [ref=e314]:
                          - button "Select over 0.5 RBIs for 0 times" [disabled] [ref=e315]
                          - generic [ref=e316]: 0.5 RBIs
                          - button "Select over 0.5 RBIs for 2.72 times" [ref=e317]: 2.72x
                        - generic [ref=e318]:
                          - button "Select over 1.5 RBIs for 0 times" [disabled] [ref=e319]
                          - generic [ref=e320]: 1.5 RBIs
                          - button "Select over 1.5 RBIs for 5.02 times" [ref=e321]: 5.02x
                    - generic [ref=e322]:
                      - generic [ref=e323]:
                        - generic [ref=e325] [cursor=pointer]:
                          - text: Less
                          - img [ref=e326]
                        - generic [ref=e328]: Homeruns
                        - generic [ref=e330] [cursor=pointer]:
                          - text: More
                          - img [ref=e331]
                      - generic [ref=e333]:
                        - generic [ref=e334]:
                          - button "Select over 0.5 Homeruns for 0 times" [disabled] [ref=e335]
                          - generic [ref=e336]: 0.5 Homeruns
                          - button "Select over 0.5 Homeruns for 5.34 times" [ref=e337]: 5.34x
                        - generic [ref=e338]:
                          - button "Select over 1.5 Homeruns for 0 times" [disabled] [ref=e339]
                          - generic [ref=e340]: 1.5 Homeruns
                          - button "Select over 1.5 Homeruns for 44.8 times" [ref=e341]: 44.8x
                    - generic [ref=e342]:
                      - generic [ref=e343]:
                        - generic [ref=e345] [cursor=pointer]:
                          - text: Less
                          - img [ref=e346]
                        - generic [ref=e348]: Total Bases
                        - generic [ref=e350] [cursor=pointer]:
                          - text: More
                          - img [ref=e351]
                      - generic [ref=e353]:
                        - generic [ref=e354]:
                          - button "Select over 1.5 Total Bases for 0 times" [disabled] [ref=e355]
                          - generic [ref=e356]: 1.5 Total Bases
                          - button "Select over 1.5 Total Bases for 2.26 times" [ref=e357]: 2.26x
                        - generic [ref=e358]:
                          - button "Select over 2.5 Total Bases for 0 times" [disabled] [ref=e359]
                          - generic [ref=e360]: 2.5 Total Bases
                          - button "Select over 2.5 Total Bases for 3.37 times" [ref=e361]: 3.37x
                        - generic [ref=e362]:
                          - button "Select over 3.5 Total Bases for 0 times" [disabled] [ref=e363]
                          - generic [ref=e364]: 3.5 Total Bases
                          - button "Select over 3.5 Total Bases for 4.19 times" [ref=e365]: 4.19x
                        - generic [ref=e366]:
                          - button "Select over 4.5 Total Bases for 0 times" [disabled] [ref=e367]
                          - generic [ref=e368]: 4.5 Total Bases
                          - button "Select over 4.5 Total Bases for 6.91 times" [ref=e369]: 6.91x
                  - button "Show More Stats" [ref=e371]:
                    - img [ref=e372]
              - generic [ref=e509]:
                - generic [ref=e512]: Please select your 1st pick
                - generic [ref=e515]:
                  - img "arrow" [ref=e516]
                  - heading "Let's Start!" [level=2] [ref=e517]
                  - generic [ref=e518]:
                    - text: Pick at least two players
                    - text: from different teams to play
          - generic [ref=e521]:
            - generic [ref=e522]:
              - link "Parlay Play Logo" [ref=e523] [cursor=pointer]:
                - /url: /
                - img "Parlay Play Logo" [ref=e525]
              - generic [ref=e526]:
                - generic [ref=e527]: Improve your experience. Download our app.
                - generic [ref=e528]:
                  - link "Apple Store" [ref=e529] [cursor=pointer]:
                    - /url: https://parlayplay.onelink.me/oLJk/gnqpwjha
                    - img "Apple Store" [ref=e530]
                  - link "Google Play Store" [ref=e531] [cursor=pointer]:
                    - /url: https://parlayplay.onelink.me/oLJk/fh7u6juo
                    - img "Google Play Store" [ref=e532]
            - generic [ref=e533]:
              - link "Privacy" [ref=e534] [cursor=pointer]:
                - /url: /privacy-policy
              - link "Fantasy Terms" [ref=e535] [cursor=pointer]:
                - /url: /terms
              - link "Packs Terms" [ref=e536] [cursor=pointer]:
                - /url: /terms/packs
              - link "Responsible Gaming" [ref=e537] [cursor=pointer]:
                - /url: /responsible-gaming
              - link "Gaming Rules" [ref=e538] [cursor=pointer]:
                - /url: /rules
              - link "FAQ" [ref=e539] [cursor=pointer]:
                - /url: https://intercom.help/parlayplay/en/
              - link "Contact Us" [ref=e540] [cursor=pointer]:
                - /url: /
              - paragraph [ref=e541]: © ParlayPlay 2026 - All Rights Reserved
            - list [ref=e542]:
              - listitem [ref=e543]:
                - generic [ref=e544]:
                  - log [ref=e546]
                  - generic [ref=e547]:
                    - generic [ref=e548]:
                      - generic [ref=e549]: 🇺🇸English
                      - combobox "Select language" [ref=e550]
                    - img [ref=e554]
              - listitem [ref=e556]:
                - img "18+-icon" [ref=e557]
              - listitem [ref=e558]:
                - link "ParlayPlay on Twitter" [ref=e559] [cursor=pointer]:
                  - /url: https://twitter.com/parlay_play?lang=en
                  - img [ref=e560]
              - listitem [ref=e562]:
                - link "ParlayPlay on Facebook" [ref=e563] [cursor=pointer]:
                  - /url: https://www.facebook.com/ParlayPlay.io/
                  - img [ref=e564]
              - listitem [ref=e566]:
                - link "ParlayPlay on Instagram" [ref=e567] [cursor=pointer]:
                  - /url: https://www.instagram.com/parlayplay_?igsh=bHBldWQyMmV2b3Y4
                  - img [ref=e568]
              - listitem [ref=e570]:
                - link "ParlayPlay on Discord" [ref=e571] [cursor=pointer]:
                  - /url: https://discord.com/invite/parlayplay
                  - img [ref=e572]
    - generic:
      - region "Notifications Alt+T"
  - alert [ref=e574]
```

# Test source

```ts
  308 |             const stat = apiPlayer?.stats.find((s) => s.challengeName === statName);
  309 |             const ml = stat ? mainLine(stat) : null;
  310 |             if (!apiPlayer || !stat) {
  311 |               persistent.push(
  312 |                 `card player-${card.playerId}: not offered for "${statName}" (fresh fetch)`,
  313 |               );
  314 |             } else if (
  315 |               ml &&
  316 |               card.statValue !== null &&
  317 |               Number(card.statValue) !== ml.selectionPoints
  318 |             ) {
  319 |               persistent.push(
  320 |                 `card player-${card.playerId}: shows ${card.statValue}, fresh API main line is ${ml.selectionPoints}`,
  321 |               );
  322 |             }
  323 |           }
  324 |           expect(persistent, persistent.join('\n')).toEqual([]);
  325 |         }
  326 |       });
  327 |     }
  328 |   });
  329 | 
  330 |   test('Stats selector tabs equal the API stat names for the default league', async ({
  331 |     loggedInPage: page,
  332 |   }) => {
  333 |     test.skip(isDesktopProject(), 'desktop feed has no stat-tab selector to compare');
  334 |     const home = new HomePage(page);
  335 | 
  336 |     const offeringPromise = waitForOffering(page);
  337 |     await page.goto('/');
  338 |     const offering = await offeringPromise;
  339 |     await home.waitForFeedReady();
  340 | 
  341 |     // The default-selected league is the first tab (highest popularity).
  342 |     const firstLeagueId = (await home.leagueButtons.first().getAttribute('id')) ?? '';
  343 |     const leagueShort = firstLeagueId.replace(/^league-/, '');
  344 |     expect(leagueShort, 'could not derive default league from DOM').not.toEqual('');
  345 |     // Promo swaps the stats selector for a league list, combo renders packaged
  346 |     // lines, and Live / desktop "All" aggregate across leagues — none map onto
  347 |     // per-stat challengeNames for a single league.
  348 |     test.skip(
  349 |       /promo|combo/i.test(leagueShort) || isAggregatorLeague(leagueShort),
  350 |       `default league tab is ${leagueShort}; stats selector not comparable`,
  351 |     );
  352 | 
  353 |     const domStats = (await home.statsTabs.allInnerTexts())
  354 |       .map((t) => t.replace(/\s+/g, ' ').trim())
  355 |       .filter(Boolean)
  356 |       .sort();
  357 |     const apiStats = statNamesForLeague(offering, leagueShort);
  358 | 
  359 |     expect(apiStats.length, `API offers no FG stats for ${leagueShort}`).toBeGreaterThan(0);
  360 |     expect(domStats, `stats selector for ${leagueShort} diverges from API challengeNames`).toEqual(
  361 |       apiStats,
  362 |     );
  363 |   });
  364 | 
  365 |   test('League selector tabs correspond to leagues present in the API', async ({
  366 |     loggedInPage: page,
  367 |   }) => {
  368 |     const home = new HomePage(page);
  369 | 
  370 |     const offeringPromise = waitForOffering(page);
  371 |     await page.goto('/');
  372 |     const offering = await offeringPromise;
  373 |     await home.waitForFeedReady();
  374 | 
  375 |     const apiLeagues = new Set(
  376 |       offering.players
  377 |         .map((p) => p.match.league?.leagueNameShort)
  378 |         .filter((l): l is string => Boolean(l)),
  379 |     );
  380 | 
  381 |     const buttons = await home.listLeagueButtons();
  382 |     expect(buttons.length, 'league selector rendered no tabs').toBeGreaterThan(0);
  383 | 
  384 |     const errors: string[] = [];
  385 |     const seenBaseLeagues = new Set<string>();
  386 |     for (const button of buttons) {
  387 |       const id = (await button.getAttribute('id')) ?? '';
  388 |       const lower = id.toLowerCase();
  389 |       if (lower.includes('promo')) continue; // promo pseudo-league
  390 |       // Tab ids: league-MLB, league-WNBA-H1, league-WNBA-combo. Try the full
  391 |       // remainder first (hyphenated league names), then the first token
  392 |       // (period/combo variants like WNBA-H1).
  393 |       const remainder = id.replace(/^league-/, '');
  394 |       // Live / desktop "All" aggregate across leagues — the API has no league
  395 |       // named "Live"/"All", so comparing them would report a phantom mismatch.
  396 |       if (isAggregatorLeague(remainder)) continue;
  397 |       const base = apiLeagues.has(remainder) ? remainder : remainder.split('-')[0];
  398 |       seenBaseLeagues.add(base);
  399 |       if (!apiLeagues.has(base)) {
  400 |         errors.push(`league tab "${id}" has no players for "${base}" in the API`);
  401 |       }
  402 |     }
  403 |     for (const league of apiLeagues) {
  404 |       if (!seenBaseLeagues.has(league)) {
  405 |         errors.push(`API offers league "${league}" but no league tab renders it`);
  406 |       }
  407 |     }
> 408 |     expect(errors, errors.join('\n')).toEqual([]);
      |                                       ^ Error: league tab "league-NFL-combo" has no players for "NFL" in the API
  409 |   });
  410 | 
  411 |   test('Match selector lists every API match for the default league', async ({
  412 |     loggedInPage: page,
  413 |   }) => {
  414 |     const home = new HomePage(page);
  415 | 
  416 |     const offeringPromise = waitForOffering(page);
  417 |     await page.goto('/');
  418 |     const offering = await offeringPromise;
  419 |     await home.waitForFeedReady();
  420 | 
  421 |     const firstLeagueId = (await home.leagueButtons.first().getAttribute('id')) ?? '';
  422 |     const leagueShort = firstLeagueId.replace(/^league-/, '');
  423 |     // Live / desktop "All" aggregate across leagues — there is no single
  424 |     // league's match list to compare against.
  425 |     test.skip(
  426 |       isAggregatorLeague(leagueShort),
  427 |       `default league tab is the ${leagueShort} aggregator — match selector not comparable per league`,
  428 |     );
  429 | 
  430 |     // Distinct non-live matchups the API offers for this league.
  431 |     const apiMatchups = new Map<string, string>(); // matchup -> matchDate
  432 |     for (const p of playersForLeague(offering, leagueShort)) {
  433 |       if (p.match.matchStatus === MATCH_STATUS_LIVE) continue;
  434 |       const label = matchupLabel(p);
  435 |       if (label) apiMatchups.set(label, p.match.matchDate);
  436 |     }
  437 |     test.skip(apiMatchups.size === 0, `no upcoming ${leagueShort} matches in the API`);
  438 | 
  439 |     const matchSelector = page.getByTestId('match-selector').filter({ visible: true }).first();
  440 |     await expect(matchSelector).toBeVisible();
  441 |     const buttonTexts = (await matchSelector.locator('button').allInnerTexts()).map((t) =>
  442 |       t.replace(/\s+/g, ' ').trim(),
  443 |     );
  444 | 
  445 |     const errors: string[] = [];
  446 |     for (const [label] of apiMatchups) {
  447 |       const button = buttonTexts.find((t) => t.startsWith(label));
  448 |       if (!button) {
  449 |         errors.push(
  450 |           `API match "${label}" missing from match selector [${buttonTexts.join(' | ')}]`,
  451 |         );
  452 |         continue;
  453 |       }
  454 |       // Time suffix: "h:mmAM" for today, "ddd hAM" otherwise (browser tz).
  455 |       const timeText = button.slice(label.length).trim();
  456 |       if (!/^(\d{1,2}:\d{2}(AM|PM)|(Sun|Mon|Tue|Wed|Thu|Fri|Sat) \d{1,2}(AM|PM))$/.test(timeText)) {
  457 |         errors.push(`match "${label}": start time rendered as "${timeText}"`);
  458 |       }
  459 |     }
  460 |     expect(errors, errors.join('\n')).toEqual([]);
  461 |   });
  462 | });
  463 | 
```