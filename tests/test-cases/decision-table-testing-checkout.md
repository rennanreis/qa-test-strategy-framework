# Decision Table Testing Test Case - Checkout

## Test Case ID:
DT-001

## Related Requirement:
FR07 - User must be able to complete the checkout process  
FR08 - User must fill in first name, last name, and postal code during checkout  
FR09 - System must validate required fields during checkout  
FR10 - System must confirm successful order placement

## Title:
Validate checkout form field combinations

## Objective:
Verify that the system correctly validates all required fields during checkout and only allows the process to continue when all fields are properly filled.

## Preconditions:
- User is logged in on Sauce Labs Demo
- User has at least one product in the cart
- User is on the "Checkout: Your Information" page

## Test Steps:
1. Enter combinations of field values as per the decision table.
2. Click the "Continue" button.
3. For successful combinations, complete the checkout process.

## Decision Table:
| Scenario | First Name | Last Name | Postal Code | Expected Result                   |
|----------|------------|-----------|-------------|-----------------------------------|
| Case 1   | filled     | filled    | filled      | Proceed to checkout overview      |
| Case 2   | empty      | filled    | filled      | Error: "First Name is required"   |
| Case 3   | filled     | empty     | filled      | Error: "Last Name is required"    |
| Case 4   | filled     | filled    | empty       | Error: "Postal Code is required"  |
| Case 5   | empty      | empty     | empty       | Error: "First Name is required"   |

## Postconditions:
- User proceeds to the next checkout step or sees a validation error.
- For complete checkout, user sees order confirmation page.

## Evidence

### Successful Checkout
![Successful checkout - Products](../evidence/checkout-success-001.png)
![Successful checkout - Cart](../evidence/checkout-success-002.png)
![Successful checkout - Checkout: Your Information](../evidence/checkout-success-003.png)
![Successful checkout - Checkout: Overview](../evidence/checkout-success-004.png)
![Successful checkout - Checkout: Complete!](../evidence/checkout-success-005.png)

### Error: Missing First Name
![Checkout error - Checkout: Your Information](../evidence/checkout-error-missing-firstname.png)