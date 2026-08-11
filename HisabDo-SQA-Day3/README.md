# SQA Internship – Day 3 | HisabDo
Real Website QA Testing – OpenCart Demo Store

## 👤 Tester
Mohamed Hany – Junior Software Tester (ISTQB CTFL v4)

## 🌐 Application Under Test
- Website: https://demo.opencart.com (public OpenCart demo store)
- Environment: Chrome, Version 151.0.7922.71 (Official Build) (64-bit)
- Date of testing: August 3, 2026

## 🎯 Scope
Manual functional testing covering:
- Homepage (navigation, search, categories, links, buttons)
- Product section (details, images, availability, add to cart)
- Shopping cart (add/remove, quantity, price calculation, cart update)
- Forms (registration, contact us — required fields, valid/invalid inputs)

## 📊 Test Summary

| Metric | Count |
|---|---|
| Total test cases executed | 25 |
| Passed | 22 |
| Failed | 3 |
| Positive test cases | 10 |
| Negative test cases | 10 |
| Boundary/validation test cases | 5 |
| Bugs found | 3 |

## 🐞 Bugs Found

All 3 bugs relate to the same root cause: the Add to Cart quantity field is not validated before the product is added.

| Bug ID | Title | Module | Severity | Priority | Status |
|---|---|---|---|---|---|
| Bug_001 | Product is added to cart with a success message even when the quantity field is left empty | Product | Medium | Medium | Open |
| Bug_002 | Product is added to cart with a success message even when a negative quantity (-1) is entered | Product | Medium | Medium | Open |
| Bug_003 | Product is added to cart with a success message even when quantity is set to 0 | Product | Medium | Medium | Open |

Expected behavior: the system should either default an empty quantity to 1, or reject empty/negative/zero quantities with a validation error — not silently accept them and show a success message.

Only 3 genuine bugs were identified during this round of testing; per the task instructions, no additional bugs were fabricated to reach a count of 5.

## 📁 Files in this Repository
- Day3_QA_TC_Bug_reports.xlsx — full QA document containing:
  - Test Cases sheet: 25 executed test cases (ID, Module, Type, Scenario, Precondition, Steps, Test Data, Expected Result, Actual Result, Status)
  - Bug Report sheet: detailed defect reports for Bug_001, Bug_002, Bug_003
  - Bug Report (2) sheet: blank template (no further genuine bugs found)

## 🧰 Testing Technique Applied
Requirement Analysis → Test Scenario Design → Test Case Writing → Positive/Negative Testing → Boundary Value Analysis → Manual Execution → Bug Reporting
