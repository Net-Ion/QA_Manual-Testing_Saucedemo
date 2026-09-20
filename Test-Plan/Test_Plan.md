# Test Plan — SauceDemo QA Testing

## 1. Introduction & Objectives
The purpose of this test plan is to define the testing approach, scope, resources, environment, and deliverables for the **SauceDemo** web application[cite: 2]. The primary objective is to validate the core functional behavior of the e-commerce workflows through structured manual black-box testing, ensuring requirement coverage and documenting defects systematically[cite: 2].

* **Application Name:** SauceDemo[cite: 2]
* **Application Type:** E-Commerce Web Application[cite: 2]
* **Target URL:** [https://www.saucedemo.com/](https://www.saucedemo.com/)[cite: 2]
* **Tested By:** Nilanchal Pradhan[cite: 2]
* **Testing Type:** Functional Black-Box Manual Testing[cite: 2]

---

## 2. Scope of Testing

### 2.1 In Scope
* **Authentication (Login):** Valid credentials, invalid credentials (empty fields, invalid username/password), and error message triggers[cite: 2].
* **Product Catalog (Inventory):** Product listing display, product details, item sorting (Name A-Z/Z-A, Price low-high/high-low), and direct cart addition/removal[cite: 2].
* **Cart Operations (Your Cart):** Cart navigation, single/multiple item display, item removal, cart badge counter synchronization, and "Continue Shopping" navigation[cite: 2].
* **Checkout Workflow:** Customer information input validation (First Name, Postal Code), navigation restrictions (preventing empty cart checkout), order summary review, and order completion flow[cite: 2].

### 2.2 Out of Scope
* Performance and stress/load testing[cite: 2].
* Security, penetration testing, and VAPT[cite: 2].
* Cross-browser and mobile device compatibility testing beyond Google Chrome[cite: 2].
* API and automated Selenium testing (manual execution focus for this phase)[cite: 2].

---

## 3. Test Approach & Methodology
* **Black-Box Testing:** Testing functionality without inspecting internal code structures[cite: 2].
* **Test Case Design:** Utilizing Boundary Value Analysis (BVA) and Equivalence Partitioning (EP) for form fields and checkout validation.
* **Traceability:** Bidirectional traceability maintained through a Requirements Traceability Matrix (RTM) linking Requirements $\leftrightarrow$ Test Cases $\leftrightarrow$ Bug Reports[cite: 2].
* **Defect Management:** Logging reproduction steps, expected vs. actual results, severity, and priority for all failing scenarios[cite: 2].

---

## 4. Test Environment

| Parameter | Configuration |
| :--- | :--- |
| **Application** | SauceDemo (Sauce Labs demo application)[cite: 2] |
| **Browser** | Google Chrome (Latest Stable Version)[cite: 2] |
| **OS** | Windows 11 |
| **Primary Test User** | `standard_user`[cite: 2] |
| **Password** | `secret_sauce`[cite: 2] |
| **Modules Tested** | Login, Inventory, Your Cart, Checkout[cite: 2] |

---

## 5. Test Execution Summary

| Module | Total TCs | Passed | Failed | Blocked | Pass Rate | Defect IDs |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: |
| **Login** | 6 | 6 | 0 | 0 | 100% | None |
| **Inventory** | 11 | 9 | 2 | 0 | 81.8% | Bug-01, Bug-02 |
| **Your Cart** | 10 | 9 | 1 | 0 | 90.0% | Bug-03 |
| **Checkout** | 8 | 7 | 1 | 0 | 87.5% | Bug-04 |
| **Total** | **35** | **31** | **4** | **0** | **88.6%** | **4 Defects** |

---

## 6. Defect Log Summary

| Bug ID | Related TC | Module | Summary / Description | Severity | Priority | Status |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **Bug-01** | `TC_I_02` | Inventory | Incorrect product name displayed for the last item (T-Shirt RED) | Low | P3 | Open |
| **Bug-02** | `TC_I_09` | Inventory | Sorting dropdown arrow icon is unclickable | Low | P3 | Open |
| **Bug-03** | `TC_YC_07` | Your Cart | User is able to proceed to checkout with an empty cart | Medium | P2 | Open |
| **Bug-04** | `TC_CKF_04` | Checkout | Checkout form accepts invalid non-numeric postal codes (e.g., text) | High | P1 | Open |

---

## 7. Entry & Exit Criteria

### 7.1 Entry Criteria
* Target web application is accessible and stable at the test URL[cite: 2].
* Test credentials (`standard_user`) are active and valid[cite: 2].
* Test cases and scenarios have been authored and reviewed[cite: 2].

### 7.2 Exit Criteria
* 100% of planned 35 test cases executed[cite: 2].
* All defects identified during execution are documented with reproduction steps and severity levels[cite: 2].
* Requirements Traceability Matrix (RTM) completed and mapped[cite: 2].
* Test execution summary and completion reports generated[cite: 2].

---

## 8. Test Deliverables
* **Test Plan Document (`test-plan.md`)**[cite: 2]
* **Excel Test Suite (`SauceDemo QA Test Case.xlsx`):** Test cases across 4 modules[cite: 2]
* **Requirements Traceability Matrix (RTM)**[cite: 2]
* **Bug Reports:** Detailed defect documentation[cite: 2]
* **Test Summary Report**[cite: 2]

---

## 9. Risks & Mitigations
* **Application Stability:** SauceDemo is an external sandbox maintained by Sauce Labs with mock user profiles; behavior changes or intentional flaws were isolated against user personas[cite: 3].
* **Execution Evidence:** Test statuses reflect functional manual passes and fails recorded in the primary workbook suite[cite: 2].
