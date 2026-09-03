# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: signup/signup.spec.ts >> Signup - Validation >> Shows an error when the email is already taken
- Location: tests/signup/signup.spec.ts:213:3

# Error details

```
Error: expect(locator).toBeVisible() failed

Locator: locator('p.text-status-bad').filter({ visible: true }).first().filter({ hasText: 'A user with this email address already exists.' })
Expected: visible
Timeout: 15000ms
Error: element(s) not found

Call log:
  - Expect "toBeVisible" with timeout 15000ms
  - waiting for locator('p.text-status-bad').filter({ visible: true }).first().filter({ hasText: 'A user with this email address already exists.' })

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
          - link "Login" [ref=e10]:
            - /url: /account/login
            - generic [ref=e12]: Login
      - main [ref=e13]:
        - generic [ref=e19]:
          - text: Account Creation
          - button "Back" [ref=e20] [cursor=pointer]:
            - img [ref=e21]
            - generic [ref=e23]: Back
          - generic [ref=e25]:
            - generic [ref=e26]: Choose your Username
            - textbox "Choose your Username" [ref=e29]:
              - /placeholder: Username
            - generic [ref=e30]: Choose your Password
            - generic [ref=e33]:
              - textbox "Choose your Password" [ref=e34]:
                - /placeholder: Password
              - separator [ref=e35]
              - button "Show or Hide Password" [ref=e36]:
                - img [ref=e37]
            - generic [ref=e41]:
              - textbox "Confirm Password" [ref=e42]
              - separator [ref=e43]
              - button "Show or Hide Password" [ref=e44]:
                - img [ref=e45]
            - paragraph [ref=e48]: Enter your name and date of birth exactly as shown on your ID or passport.
            - generic [ref=e49]: First Name
            - textbox "First Name" [ref=e52]
            - generic [ref=e53]: Last Name
            - textbox "Last Name" [ref=e56]
            - generic [ref=e57]: Date of Birth
            - textbox "Date of birth" [ref=e59]
            - generic [ref=e60]: Referral Code (optional)
            - textbox "Referral Code" [ref=e63]
            - generic [ref=e64]: E-mail Address
            - textbox "E-mail Address" [ref=e67]: taken@example.com
            - generic [ref=e68]: Phone number
            - generic [ref=e70]:
              - generic [ref=e71]:
                - combobox "Phone number country" [ref=e72] [cursor=pointer]:
                  - option "Canada"
                  - option "United States" [selected]
                - img [ref=e74]
              - textbox "Phone number" [ref=e80]
            - button "Text me a Code" [disabled] [ref=e82]
    - generic:
      - region "Notifications Alt+T"
  - alert [ref=e83]
```

# Test source

```ts
  130 |   test.beforeEach(async ({ page }) => {
  131 |     const termsPage = new TermsPage(page);
  132 |     await termsPage.openTermsPage();
  133 |     await termsPage.setAccept(true);
  134 |     await termsPage.proceed();
  135 |     await new SignupPage(page).assertReady();
  136 |   });
  137 | 
  138 |   test('"Text me a Code" opens the OTP modal', async ({ page }) => {
  139 |     const signupPage = new SignupPage(page);
  140 |     const otpModal = new OTPModalPage(page);
  141 | 
  142 |     await test.step('Fill the signup form with valid data', async () => {
  143 |       const testData = generateTestData();
  144 |       await signupPage.fill({
  145 |         username: testData.username,
  146 |         password: testData.password,
  147 |         confirmPassword: testData.password,
  148 |         firstName: testData.firstName,
  149 |         lastName: testData.lastName,
  150 |         email: testData.email,
  151 |         phoneNumber: testData.phoneNumber,
  152 |         dob: true,
  153 |       });
  154 |     });
  155 | 
  156 |     await test.step('Click "Text me a Code" — OTP modal opens', async () => {
  157 |       await signupPage.clickTextMeCodeBtn();
  158 |       await otpModal.waitForModal();
  159 |       await otpModal.assertReady();
  160 |     });
  161 |   });
  162 | 
  163 |   test(
  164 |     'Signup completes with the mocked OTP',
  165 |     { tag: ['@smoke', '@creates-user'] },
  166 |     async ({ page }) => {
  167 |       const signupPage = new SignupPage(page);
  168 |       const otpModal = new OTPModalPage(page);
  169 |       const successPage = new SignupSuccessPage(page);
  170 | 
  171 |       await test.step('Fill the signup form with valid data', async () => {
  172 |         const testData = generateTestData();
  173 |         await signupPage.fill({
  174 |           username: testData.username,
  175 |           password: testData.password,
  176 |           confirmPassword: testData.password,
  177 |           firstName: testData.firstName,
  178 |           lastName: testData.lastName,
  179 |           email: testData.email,
  180 |           phoneNumber: testData.phoneNumber,
  181 |           dob: true,
  182 |         });
  183 |       });
  184 | 
  185 |       await test.step('Click "Text me a Code" — OTP modal opens', async () => {
  186 |         await signupPage.clickTextMeCodeBtn();
  187 |         await otpModal.waitForModal();
  188 |       });
  189 | 
  190 |       await test.step('Enter the mocked OTP and authorize', async () => {
  191 |         await expect(otpModal.otpInput).toBeVisible();
  192 |         await otpModal.enterOTP('123456');
  193 |         await expect(otpModal.authorizeBtn).toBeEnabled();
  194 |         await otpModal.authorizeBtn.click();
  195 |       });
  196 | 
  197 |       await test.step('Signup success page shows the Deposit Now button', async () => {
  198 |         await expect(successPage.depositNowButton).toBeEnabled();
  199 |       });
  200 |     },
  201 |   );
  202 | });
  203 | 
  204 | test.describe('Signup - Validation', { tag: ['@signup', '@validation'] }, () => {
  205 |   test.beforeEach(async ({ page }) => {
  206 |     const termsPage = new TermsPage(page);
  207 |     await termsPage.openTermsPage();
  208 |     await termsPage.setAccept(true);
  209 |     await termsPage.proceed();
  210 |     await new SignupPage(page).assertReady();
  211 |   });
  212 | 
  213 |   test('Shows an error when the email is already taken', async ({ page, mockEmailExists }) => {
  214 |     const signupPage = new SignupPage(page);
  215 | 
  216 |     await test.step('Stub /check_email to return "already exists"', async () => {
  217 |       await mockEmailExists();
  218 |     });
  219 | 
  220 |     await test.step('Enter the taken email and blur the field', async () => {
  221 |       await signupPage.email.fill('taken@example.com');
  222 |       await signupPage.email.blur();
  223 |     });
  224 | 
  225 |     await test.step('Inline error "A user with this email address already exists." is shown', async () => {
  226 |       await expect(
  227 |         signupPage.errorMessage.filter({
  228 |           hasText: 'A user with this email address already exists.',
  229 |         }),
> 230 |       ).toBeVisible();
      |         ^ Error: expect(locator).toBeVisible() failed
  231 |     });
  232 |   });
  233 | });
  234 | 
```