# QA Test Strategy Framework

[![License](https://img.shields.io/badge/license-MIT-green)](LICENSE)
[![Status](https://img.shields.io/badge/status-active-brightgreen)]()
[![Last Update](https://img.shields.io/github/last-commit/rennanreis/qa-test-strategy-framework)](https://github.com/rennanreis/qa-test-strategy-framework/commits/main)

> **Note:** This project is intended for personal portfolio purposes. External contributions (pull requests, issues) are not being accepted at this time.

A practical framework for data quality test strategy, featuring ISTQB-based templates, real-world examples (using Sauce Labs demo site), and defect management best practices for Agile teams.

For more details about the rationale behind this framework, practical examples, and a step-by-step guide, read the full article on Medium:
[QA Test Strategy Framework: How I Built a Real-World Manual Testing Portfolio with ISTQB Templates](https://medium.com/@rennanreis/qa-test-strategy-framework-how-i-built-a-real-world-manual-testing-portfolio-with-istqb-templates-39bff28f8926)

## Quick Start

1. **Clone this repository**
2. **Browse the `/templates/` and `/tests/` folders** for ready-to-use examples and templates
3. **For detailed instructions, see the "How to Use" section below**

## Repository Structure

```
├── LICENSE
├── README.md
├── requirements.md
├── templates/
│ ├── defect-management/
│ │ ├── bug-report-template.md
│ │ └── defect-life-cycle.md
│ └── test-cases/
│ ├── boundary-value-analysis.md
│ ├── decision-table-testing.md
│ ├── equivalence-partitioning.md
│ └── state-transition-testing.md
├── tests/
│ ├── defect-management/
│ │ ├── bug-report-example.md
│ │ └── defect-life-cycle-example.md
| ├── evidence/
│ └── test-cases/
│ ├── equivalence-partitioning-login.md
│ ├── boundary-value-analysis-postalcode.md
│ ├── decision-table-testing-checkout.md
│ └── state-transition-testing-cart-checkout.md
```

## What’s Inside

- **/templates/defect-management/**  
  - Defect life cycle documentation template
  - Clear and reproducible bug report template

- **/templates/test-cases/**  
  Ready-to-use test case templates using industry-standard techniques:
  - Equivalence Partitioning
  - Boundary Value Analysisgit log
  - Decision Table Testing
  - State Transition Testing

- **/tests/defect-management/**  
  Real examples of defect documentation:
  - `bug-report-example.md`: Example bug report for a checkout defect
  - `defect-life-cycle-example.md`: Example defect life cycle for the same bug

- **/tests/evidence/**  
  Screenshots proving test execution results (success, errors, defects).

- **/tests/test-cases/**  
  Filled examples of test cases applied to real scenarios from the Sauce Labs Demo site:
  - `equivalence-partitioning-login.md`: Login with valid and invalid credentials
  - `boundary-value-analysis-postalcode.md`: Postal code field validation in checkout
  - `decision-table-testing-checkout.md`: Checkout input combinations
  - `state-transition-testing-cart-checkout.md`: Cart to checkout flow

- **requirements.md**  
  List of functional requirements covered by the tests.

- **traceability-matrix.md**:
   Matrix mapping each functional requirement to its corresponding test cases, ensuring complete coverage and traceability.

## About Test Evidence and Equivalence Classes

Each screenshot in this repository is a representative example for an equivalence class or unique system response, following the Equivalence Partitioning technique. For each group of inputs that produce the same system behavior (e.g., valid login, invalid login), only one representative test and its evidence are documented. If multiple invalid inputs (such as wrong credentials or empty fields) trigger the same error message, a single screenshot is provided for that equivalence class. This approach keeps the documentation concise and focused, while ensuring full coverage.

## How to Use

1. **Clone this repository**
2. **Use the test plan and test case templates** in `/templates/test-cases/` to design your own tests
3. **Apply the bug report and defect life cycle templates** in `/templates/defect-management/` to track and communicate defects
4. **Review the real-world examples** in `/tests/test-cases/` and `/tests/defect-management/` for practical inspiration
5. **Refer to the traceability matrix** (`traceability-matrix.md`) to ensure your test cases cover all functional requirements
6. **For a step-by-step walkthrough and rationale, see the Medium article linked above**

## Real-World Example

All templates and examples are applied to the [Sauce Labs Demo Site](https://www.saucedemo.com/).

## Why Use This Framework?

- Reduce bug correction costs by up to 40%
- Improve communication between QA, developers, and stakeholders
- Increase product reliability and team agility

## References

- Crispin, L., & Gregory, J. (2009). *Agile Testing: A Practical Guide for Testers and Agile Teams*
- Knorr, F., & Gonçalves, P. (2020). *Agile Testing Condensed – PT-BR Edition*
- Myers, G. J., Sandler, C., & Badgett, T. (2011). *The Art of Software Testing*
- Black, R. (2009). *Managing the Testing Process*
- Kaner, C., Bach, J., & Pettichord, B. (2002). *Lessons Learned in Software Testing*

---

*Feel free to fork, contribute, and use this framework in your own projects!*