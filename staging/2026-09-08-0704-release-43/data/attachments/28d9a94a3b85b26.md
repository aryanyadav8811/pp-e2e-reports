# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: menu/account-dropdown-desktop.spec.ts >> Menu - Desktop Account Dropdown >> Menu items link to the same destinations as the mobile Account Center
- Location: tests/menu/account-dropdown-desktop.spec.ts:47:3

# Error details

```
Error: expect(locator).toBeVisible() failed

Locator: getByRole('dialog').filter({ has: getByRole('link', { name: 'Transaction History' }) }).first()
Expected: visible
Timeout: 15000ms
Error: element(s) not found

Call log:
  - Expect "toBeVisible" with timeout 15000ms
  - waiting for getByRole('dialog').filter({ has: getByRole('link', { name: 'Transaction History' }) }).first()

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
                - link "Rewards 44" [ref=e24] [cursor=pointer]:
                  - /url: /rewards
                  - generic [ref=e25]:
                    - generic [ref=e26]: Rewards
                    - generic [ref=e27]: "44"
              - listitem [ref=e28]:
                - link "Track Picks 82" [ref=e29] [cursor=pointer]:
                  - /url: /challenges/pending
                  - generic [ref=e30]:
                    - generic [ref=e31]: Track Picks
                    - generic [ref=e32]: "82"
            - button "Claim your $100 Deposit Match" [ref=e33] [cursor=pointer]
            - generic [ref=e34]:
              - generic [ref=e36]:
                - generic [ref=e37]: $570.24
                - generic [ref=e38]:
                  - img "gift-icon" [ref=e39]
                  - text: "43.00"
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
                - button "SerieA" [ref=e88] [cursor=pointer]
                - button "EPL" [ref=e89] [cursor=pointer]
                - button "UCL" [ref=e90] [cursor=pointer]
                - button "MLS" [ref=e91] [cursor=pointer]
                - button "NFLSZN" [ref=e92] [cursor=pointer]
                - button "LaLiga" [ref=e93] [cursor=pointer]
                - button "UFC" [ref=e94] [cursor=pointer]
              - button "right chevron sign Filter" [ref=e96] [cursor=pointer]:
                - img "right chevron sign" [ref=e97]
                - text: Filter
            - generic [ref=e98]:
              - generic [ref=e101]:
                - generic [ref=e104]:
                  - generic [ref=e105]:
                    - img "Tanner Bibee" [ref=e107]
                    - generic [ref=e108]:
                      - generic [ref=e109]: Tanner Bibee
                      - generic [ref=e110]: SP - CLE
                      - generic [ref=e113]: CLE @ BAL 6:35 PM
                    - button "Open expert opinion for Tanner Bibee" [ref=e114]:
                      - img [ref=e115]
                  - generic [ref=e119]:
                    - generic [ref=e120]:
                      - generic [ref=e121]:
                        - generic [ref=e123] [cursor=pointer]:
                          - text: Less
                          - img [ref=e124]
                        - generic [ref=e126]: Strikeouts (K)
                        - generic [ref=e128] [cursor=pointer]:
                          - text: More
                          - img [ref=e129]
                      - generic [ref=e131]:
                        - generic [ref=e132]:
                          - button "Select over 3.5 Strikeouts (K) for 0 times" [disabled] [ref=e133]
                          - generic [ref=e134]: 3.5 Strikeouts (K)
                          - button "Select over 3.5 Strikeouts (K) for 1.12 times" [ref=e135]: 1.12x
                        - generic [ref=e136]:
                          - button "Select over 4.5 Strikeouts (K) for 2.14 times" [ref=e137]: 2.14x
                          - generic [ref=e138]: 4.5 Strikeouts (K)
                          - button "Select over 4.5 Strikeouts (K) for 1.5 times" [ref=e139]: 1.5x
                        - generic [ref=e140]:
                          - button "Select over 5.5 Strikeouts (K) for 1.64 times" [ref=e141]: 1.64x
                          - generic [ref=e142]: 5.5 Strikeouts (K)
                          - button "Select over 5.5 Strikeouts (K) for 2.1 times" [ref=e143]: 2.1x
                        - generic [ref=e144]:
                          - button "Select over 6.5 Strikeouts (K) for 0 times" [disabled] [ref=e145]
                          - generic [ref=e146]: 6.5 Strikeouts (K)
                          - button "Select over 6.5 Strikeouts (K) for 3.16 times" [ref=e147]: 3.16x
                        - generic [ref=e148]:
                          - button "Select over 7.5 Strikeouts (K) for 0 times" [disabled] [ref=e149]
                          - generic [ref=e150]: 7.5 Strikeouts (K)
                          - button "Select over 7.5 Strikeouts (K) for 5.04 times" [ref=e151]: 5.04x
                        - button "Show more Strikeouts (K) lines (6)" [ref=e152]:
                          - img [ref=e153]
                          - text: Show more Strikeouts (K) lines (6)
                    - generic [ref=e155]:
                      - generic [ref=e156]:
                        - generic [ref=e158] [cursor=pointer]:
                          - text: Less
                          - img [ref=e159]
                        - generic [ref=e161]: Pitching Outs
                        - generic [ref=e163] [cursor=pointer]:
                          - text: More
                          - img [ref=e164]
                      - generic [ref=e167]:
                        - button "Select over 17.5 Pitching Outs for 1.86 times" [ref=e168]: 1.86x
                        - generic [ref=e169]: 17.5 Pitching Outs
                        - button "Select over 17.5 Pitching Outs for 1.74 times" [ref=e170]: 1.74x
                  - button "Show More Stats" [ref=e172]:
                    - img [ref=e173]
                - generic [ref=e177]:
                  - generic [ref=e178]:
                    - img "Brayan Rocchio" [ref=e180]
                    - generic [ref=e181]:
                      - generic [ref=e182]: B. Rocchio
                      - generic [ref=e183]: SS - CLE
                      - generic [ref=e186]: CLE @ BAL 6:35 PM
                    - button "Open expert opinion for Brayan Rocchio" [ref=e187]:
                      - img [ref=e188]
                  - generic [ref=e192]:
                    - generic [ref=e193]:
                      - generic [ref=e194]:
                        - generic [ref=e196] [cursor=pointer]:
                          - text: Less
                          - img [ref=e197]
                        - generic [ref=e199]: Hits
                        - generic [ref=e201] [cursor=pointer]:
                          - text: More
                          - img [ref=e202]
                      - generic [ref=e204]:
                        - generic [ref=e205]:
                          - button "Select over 0.5 Hits for 2.2 times" [ref=e206]: 2.2x
                          - generic [ref=e207]: 0.5 Hits
                          - button "Select over 0.5 Hits for 1.5 times" [ref=e208]: 1.5x
                        - generic [ref=e209]:
                          - button "Select over 1.5 Hits for 0 times" [disabled] [ref=e210]
                          - generic [ref=e211]: 1.5 Hits
                          - button "Select over 1.5 Hits for 3.82 times" [ref=e212]: 3.82x
                        - generic [ref=e213]:
                          - button "Select over 2.5 Hits for 0 times" [disabled] [ref=e214]
                          - generic [ref=e215]: 2.5 Hits
                          - button "Select over 2.5 Hits for 12.04 times" [ref=e216]: 12.04x
                    - generic [ref=e217]:
                      - generic [ref=e218]:
                        - generic [ref=e220] [cursor=pointer]:
                          - text: Less
                          - img [ref=e221]
                        - generic [ref=e223]: Hits + Runs + RBIs
                        - generic [ref=e225] [cursor=pointer]:
                          - text: More
                          - img [ref=e226]
                      - generic [ref=e228]:
                        - generic [ref=e229]:
                          - button "Select over 0.5 Hits + Runs + RBIs for 0 times" [disabled] [ref=e230]
                          - generic [ref=e231]: 0.5 H+R+R
                          - button "Select over 0.5 Hits + Runs + RBIs for 1.32 times" [ref=e232]: 1.32x
                        - generic [ref=e233]:
                          - button "Select over 1.5 Hits + Runs + RBIs for 0 times" [disabled] [ref=e234]
                          - generic [ref=e235]: 1.5 H+R+R
                          - button "Select over 1.5 Hits + Runs + RBIs for 2.05 times" [ref=e236]: 2.05x
                        - generic [ref=e237]:
                          - button "Select over 2.5 Hits + Runs + RBIs for 0 times" [disabled] [ref=e238]
                          - generic [ref=e239]: 2.5 H+R+R
                          - button "Select over 2.5 Hits + Runs + RBIs for 3.07 times" [ref=e240]: 3.07x
                        - generic [ref=e241]:
                          - button "Select over 3.5 Hits + Runs + RBIs for 0 times" [disabled] [ref=e242]
                          - generic [ref=e243]: 3.5 H+R+R
                          - button "Select over 3.5 Hits + Runs + RBIs for 4.77 times" [ref=e244]: 4.77x
                        - generic [ref=e245]:
                          - button "Select over 4.5 Hits + Runs + RBIs for 0 times" [disabled] [ref=e246]
                          - generic [ref=e247]: 4.5 H+R+R
                          - button "Select over 4.5 Hits + Runs + RBIs for 7.52 times" [ref=e248]: 7.52x
                    - generic [ref=e249]:
                      - generic [ref=e250]:
                        - generic [ref=e252] [cursor=pointer]:
                          - text: Less
                          - img [ref=e253]
                        - generic [ref=e255]: Singles
                        - generic [ref=e257] [cursor=pointer]:
                          - text: More
                          - img [ref=e258]
                      - generic [ref=e260]:
                        - generic [ref=e261]:
                          - button "Select over 0.5 Singles for 0 times" [disabled] [ref=e262]
                          - generic [ref=e263]: 0.5 Singles
                          - button "Select over 0.5 Singles for 1.92 times" [ref=e264]: 1.92x
                        - generic [ref=e265]:
                          - button "Select over 1.5 Singles for 0 times" [disabled] [ref=e266]
                          - generic [ref=e267]: 1.5 Singles
                          - button "Select over 1.5 Singles for 5.71 times" [ref=e268]: 5.71x
                    - generic [ref=e269]:
                      - generic [ref=e270]:
                        - generic [ref=e272] [cursor=pointer]:
                          - text: Less
                          - img [ref=e273]
                        - generic [ref=e275]: Doubles
                        - generic [ref=e277] [cursor=pointer]:
                          - text: More
                          - img [ref=e278]
                      - generic [ref=e281]:
                        - button "Select over 0.5 Doubles for 0 times" [disabled] [ref=e282]
                        - generic [ref=e283]: 0.5 Doubles
                        - button "Select over 0.5 Doubles for 4.73 times" [ref=e284]: 4.73x
                    - generic [ref=e285]:
                      - generic [ref=e286]:
                        - generic [ref=e288] [cursor=pointer]:
                          - text: Less
                          - img [ref=e289]
                        - generic [ref=e291]: Triples
                        - generic [ref=e293] [cursor=pointer]:
                          - text: More
                          - img [ref=e294]
                      - generic [ref=e297]:
                        - button "Select over 0.5 Triples for 0 times" [disabled] [ref=e298]
                        - generic [ref=e299]: 0.5 Triples
                        - button "Select over 0.5 Triples for 24.4 times" [ref=e300]: 24.4x
                    - generic [ref=e301]:
                      - generic [ref=e302]:
                        - generic [ref=e304] [cursor=pointer]:
                          - text: Less
                          - img [ref=e305]
                        - generic [ref=e307]: Runs
                        - generic [ref=e309] [cursor=pointer]:
                          - text: More
                          - img [ref=e310]
                      - generic [ref=e312]:
                        - generic [ref=e313]:
                          - button "Select over 0.5 Runs for 0 times" [disabled] [ref=e314]
                          - generic [ref=e315]: 0.5 Runs
                          - button "Select over 0.5 Runs for 2.45 times" [ref=e316]: 2.45x
                        - generic [ref=e317]:
                          - button "Select over 1.5 Runs for 0 times" [disabled] [ref=e318]
                          - generic [ref=e319]: 1.5 Runs
                          - button "Select over 1.5 Runs for 7.64 times" [ref=e320]: 7.64x
                    - generic [ref=e321]:
                      - generic [ref=e322]:
                        - generic [ref=e324] [cursor=pointer]:
                          - text: Less
                          - img [ref=e325]
                        - generic [ref=e327]: RBIs
                        - generic [ref=e329] [cursor=pointer]:
                          - text: More
                          - img [ref=e330]
                      - generic [ref=e332]:
                        - generic [ref=e333]:
                          - button "Select over 0.5 RBIs for 0 times" [disabled] [ref=e334]
                          - generic [ref=e335]: 0.5 RBIs
                          - button "Select over 0.5 RBIs for 2.9 times" [ref=e336]: 2.9x
                        - generic [ref=e337]:
                          - button "Select over 1.5 RBIs for 0 times" [disabled] [ref=e338]
                          - generic [ref=e339]: 1.5 RBIs
                          - button "Select over 1.5 RBIs for 6.29 times" [ref=e340]: 6.29x
                    - generic [ref=e341]:
                      - generic [ref=e342]:
                        - generic [ref=e344] [cursor=pointer]:
                          - text: Less
                          - img [ref=e345]
                        - generic [ref=e347]: Homeruns
                        - generic [ref=e349] [cursor=pointer]:
                          - text: More
                          - img [ref=e350]
                      - generic [ref=e352]:
                        - generic [ref=e353]:
                          - button "Select over 0.5 Homeruns for 0 times" [disabled] [ref=e354]
                          - generic [ref=e355]: 0.5 Homeruns
                          - button "Select over 0.5 Homeruns for 6.16 times" [ref=e356]: 6.16x
                        - generic [ref=e357]:
                          - button "Select over 1.5 Homeruns for 0 times" [disabled] [ref=e358]
                          - generic [ref=e359]: 1.5 Homeruns
                          - button "Select over 1.5 Homeruns for 61 times" [ref=e360]: 61x
                    - generic [ref=e361]:
                      - generic [ref=e362]:
                        - generic [ref=e364] [cursor=pointer]:
                          - text: Less
                          - img [ref=e365]
                        - generic [ref=e367]: Total Bases
                        - generic [ref=e369] [cursor=pointer]:
                          - text: More
                          - img [ref=e370]
                      - generic [ref=e372]:
                        - generic [ref=e373]:
                          - button "Select over 1.5 Total Bases for 0 times" [disabled] [ref=e374]
                          - generic [ref=e375]: 1.5 Total Bases
                          - button "Select over 1.5 Total Bases for 2.6 times" [ref=e376]: 2.6x
                        - generic [ref=e377]:
                          - button "Select over 2.5 Total Bases for 0 times" [disabled] [ref=e378]
                          - generic [ref=e379]: 2.5 Total Bases
                          - button "Select over 2.5 Total Bases for 4.22 times" [ref=e380]: 4.22x
                        - generic [ref=e381]:
                          - button "Select over 3.5 Total Bases for 0 times" [disabled] [ref=e382]
                          - generic [ref=e383]: 3.5 Total Bases
                          - button "Select over 3.5 Total Bases for 5.56 times" [ref=e384]: 5.56x
                        - generic [ref=e385]:
                          - button "Select over 4.5 Total Bases for 0 times" [disabled] [ref=e386]
                          - generic [ref=e387]: 4.5 Total Bases
                          - button "Select over 4.5 Total Bases for 11.4 times" [ref=e388]: 11.4x
                  - button "Show More Stats" [ref=e390]:
                    - img [ref=e391]
              - generic [ref=e1563]:
                - generic [ref=e1566]: Please select your 1st pick
                - generic [ref=e1569]:
                  - img "arrow" [ref=e1570]
                  - heading "Let's Start!" [level=2] [ref=e1571]
                  - generic [ref=e1572]:
                    - text: Pick at least two players
                    - text: from different teams to play
          - generic [ref=e1575]:
            - generic [ref=e1576]:
              - link "Parlay Play Logo" [ref=e1577] [cursor=pointer]:
                - /url: /
                - img "Parlay Play Logo" [ref=e1579]
              - generic [ref=e1580]:
                - generic [ref=e1581]: Improve your experience. Download our app.
                - generic [ref=e1582]:
                  - link "Apple Store" [ref=e1583] [cursor=pointer]:
                    - /url: https://parlayplay.onelink.me/oLJk/gnqpwjha
                    - img "Apple Store" [ref=e1584]
                  - link "Google Play Store" [ref=e1585] [cursor=pointer]:
                    - /url: https://parlayplay.onelink.me/oLJk/fh7u6juo
                    - img "Google Play Store" [ref=e1586]
            - generic [ref=e1587]:
              - link "Privacy" [ref=e1588] [cursor=pointer]:
                - /url: /privacy-policy
              - link "Fantasy Terms" [ref=e1589] [cursor=pointer]:
                - /url: /terms
              - link "Packs Terms" [ref=e1590] [cursor=pointer]:
                - /url: /terms/packs
              - link "Responsible Gaming" [ref=e1591] [cursor=pointer]:
                - /url: /responsible-gaming
              - link "Gaming Rules" [ref=e1592] [cursor=pointer]:
                - /url: /rules
              - link "FAQ" [ref=e1593] [cursor=pointer]:
                - /url: https://intercom.help/parlayplay/en/
              - link "Contact Us" [ref=e1594] [cursor=pointer]:
                - /url: /
              - paragraph [ref=e1595]: © ParlayPlay 2026 - All Rights Reserved
            - list [ref=e1596]:
              - listitem [ref=e1597]:
                - generic [ref=e1598]:
                  - log [ref=e1600]
                  - generic [ref=e1601]:
                    - generic [ref=e1602]:
                      - generic [ref=e1603]: 🇺🇸English
                      - combobox "Select language" [ref=e1604]
                    - img [ref=e1608]
              - listitem [ref=e1610]:
                - img "18+-icon" [ref=e1611]
              - listitem [ref=e1612]:
                - link "ParlayPlay on Twitter" [ref=e1613] [cursor=pointer]:
                  - /url: https://twitter.com/parlay_play?lang=en
                  - img [ref=e1614]
              - listitem [ref=e1616]:
                - link "ParlayPlay on Facebook" [ref=e1617] [cursor=pointer]:
                  - /url: https://www.facebook.com/ParlayPlay.io/
                  - img [ref=e1618]
              - listitem [ref=e1620]:
                - link "ParlayPlay on Instagram" [ref=e1621] [cursor=pointer]:
                  - /url: https://www.instagram.com/parlayplay_?igsh=bHBldWQyMmV2b3Y4
                  - img [ref=e1622]
              - listitem [ref=e1624]:
                - link "ParlayPlay on Discord" [ref=e1625] [cursor=pointer]:
                  - /url: https://discord.com/invite/parlayplay
                  - img [ref=e1626]
    - generic:
      - region "Notifications Alt+T"
    - generic [ref=e1629]:
      - button [ref=e1630]
      - dialog [ref=e1632]:
        - generic [ref=e1633]:
          - button [active]
  - alert [ref=e1636]
  - iframe [ref=e1637]:
    
  - button "Open Intercom Messenger" [ref=e1638] [cursor=pointer]:
    - img [ref=e1640]
    - generic:
      - img
```

# Test source

```ts
  1  | /**
  2  |  * Desktop account dropdown: the desktop counterpart to the mobile Account
  3  |  * Center. The wallet-pill burger opens NavBarDropdown inside a dialog with a
  4  |  * Deposit CTA, Account / Rewards / Support link groups and a Log Out button.
  5  |  * Desktop project only (`desktopOnlySpecs`).
  6  |  */
  7  | import { test, expect } from '../../fixtures/test.extend';
  8  | import { DesktopNavPage } from '@pages/desktopNav.page';
  9  | import { HomePage } from '@pages/home.page';
  10 | 
  11 | test.describe('Menu - Desktop Account Dropdown', { tag: ['@desktop', '@menu', '@prod'] }, () => {
  12 |   // Read-only (no logout, no Contact, isolated context per test) — parallel.
  13 |   test.describe.configure({ mode: 'parallel' });
  14 | 
  15 |   test.beforeEach(async ({ loggedInPage }) => {
  16 |     const homePage = new HomePage(loggedInPage);
  17 |     const nav = new DesktopNavPage(loggedInPage);
  18 |     await loggedInPage.goto('/');
  19 |     await homePage.waitForFeedReady();
  20 |     await nav.toggleMenuBtn.click();
> 21 |     await expect(nav.accountDropdown).toBeVisible();
     |                                       ^ Error: expect(locator).toBeVisible() failed
  22 |   });
  23 | 
  24 |   test('Dropdown shows the Deposit CTA and the Account/Rewards/Support groups', async ({
  25 |     loggedInPage: page,
  26 |   }) => {
  27 |     const nav = new DesktopNavPage(page);
  28 |     const dropdown = nav.accountDropdown;
  29 | 
  30 |     await test.step('Deposit CTA links to /payments/deposit and all three groups are shown', async () => {
  31 |       await expect(dropdown.getByRole('link', { name: 'Deposit' })).toHaveAttribute(
  32 |         'href',
  33 |         '/payments/deposit',
  34 |       );
  35 | 
  36 |       for (const group of ['Account', 'Rewards', 'Support']) {
  37 |         await expect(dropdown.getByText(group, { exact: true })).toBeVisible();
  38 |       }
  39 |     });
  40 | 
  41 |     await test.step('Contact and Log Out render as buttons (mobile renders Log Out as a link)', async () => {
  42 |       await expect(dropdown.getByRole('button', { name: 'Contact' })).toBeVisible();
  43 |       await expect(dropdown.getByRole('button', { name: 'Log Out' })).toBeVisible();
  44 |     });
  45 |   });
  46 | 
  47 |   test('Menu items link to the same destinations as the mobile Account Center', async ({
  48 |     loggedInPage: page,
  49 |   }) => {
  50 |     const nav = new DesktopNavPage(page);
  51 |     const dropdown = nav.accountDropdown;
  52 | 
  53 |     const expected: Record<string, string> = {
  54 |       Settings: '/account/update',
  55 |       'Transaction History': '/transactions',
  56 |       Withdraw: '/payments/withdraw',
  57 |       'My Entries': '/challenges/pending',
  58 |       Taxes: '/payments/taxes',
  59 |       'Responsible Play': '/account/responsible-play',
  60 |       Promotions: '/rewards/promotions',
  61 |       'Partner Rewards': '/rewards',
  62 |       'Refer a friend': '/account/referrals',
  63 |     };
  64 | 
  65 |     for (const [label, href] of Object.entries(expected)) {
  66 |       await test.step(`"${label}" links to ${href}`, async () => {
  67 |         await expect(dropdown.getByRole('link', { name: label, exact: true })).toHaveAttribute(
  68 |           'href',
  69 |           href,
  70 |         );
  71 |       });
  72 |     }
  73 |   });
  74 | 
  75 |   test('Navigating via a menu item closes the dropdown and routes', async ({
  76 |     loggedInPage: page,
  77 |   }) => {
  78 |     const nav = new DesktopNavPage(page);
  79 | 
  80 |     await test.step('Click "Settings" in the dropdown', async () => {
  81 |       await nav.accountDropdown.getByRole('link', { name: 'Settings', exact: true }).click();
  82 |     });
  83 | 
  84 |     await test.step('Route is /account/update and the dropdown is closed', async () => {
  85 |       await page.waitForURL('**/account/update');
  86 |       await expect(nav.accountDropdown).toBeHidden();
  87 |     });
  88 |   });
  89 | });
  90 | 
```