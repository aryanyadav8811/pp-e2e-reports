# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: rewards/partner-rewards.spec.ts >> Rewards - Partner Rewards >> Partner offer cards render, or the empty state when none are available
- Location: tests/rewards/partner-rewards.spec.ts:38:3

# Error details

```
TimeoutError: locator.waitFor: Timeout 15000ms exceeded.
Call log:
  - waiting for locator('article[data-testid^="partner-reward-card-"]').first() to be visible
    19 × locator resolved to hidden <article data-state="available" data-testid="partner-reward-card-clash5" class="flex flex-col w-full rounded-2xl border border-borderPrimary shadow-sm p-5 gap-4 cursor-pointer">…</article>

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
              - generic [ref=e13]: $667.77
              - generic [ref=e14]:
                - img "gift-icon" [ref=e15]
                - text: "9.00"
            - button "Toggle Menu" [ref=e16]:
              - img [ref=e17]
      - main [ref=e19]:
        - generic [ref=e22]:
          - navigation [ref=e23]:
            - list [ref=e24]:
              - listitem [ref=e25]:
                - button "Partner Rewards 1" [ref=e26]:
                  - text: Partner Rewards
                  - generic [ref=e27]: "1"
              - listitem [ref=e28]:
                - button "Promotions 9" [ref=e29]:
                  - text: Promotions
                  - generic [ref=e30]: "9"
          - generic [ref=e32]:
            - article [ref=e33] [cursor=pointer]:
              - generic [ref=e34]:
                - generic [ref=e35]:
                  - generic [ref=e36]:
                    - generic [ref=e37]: Clash5
                    - heading "$9 in Rewards" [level=3] [ref=e38]
                  - img "Clash5 logo" [ref=e39]
                - generic [ref=e40]: $4 on ParlayPlay + $5 on Clash5
              - paragraph [ref=e41]: Your first battle awaits. Collect powerful cards, battle real players, and enjoy casino-style games as you climb the ranks in Clash5.
              - button "Claim Free $9 Now" [ref=e42]
            - article [ref=e43] [cursor=pointer]:
              - generic [ref=e44]:
                - generic [ref=e45]:
                  - generic [ref=e46]:
                    - generic [ref=e47]: Stake
                    - heading "$10 Free Entry + $40 Stake Cash" [level=3] [ref=e48]
                  - img "Stake logo" [ref=e49]
                - generic [ref=e50]: $50 in rewards with $20 purchase
              - paragraph [ref=e51]: Start playing casino games with fast, seamless gameplay.
              - button "Claim $50" [ref=e52]
            - article [ref=e53] [cursor=pointer]:
              - generic [ref=e54]:
                - generic [ref=e55]:
                  - generic [ref=e56]:
                    - generic [ref=e57]: WOW Vegas
                    - heading "$35 Free Sweeps Coins" [level=3] [ref=e58]
                  - img "WOW Vegas logo" [ref=e59]
                - generic [ref=e60]: Get $35 in rewards with your first $10 purchase
              - paragraph [ref=e61]: Make your first purchase to unlock rewards and more play. Enjoy top social casino games and daily bonuses.
              - button "Claim $35" [ref=e62]
            - article [ref=e63] [cursor=pointer]:
              - generic [ref=e64]:
                - generic [ref=e65]:
                  - generic [ref=e66]:
                    - generic [ref=e67]: SpinPals
                    - heading "$9 in Rewards" [level=3] [ref=e68]
                  - img "SpinPals logo" [ref=e69]
                - generic [ref=e70]: $3 on ParlayPlay + $6 on SpinPals
              - paragraph [ref=e71]: Join the fun with SpinPals and unlock 5% cash back on all eligible activity through our Partner Rewards Promotion!
              - button "Unlock Rewards" [ref=e72]
      - contentinfo [ref=e73]:
        - navigation [ref=e74]:
          - list [ref=e75]:
            - listitem [ref=e76]:
              - button "Home" [ref=e77] [cursor=pointer]:
                - generic [ref=e78]:
                  - img [ref=e79]
                  - generic [ref=e80]: Home
            - listitem [ref=e81]:
              - button "Entries 150" [ref=e82] [cursor=pointer]:
                - generic [ref=e83]:
                  - img [ref=e84]
                  - generic [ref=e85]: Entries
                - generic [ref=e86]: "150"
            - listitem [ref=e87]:
              - button "Feed" [ref=e88] [cursor=pointer]:
                - generic [ref=e89]:
                  - img [ref=e90]
                  - generic [ref=e91]: Feed
            - listitem [ref=e92]:
              - button "Rewards 10" [ref=e93] [cursor=pointer]:
                - generic [ref=e94]:
                  - img [ref=e95]
                  - generic [ref=e96]: Rewards
                - generic [ref=e97]: "10"
            - listitem [ref=e98]:
              - button "Packs" [ref=e99] [cursor=pointer]:
                - generic [ref=e100]:
                  - img [ref=e101]
                  - generic [ref=e102]: Packs
    - generic:
      - region "Notifications Alt+T"
  - alert [ref=e103]
```

# Test source

```ts
  1  | import { Locator, Page, expect } from '@playwright/test';
  2  | import { BasePage } from './base.page';
  3  | 
  4  | export class RewardsPage extends BasePage {
  5  |   readonly promotionsTab = this.byRole('button', { name: 'Promotions' });
  6  |   readonly promoCards = this.page.locator('[data-testid="promotion-card"]');
  7  |   readonly makeYourPickBtn = this.byRole('button', { name: 'Make your pick!' });
  8  |   readonly firstPromoUseButton = this.locator('button:has(span:text-is("Use"))');
  9  |   readonly enterContestBtn = this.byRole('button', { name: 'Enter Contest' });
  10 | 
  11 |   readonly partnerTab = this.byRole('button', { name: 'Partner Rewards' });
  12 |   readonly partnerCards = this.page.locator('article[data-testid^="partner-reward-card-"]');
  13 |   readonly partnerEmptyState = this.byTestId('partner-rewards-empty');
  14 | 
  15 |   constructor(page: Page) {
  16 |     super(page);
  17 |   }
  18 | 
  19 |   async enterPromotions(): Promise<void> {
  20 |     await this.promotionsTab.click();
  21 |   }
  22 | 
  23 |   async waitForPartnerRewardsReady(timeout = 15_000): Promise<void> {
  24 |     // partnerEmptyState goes through byTestId (visible-filtered + first) — the
  25 |     // raw testid resolves to 2 nodes (mobile + desktop) and trips strict mode.
  26 |     await Promise.race([
> 27 |       this.partnerCards.first().waitFor({ state: 'visible', timeout }),
     |                                 ^ TimeoutError: locator.waitFor: Timeout 15000ms exceeded.
  28 |       this.partnerEmptyState.waitFor({ state: 'visible', timeout }),
  29 |     ]);
  30 |   }
  31 | 
  32 |   async isPartnerRewardsEmpty(): Promise<boolean> {
  33 |     return this.partnerEmptyState.isVisible().catch(() => false);
  34 |   }
  35 | 
  36 |   async getPartnerCardStates(): Promise<string[]> {
  37 |     const count = await this.partnerCards.count();
  38 |     const states: string[] = [];
  39 |     for (let i = 0; i < count; i++) {
  40 |       states.push((await this.partnerCards.nth(i).getAttribute('data-state')) ?? '');
  41 |     }
  42 |     return states;
  43 |   }
  44 | 
  45 |   partnerCardInState(state: string): Locator {
  46 |     return this.page
  47 |       .locator(`article[data-testid^="partner-reward-card-"][data-state="${state}"]`)
  48 |       .first();
  49 |   }
  50 | 
  51 |   async verifyPromotionsAvailable(): Promise<void> {
  52 |     await expect(this.firstPromoUseButton).toBeVisible();
  53 |   }
  54 | 
  55 |   async usePromo(): Promise<void> {
  56 |     await this.firstPromoUseButton.click();
  57 |   }
  58 | 
  59 |   async verifyPromoSelected(): Promise<void> {
  60 |     const classes = (await this.firstPromoUseButton.getAttribute('class')) ?? '';
  61 |     expect(classes).toContain('playYellow');
  62 |   }
  63 | 
  64 |   async verifyPromoNotSelected(): Promise<void> {
  65 |     const classes = (await this.firstPromoUseButton.getAttribute('class')) ?? '';
  66 |     expect(classes).not.toContain('playYellow');
  67 |   }
  68 | 
  69 |   async isPromoSelected(): Promise<boolean> {
  70 |     const classes = (await this.firstPromoUseButton.getAttribute('class')) ?? '';
  71 |     return classes.includes('playYellow');
  72 |   }
  73 | }
  74 | 
```