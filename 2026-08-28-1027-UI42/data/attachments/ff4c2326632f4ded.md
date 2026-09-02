# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: slip_sharing/slip_sharing_and_tailing.spec.ts >> Slip sharing & tailing >> Logged-out tailer signs in via the tail link, then auto-tails and submits
- Location: tests/slip_sharing/slip_sharing_and_tailing.spec.ts:173:5

# Error details

```
Error: expect(locator).toBeVisible() failed

Locator: getByRole('button').filter({ has: getByAltText('share', { exact: true }) }).filter({ visible: true }).first()
Expected: visible
Timeout: 15000ms
Error: element(s) not found

Call log:
  - Expect "toBeVisible" with timeout 15000ms
  - waiting for getByRole('button').filter({ has: getByAltText('share', { exact: true }) }).filter({ visible: true }).first()

```

# Test source

```ts
  1  | import { BasePage } from "./base.page";
  2  | import { expect, test } from "@playwright/test";
  3  | 
  4  | export class ContestSuccessPage extends BasePage {
  5  |   // locators starts
  6  | 
  7  |   correctLabel = this.byText("Correct", { exact: true });
  8  |   correctPicksNumbers = this.correctLabel.locator("..").locator("div").nth(1);
  9  |   continueBtn = this.byRole("button", { name: "Continue" });
  10 |   // The confirmation screen's share affordance is now an icon-only button
  11 |   // (screens/Contest/confirmation.tsx) — `<img alt="share">`, no "Share Slip"
  12 |   // text — so match it by that image rather than an accessible name.
  13 |   shareSlipBtn = this.page
  14 |     .getByRole("button")
  15 |     .filter({ has: this.page.getByAltText("share", { exact: true }) })
  16 |     .filter({ visible: true })
  17 |     .first();
  18 |   // UI Release 32: a dedicated description CTA on the Picks Submitted screen.
  19 |   // Reads "Add Description" or "Edit Description" depending on whether the
  20 |   // contest already has one (contestConfirmation.addDescription/editDescription).
  21 |   descriptionCta = this.byRole("button", {
  22 |     name: /(Add|Edit) Description/,
  23 |   });
  24 |   // The inline editor the CTA opens (ConfirmationDescriptionEditor) — its
  25 |   // textarea is labelled "Edit entry description".
  26 |   descriptionEditor = this.page
  27 |     .getByLabel("Edit entry description")
  28 |     .filter({ visible: true })
  29 |     .first();
  30 | 
  31 |   //locators ends
  32 | 
  33 |   async getPickNumbers() {
  34 |     const picks = await this.correctPicksNumbers.textContent();
  35 |     const match = picks?.match(/(\d+)\s*\/\s*(\d+)/);
  36 | 
  37 |     if (!match) throw new Error("Could not parse correct score");
  38 |     return { toBecorrect: +match[1], total: +match[2] };
  39 |   }
  40 | 
  41 |   async verifyPicksNumbers(toBeCorrectPicks: number, totalPicks: number) {
  42 |     const { toBecorrect, total } = await this.getPickNumbers();
  43 |     await expect(toBecorrect).toBe(toBeCorrectPicks);
  44 |     await expect(total).toBe(totalPicks);
  45 |   }
  46 | 
  47 |   // The confirmation heading (contestConfirmation.picksSubmitted). Mobile
  48 |   // renders it on its own screen; desktop (DFS-2467) in a modal over the lobby.
  49 |   picksSubmittedHeading = this.page
  50 |     .getByText("Picks Submitted", { exact: true })
  51 |     .filter({ visible: true })
  52 |     .first();
  53 | 
  54 |   async continueToHomePage() {
  55 |     await this.continueBtn.click();
  56 |     // Mobile: Continue routes the confirmation screen → "/", unmounting it.
  57 |     // Desktop: the confirmation is a modal over a lobby that is already at
  58 |     // "/" — seen on staging 2026-08-26: the modal stayed mounted after the
  59 |     // click and its backdrop then swallowed every later click (Track Picks
  60 |     // nav link) until the test timed out. Wait for it to go; if it doesn't,
  61 |     // reload the lobby to dismiss it and record that the fallback was needed
  62 |     // so the report shows it.
  63 |     try {
  64 |       await this.picksSubmittedHeading.waitFor({ state: "hidden", timeout: 5_000 });
  65 |     } catch {
  66 |       test.info().annotations.push({
  67 |         type: "note",
  68 |         description:
  69 |           "Picks Submitted modal stayed open after Continue — dismissed by reloading the lobby",
  70 |       });
  71 |       await this.page.goto("/");
  72 |       await expect(this.picksSubmittedHeading).toBeHidden();
  73 |     }
  74 |   }
  75 | 
  76 |   async assertContestShareable() {
> 77 |     await expect(this.shareSlipBtn).toBeVisible();
     |                                     ^ Error: expect(locator).toBeVisible() failed
  78 |   }
  79 | 
  80 |   /** Clicks the Add/Edit Description CTA and waits for the inline editor. */
  81 |   async openDescriptionEditor() {
  82 |     await expect(this.descriptionCta).toBeVisible();
  83 |     await this.descriptionCta.click();
  84 |     await expect(this.descriptionEditor).toBeVisible();
  85 |   }
  86 | }
  87 | 
```