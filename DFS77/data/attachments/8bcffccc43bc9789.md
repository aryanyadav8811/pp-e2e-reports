# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: packs/access.spec.ts >> Packs access (DFS-2146) >> staff user sees the Packs entry and can open the lobby
- Location: tests/packs/access.spec.ts:26:3

# Error details

```
Error: expect(locator).toBeVisible() failed

Locator: getByRole('link', { name: 'Packs', exact: true }).or(getByRole('button', { name: 'Packs', exact: true })).filter({ visible: true }).first()
Expected: visible
Timeout: 30000ms
Error: element(s) not found

Call log:
  - Expect "toBeVisible" with timeout 30000ms
  - waiting for getByRole('link', { name: 'Packs', exact: true }).or(getByRole('button', { name: 'Packs', exact: true })).filter({ visible: true }).first()

```

# Page snapshot

```yaml
- generic [active] [ref=e1]:
  - main [ref=e2]:
    - generic [ref=e3]:
      - heading "staging.parlayplay.io" [level=1] [ref=e5]
      - heading "Performing security verification" [level=2] [ref=e6]
      - paragraph [ref=e7]: This website uses a security service to protect against malicious bots. This page is displayed while the website verifies you are not a bot.
  - contentinfo [ref=e11]:
    - generic [ref=e13]:
      - generic [ref=e15]:
        - text: "Ray ID:"
        - code [ref=e16]: a2aacb2a191ee8eb
      - generic [ref=e17]:
        - generic [ref=e18]:
          - text: Performance and Security by
          - link "Cloudflare, opens in a new tab" [ref=e19] [cursor=pointer]:
            - /url: https://www.cloudflare.com?utm_source=challenge&utm_campaign=m
            - text: Cloudflare
        - link "Privacy, opens in a new tab" [ref=e21] [cursor=pointer]:
          - /url: https://www.cloudflare.com/privacypolicy/
          - text: Privacy
```

# Test source

```ts
  1  | /**
  2  |  * Packs access control — DFS-2146 (kill switch).
  3  |  *
  4  |  * /packs is auth-gated and additionally hidden behind packsVisibility
  5  |  * (enabled / staff_only / disabled). Flipping the platform setting needs admin
  6  |  * state changes, so this file covers the two ends we can drive from the client:
  7  |  *   • unauthenticated → redirected to login (ACC-05)
  8  |  *   • staff user (***) → Packs entry visible and lobby reachable (ACC-03)
  9  |  * The visibility-matrix cases (staff_only vs non-staff, disabled) stay manual.
  10 |  */
  11 | import { test, expect } from "../../fixtures/packs.extend";
  12 | import { PacksPage } from "@pages/packs.page";
  13 | 
  14 | test.describe("Packs access (DFS-2146)", { tag: ["@packs", "@dfs2146"] }, () => {
  15 |   test(
  16 |     "unauthenticated visit to /packs redirects to login with a next param",
  17 |     { tag: "@smoke" },
  18 |     async ({ page }) => {
  19 |       // Default `page` fixture is unauthenticated.
  20 |       await page.goto("/packs");
  21 |       await expect(page).toHaveURL(/\/account\/login/);
  22 |       await expect(page).toHaveURL(/next=%2Fpacks|next=\/packs/);
  23 |     },
  24 |   );
  25 | 
  26 |   test("staff user sees the Packs entry and can open the lobby", async ({
  27 |     packsPage: page,
  28 |   }) => {
  29 |     const packs = new PacksPage(page);
  30 | 
  31 |     await page.goto("/");
> 32 |     await expect(packs.packsNavEntry).toBeVisible({ timeout: 30_000 });
     |                                       ^ Error: expect(locator).toBeVisible() failed
  33 | 
  34 |     await packs.openLobby();
  35 |     await expect(packs.openAPackHeading).toBeVisible();
  36 |   });
  37 | });
  38 | 
```