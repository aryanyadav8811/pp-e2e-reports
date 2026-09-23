# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: entries/entries.spec.ts >> My Entries - Active and History >> User can switch between the Active and History tabs
- Location: tests/entries/entries.spec.ts:96:3

# Error details

```
Test timeout of 180000ms exceeded.
```

```
Error: page.waitForURL: Target page, context or browser has been closed
=========================== logs ===========================
waiting for navigation to "**/challenges/pending" until "load"
============================================================
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
            - generic [ref=e13]: $609.48
            - button "Toggle Menu" [ref=e14]:
              - img [ref=e15]
      - main [ref=e17]:
        - generic [ref=e20]:
          - navigation [ref=e21]:
            - list [ref=e22]:
              - listitem [ref=e23]:
                - button "Active" [ref=e24]
              - listitem [ref=e25]:
                - button "History" [ref=e26]
          - generic [ref=e27]:
            - generic [ref=e28]:
              - generic [ref=e29]:
                - button "7 Days" [ref=e30]
                - button "30 Days" [ref=e31]
                - button "6 Months" [ref=e32]
              - generic [ref=e34]:
                - generic [ref=e35]:
                  - generic [ref=e36]: 57Entries Placed
                  - generic [ref=e37]:
                    - generic [ref=e38]:
                      - generic [ref=e39]: "2"
                      - text: Entries Won
                    - img [ref=e41]
                - generic [ref=e43]:
                  - generic [ref=e44]:
                    - generic [ref=e45]: Entry Amount
                    - generic [ref=e46]: $171
                  - generic [ref=e47]:
                    - generic [ref=e48]: Total Won
                    - generic [ref=e49]: $18.48
                  - generic [ref=e50]:
                    - generic [ref=e51]: Biggest Payout
                    - generic [ref=e52]: $9.2
            - generic [ref=e53]:
              - region [ref=e54]:
                - button "Expand entry details" [ref=e55]:
                  - generic [ref=e56]:
                    - generic [ref=e57]:
                      - generic [ref=e59]: $3
                      - generic [ref=e60]: To win $17.73
                    - generic [ref=e62]: Lost
                - button "Expand entry details" [ref=e65]:
                  - img "Expand" [ref=e66]
              - region [ref=e67]:
                - button "Expand entry details" [ref=e68]:
                  - generic [ref=e69]:
                    - generic [ref=e70]:
                      - generic [ref=e72]: $3
                      - generic [ref=e73]: To win $18.03
                    - generic [ref=e75]: Lost
                - button "Expand entry details" [ref=e78]:
                  - img "Expand" [ref=e79]
              - region [ref=e80]:
                - button "Expand entry details" [ref=e81]:
                  - generic [ref=e82]:
                    - generic [ref=e83]:
                      - generic [ref=e85]: $3
                      - generic [ref=e86]: To win $17.82
                    - generic [ref=e88]: Lost
                - button "Expand entry details" [ref=e91]:
                  - img "Expand" [ref=e92]
              - region [ref=e93]:
                - button "Expand entry details" [ref=e94]:
                  - generic [ref=e95]:
                    - generic [ref=e96]:
                      - generic [ref=e98]: $3
                      - generic [ref=e99]: To win $18.03
                    - generic [ref=e101]: Lost
                - button "Expand entry details" [ref=e104]:
                  - img "Expand" [ref=e105]
              - region [ref=e106]:
                - button "Expand entry details" [ref=e107]:
                  - generic [ref=e108]:
                    - generic [ref=e109]:
                      - generic [ref=e111]: $3
                      - generic [ref=e112]: To win $18.12
                    - generic [ref=e114]: Lost
                - button "Expand entry details" [ref=e117]:
                  - img "Expand" [ref=e118]
              - region [ref=e119]:
                - button "Expand entry details" [ref=e120]:
                  - generic [ref=e121]:
                    - generic [ref=e122]:
                      - generic [ref=e124]: $3
                      - generic [ref=e125]: To win $18.03
                    - generic [ref=e127]: Lost
                - button "Expand entry details" [ref=e130]:
                  - img "Expand" [ref=e131]
              - region [ref=e132]:
                - button "Expand entry details" [ref=e133]:
                  - generic [ref=e134]:
                    - generic [ref=e135]:
                      - generic [ref=e137]: $3
                      - generic [ref=e138]: To win $76.53
                    - generic [ref=e140]: Lost
                - button "Expand entry details" [ref=e143]:
                  - img "Expand" [ref=e144]
              - region [ref=e145]:
                - button "Expand entry details" [ref=e146]:
                  - generic [ref=e147]:
                    - generic [ref=e148]:
                      - generic [ref=e150]: $3
                      - generic [ref=e151]: To win $11.04
                    - generic [ref=e153]: Lost
                - button "Expand entry details" [ref=e156]:
                  - img "Expand" [ref=e157]
              - region [ref=e158]:
                - button "Expand entry details" [ref=e159]:
                  - generic [ref=e160]:
                    - generic [ref=e161]:
                      - generic [ref=e163]: $3
                      - generic [ref=e164]: To win $18.12
                    - generic [ref=e166]: Lost
                - button "Expand entry details" [ref=e169]:
                  - img "Expand" [ref=e170]
              - region [ref=e171]:
                - button "Expand entry details" [ref=e172]:
                  - generic [ref=e173]:
                    - generic [ref=e174]:
                      - generic [ref=e176]: $3
                      - generic [ref=e177]: To win $76.53
                    - generic [ref=e179]: Lost
                - button "Expand entry details" [ref=e182]:
                  - img "Expand" [ref=e183]
              - region [ref=e184]:
                - button "Expand entry details" [ref=e185]:
                  - generic [ref=e186]:
                    - generic [ref=e187]:
                      - generic [ref=e189]: $3
                      - generic [ref=e190]: To win $17.82
                    - generic [ref=e192]: Lost
                - button "Expand entry details" [ref=e195]:
                  - img "Expand" [ref=e196]
              - region [ref=e197]:
                - button "Expand entry details" [ref=e198]:
                  - generic [ref=e199]:
                    - generic [ref=e200]:
                      - generic [ref=e202]: $3
                      - generic [ref=e203]: To win $17.82
                    - generic [ref=e205]: Lost
                - button "Expand entry details" [ref=e208]:
                  - img "Expand" [ref=e209]
              - region [ref=e210]:
                - button "Expand entry details" [ref=e211]:
                  - generic [ref=e212]:
                    - generic [ref=e213]:
                      - generic [ref=e215]: $3
                      - generic [ref=e216]: To win $18.12
                    - generic [ref=e218]: Lost
                - button "Expand entry details" [ref=e221]:
                  - img "Expand" [ref=e222]
              - region [ref=e223]:
                - button "Expand entry details" [ref=e224]:
                  - generic [ref=e225]:
                    - generic [ref=e226]:
                      - generic [ref=e228]: $3
                      - generic [ref=e229]: To win $18.12
                    - generic [ref=e231]: Lost
                - button "Expand entry details" [ref=e234]:
                  - img "Expand" [ref=e235]
              - region [ref=e236]:
                - button "Expand entry details" [ref=e237]:
                  - generic [ref=e238]:
                    - generic [ref=e239]:
                      - generic [ref=e241]: $3
                      - generic [ref=e242]: To win $76.53
                    - generic [ref=e244]: Lost
                - button "Expand entry details" [ref=e247]:
                  - img "Expand" [ref=e248]
              - region [ref=e249]:
                - button "Expand entry details" [ref=e250]:
                  - generic [ref=e251]:
                    - generic [ref=e252]:
                      - generic [ref=e254]: $3
                      - generic [ref=e255]: To win $17.73
                    - generic [ref=e257]: Lost
                - button "Expand entry details" [ref=e260]:
                  - img "Expand" [ref=e261]
          - generic [ref=e263]:
            - button [disabled] [ref=e264]:
              - img [ref=e265]
            - button "1" [ref=e267]:
              - generic [ref=e268]: "1"
            - button "2" [ref=e269]:
              - generic [ref=e270]: "2"
            - button "3" [ref=e271]:
              - generic [ref=e272]: "3"
            - button "4" [ref=e273]:
              - generic [ref=e274]: "4"
            - button [ref=e275]:
              - img [ref=e276]
      - contentinfo [ref=e278]:
        - navigation [ref=e279]:
          - list [ref=e280]:
            - listitem [ref=e281]:
              - button "Home" [ref=e282] [cursor=pointer]:
                - generic [ref=e283]:
                  - img [ref=e284]
                  - generic [ref=e285]: Home
            - listitem [ref=e286]:
              - button "Entries 191" [ref=e287] [cursor=pointer]:
                - generic [ref=e288]:
                  - img [ref=e289]
                  - generic [ref=e290]: Entries
                - generic [ref=e291]: "191"
            - listitem [ref=e292]:
              - button "Feed" [ref=e293] [cursor=pointer]:
                - generic [ref=e294]:
                  - img [ref=e295]
                  - generic [ref=e296]: Feed
            - listitem [ref=e297]:
              - button "Rewards 1" [ref=e298] [cursor=pointer]:
                - generic [ref=e299]:
                  - img [ref=e300]
                  - generic [ref=e301]: Rewards
                - generic [ref=e302]: "1"
            - listitem [ref=e303]:
              - button "Packs" [ref=e304] [cursor=pointer]:
                - generic [ref=e305]:
                  - img [ref=e306]
                  - generic [ref=e307]: Packs
    - generic:
      - region "Notifications Alt+T"
  - alert [ref=e308]: ParlayPlay | Fun Fantasy Sports - My Entries - History
```

# Test source

```ts
  67  |     await expect(this.historyTab).toBeVisible({ timeout: 60000 });
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
> 167 |     await this.page.waitForURL('**/challenges/pending');
      |                     ^ Error: page.waitForURL: Target page, context or browser has been closed
  168 |   }
  169 | 
  170 |   async assertHistoryTabLoaded() {
  171 |     await this.page.waitForURL('**/challenges/history');
  172 |   }
  173 | 
  174 |   async getTotalPaginationPages() {
  175 |     return await this.getNumberedPaginationButtons.count();
  176 |   }
  177 | 
  178 |   async gotoTrueLastPage() {
  179 |     const count = await this.pageButtons.count();
  180 | 
  181 |     if (count === 0) return;
  182 | 
  183 |     const numbers: number[] = [];
  184 |     for (let i = 0; i < count; i++) {
  185 |       const txt = await this.pageButtons.nth(i).innerText();
  186 |       numbers.push(parseInt(txt, 10));
  187 |     }
  188 |     const maxVisible = Math.max(...numbers);
  189 | 
  190 |     // The pager shows at most 5 page numbers; beyond that, hop to 5 first to
  191 |     // reveal the rest.
  192 |     if (maxVisible <= 5) {
  193 |       await this.pageButtons.filter({ hasText: String(maxVisible) }).click();
  194 |     } else {
  195 |       await this.pageButtons.filter({ hasText: '5' }).click();
  196 |       const refreshed = this.pageButtons;
  197 |       const refreshedCount = await refreshed.count();
  198 |       const refreshedNumbers: number[] = [];
  199 |       for (let i = 0; i < refreshedCount; i++) {
  200 |         const txt = await refreshed.nth(i).innerText();
  201 |         refreshedNumbers.push(parseInt(txt, 10));
  202 |       }
  203 |       const lastPage = Math.max(...refreshedNumbers);
  204 |       await refreshed.filter({ hasText: String(lastPage) }).click();
  205 |     }
  206 | 
  207 |     await expect(this.nextArrow).toBeDisabled();
  208 |   }
  209 | 
  210 |   async verifyLastEntryIs(submissionId: string) {
  211 |     await this.gotoTrueLastPage();
  212 | 
  213 |     await this.lastCard.scrollIntoViewIfNeeded();
  214 |     await this.lastCard.click();
  215 | 
  216 |     await expect(this.lastCard).toContainText(submissionId);
  217 |   }
  218 | 
  219 |   // A card's header and its bottom-right chevron both toggle expand/collapse
  220 |   // and share the same accessible name ("Expand/Collapse entry details"), so
  221 |   // they're only distinguishable by DOM order — header first, chevron last.
  222 |   headerToggle(card: Locator): Locator {
  223 |     return card.getByRole('button', { name: /entry details/ }).first();
  224 |   }
  225 | 
  226 |   chevronToggle(card: Locator): Locator {
  227 |     return card.getByRole('button', { name: /entry details/ }).last();
  228 |   }
  229 | 
  230 |   async expandCard(card: Locator): Promise<void> {
  231 |     if ((await card.getAttribute('aria-expanded')) === 'true') return;
  232 |     await this.headerToggle(card).click();
  233 |     await expect(card).toHaveAttribute('aria-expanded', 'true');
  234 |   }
  235 | 
  236 |   /**
  237 |    * An entry is only cancellable within 5 minutes of creation and while none
  238 |    * of its picks have gone live. The matched card is left expanded.
  239 |    */
  240 |   async findCancellableCardOnCurrentPage(): Promise<Locator | null> {
  241 |     const count = await this.cardDivs.count();
  242 |     for (let i = 0; i < count; i++) {
  243 |       const card = this.cardDivs.nth(i);
  244 |       await this.expandCard(card);
  245 |       const cancelButton = card.getByRole('button', { name: /Cancel Entry/ });
  246 |       if (await cancelButton.isVisible().catch(() => false)) return card;
  247 |     }
  248 |     return null;
  249 |   }
  250 | 
  251 |   /**
  252 |    * A freshly-placed entry sorts to the *end* of the Active list, so it lands
  253 |    * on the last page — jump there and walk backwards. The matched card is
  254 |    * left expanded on its page.
  255 |    */
  256 |   async findCancellableCard(): Promise<Locator | null> {
  257 |     if (!(await this.nextArrow.isVisible().catch(() => false))) {
  258 |       return await this.findCancellableCardOnCurrentPage();
  259 |     }
  260 | 
  261 |     // Walk forward without expanding anything (cheap), then scan backwards.
  262 |     const canGoNext = async () =>
  263 |       (await this.nextArrow.isVisible().catch(() => false)) &&
  264 |       !(await this.nextArrow.isDisabled().catch(() => true));
  265 |     while (await canGoNext()) {
  266 |       await this.nextArrow.click();
  267 |       await this.cardDivs.first().waitFor({ state: 'visible' });
```