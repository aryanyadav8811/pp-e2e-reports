# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: entries/entry-card.spec.ts >> My Entries - entry card >> View Leaderboard opens the contest-group leaderboard modal
- Location: tests/entries/entry-card.spec.ts:211:3

# Error details

```
Error: expect(locator).toBeVisible() failed

Locator: getByRole('button', { name: 'History' }).filter({ visible: true }).first()
Expected: visible
Timeout: 60000ms
Error: element(s) not found

Call log:
  - Expect "toBeVisible" with timeout 60000ms
  - waiting for getByRole('button', { name: 'History' }).filter({ visible: true }).first()

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
              - generic [ref=e13]: $762.00
              - generic [ref=e14]:
                - img "gift-icon" [ref=e15]
                - text: "60.00"
            - button "Toggle Menu" [ref=e16]:
              - img [ref=e17]
      - main [ref=e19]:
        - generic [ref=e22]:
          - generic [ref=e23]:
            - generic [ref=e24]: It looks like you're already logged in!
            - button "Make your picks now!" [ref=e26] [cursor=pointer]
          - generic [ref=e27]:
            - button "Close banner" [ref=e28]:
              - img [ref=e29]
            - generic [ref=e32]:
              - generic [ref=e33]:
                - paragraph [ref=e34]: $5
                - generic [ref=e35]:
                  - paragraph [ref=e36]: "*Terms Apply"
                  - paragraph [ref=e37]: Free on Sign Up
              - paragraph [ref=e38]: No deposit required
              - link "Sign up!" [ref=e39] [cursor=pointer]:
                - /url: /account/signup
                - generic [ref=e40]: Sign up!
    - generic:
      - region "Notifications Alt+T"
  - alert [ref=e41]: ParlayPlay | Fun Fantasy Sports - Login
  - iframe [ref=e42]:
    
```

# Test source

```ts
  1   | import { type Locator, expect, Page } from '@playwright/test';
  2   | import { BasePage } from './base.page';
  3   | import { parseStatValue } from '@utils/helpers';
  4   | 
  5   | export class EntriesPage extends BasePage {
  6   |   cardsPerPage = 16;
  7   | 
  8   |   readonly historyTab = this.byRole('button', { name: 'History' });
  9   |   readonly activeTab = this.byRole('button', { name: 'Active' });
  10  |   readonly dropdown = this.locator('select');
  11  |   readonly browseNow = this.byRole('button', { name: /^Browse now!?$/i });
  12  | 
  13  |   readonly entryAmountStat = this.byText('Entry Amount').locator('..');
  14  |   readonly maxPayoutStat = this.byText('Max Payout').locator('..');
  15  | 
  16  |   readonly entriesPlacedStat = this.byText('Entries Placed')
  17  |     .locator('..')
  18  |     .locator('.font-museo')
  19  |     .first();
  20  |   readonly entriesWonStat = this.byText('Entries Won').locator('..').locator('.font-museo').first();
  21  |   readonly historyEntryAmountStat = this.byText('Entry Amount')
  22  |     .locator('..')
  23  |     .locator('.font-museo')
  24  |     .first();
  25  |   readonly totalWonStat = this.byText('Total Won').locator('..').locator('.font-museo').first();
  26  |   readonly biggestPayoutStat = this.byText('Biggest Payout')
  27  |     .locator('..')
  28  |     .locator('.font-museo')
  29  |     .first();
  30  | 
  31  |   readonly nextArrow = this.locator('button:has(svg.fa-arrow-right)');
  32  | 
  33  |   // Collections: the base `locator()` helper appends `.first()`, so these go
  34  |   // through `this.page.locator(...)` directly.
  35  |   readonly cardDivs = this.page
  36  |     .locator('section div[role="region"][aria-controls^="entry-"]')
  37  |     .filter({ visible: true });
  38  |   readonly paginationButtons = this.page
  39  |     .locator('div.w-full.flex.items-center.justify-evenly button')
  40  |     .filter({ visible: true });
  41  |   readonly getNumberedPaginationButtons = this.page
  42  |     .locator('div.w-full.flex.items-center.justify-evenly button span')
  43  |     .filter({ hasText: /^[0-9]+$/ })
  44  |     .locator('..')
  45  |     .filter({ visible: true });
  46  |   readonly pageButtons = this.page
  47  |     .getByRole('button')
  48  |     .filter({ hasText: /^[0-9]+$/ })
  49  |     .filter({ visible: true });
  50  |   readonly lastCard = this.page
  51  |     .locator('div[role="region"][aria-controls^="entry-"]')
  52  |     .filter({ visible: true })
  53  |     .last();
  54  | 
  55  |   constructor(page: Page) {
  56  |     super(page);
  57  |   }
  58  | 
  59  |   async getStatText(locator: Locator): Promise<string> {
  60  |     const text = await locator.textContent();
  61  |     return text ?? '';
  62  |   }
  63  | 
  64  |   async assertEntriesPageLoaded() {
  65  |     await super.assertReady();
  66  |     // Bounded so a broken page fails here instead of burning the test timeout.
> 67  |     await expect(this.historyTab).toBeVisible({ timeout: 60000 });
      |                                   ^ Error: expect(locator).toBeVisible() failed
  68  |     await this.waitForEntriesReady();
  69  |   }
  70  | 
  71  |   async waitForEntriesReady(timeout = 15_000): Promise<void> {
  72  |     await Promise.race([
  73  |       this.cardDivs.first().waitFor({ state: 'visible', timeout }),
  74  |       this.browseNow.waitFor({ state: 'visible', timeout }),
  75  |     ]);
  76  |   }
  77  | 
  78  |   async enterHistorytab() {
  79  |     await this.historyTab.click();
  80  |   }
  81  | 
  82  |   async selectTimeRangeValue(range: '7 Days' | '30 Days' | '6 Months'): Promise<void> {
  83  |     await this.byRole('button', { name: range }).click();
  84  |   }
  85  | 
  86  |   readonly prevArrow = this.locator('button:has(svg.fa-arrow-left)');
  87  | 
  88  |   /**
  89  |    * The pagination row sits under the mobile fixed bottom nav, whose tabs
  90  |    * "intercept pointer events" and make a plain click retry until the test
  91  |    * times out. Fall back to dispatchEvent, which bypasses hit-testing.
  92  |    */
  93  |   async clickPaginationControl(control: Locator): Promise<void> {
  94  |     await control.scrollIntoViewIfNeeded();
  95  |     try {
  96  |       await control.click({ timeout: 5_000 });
  97  |     } catch {
  98  |       await control.dispatchEvent('click');
  99  |     }
  100 |   }
  101 | 
  102 |   async getEntriesCount() {
  103 |     let total = await this.cardDivs.count();
  104 | 
  105 |     if (!(await this.nextArrow.isVisible().catch(() => false))) return total;
  106 | 
  107 |     do {
  108 |       await this.clickPaginationControl(this.nextArrow);
  109 |       await this.cardDivs.first().waitFor({ state: 'visible' });
  110 |       total += await this.cardDivs.count();
  111 |     } while (!(await this.nextArrow.isDisabled()));
  112 | 
  113 |     while (!(await this.prevArrow.isDisabled())) {
  114 |       await this.clickPaginationControl(this.prevArrow);
  115 |       await this.cardDivs.first().waitFor({ state: 'visible' });
  116 |     }
  117 | 
  118 |     return total;
  119 |   }
  120 | 
  121 |   async verifyNumberGreaterThan(minCount: number, timeout = 15_000) {
  122 |     await this.waitForEntriesReady(timeout);
  123 |     const count = await this.getEntriesCount();
  124 |     expect(count).toBeGreaterThan(minCount);
  125 |   }
  126 | 
  127 |   async verifyCardsInFirstPage() {
  128 |     const cardsCount = await this.cardDivs.count();
  129 |     expect(cardsCount).toBe(this.cardsPerPage);
  130 |   }
  131 | 
  132 |   async isNoDataVisible() {
  133 |     return await this.browseNow.isVisible();
  134 |   }
  135 | 
  136 |   async getStats() {
  137 |     const rawEntryAmount = await this.getStatText(this.entryAmountStat);
  138 |     const rawMaxPayout = await this.getStatText(this.maxPayoutStat);
  139 | 
  140 |     return {
  141 |       entryAmount: parseStatValue(rawEntryAmount),
  142 |       maxPayout: parseStatValue(rawMaxPayout),
  143 |     };
  144 |   }
  145 | 
  146 |   async getHistoryStats() {
  147 |     const rawPlaced = await this.getStatText(this.entriesPlacedStat);
  148 |     const rawWon = await this.getStatText(this.entriesWonStat);
  149 |     const rawEntryAmount = await this.getStatText(this.historyEntryAmountStat);
  150 |     const rawTotalWon = await this.getStatText(this.totalWonStat);
  151 |     const rawBiggestPayout = await this.getStatText(this.biggestPayoutStat);
  152 | 
  153 |     return {
  154 |       placed: parseStatValue(rawPlaced),
  155 |       won: parseStatValue(rawWon),
  156 |       amount: parseStatValue(rawEntryAmount),
  157 |       totalWon: parseStatValue(rawTotalWon),
  158 |       biggestPayout: parseStatValue(rawBiggestPayout),
  159 |     };
  160 |   }
  161 | 
  162 |   async enterActiveTab() {
  163 |     await this.activeTab.click();
  164 |   }
  165 | 
  166 |   async assertActiveTabLoaded() {
  167 |     await this.page.waitForURL('**/challenges/pending');
```