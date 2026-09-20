# Test Summary Report — SauceDemo QA Testing

## 1. Project Overview
This document provides the final test summary for the manual functional black-box testing performed on the **SauceDemo** sample e-commerce application[cite: 5]. Testing covered end-to-end user workflows across the **Login**, **Inventory**, **Your Cart**, and **Checkout** modules[cite: 5].

* **Target Application:** SauceDemo ([https://www.saucedemo.com/](https://www.saucedemo.com/))[cite: 2]
* **Testing Methodology:** Functional Black-Box Testing[cite: 5]
* **Execution Environment:** Google Chrome (Latest Stable Version)[cite: 2]
* **Prepared By:** Nilanchal Pradhan[cite: 2]

---

## 2. Test Execution Results

| Measure | Result | Notes |
| :--- | :---: | :--- |
| **Total Test Cases Planned & Executed** | 35 | 100% of planned test cases executed[cite: 4, 5] |
| **Passed Test Cases** | 31 | Met expected acceptance criteria[cite: 4, 5] |
| **Failed Test Cases** | 4 | Logged with reproduction steps and actual behavior[cite: 4, 5] |
| **Overall Pass Rate** | **88.57%** | Calculated across all 4 core modules[cite: 4, 5] |
| **Requirements Traced (RTM)** | 15 | Total business & functional requirements mapped[cite: 4, 5] |
| **Requirement Coverage** | **100%** | Full bidirectional traceability achieved[cite: 4, 5] |
| **Defects Logged** | 4 | Categorized by severity and priority[cite: 4, 5] |

---

## 3. Defect Distribution by Severity

| Severity Level | Count | Defect IDs | Impact Analysis |
| :--- | :---: | :--- | :--- |
| **High** | 1 | `Bug-04` | Postal code field validation accepts invalid string/name input during checkout step 1[cite: 4, 5]. |
| **Medium** | 1 | `Bug-03` | System allows checkout navigation with zero items in the cart without a warning banner[cite: 4, 5]. |
| **Low** | 2 | `Bug-01`, `Bug-02` | UI / usability defects (incorrect product title display on last item; unresponsive sorting arrow icon)[cite: 4, 5]. |
| **Total** | **4** | — | — |

---

## 4. Key Findings & Observations

* **Login Functionality (100% Pass):** All 6 authentication scenarios passed, correctly handling valid logins, invalid credentials, and required-field error messaging[cite: 4, 5].
* **Inventory Module (81.82% Pass):** Catalog display and sorting functionality performed as expected, with failures isolated to one inaccurate item title (`T-Shirt RED`) and an unresponsive dropdown arrow icon[cite: 4, 5].
* **Your Cart Module (90.00% Pass):** Product quantity, cart badges, and navigation passed, but checkout initiation with an empty cart failed due to absent validation restrictions[cite: 4, 5].
* **Checkout Workflow (87.50% Pass):** Order computations, cancellations, and order completion passed, while input validation failed on step 1 due to accepting non-numeric postal codes[cite: 4, 5].

---

## 5. QA Project Artifacts

* **Test Plan (`Test_Plan.md`):** Complete test scope, environment parameters, criteria, and strategy[cite: 2, 5].
* **Test Case Suite (`SauceDemo QA Test Case.xlsx`):** 35 detailed test cases spanning 4 modules[cite: 5].
* **Requirements Traceability Matrix (RTM):** Bidirectional matrix mapping requirements to test IDs and bugs[cite: 5].
* **Defect Reports:** Documented bug reports with reproduction steps, severity, and screenshots[cite: 2, 5].
* **Test Execution Report (`Test_Execution_Report.md`):** Module-level execution metrics and breakdown[cite: 4, 5].

---

## 6. Project & Submission Notes
This summary reflects manual test execution statuses recorded in the primary QA workbook and is structured as a portfolio demonstration of end-to-end software quality assurance processes[cite: 5].
