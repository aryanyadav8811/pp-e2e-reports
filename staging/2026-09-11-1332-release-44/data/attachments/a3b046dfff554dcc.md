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
          - link "Parlay Play Logo" [ref=e6]:
            - /url: /
            - img "Parlay Play Logo" [ref=e8]
          - generic [ref=e10]:
            - generic [ref=e12]:
              - generic [ref=e13]: $894.00
              - generic [ref=e14]:
                - img "gift-icon" [ref=e15]
                - text: "67.00"
            - button "Toggle Menu" [ref=e16]:
              - img [ref=e17]
      - main [ref=e19]:
        - generic [ref=e24]:
          - generic [ref=e25]:
            - generic [ref=e26]:
              - list [ref=e28]:
                - button "MLB" [ref=e29] [cursor=pointer]
                - button "NFL-Combos" [ref=e30] [cursor=pointer]
                - button "SerieA" [ref=e31] [cursor=pointer]
                - button "EPL" [ref=e32] [cursor=pointer]
                - button "MLS" [ref=e33] [cursor=pointer]
                - button "NFLSZN" [ref=e34] [cursor=pointer]
                - button "UFC" [ref=e35] [cursor=pointer]
                - button "Bundes" [ref=e36] [cursor=pointer]
              - list [ref=e38]:
                - listitem [ref=e39]:
                  - button "ALL" [ref=e40] [cursor=pointer]:
                    - generic [ref=e41]: ALL
                - listitem [ref=e42]:
                  - button "NYM@NYY 7:05PM" [ref=e43] [cursor=pointer]:
                    - text: NYM@NYY
                    - generic [ref=e44]: 7:05PM
                - listitem [ref=e45]:
                  - button "LAD@MIA 7:10PM" [ref=e46] [cursor=pointer]:
                    - text: LAD@MIA
                    - generic [ref=e47]: 7:10PM
                - listitem [ref=e48]:
                  - button "CIN@MIL 7:45PM" [ref=e49] [cursor=pointer]:
                    - text: CIN@MIL
                    - generic [ref=e50]: 7:45PM
                - listitem [ref=e51]:
                  - button "CLE@MIN 8:10PM" [ref=e52] [cursor=pointer]:
                    - text: CLE@MIN
                    - generic [ref=e53]: 8:10PM
                - listitem [ref=e54]:
                  - button "TEX@ARI 9:40PM" [ref=e55] [cursor=pointer]:
                    - text: TEX@ARI
                    - generic [ref=e56]: 9:40PM
                - listitem [ref=e57]:
                  - button "SD@SF 10:15PM" [ref=e58] [cursor=pointer]:
                    - text: SD@SF
                    - generic [ref=e59]: 10:15PM
              - generic [ref=e60]:
                - generic [ref=e61]:
                  - generic [ref=e64]:
                    - generic:
                      - img
                    - textbox "Search player or team" [ref=e65]
                  - button "Change card style from grid" [ref=e67]
                - list [ref=e69]:
                  - listitem [ref=e70]:
                    - button "Strikeouts (K)" [ref=e71]
                  - listitem [ref=e72]:
                    - button "Hits" [ref=e73]
                  - listitem [ref=e74]:
                    - button "Hits + Runs + RBIs" [ref=e75]
                  - listitem [ref=e76]:
                    - button "Singles" [ref=e77]
                  - listitem [ref=e78]:
                    - button "Doubles" [ref=e79]
                  - listitem [ref=e80]:
                    - button "Triples" [ref=e81]
                  - listitem [ref=e82]:
                    - button "Runs" [ref=e83]
                  - listitem [ref=e84]:
                    - button "RBIs" [ref=e85]
                  - listitem [ref=e86]:
                    - button "Homeruns" [ref=e87]
                  - listitem [ref=e88]:
                    - button "Total Bases" [ref=e89]
            - generic [ref=e90]:
              - generic [ref=e95]:
                - generic [ref=e98] [cursor=pointer]:
                  - generic [ref=e99]:
                    - generic [ref=e100]:
                      - generic [ref=e101]: 100%
                      - generic [ref=e102]: Deposit Match
                    - generic [ref=e103]: New User Promotion
                  - button "Deposit" [ref=e105]
                - generic [ref=e109] [cursor=pointer]:
                  - generic [ref=e110]: Pull real graded cards worth up to $10,000
                  - generic [ref=e111]: Sell or ship instantly
                  - button "Rip a pack" [ref=e112]:
                    - generic [ref=e113]:
                      - img [ref=e114]
                      - text: Rip a pack
                - generic [ref=e119] [cursor=pointer]:
                  - generic [ref=e120]:
                    - generic [ref=e121]: Refer a friend, get a $20 Free Entry
                    - generic [ref=e122]: Referral bonus
                  - button "Refer" [ref=e123]
                - generic [ref=e126] [cursor=pointer]:
                  - generic [ref=e127]:
                    - generic [ref=e128]:
                      - img [ref=e129]
                      - generic [ref=e133]: Boosted Picks
                    - generic [ref=e134]: "Every Pick Pays: Up to a 35% Boost!"
                  - button "Details" [ref=e136]
              - generic [ref=e143]:
                - generic [ref=e146]:
                  - button "Open expert opinion for Nolan McLean" [ref=e147]:
                    - img [ref=e148]
                  - img "Nolan McLean" [ref=e151]
                - generic [ref=e152]:
                  - generic [ref=e153]: Nolan McLean
                  - button "6.5 SO (K)" [ref=e154]:
                    - generic [ref=e155]:
                      - img [ref=e156]
                      - img [ref=e158]
                    - generic [ref=e160]: "6.5"
                    - generic [ref=e161]: SO (K)
                  - generic [ref=e162]:
                    - generic [ref=e163]: NYM@NYY
                    - generic [ref=e164]: 7:05PM
                  - generic [ref=e165]:
                    - button "Select over 6.5 Strikeouts (K) for 1.71 times" [ref=e166]:
                      - img [ref=e167]
                      - generic [ref=e169]: 1.71x
                    - button "Select over 6.5 Strikeouts (K) for 1.93 times" [ref=e170]:
                      - generic [ref=e171]: 1.93x
                      - img [ref=e172]
          - generic [ref=e175]:
            - generic [ref=e177]:
              - link "Download ParlayPlay On The App Store" [ref=e178]:
                - /url: https://parlayplay.onelink.me/oLJk/gnqpwjha
                - img "Download ParlayPlay On The App Store" [ref=e179]
              - paragraph [ref=e180]:
                - text: Get the app.
                - text: Better. Faster. Convenient
            - navigation [ref=e181]:
              - link "Privacy" [ref=e182]:
                - /url: /privacy-policy
              - link "Fantasy Terms" [ref=e183]:
                - /url: /terms
              - link "Packs Terms" [ref=e184]:
                - /url: /terms/packs
              - link "Responsible Gaming" [ref=e185]:
                - /url: /responsible-gaming
              - link "Gaming Rules" [ref=e186]:
                - /url: /rules
              - link "FAQ" [ref=e187]:
                - /url: https://intercom.help/parlayplay/en/
            - navigation [ref=e188]:
              - generic [ref=e189]:
                - paragraph [ref=e190]: © ParlayPlay 2026
                - generic [ref=e191]:
                  - link "ParlayPlay on Facebook" [ref=e192]:
                    - /url: https://www.facebook.com/parlayplay.io
                    - img [ref=e193]
                  - link "ParlayPlay on Instagram" [ref=e195]:
                    - /url: https://www.instagram.com/parlayplay_?igsh=bHBldWQyMmV2b3Y4
                    - img [ref=e196]
                  - link "ParlayPlay on Twitter" [ref=e198]:
                    - /url: https://www.twitter.com/parlay_play
                    - img [ref=e199]
                  - link "ParlayPlay on Discord" [ref=e201]:
                    - /url: https://discord.com/invite/parlayplay
                    - img [ref=e202]
                - img "18+ icon" [ref=e204]
            - paragraph [ref=e206]
      - contentinfo [ref=e207]:
        - navigation [ref=e208]:
          - list [ref=e209]:
            - listitem [ref=e210]:
              - button "Home" [ref=e211] [cursor=pointer]:
                - generic [ref=e212]:
                  - img [ref=e213]
                  - generic [ref=e214]: Home
            - listitem [ref=e215]:
              - button "Entries 85" [ref=e216] [cursor=pointer]:
                - generic [ref=e217]:
                  - img [ref=e218]
                  - generic [ref=e219]: Entries
                - generic [ref=e220]: "85"
            - listitem [ref=e221]:
              - button "Feed" [ref=e222] [cursor=pointer]:
                - generic [ref=e223]:
                  - img [ref=e224]
                  - generic [ref=e225]: Feed
            - listitem [ref=e226]:
              - button "Rewards 68" [ref=e227] [cursor=pointer]:
                - generic [ref=e228]:
                  - img [ref=e229]
                  - generic [ref=e230]: Rewards
                - generic [ref=e231]: "68"
            - listitem [ref=e232]:
              - button "Packs" [ref=e233] [cursor=pointer]:
                - generic [ref=e234]:
                  - img [ref=e235]
                  - generic [ref=e236]: Packs
    - generic:
      - region "Notifications Alt+T"
  - alert [ref=e237]
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