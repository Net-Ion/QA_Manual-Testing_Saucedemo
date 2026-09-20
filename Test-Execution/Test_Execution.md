# Test Execution Report — SauceDemo QA Testing

## 1. Executive Summary
This report summarizes the manual functional black-box test execution results for the **SauceDemo** web application, based on the test suite recorded in the project workbook[cite: 4].

| Metric | Result |
| :--- | :---: |
| **Total Test Cases Executed** | 35[cite: 4] |
| **Passed** | 31[cite: 4] |
| **Failed** | 4[cite: 4] |
| **Pass Rate** | 88.57%[cite: 4] |
| **Defects Logged** | 4[cite: 4] |
| **Total Requirements (RTM)** | 15[cite: 4] |
| **Requirement Coverage** | 100%[cite: 4] |

---

## 2. Module-wise Test Execution

| Module | Total TCs | PASS | FAIL | Pass Rate | Defects Identified |
| :--- | :---: | :---: | :---: | :---: | :--- |
| **Login** | 6 | 6 | 0 | 100% | None[cite: 4] |
| **Inventory** | 11 | 9 | 2 | 81.82% | Bug-01, Bug-02[cite: 4] |
| **Your Cart** | 10 | 9 | 1 | 90.00% | Bug-03[cite: 4] |
| **Checkout** | 8 | 7 | 1 | 87.50% | Bug-04[cite: 4] |
| **TOTAL** | **35** | **31** | **4** | **88.57%** | **4 Logged Defects**[cite: 4] |

---

## 3. Failed Test Cases Detail

| Test Case ID | Module | Scenario / Description | Associated Defect | Root Cause / Behavior |
| :--- | :--- | :--- | :--- | :--- |
| **TC_I_02** | Inventory | Verify product names are visible[cite: 4] | **Bug-01**[cite: 4] | Incorrect product name displayed for the last item in inventory (`T-Shirt RED`)[cite: 4]. |
| **TC_I_09** | Inventory | Verify Icons Working[cite: 4] | **Bug-02**[cite: 4] | The sorting dropdown arrow icon is unclickable and fails to expand options[cite: 4]. |
| **TC_YC_07** | Your Cart | Verify "Checkout" navigation without products[cite: 4] | **Bug-03**[cite: 4] | Application allows proceeding to checkout with an empty cart without validation[cite: 4]. |
| **TC_CKF_04** | Checkout | Verify checkout with Invalid postal code (ex: name)[cite: 4] | **Bug-04**[cite: 4] | Form accepts non-numeric text input for postal code and navigates to the overview page[cite: 4]. |

---

## 4. Defect Summary & Tracking

| Defect ID | Related TC | Severity | Priority | Status | Summary |
| :--- | :--- | :---: | :---: | :---: | :--- |
| **Bug-01** | `TC_I_02`[cite: 4] | LOW[cite: 4] | P3[cite: 4] | Open[cite: 4] | Incorrect product title rendered for the final inventory item[cite: 4]. |
| **Bug-02** | `TC_I_09`[cite: 4] | LOW[cite: 4] | P3[cite: 4] | Open[cite: 4] | Dropdown toggle arrow icon is inactive on click[cite: 4]. |
| **Bug-03** | `TC_YC_07`[cite: 4] | MEDIUM[cite: 4] | P2[cite: 4] | Open[cite: 4] | User can navigate to checkout step 1 with 0 items in cart[cite: 4]. |
| **Bug-04** | `TC_CKF_04`[cite: 4] | HIGH[cite: 4] | P1[cite: 4] | Open[cite: 4] | Missing alphanumeric validation on postal code field at checkout[cite: 4]. |

---

## 5. Execution Observations & Notes
* All 35 test cases were manually executed against Google Chrome in the recorded QA test workbook[cite: 2, 4].
* Detailed actual results, reproduction steps, and severity ratings are documented for all 4 failing tests[cite: 4].
* The application demonstrates high stability across critical paths (88.57% pass rate), with zero blocking failures in core authentication flows[cite: 4].
