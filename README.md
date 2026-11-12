# SauceDemo – Manual Testing Project

![Testing](https://img.shields.io/badge/Testing-Manual-blue)
![Domain](https://img.shields.io/badge/Domain-E--commerce-orange)
![Status](https://img.shields.io/badge/Status-In%20Progress-yellow)

## Project Overview

This project covers manual testing of the **SauceDemo** e-commerce web application.
The objective is to verify application functionality, identify defects, and document all testing activities using industry-standard QA practices (requirements analysis, test design, traceability, execution and defect reporting).

## Application Under Test

| Item | Details |
|------|---------|
| Application | [https://www.saucedemo.com/](https://www.saucedemo.com/) |
| Testing Type | Manual Testing (Functional, UI, Negative) |
| Domain | E-commerce |
| Browser | Google Chrome |

## Testing Scope

**In scope**

- Login and Authentication
- Product Inventory
- Product Sorting
- Shopping Cart
- Checkout
- Logout

**Out of scope**

- Performance, security and load testing
- Automation testing
- Mobile / responsive testing

## Test Data

SauceDemo publishes its demo accounts on the login page. Password for all users: `secret_sauce`

| Username | Purpose |
|----------|---------|
| `standard_user` | Normal user used for most positive test cases |
| `locked_out_user` | Locked account, used for negative login testing |
| `problem_user` | Account with known UI/functional issues, used for defect finding |
| `performance_glitch_user` | Slow-responding account |

## Testing Tools

| Tool | Usage |
|------|-------|
| Microsoft Excel | Test documentation |
| Jira | Defect tracking |
| Google Chrome | Manual testing |
| GitHub | Project documentation |

## Project Structure

```
SauceDemo-Manual-Testing/
│
├── README.md
├── Documents/
│   ├── Requirement_Specification.xlsx
│   ├── Test_Scenarios.xlsx
│   ├── Test_Cases.xlsx
│   ├── RTM.xlsx
│   └── Test_Execution_Report.xlsx
│
├── Bug_Reports/
│   ├── Bug_Report_001.pdf
│   └── Screenshots/
│
└── Test_Evidence/
```

## Project Deliverables

| Deliverable | File | Description |
|-------------|------|-------------|
| Requirement Specification | `Documents/Requirement_Specification.xlsx` | 25 functional requirements (REQ-XXX-NN) grouped by module |
| Test Scenarios | `Documents/Test_Scenarios.xlsx` | 21 high-level scenarios mapped to requirements |
| Test Cases | `Documents/Test_Cases.xlsx` | 42 detailed test cases with steps, data and expected results, plus a Test Data sheet |
| Requirement Traceability Matrix | `Documents/RTM.xlsx` | Requirement → Scenario → Test Case mapping with coverage counts |
| Test Execution Report | `Documents/Test_Execution_Report.xlsx` | Execution log with status dropdowns and an auto-calculating summary |
| Bug Reports | `Bug_Reports/Bug_Report_001.pdf` | Defect report in a standard format |

## Testing Process

1. **Requirement Analysis** – derive requirements from the application's behavior
2. **Test Scenario Design** – identify what to test per requirement
3. **Test Case Design** – write detailed, repeatable test cases
4. **Traceability** – map requirements to scenarios and test cases (RTM)
5. **Test Execution** – run test cases in Chrome, record results and evidence
6. **Defect Reporting** – log defects in Jira and document them in `Bug_Reports/`
7. **Reporting** – summarise results in the Test Execution Report

## ID Conventions

| Artifact | Format | Example |
|----------|--------|---------|
| Requirement | `REQ-<MODULE>-<NN>` | `REQ-LOG-01` |
| Test Scenario | `TS-<NNN>` | `TS-001` |
| Test Case | `TC-<NNN>` | `TC-001` |
| Bug | `BUG-<NNN>` | `BUG-001` |

Modules: `LOG` Login · `INV` Inventory · `SRT` Sorting · `CRT` Cart · `CHK` Checkout · `LGO` Logout

## How to Use This Repository

1. Read `Requirement_Specification.xlsx` to understand what is being tested.
2. Follow `Test_Cases.xlsx` to execute each test case on https://www.saucedemo.com/.
3. Update the **Status** dropdown, **Actual Result**, **Execution Date** and **Bug ID** in `Test_Execution_Report.xlsx`. The Summary sheet recalculates automatically.
4. Save screenshots of failures in `Bug_Reports/Screenshots/` and pass/fail proof in `Test_Evidence/`, named after the test case or bug ID (e.g. `TC-013_Pass.png`, `BUG-001_Inventory_Images.png`).

## Project Status

**In Progress** – documentation is complete; test execution and defect logging are ongoing.

## Author

**Nitu Yadav**
