# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: slip_sharing/tail_feed.spec.ts >> Tail Feed >> Share toggle ON — newly-placed contest appears on You tab and Tail Entry tails it
- Location: tests/slip_sharing/tail_feed.spec.ts:177:5

# Error details

```
Error: expect(locator).toBeVisible() failed

Locator: getByTestId('feed-card').filter({ visible: true }).first()
Expected: visible
Timeout: 15000ms
Error: element(s) not found

Call log:
  - Expect "toBeVisible" with timeout 15000ms
  - waiting for getByTestId('feed-card').filter({ visible: true }).first()

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
                - link "Rewards 51" [ref=e24] [cursor=pointer]:
                  - /url: /rewards
                  - generic [ref=e25]:
                    - generic [ref=e26]: Rewards
                    - generic [ref=e27]: "51"
              - listitem [ref=e28]:
                - link "Track Picks 59" [ref=e29] [cursor=pointer]:
                  - /url: /challenges/pending
                  - generic [ref=e30]:
                    - generic [ref=e31]: Track Picks
                    - generic [ref=e32]: "59"
            - button "Claim your $100 Deposit Match" [ref=e33] [cursor=pointer]
            - generic [ref=e34]:
              - generic [ref=e36]:
                - generic [ref=e37]: $861.00
                - generic [ref=e38]:
                  - img "gift-icon" [ref=e39]
                  - text: "51.00"
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
          - generic [ref=e79]:
            - img "warning icon" [ref=e80]
            - paragraph [ref=e81]: Something Went Wrong
            - paragraph [ref=e82]:
              - text: Sorry an unexpected error occurred!
              - text: Our team has been notified.
            - paragraph [ref=e83]:
              - text: If you require additional support please
              - button "contact us" [ref=e84] [cursor=pointer]
              - text: .
          - generic [ref=e87]:
            - generic [ref=e88]:
              - link "Parlay Play Logo" [ref=e89] [cursor=pointer]:
                - /url: /
                - img "Parlay Play Logo" [ref=e91]
              - generic [ref=e92]:
                - generic [ref=e93]: Improve your experience. Download our app.
                - generic [ref=e94]:
                  - link "Apple Store" [ref=e95] [cursor=pointer]:
                    - /url: https://parlayplay.onelink.me/oLJk/gnqpwjha
                    - img "Apple Store" [ref=e96]
                  - link "Google Play Store" [ref=e97] [cursor=pointer]:
                    - /url: https://parlayplay.onelink.me/oLJk/fh7u6juo
                    - img "Google Play Store" [ref=e98]
            - generic [ref=e99]:
              - link "Privacy" [ref=e100] [cursor=pointer]:
                - /url: /privacy-policy
              - link "Fantasy Terms" [ref=e101] [cursor=pointer]:
                - /url: /terms
              - link "Packs Terms" [ref=e102] [cursor=pointer]:
                - /url: /terms/packs
              - link "Responsible Gaming" [ref=e103] [cursor=pointer]:
                - /url: /responsible-gaming
              - link "Gaming Rules" [ref=e104] [cursor=pointer]:
                - /url: /rules
              - link "FAQ" [ref=e105] [cursor=pointer]:
                - /url: https://intercom.help/parlayplay/en/
              - link "Contact Us" [ref=e106] [cursor=pointer]:
                - /url: /
              - paragraph [ref=e107]: © ParlayPlay 2026 - All Rights Reserved
            - list [ref=e108]:
              - listitem [ref=e109]:
                - generic [ref=e110]:
                  - log [ref=e112]
                  - generic [ref=e113]:
                    - generic [ref=e114]:
                      - generic [ref=e115]: 🇺🇸English
                      - combobox "Select language" [ref=e116]
                    - img [ref=e120]
              - listitem [ref=e122]:
                - img "18+-icon" [ref=e123]
              - listitem [ref=e124]:
                - link "ParlayPlay on Twitter" [ref=e125] [cursor=pointer]:
                  - /url: https://twitter.com/parlay_play?lang=en
                  - img [ref=e126]
              - listitem [ref=e128]:
                - link "ParlayPlay on Facebook" [ref=e129] [cursor=pointer]:
                  - /url: https://www.facebook.com/ParlayPlay.io/
                  - img [ref=e130]
              - listitem [ref=e132]:
                - link "ParlayPlay on Instagram" [ref=e133] [cursor=pointer]:
                  - /url: https://www.instagram.com/parlayplay_?igsh=bHBldWQyMmV2b3Y4
                  - img [ref=e134]
              - listitem [ref=e136]:
                - link "ParlayPlay on Discord" [ref=e137] [cursor=pointer]:
                  - /url: https://discord.com/invite/parlayplay
                  - img [ref=e138]
    - generic:
      - region "Notifications Alt+T"
  - iframe [ref=e140]:
    
  - button "Open Intercom Messenger" [ref=e141] [cursor=pointer]:
    - img [ref=e143]
    - generic:
      - img
  - alert [ref=e145]
```

# Test source

```ts
  44  | 
  45  |     // Empty-state copy comes from public/locales/en/common.json under "feed.empty".
  46  |     this.forYouEmptyTitle = this.byText(/check back soon/i);
  47  |     this.followingEmptyTitle = this.byText(/build your following feed/i);
  48  |     this.youEmptyTitle = this.byText(/no entries yet/i);
  49  |   }
  50  | 
  51  |   async open(initialTab?: FeedTab): Promise<void> {
  52  |     // The page itself initialises `tab` from useState("for_you"); we can't
  53  |     // deep-link via URL today. Open and then call `switchTab` if needed.
  54  |     await this.page.goto("/challenges/feed");
  55  |     if (initialTab && initialTab !== "for_you") {
  56  |       await this.switchTab(initialTab);
  57  |     } else {
  58  |       await this.waitForFeedResponse("for_you").catch(() => undefined);
  59  |     }
  60  |   }
  61  | 
  62  |   /**
  63  |    * Wait for a successful GET /api/v1/feed/entries/?tab=<tab> response.
  64  |    * Returns the parsed JSON envelope so callers can inspect `results`.
  65  |    */
  66  |   async waitForFeedResponse(tab: FeedTab, timeout = 30_000): Promise<{
  67  |     results: Array<{ id: number; contestUuid: string }>;
  68  |     nextCursor: string | null;
  69  |     hasFollowing: boolean;
  70  |   }> {
  71  |     const resp: Response = await this.page.waitForResponse(
  72  |       (r) => {
  73  |         const url = new URL(r.url());
  74  |         return (
  75  |           FEED_ENTRIES_PATH.test(url.pathname) &&
  76  |           url.searchParams.get("tab") === tab &&
  77  |           r.request().method() === "GET" &&
  78  |           r.status() === 200
  79  |         );
  80  |       },
  81  |       { timeout },
  82  |     );
  83  |     return resp.json();
  84  |   }
  85  | 
  86  |   async switchTab(tab: FeedTab): Promise<{
  87  |     results: Array<{ id: number; contestUuid: string }>;
  88  |     nextCursor: string | null;
  89  |     hasFollowing: boolean;
  90  |   } | null> {
  91  |     const target =
  92  |       tab === "for_you"
  93  |         ? this.forYouTab
  94  |         : tab === "following"
  95  |           ? this.followingTab
  96  |           : this.youTab;
  97  | 
  98  |     // The hook keeps a per-(tab,category) cache slot. A second visit within
  99  |     // CACHE_STALE_MS reads from cache without firing a new request — race a
  100 |     // response against a short timeout so we proceed either way.
  101 |     const respPromise = this.waitForFeedResponse(tab, 10_000).catch(() => null);
  102 |     await target.click();
  103 |     return respPromise;
  104 |   }
  105 | 
  106 |   /**
  107 |    * Reads the You-tab feed and returns true iff any returned entry has
  108 |    * `contestUuid === uuid`. Uses the network envelope rather than DOM
  109 |    * scraping because the FeedCard doesn't expose the uuid in markup.
  110 |    */
  111 |   async youTabContainsContestUuid(uuid: string): Promise<boolean> {
  112 |     const envelope = await this.waitForFeedResponse("my_entries");
  113 |     return envelope.results.some((e) => e.contestUuid === uuid);
  114 |   }
  115 | 
  116 |   async assertForYouEmpty(): Promise<void> {
  117 |     await expect(this.forYouEmptyTitle).toBeVisible();
  118 |     await expect(this.feedCards).toHaveCount(0);
  119 |   }
  120 | 
  121 |   /**
  122 |    * Looser variant for environments where other-user entries may already
  123 |    * exist: the For You tab is up either way as long as we see the empty
  124 |    * hero OR at least one card. Pairs with the network-level 200 check the
  125 |    * caller does via `waitForFeedResponse('for_you')`.
  126 |    */
  127 |   async assertForYouRendered(): Promise<void> {
  128 |     const hasEmpty = await this.forYouEmptyTitle
  129 |       .isVisible({ timeout: 5_000 })
  130 |       .catch(() => false);
  131 |     if (hasEmpty) {
  132 |       await expect(this.feedCards).toHaveCount(0);
  133 |       return;
  134 |     }
  135 |     await expect(this.feedCards.first()).toBeVisible({ timeout: 15_000 });
  136 |   }
  137 | 
  138 |   async assertFollowingEmpty(): Promise<void> {
  139 |     await expect(this.followingEmptyTitle).toBeVisible();
  140 |     await expect(this.feedCards).toHaveCount(0);
  141 |   }
  142 | 
  143 |   async assertYouHasAtLeastOneCard(): Promise<void> {
> 144 |     await expect(this.feedCards.first()).toBeVisible();
      |                                          ^ Error: expect(locator).toBeVisible() failed
  145 |   }
  146 | 
  147 |   async tailFirstCard(): Promise<void> {
  148 |     await expect(this.firstCardTailBtn).toBeVisible();
  149 |     await this.firstCardTailBtn.click();
  150 |   }
  151 | }
  152 | 
```