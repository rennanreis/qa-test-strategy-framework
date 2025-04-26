# Traceability Matrix

This matrix maps each functional requirement to the test cases that validate it.

| Requirement ID | Requirement Description                                         | Test Case(s)                                          |
|----------------|----------------------------------------------------------------|-------------------------------------------------------|
| FR01           | User must be able to log in with valid credentials             | [equivalence-partitioning-login.md](tests/test-cases/equivalence-partitioning-login.md)                     |
| FR02           | System must display an error message for invalid login attempts| [equivalence-partitioning-login.md](tests/test-cases/equivalence-partitioning-login.md)                     |
| FR03           | User must view the list of available products                  | (covered as precondition in test cases)               |
| FR04           | User can add products to the cart                              | [state-transition-testing-cart-checkout.md](tests/test-cases/state-transition-testing-cart-checkout.md)             |
| FR05           | User can remove products from the cart                         | [state-transition-testing-cart-checkout.md](tests/test-cases/state-transition-testing-cart-checkout.md)             |
| FR06           | User can view cart items                                       | [state-transition-testing-cart-checkout.md](tests/test-cases/state-transition-testing-cart-checkout.md)             |
| FR07           | User can start the checkout process                            | [decision-table-testing-checkout.md](tests/test-cases/decision-table-testing-checkout.md), [state-transition-testing-cart-checkout.md](tests/test-cases/state-transition-testing-cart-checkout.md) |
| FR08           | User must fill in first name, last name, and postal code during checkout | [boundary-value-analysis-postalcode.md](tests/test-cases/boundary-value-analysis-postalcode.md), [decision-table-testing-checkout.md](tests/test-cases/decision-table-testing-checkout.md) |
| FR09           | System must validate required fields during checkout           | [boundary-value-analysis-postalcode.md](tests/test-cases/boundary-value-analysis-postalcode.md), [decision-table-testing-checkout.md](tests/test-cases/decision-table-testing-checkout.md) |
| FR10           | User can successfully complete a purchase                      | [decision-table-testing-checkout.md](tests/test-cases/decision-table-testing-checkout.md), [state-transition-testing-cart-checkout.md](tests/test-cases/state-transition-testing-cart-checkout.md) |
| FR11           | User can log out of the application                            | (optional: add if you document a logout test case)    |

---

**Note:**  
- The test case filenames now link directly to files in `/tests/test-cases/`.