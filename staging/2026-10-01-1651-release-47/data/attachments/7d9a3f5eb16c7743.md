# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: entries/entries.spec.ts >> My Entries - Active and History >> Active tab shows the Entry Amount and Max Payout stats
- Location: tests/entries/entries.spec.ts:19:3

# Error details

```
Test timeout of 180000ms exceeded.
```

```
Error: locator.textContent: Target page, context or browser has been closed
Call log:
  - waiting for getByText('Entry Amount').filter({ visible: true }).first().locator('..')

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
                - link "Track Picks" [active] [ref=e29] [cursor=pointer]:
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
                  - text: $100
                  - img "black lightning bol" [ref=e55]
                - generic [ref=e57]: =
                - generic [ref=e58]:
                  - text: $200
                  - img "black lightning bol" [ref=e59]
                - generic [ref=e60]:
                  - text: We match your 1st deposit
                  - text: We match your first deposit up to $100.
                  - button "Deposit Now" [ref=e62] [cursor=pointer]
              - generic [ref=e64]:
                - generic [ref=e65]:
                  - generic [ref=e66]: Receive a referral Bonus!
                  - generic [ref=e67]: $20
                - generic [ref=e68]:
                  - text: Refer a Friend
                  - text: when they make their first deposit
                  - button "Invite Now" [ref=e70] [cursor=pointer]
            - button "next slide" [ref=e71] [cursor=pointer]:
              - img [ref=e72]
          - generic [ref=e75]:
            - navigation [ref=e76]:
              - list [ref=e77]:
                - listitem [ref=e78]:
                  - button "Active" [ref=e79]
                - listitem [ref=e80]:
                  - button "History" [ref=e81]
            - generic [ref=e84]:
              - generic [ref=e85]: Looks like you don't have any pending entries.
              - button "Browse now" [ref=e87] [cursor=pointer]
          - generic [ref=e90]:
            - generic [ref=e91]:
              - link "Parlay Play Logo" [ref=e92] [cursor=pointer]:
                - /url: /
                - img "Parlay Play Logo" [ref=e94]
              - generic [ref=e95]:
                - generic [ref=e96]: Improve your experience. Download our app.
                - generic [ref=e97]:
                  - link "Apple Store" [ref=e98] [cursor=pointer]:
                    - /url: https://apps.apple.com/us/app/parlayplay-fantasy-sports-game/id1634803703
                    - img "Apple Store" [ref=e99]
                  - link "Google Play Store" [ref=e100] [cursor=pointer]:
                    - /url: https://play.google.com/store/apps/details?id=com.parlayplay.app&hl=en_US
                    - img "Google Play Store" [ref=e101]
            - generic [ref=e102]:
              - link "Privacy" [ref=e103] [cursor=pointer]:
                - /url: /privacy-policy
              - link "Fantasy Terms" [ref=e104] [cursor=pointer]:
                - /url: /terms
              - link "Packs Terms" [ref=e105] [cursor=pointer]:
                - /url: /terms/packs
              - link "Responsible Gaming" [ref=e106] [cursor=pointer]:
                - /url: /responsible-gaming
              - link "Gaming Rules" [ref=e107] [cursor=pointer]:
                - /url: /rules
              - link "FAQ" [ref=e108] [cursor=pointer]:
                - /url: https://intercom.help/parlayplay/en/
              - link "Contact Us" [ref=e109] [cursor=pointer]:
                - /url: /
              - paragraph [ref=e110]: © ParlayPlay 2026 - All Rights Reserved
            - list [ref=e111]:
              - listitem [ref=e112]:
                - generic [ref=e113]:
                  - log [ref=e115]
                  - generic [ref=e116]:
                    - generic [ref=e117]:
                      - generic [ref=e118]: 🇺🇸English
                      - combobox "Select language" [ref=e119]
                    - img [ref=e123]
              - listitem [ref=e125]:
                - img "18+-icon" [ref=e126]
              - listitem [ref=e127]:
                - link "ParlayPlay on Twitter" [ref=e128] [cursor=pointer]:
                  - /url: https://twitter.com/parlay_play?lang=en
                  - img [ref=e129]
              - listitem [ref=e131]:
                - link "ParlayPlay on Facebook" [ref=e132] [cursor=pointer]:
                  - /url: https://www.facebook.com/ParlayPlay.io/
                  - img [ref=e133]
              - listitem [ref=e135]:
                - link "ParlayPlay on Instagram" [ref=e136] [cursor=pointer]:
                  - /url: https://www.instagram.com/parlayplay_?igsh=bHBldWQyMmV2b3Y4
                  - img [ref=e137]
              - listitem [ref=e139]:
                - link "ParlayPlay on Discord" [ref=e140] [cursor=pointer]:
                  - /url: https://discord.com/invite/parlayplay
                  - img [ref=e141]
    - generic:
      - region "Notifications Alt+T"
  - alert [ref=e143]: ParlayPlay | Fun Fantasy Sports - My Entries
  - iframe [ref=e144]:
    
  - button "Open Intercom Messenger" [ref=e145] [cursor=pointer]:
    - img [ref=e147]
    - generic:
      - img
```

# Test source

```ts
  1   | import { type Locator, expect, Page } from '@playwright/test';
  2   | import { BasePage } from './base.page';
  3   | import { parseStatValue } from '@utils/helpers';
  4   | import { findPendingEntry } from '@utils/apiHelpers';
  5   | 
  6   | export class EntriesPage extends BasePage {
  7   |   cardsPerPage = 16;
  8   | 
  9   |   readonly historyTab = this.byRole('button', { name: 'History' });
  10  |   readonly activeTab = this.byRole('button', { name: 'Active' });
  11  |   readonly dropdown = this.locator('select');
  12  |   readonly browseNow = this.byRole('button', { name: /^Browse now!?$/i });
  13  | 
  14  |   readonly entryAmountStat = this.byText('Entry Amount').locator('..');
  15  |   readonly maxPayoutStat = this.byText('Max Payout').locator('..');
  16  | 
  17  |   readonly entriesPlacedStat = this.byText('Entries Placed')
  18  |     .locator('..')
  19  |     .locator('.font-museo')
  20  |     .first();
  21  |   readonly entriesWonStat = this.byText('Entries Won').locator('..').locator('.font-museo').first();
  22  |   readonly historyEntryAmountStat = this.byText('Entry Amount')
  23  |     .locator('..')
  24  |     .locator('.font-museo')
  25  |     .first();
  26  |   readonly totalWonStat = this.byText('Total Won').locator('..').locator('.font-museo').first();
  27  |   readonly biggestPayoutStat = this.byText('Biggest Payout')
  28  |     .locator('..')
  29  |     .locator('.font-museo')
  30  |     .first();
  31  | 
  32  |   readonly nextArrow = this.locator('button:has(svg.fa-arrow-right)');
  33  | 
  34  |   // Collections: the base `locator()` helper appends `.first()`, so these go
  35  |   // through `this.page.locator(...)` directly.
  36  |   readonly cardDivs = this.page
  37  |     .locator('section div[role="region"][aria-controls^="entry-"]')
  38  |     .filter({ visible: true });
  39  |   readonly paginationButtons = this.page
  40  |     .locator('div.w-full.flex.items-center.justify-evenly button')
  41  |     .filter({ visible: true });
  42  |   readonly getNumberedPaginationButtons = this.page
  43  |     .locator('div.w-full.flex.items-center.justify-evenly button span')
  44  |     .filter({ hasText: /^[0-9]+$/ })
  45  |     .locator('..')
  46  |     .filter({ visible: true });
  47  |   readonly pageButtons = this.page
  48  |     .getByRole('button')
  49  |     .filter({ hasText: /^[0-9]+$/ })
  50  |     .filter({ visible: true });
  51  |   readonly lastCard = this.page
  52  |     .locator('div[role="region"][aria-controls^="entry-"]')
  53  |     .filter({ visible: true })
  54  |     .last();
  55  | 
  56  |   constructor(page: Page) {
  57  |     super(page);
  58  |   }
  59  | 
  60  |   async getStatText(locator: Locator): Promise<string> {
> 61  |     const text = await locator.textContent();
      |                                ^ Error: locator.textContent: Target page, context or browser has been closed
  62  |     return text ?? '';
  63  |   }
  64  | 
  65  |   async assertEntriesPageLoaded() {
  66  |     await super.assertReady();
  67  |     // Bounded so a broken page fails here instead of burning the test timeout.
  68  |     await expect(this.historyTab).toBeVisible({ timeout: 60000 });
  69  |     await this.waitForEntriesReady();
  70  |   }
  71  | 
  72  |   async waitForEntriesReady(timeout = 15_000): Promise<void> {
  73  |     await Promise.race([
  74  |       this.cardDivs.first().waitFor({ state: 'visible', timeout }),
  75  |       this.browseNow.waitFor({ state: 'visible', timeout }),
  76  |     ]);
  77  |   }
  78  | 
  79  |   async enterHistorytab() {
  80  |     await this.historyTab.click();
  81  |   }
  82  | 
  83  |   async selectTimeRangeValue(range: '7 Days' | '30 Days' | '6 Months'): Promise<void> {
  84  |     await this.byRole('button', { name: range }).click();
  85  |   }
  86  | 
  87  |   readonly prevArrow = this.locator('button:has(svg.fa-arrow-left)');
  88  | 
  89  |   /**
  90  |    * The pagination row sits under the mobile fixed bottom nav, whose tabs
  91  |    * "intercept pointer events" and make a plain click retry until the test
  92  |    * times out. Fall back to dispatchEvent, which bypasses hit-testing.
  93  |    */
  94  |   async clickPaginationControl(control: Locator): Promise<void> {
  95  |     await control.scrollIntoViewIfNeeded({ timeout: 15_000 });
  96  |     try {
  97  |       await control.click({ timeout: 5_000 });
  98  |     } catch {
  99  |       await control.dispatchEvent('click');
  100 |     }
  101 |   }
  102 | 
  103 |   async getEntriesCount() {
  104 |     let total = await this.cardDivs.count();
  105 | 
  106 |     if (!(await this.nextArrow.isVisible().catch(() => false))) return total;
  107 | 
  108 |     do {
  109 |       await this.clickPaginationControl(this.nextArrow);
  110 |       await this.cardDivs.first().waitFor({ state: 'visible' });
  111 |       total += await this.cardDivs.count();
  112 |     } while (!(await this.nextArrow.isDisabled()));
  113 | 
  114 |     while (!(await this.prevArrow.isDisabled())) {
  115 |       await this.clickPaginationControl(this.prevArrow);
  116 |       await this.cardDivs.first().waitFor({ state: 'visible' });
  117 |     }
  118 | 
  119 |     return total;
  120 |   }
  121 | 
  122 |   async verifyNumberGreaterThan(minCount: number, timeout = 15_000) {
  123 |     await this.waitForEntriesReady(timeout);
  124 |     const count = await this.getEntriesCount();
  125 |     expect(count).toBeGreaterThan(minCount);
  126 |   }
  127 | 
  128 |   async verifyCardsInFirstPage() {
  129 |     const cardsCount = await this.cardDivs.count();
  130 |     expect(cardsCount).toBe(this.cardsPerPage);
  131 |   }
  132 | 
  133 |   async isNoDataVisible() {
  134 |     return await this.browseNow.isVisible();
  135 |   }
  136 | 
  137 |   async getStats() {
  138 |     const rawEntryAmount = await this.getStatText(this.entryAmountStat);
  139 |     const rawMaxPayout = await this.getStatText(this.maxPayoutStat);
  140 | 
  141 |     return {
  142 |       entryAmount: parseStatValue(rawEntryAmount),
  143 |       maxPayout: parseStatValue(rawMaxPayout),
  144 |     };
  145 |   }
  146 | 
  147 |   async getHistoryStats() {
  148 |     const rawPlaced = await this.getStatText(this.entriesPlacedStat);
  149 |     const rawWon = await this.getStatText(this.entriesWonStat);
  150 |     const rawEntryAmount = await this.getStatText(this.historyEntryAmountStat);
  151 |     const rawTotalWon = await this.getStatText(this.totalWonStat);
  152 |     const rawBiggestPayout = await this.getStatText(this.biggestPayoutStat);
  153 | 
  154 |     return {
  155 |       placed: parseStatValue(rawPlaced),
  156 |       won: parseStatValue(rawWon),
  157 |       amount: parseStatValue(rawEntryAmount),
  158 |       totalWon: parseStatValue(rawTotalWon),
  159 |       biggestPayout: parseStatValue(rawBiggestPayout),
  160 |     };
  161 |   }
```