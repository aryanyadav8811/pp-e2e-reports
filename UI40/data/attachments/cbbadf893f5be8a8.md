# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: entries/entries.spec.ts >> User entries >> Navigating to last page then switching dropdown resets view and verify data
- Location: tests/entries/entries.spec.ts:249:5

# Error details

```
Error: expect(locator).toBeVisible() failed

Locator: getByAltText('Parlay Play text').filter({ visible: true }).first()
Expected: visible
Timeout: 15000ms
Error: element(s) not found

Call log:
  - Expect "toBeVisible" with timeout 15000ms
  - waiting for getByAltText('Parlay Play text').filter({ visible: true }).first()

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
          - generic [ref=e10]:
            - generic [ref=e12]:
              - generic [ref=e13]: $465.89
              - generic [ref=e14]:
                - img "gift-icon" [ref=e15]
                - text: "8.00"
            - button "Toggle Menu" [ref=e16]:
              - img [ref=e17]
      - main [ref=e19]:
        - generic [ref=e22]:
          - navigation [ref=e23]:
            - list [ref=e24]:
              - listitem [ref=e25]:
                - button "Active" [ref=e26]
              - listitem [ref=e27]:
                - button "History" [ref=e28]
          - generic [ref=e29]:
            - generic [ref=e31]:
              - generic [ref=e32]:
                - generic [ref=e33]: $30
                - generic [ref=e34]: Entry Amount
              - img "chest-icon" [ref=e35]
              - generic [ref=e36]:
                - generic [ref=e37]: $368.07
                - generic [ref=e38]: Max Payout
            - generic [ref=e39]:
              - region [ref=e40]:
                - button "Expand entry details" [ref=e41]:
                  - generic [ref=e43]:
                    - generic [ref=e45]:
                      - text: $3
                      - generic [ref=e46]: for $53.04
                    - generic [ref=e47]: All In 17.68x
                  - generic [ref=e48]:
                    - generic [ref=e50]: "1"
                    - generic [ref=e52]: "2"
                    - generic [ref=e54]: "3"
                    - generic [ref=e56]: "4"
                - button "Expand entry details" [ref=e60]:
                  - img "Expand" [ref=e61]
              - region [ref=e62]:
                - button "Expand entry details" [ref=e63]:
                  - generic [ref=e65]:
                    - generic [ref=e67]:
                      - text: $3
                      - generic [ref=e68]: for $53.04
                    - generic [ref=e69]: All In 17.68x
                  - generic [ref=e70]:
                    - generic [ref=e72]: "1"
                    - generic [ref=e74]: "2"
                    - generic [ref=e76]: "3"
                    - generic [ref=e78]: "4"
                - button "Expand entry details" [ref=e82]:
                  - img "Expand" [ref=e83]
              - region [ref=e84]:
                - button "Expand entry details" [ref=e85]:
                  - generic [ref=e87]:
                    - generic [ref=e89]:
                      - text: $3
                      - generic [ref=e90]: for $53.04
                    - generic [ref=e91]: All In 17.68x
                  - generic [ref=e92]:
                    - generic [ref=e94]: "1"
                    - generic [ref=e96]: "2"
                    - generic [ref=e98]: "3"
                    - generic [ref=e100]: "4"
                - button "Expand entry details" [ref=e104]:
                  - img "Expand" [ref=e105]
              - region [ref=e106]:
                - button "Expand entry details" [ref=e107]:
                  - generic [ref=e109]:
                    - generic [ref=e111]:
                      - text: $3
                      - generic [ref=e112]: for $68.4
                    - generic [ref=e113]: All In 22.8x
                - generic [ref=e121]:
                  - button "Share entry" [ref=e122]:
                    - img "share" [ref=e123]
                  - button "Expand entry details" [ref=e124]:
                    - img "Expand" [ref=e125]
              - region [ref=e126]:
                - button "Expand entry details" [ref=e127]:
                  - generic [ref=e129]:
                    - generic [ref=e131]:
                      - text: $3
                      - generic [ref=e132]: for $14.43
                    - generic [ref=e133]: All In 4.81x
                - generic [ref=e139]:
                  - button "Share entry" [ref=e140]:
                    - img "share" [ref=e141]
                  - button "Expand entry details" [ref=e142]:
                    - img "Expand" [ref=e143]
              - region [ref=e144]:
                - button "Expand entry details" [ref=e145]:
                  - generic [ref=e147]:
                    - generic [ref=e149]:
                      - text: $3
                      - generic [ref=e150]: for $14.43
                    - generic [ref=e151]: All In 4.81x
                - generic [ref=e157]:
                  - button "Share entry" [ref=e158]:
                    - img "share" [ref=e159]
                  - button "Expand entry details" [ref=e160]:
                    - img "Expand" [ref=e161]
              - region [ref=e162]:
                - button "Expand entry details" [ref=e163]:
                  - generic [ref=e165]:
                    - generic [ref=e167]:
                      - text: $3
                      - generic [ref=e168]: for $14.43
                    - generic [ref=e169]: All In 4.81x
                - generic [ref=e175]:
                  - button "Share entry" [ref=e176]:
                    - img "share" [ref=e177]
                  - button "Expand entry details" [ref=e178]:
                    - img "Expand" [ref=e179]
              - region [ref=e180]:
                - button "Expand entry details" [ref=e181]:
                  - generic [ref=e183]:
                    - generic [ref=e185]:
                      - text: $3
                      - generic [ref=e186]: for $68.4
                    - generic [ref=e187]: All In 22.8x
                - generic [ref=e195]:
                  - button "Share entry" [ref=e196]:
                    - img "share" [ref=e197]
                  - button "Expand entry details" [ref=e198]:
                    - img "Expand" [ref=e199]
              - region [ref=e200]:
                - button "Expand entry details" [ref=e201]:
                  - generic [ref=e203]:
                    - generic [ref=e205]:
                      - text: $3
                      - generic [ref=e206]: for $14.43
                    - generic [ref=e207]: All In 4.81x
                - generic [ref=e213]:
                  - button "Share entry" [ref=e214]:
                    - img "share" [ref=e215]
                  - button "Expand entry details" [ref=e216]:
                    - img "Expand" [ref=e217]
              - region [ref=e218]:
                - button "Expand entry details" [ref=e219]:
                  - generic [ref=e221]:
                    - generic [ref=e223]:
                      - text: $3
                      - generic [ref=e224]: for $14.43
                    - generic [ref=e225]: All In 4.81x
                - generic [ref=e231]:
                  - button "Share entry" [ref=e232]:
                    - img "share" [ref=e233]
                  - button "Expand entry details" [ref=e234]:
                    - img "Expand" [ref=e235]
      - contentinfo [ref=e236]:
        - navigation [ref=e237]:
          - list [ref=e238]:
            - listitem [ref=e239]:
              - button "Home" [ref=e240] [cursor=pointer]:
                - generic [ref=e241]:
                  - img [ref=e242]
                  - generic [ref=e243]: Home
            - listitem [ref=e244]:
              - button "Entries 10" [active] [ref=e245] [cursor=pointer]:
                - generic [ref=e246]:
                  - img [ref=e247]
                  - generic [ref=e248]: Entries
                - generic [ref=e249]: "10"
            - listitem [ref=e250]:
              - button "Feed" [ref=e251] [cursor=pointer]:
                - generic [ref=e252]:
                  - img [ref=e253]
                  - generic [ref=e254]: Feed
            - listitem [ref=e255]:
              - button "Rewards 8" [ref=e256] [cursor=pointer]:
                - generic [ref=e257]:
                  - img [ref=e258]
                  - generic [ref=e259]: Rewards
                - generic [ref=e260]: "8"
            - listitem [ref=e261]:
              - button "Packs" [ref=e262] [cursor=pointer]:
                - generic [ref=e263]:
                  - img [ref=e264]
                  - generic [ref=e265]: Packs
    - region "Notifications Alt+T"
  - alert [ref=e266]: ParlayPlay | Fun Fantasy Sports - My Entries
  - iframe [ref=e267]:
    
```

# Test source

```ts
  1  | // base page to collect all common helpers for interacting the pages, will be extended by all other pages
  2  | 
  3  | import { type Page, expect, type Locator } from "@playwright/test";
  4  | 
  5  | export class BasePage {
  6  |   protected readonly page: Page;
  7  |   readonly homeLink: Locator;
  8  | 
  9  |   constructor(page: Page) {
  10 |     this.page = page;
  11 |     this.homeLink = this.locator('a[href="/"]');
  12 |   }
  13 | 
  14 |   async clickHomeLink(): Promise<void> {
  15 |     await this.homeLink.click();
  16 |   }
  17 | 
  18 |   async open(pathname: string = "/"): Promise<void> {
  19 |     await this.page.goto(pathname);
  20 |   }
  21 | 
  22 |   /**
  23 |    * Takes any locator and returns a strict-safe version:
  24 |    * filters to visible elements, then picks the first match.
  25 |    * Use on ad-hoc or chained locators that may resolve to multiple elements.
  26 |    */
  27 |   visible(locator: Locator): Locator {
  28 |     return locator.filter({ visible: true }).first();
  29 |   }
  30 | 
  31 |   locator(selector: string, options?: Parameters<Page["locator"]>[1]): Locator {
  32 |     return this.visible(this.page.locator(selector, options));
  33 |   }
  34 | 
  35 |   byRole(
  36 |     role: Parameters<Page["getByRole"]>[0],
  37 |     options?: Parameters<Page["getByRole"]>[1]
  38 |   ): Locator {
  39 |     return this.visible(this.page.getByRole(role, options));
  40 |   }
  41 | 
  42 |   byText(
  43 |     text: string | RegExp,
  44 |     options?: Parameters<Page["getByText"]>[1]
  45 |   ): Locator {
  46 |     return this.visible(this.page.getByText(text, options));
  47 |   }
  48 | 
  49 |   byTestId(testId: string | RegExp): Locator {
  50 |     return this.visible(this.page.getByTestId(testId));
  51 |   }
  52 | 
  53 |   byLabel(
  54 |     label: string | RegExp,
  55 |     options?: Parameters<Page["getByLabel"]>[1]
  56 |   ): Locator {
  57 |     return this.visible(this.page.getByLabel(label, options));
  58 |   }
  59 | 
  60 |   byAltText(
  61 |     text: string | RegExp,
  62 |     options?: Parameters<Page["getByAltText"]>[1]
  63 |   ): Locator {
  64 |     return this.visible(this.page.getByAltText(text, options));
  65 |   }
  66 | 
  67 |   byPlaceholder(
  68 |     text: string | RegExp,
  69 |     options?: Parameters<Page["getByPlaceholder"]>[1]
  70 |   ): Locator {
  71 |     return this.visible(this.page.getByPlaceholder(text, options));
  72 |   }
  73 | 
  74 |   async assertReady(): Promise<void> {
  75 |     //Filter to the visible copy and take the first match.
  76 |     await expect(
  77 |       this.page
  78 |         .getByAltText("Parlay Play text")
  79 |         .filter({ visible: true })
  80 |         .first()
> 81 |     ).toBeVisible();
     |       ^ Error: expect(locator).toBeVisible() failed
  82 |   }
  83 | }
  84 | 
```