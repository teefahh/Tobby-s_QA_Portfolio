# Manual Test Plan — SauceDemo Login & Checkout

## Objective
Manually verify the core login and purchase flow on [SauceDemo](https://www.saucedemo.com) across its seeded user accounts, and document any defects surfaced by exploratory testing.

## Scope
- **In scope:** Login (valid, invalid, locked-out accounts), product listing, cart, checkout
- **Out of scope:** Backend/API validation, performance testing, accessibility audit

## Test Environment
- Application: https://www.saucedemo.com
- Browser: Chrome (latest)
- Test accounts: `standard_user`, `locked_out_user`, `problem_user`, `error_user`, `visual_user`, `performance_glitch_user` (all use password `secret_sauce`)

## Approach
1. Execute login test cases against each seeded account
2. Walk the full purchase flow (login → add to cart → checkout → order confirmation) as `standard_user`
3. Repeat key flows against the non-standard accounts to surface account-specific defects
4. Log any deviation from expected behavior as a bug report

## Risks
- SauceDemo is a public demo app and its seeded data/behavior may change without notice
- Some account-specific bugs are intentionally seeded for QA practice rather than "real" defects — noted as such in bug reports
