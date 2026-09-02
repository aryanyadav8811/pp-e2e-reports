# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: data_verification/entries-history.spec.ts >> History entries data verification >> history cards and summary render the history API data
- Location: tests/data_verification/entries-history.spec.ts:51:3

# Error details

```
TimeoutError: page.waitForResponse: Timeout 45000ms exceeded while waiting for event "response"
```

# Page snapshot

```yaml
- generic [active] [ref=e1]:
  - main [ref=e2]:
    - generic [ref=e3]:
      - heading "staging.parlayplay.io" [level=1] [ref=e5]
      - heading "Performing security verification" [level=2] [ref=e6]
      - paragraph [ref=e7]: This website uses a security service to protect against malicious bots. This page is displayed while the website verifies you are not a bot.
  - contentinfo [ref=e12]:
    - generic [ref=e14]:
      - generic [ref=e16]:
        - text: "Ray ID:"
        - code [ref=e17]: a30b172f0ccc90f3
      - generic [ref=e18]:
        - generic [ref=e19]:
          - text: Performance and Security by
          - link "Cloudflare, opens in a new tab" [ref=e20] [cursor=pointer]:
            - /url: https://www.cloudflare.com?utm_source=challenge&utm_campaign=m
            - text: Cloudflare
        - link "Privacy, opens in a new tab" [ref=e22] [cursor=pointer]:
          - /url: https://www.cloudflare.com/privacypolicy/
          - text: Privacy
```

# Test source

```ts
  1   | /*
  2   |  Data-verification suite: the History entries page (/challenges/history) must
  3   |  render exactly what GET /api/v1/entries/history-paged/ and
  4   |  /entries/history-summary/ return.
  5   | 
  6   |  Checks: card list matches the API page (ids, order), each card header shows
  7   |  the API amount + result-specific payout line ("paid $X" for won, "To win $X"
  8   |  for lost/cancelled) + result badge, and the summary tiles equal the summary
  9   |  endpoint field-for-field with the page's own formatting
  10  |  (`$${Number(x.toFixed(2))}`, see pages/challenges/history.tsx).
  11  | */
  12  | 
  13  | import { test, expect } from "../../fixtures/test.extend";
  14  | import { EntriesPage } from "../../pages/entries.page";
  15  | 
  16  | interface ApiHistoryEntry {
  17  |   id: number;
  18  |   amount: string;
  19  |   result: string; // won | lost | cancelled | hi_nearly | pending
  20  |   insured: boolean;
  21  |   eventPayoutUninsured: number;
  22  |   eventPayoutInsuredHigh: number;
  23  |   payout: string;
  24  |   promoUsed?: { promotionType?: string } | null;
  25  | }
  26  | 
  27  | interface ApiHistorySummary {
  28  |   historyCount?: number;
  29  |   entriesWon?: number;
  30  |   amountWagered?: number;
  31  |   amountWon?: number;
  32  |   largestPayout?: number;
  33  | }
  34  | 
  35  | const fmtAmount = (e: ApiHistoryEntry): string =>
  36  |   e.promoUsed?.promotionType === "free_entry"
  37  |     ? "Free entry"
  38  |     : `$${Intl.NumberFormat("en-US").format(Number(e.amount))}`;
  39  | 
  40  | const fmtPayout = (e: ApiHistoryEntry): string =>
  41  |   `$${Number((e.insured ? e.eventPayoutInsuredHigh : e.eventPayoutUninsured).toFixed(2))}`;
  42  | 
  43  | const RESULT_BADGE: Record<string, string> = {
  44  |   won: "Won",
  45  |   lost: "Lost",
  46  |   hi_nearly: "Lost",
  47  |   cancelled: "Cancelled",
  48  | };
  49  | 
  50  | test.describe("History entries data verification", { tag: "@data-verification" }, () => {
  51  |   test("history cards and summary render the history API data", async ({
  52  |     loggedInPage: page,
  53  |   }) => {
  54  |     test.setTimeout(180_000);
  55  |     const entries = new EntriesPage(page);
  56  | 
  57  |     let paged!: { count: number; results: ApiHistoryEntry[] };
  58  |     let summary!: ApiHistorySummary;
  59  |     await test.step("Load /challenges/history and capture its API responses", async () => {
> 60  |       const pagedPromise = page.waitForResponse(
      |                                 ^ TimeoutError: page.waitForResponse: Timeout 45000ms exceeded while waiting for event "response"
  61  |         (r) =>
  62  |           /\/api\/v1\/entries\/history-paged\/\?days_back=\d+&page=1\b/.test(r.url()) &&
  63  |           r.status() === 200,
  64  |         { timeout: 45_000 },
  65  |       );
  66  |       const summaryPromise = page.waitForResponse(
  67  |         (r) =>
  68  |           /\/api\/v1\/entries\/history-summary\/?(\?|$)/.test(r.url()) && r.status() === 200,
  69  |         { timeout: 45_000 },
  70  |       );
  71  |       await page.goto("/challenges/history");
  72  |       const [pagedResp, summaryResp] = await Promise.all([pagedPromise, summaryPromise]);
  73  |       paged = await pagedResp.json();
  74  |       summary = await summaryResp.json();
  75  |     });
  76  | 
  77  |     if (paged.results.length === 0) {
  78  |       await test.step("No history: page shows the browse empty state", async () => {
  79  |         await expect(entries.browseNow).toBeVisible();
  80  |         await expect(entries.cardDivs).toHaveCount(0);
  81  |       });
  82  |       return;
  83  |     }
  84  | 
  85  |     await test.step("Card list matches the API page: same ids, same order", async () => {
  86  |       await expect(entries.cardDivs).toHaveCount(paged.results.length);
  87  |       const domIds = await entries.cardDivs.evaluateAll((els) =>
  88  |         els.map((el) => el.getAttribute("aria-controls")),
  89  |       );
  90  |       expect(domIds).toEqual(paged.results.map((e) => `entry-${e.id}-content`));
  91  |     });
  92  | 
  93  |     await test.step("Card headers show the API amount, payout and result", async () => {
  94  |       const errors: string[] = [];
  95  |       for (const apiEntry of paged.results.slice(0, 8)) {
  96  |         const card = page
  97  |           .locator(`div[role="region"][aria-controls="entry-${apiEntry.id}-content"]`)
  98  |           .filter({ visible: true })
  99  |           .first();
  100 |         const text = (await card.innerText()).replace(/\s+/g, " ").trim();
  101 |         const label = `entry ${apiEntry.id} (${apiEntry.result})`;
  102 | 
  103 |         if (!text.includes(fmtAmount(apiEntry))) {
  104 |           errors.push(`${label}: amount "${fmtAmount(apiEntry)}" not in "${text}"`);
  105 |         }
  106 | 
  107 |         if (apiEntry.result === "won" && !text.includes(`paid ${fmtPayout(apiEntry)}`)) {
  108 |           errors.push(`${label}: "paid ${fmtPayout(apiEntry)}" not in "${text}"`);
  109 |         }
  110 |         if (
  111 |           (apiEntry.result === "lost" || apiEntry.result === "cancelled") &&
  112 |           !text.includes(`To win ${fmtPayout(apiEntry)}`)
  113 |         ) {
  114 |           errors.push(`${label}: "To win ${fmtPayout(apiEntry)}" not in "${text}"`);
  115 |         }
  116 | 
  117 |         const badge = RESULT_BADGE[apiEntry.result];
  118 |         if (badge && !text.includes(badge)) {
  119 |           errors.push(`${label}: result badge "${badge}" not in "${text}"`);
  120 |         }
  121 |       }
  122 |       expect(errors, errors.join("\n")).toEqual([]);
  123 |     });
  124 | 
  125 |     await test.step("Summary tiles equal the history-summary API", async () => {
  126 |       await expect(entries.entriesPlacedStat).toHaveText(String(summary.historyCount ?? 0));
  127 |       await expect(entries.entriesWonStat).toHaveText(String(summary.entriesWon ?? 0));
  128 |       await expect(entries.historyEntryAmountStat).toHaveText(
  129 |         `$${Number((summary.amountWagered ?? 0).toFixed(2))}`,
  130 |       );
  131 |       const amountWon = Number((summary.amountWon ?? 0).toFixed(2));
  132 |       await expect(entries.totalWonStat).toHaveText(
  133 |         amountWon < 0 ? `-$${Math.abs(amountWon)}` : `$${amountWon}`,
  134 |       );
  135 |       await expect(entries.biggestPayoutStat).toHaveText(
  136 |         `$${Number((summary.largestPayout ?? 0).toFixed(2))}`,
  137 |       );
  138 |     });
  139 |   });
  140 | });
  141 | 
```