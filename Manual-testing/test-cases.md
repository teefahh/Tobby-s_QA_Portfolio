# Manual Test Cases — SauceDemo Login & Checkout

| ID | Scenario | Steps | Expected Result | Actual Result | Status |
|----|----------|-------|------------------|----------------|--------|
| TC-01 | Login with valid credentials | Enter `standard_user` / `secret_sauce`, click Login | User is redirected to the Products page | User is redirected to `/inventory.html` | Pass |
| TC-02 | Login with invalid credentials | Enter an unrecognized username/password, click Login | Error message "Username and password do not match any user in this service" is shown | Error message displayed as expected | Pass |
| TC-03 | Login with locked-out account | Enter `locked_out_user` / `secret_sauce`, click Login | Error message "Epic sadface: Sorry, this user has been locked out." is shown | Error message displayed as expected | Pass |
| TC-04 | Login with blank fields | Leave both fields empty, click Login | Error message "Username is required" is shown | Error message displayed as expected | Pass |
| TC-05 | Product images render correctly | Login as `standard_user`, view Products page | Each product shows its own distinct image | All product images render correctly | Pass |
| TC-06 | Product images render correctly (problem account) | Login as `problem_user`, view Products page | Each product shows its own distinct image | All products show the same incorrect image | **Fail — see BUG-01** |
| TC-07 | Add single product to cart | Login, click "Add to cart" on one product | Cart icon shows a count of 1 | Cart icon updates to 1 | Pass |
| TC-08 | Complete checkout | Add product to cart, proceed through checkout with valid shipping info | Order confirmation ("Thank you for your order!") is shown | Order confirmation displayed as expected | Pass |
| TC-09 | Checkout with empty cart | Navigate directly to checkout with an empty cart | User cannot proceed to checkout / is blocked from placing an empty order | Checkout step is inaccessible with an empty cart | Pass |
