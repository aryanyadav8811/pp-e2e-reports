# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: rewards/partner-rewards.spec.ts >> Partner Rewards (DFS-1602 / DFS-1604) >> An available offer exposes an enabled CTA
- Location: tests/rewards/partner-rewards.spec.ts:83:5

# Error details

```
Error: locator.waitFor: Error: strict mode violation: getByTestId('partner-rewards-empty') resolved to 2 elements:
    1) <div data-testid="partner-rewards-empty" class="flex flex-col justify-center text-textPrimary items-center text-center">…</div> aka locator('#whiteContainer').getByTestId('partner-rewards-empty')
    2) <div data-testid="partner-rewards-empty" class="flex flex-col justify-center text-textPrimary items-center text-center">…</div> aka getByTestId('partner-rewards-empty').nth(1)

Call log:
  - waiting for getByTestId('partner-rewards-empty') to be visible

```

# Page snapshot

```yaml
- generic [active] [ref=e1]:
  - generic [ref=e2]:
    - generic [ref=e3]:
      - banner [ref=e4]:
        - navigation [ref=e5]:
          - link "Parlay Play LogoParlay Play text" [ref=e6] [cursor=pointer]:
            - /url: /
            - generic [ref=e7]:
              - img "Parlay Play Logo" [ref=e8]
              - img "Parlay Play text" [ref=e9]
          - generic [ref=e10]:
            - button "Switch to dark mode" [ref=e11]:
              - img [ref=e12]
            - generic [ref=e14]:
              - generic [ref=e17]: $992.58
              - button "Toggle Menu" [ref=e18]:
                - img [ref=e19]
      - main [ref=e21]:
        - generic [ref=e24]:
          - navigation [ref=e25]:
            - list [ref=e26]:
              - listitem [ref=e27]:
                - button "Partner Rewards" [ref=e28]
              - listitem [ref=e29]:
                - button "Promotions" [ref=e30]
          - generic [ref=e32]:
            - img "no-promotions-icon" [ref=e34]
            - paragraph [ref=e35]: No available partner rewards at the moment.
            - paragraph [ref=e36]: Check back soon for new offers!
            - button "Make your pick!" [ref=e37] [cursor=pointer]
      - contentinfo [ref=e38]:
        - navigation [ref=e39]:
          - list [ref=e40]:
            - listitem [ref=e41]:
              - button "Home" [ref=e42] [cursor=pointer]:
                - generic [ref=e43]:
                  - img [ref=e44]
                  - generic [ref=e45]: Home
            - listitem [ref=e46]:
              - button "Entries 168" [ref=e47] [cursor=pointer]:
                - generic [ref=e48]:
                  - img [ref=e49]
                  - generic [ref=e50]: Entries
                - generic [ref=e51]: "168"
            - listitem [ref=e52]:
              - button "Feed" [ref=e53] [cursor=pointer]:
                - generic [ref=e54]:
                  - img [ref=e55]
                  - generic [ref=e56]: Feed
            - listitem [ref=e57]:
              - button "Rewards" [ref=e58] [cursor=pointer]:
                - generic [ref=e59]:
                  - img [ref=e60]
                  - generic [ref=e61]: Rewards
            - listitem [ref=e62]:
              - button "Packs" [ref=e63] [cursor=pointer]:
                - generic [ref=e64]:
                  - img [ref=e65]
                  - generic [ref=e66]: Packs
    - region "Notifications Alt+T"
  - alert [ref=e67]
```

# Test source

```ts
  1  | import { Locator, Page, expect } from "@playwright/test";
  2  | import { BasePage } from "./base.page";
  3  | 
  4  | export class RewardsPage extends BasePage {
  5  |   readonly promotionsTab = this.byRole("button", { name: "Promotions" });
  6  |   readonly promoCards = this.page.locator('[data-testid="promotion-card"]');
  7  |   readonly makeYourPickBtn = this.byRole("button", { name: "Make your pick!" });
  8  |   readonly firstPromoUseButton = this.locator(
  9  |     'button:has(span:text-is("Use"))'
  10 |   );
  11 |   readonly enterContestBtn = this.byRole("button", { name: "Enter Contest" });
  12 | 
  13 |   // ---- Partner Rewards (DFS-1602 / DFS-1604) ----
  14 |   // The default /rewards tab now lists PartnerRewardCard offers from
  15 |   // GET /rewards/partner-rewards/. Each card is an <article> with a stable
  16 |   // data-testid + data-state; the list shows a dedicated empty state instead.
  17 |   readonly partnerTab = this.byRole("button", { name: "Partner Rewards" });
  18 |   readonly partnerCards = this.page.locator(
  19 |     'article[data-testid^="partner-reward-card-"]'
  20 |   );
  21 |   readonly partnerEmptyState = this.byTestId("partner-rewards-empty");
  22 | 
  23 |   constructor(page: Page) {
  24 |     super(page);
  25 |   }
  26 | 
  27 |   async enterPromotions(): Promise<void> {
  28 |     await this.promotionsTab.click();
  29 |   }
  30 | 
  31 |   /**
  32 |    * Waits until the partner-rewards list has settled — either the first offer
  33 |    * card or the empty state is visible. Mirrors the Active-entries readiness
  34 |    * pattern so data-dependent specs don't assert against a still-loading page.
  35 |    */
  36 |   async waitForPartnerRewardsReady(timeout = 15_000): Promise<void> {
  37 |     await Promise.race([
  38 |       this.partnerCards.first().waitFor({ state: "visible", timeout }),
  39 |       this.page
  40 |         .getByTestId("partner-rewards-empty")
> 41 |         .waitFor({ state: "visible", timeout }),
     |          ^ Error: locator.waitFor: Error: strict mode violation: getByTestId('partner-rewards-empty') resolved to 2 elements:
  42 |     ]);
  43 |   }
  44 | 
  45 |   async isPartnerRewardsEmpty(): Promise<boolean> {
  46 |     return this.partnerEmptyState.isVisible().catch(() => false);
  47 |   }
  48 | 
  49 |   /** Returns each visible card's `data-state` in DOM order. */
  50 |   async getPartnerCardStates(): Promise<string[]> {
  51 |     const count = await this.partnerCards.count();
  52 |     const states: string[] = [];
  53 |     for (let i = 0; i < count; i++) {
  54 |       states.push((await this.partnerCards.nth(i).getAttribute("data-state")) ?? "");
  55 |     }
  56 |     return states;
  57 |   }
  58 | 
  59 |   /** First card in a given state (e.g. "claimed", "available"), or a 0-match locator. */
  60 |   partnerCardInState(state: string): Locator {
  61 |     return this.page
  62 |       .locator(`article[data-testid^="partner-reward-card-"][data-state="${state}"]`)
  63 |       .first();
  64 |   }
  65 | 
  66 |   async verifyPromotionsAvailable(): Promise<void> {
  67 |     await expect(this.firstPromoUseButton).toBeVisible();
  68 |   }
  69 | 
  70 |   async usePromo(): Promise<void> {
  71 |     await this.firstPromoUseButton.click();
  72 |   }
  73 | 
  74 |   async verifyPromoSelected(): Promise<void> {
  75 |     const classes =
  76 |       (await this.firstPromoUseButton.getAttribute("class")) ?? "";
  77 |     expect(classes).toContain("playYellow");
  78 |   }
  79 | 
  80 |   async verifyPromoNotSelected(): Promise<void> {
  81 |     const classes =
  82 |       (await this.firstPromoUseButton.getAttribute("class")) ?? "";
  83 |     expect(classes).not.toContain("playYellow");
  84 |   }
  85 | 
  86 |   async isPromoSelected(): Promise<boolean> {
  87 |     const classes =
  88 |       (await this.firstPromoUseButton.getAttribute("class")) ?? "";
  89 |     return classes.includes("playYellow");
  90 |   }
  91 | }
  92 | 
```