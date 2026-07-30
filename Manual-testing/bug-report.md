# Bug Report — SauceDemo

## BUG-01: Product images are incorrect for the `problem_user` account

**Severity:** Medium
**Priority:** Medium
**Status:** Open (seeded defect on the demo application, kept for QA practice purposes)

### Environment
- URL: https://www.saucedemo.com
- Account: `problem_user` / `secret_sauce`
- Browser: Chrome (latest)

### Steps to Reproduce
1. Go to https://www.saucedemo.com
2. Log in with `problem_user` / `secret_sauce`
3. Observe the product images on the Products page

### Expected Result
Each product displays its own correct, distinct image, matching behavior for `standard_user`.

### Actual Result
All products display the same (incorrect) image instead of their individual product photos.

### Notes
This is a known, intentionally seeded defect on SauceDemo used to give QA practitioners something real to find and document — included here as an example of exploratory testing and bug reporting technique, not a claim about a production defect.
