# QA Portfolio

Manual and exploratory QA artifacts demonstrating end-to-end test process: test planning, test case design, bug reporting, and summary reporting.

For working test **automation** code, see my dedicated framework repo: [saucedemo-playwright-framework](https://github.com/teefahh/saucedemo-playwright-framework) (Playwright + TypeScript, Page Object Model, CI via GitHub Actions).

## What's here

### `Manual-testing/`
A full manual QA cycle against [SauceDemo](https://www.saucedemo.com)'s login and checkout flow:
- [`test-plan.md`](Manual-testing/test-plan.md) — scope, environment, and approach
- [`test-cases.md`](Manual-testing/test-cases.md) — 9 test cases covering login (valid/invalid/locked-out/blank), product listing, cart, and checkout
- [`bug-report.md`](Manual-testing/bug-report.md) — a defect found and documented during exploratory testing
- [`test-report.md`](Manual-testing/test-report.md) — summary of the test cycle results

### `automation/playwright/`
Early-stage test planning docs for automating login on a separate demo application ([`test-plan.md`](automation/playwright/test-plan.md), [`test-cases.md`](automation/playwright/test-cases.md)) — planning artifacts, not yet implemented in code.

## Planned additions
- API testing (Postman collection + test cases)
- Cypress automation example

## Author
**Latifat Yisa**
[GitHub](https://github.com/teefahh) · latifat.yisa@gmail.com
