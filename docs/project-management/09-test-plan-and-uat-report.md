# Test Plan & UAT Report

| Field | Detail |
| --- | --- |
| **Project** | CharterOps ERP System |
| **Document** | Test Plan & User Acceptance Testing (UAT) Report |
| **Version** | 2.0 (test plan v1.0 issued January 9, 2026) |
| **Date** | February 20, 2026 (UAT report) |
| **Status** | Final – UAT Passed |
| **Author** | Morenikeji Bankole (Project Manager) |
| **Approver** | Maryam Abubakar (Project Lead) |

---

# Part A – Test Plan

## 1. Objectives

- Confirm every P1 defect in the [Defect Log](07-defect-log-summary.md) is fixed and stays fixed.
- Confirm that dynamic service fees reach client invoices and that currency symbols render correctly.
- Confirm that UI and workflow changes do not break existing operations.
- Confirm that the Qair and Viva Jets landing pages work on common devices.
- Provide acceptance evidence for the commercial demo.

## 2. Scope

**In scope:** authentication and access, flight booking, aircraft maintenance, fuel management, system configuration (validation, additional services), payment and currency display, UI/UX changes, landing pages.

**Out of scope:** database engine migration, avionics hardware integration, third-party payment gateway renegotiation (per charter).

## 3. Test Levels and Approach

| Level | When | Performed By | Environment | Purpose |
| --- | --- | --- | --- | --- |
| Developer check | During each fix | Abubakar Suleiman | Local / preview | Reproduce and confirm fix |
| Defect verification | After each fix (Phase 2) | Sadiq Ilu | Staging | Confirm the defect is resolved against its test case |
| Regression | End of Phase 3 and before release | Sadiq Ilu, David, Ahmad | Staging | Confirm earlier fixes survive UI changes |
| Release smoke test | Phase 4 | Sadiq Ilu | Staging, then production | Confirm release is healthy |
| Landing page QA | Phase 5 | Sadiq Ilu, David, Ahmad | Preview, then production | Layout, links, responsiveness |
| User acceptance testing | Phase 6 (Feb 16 – Feb 20) | Sadiq Ilu, Morenikeji Bankole, with Maryam Abubakar accepting | Production-equivalent | Validate end-to-end journeys |

## 4. Entry and Exit Criteria

| Stage | Entry Criteria | Exit Criteria |
| --- | --- | --- |
| Defect verification | Fix deployed to staging; ClickUp task in review | Test case passes; evidence attached |
| Release (Phase 4) | All Phase 2 and 3 items verified; regression passed | No open P0/P1 defects; Go decision recorded |
| UAT (Phase 6) | Production release complete; landing pages live; UAT scripts approved | All critical journeys pass; no open P0/P1 defects; Project Lead acceptance |

## 5. Defect Severity During Testing

New defects found in testing are logged in ClickUp using the P0/P1/P2 definitions in the Defect Log. Any P0/P1 blocks the exit criteria.

## 6. Test Cases

### 6.1 Defect Verification Cases

| ID | Defect | Test Case | Expected Result |
| --- | --- | --- | --- |
| TC-01 | D-01 | Create an admin user, then edit the profile without deactivating | Edit saves; account remains active |
| TC-02 | D-02 | Create a partner account, then edit it without deactivating | Edit saves; account remains active |
| TC-03 | D-03 | Submit the crew registration form (valid data, then invalid data) | Valid: account created with confirmation. Invalid: clear error message |
| TC-04 | D-04 | Complete a flight booking and search for it | Booking appears in the booking list |
| TC-05 | D-05 | Reach the final submission step of a booking | Single, clear final action is shown |
| TC-06 | D-06 | Add passengers to an existing booking | Each passenger appears once; no duplicates |
| TC-07 | D-07 | Create a new aircraft maintenance record | Record saved without error and visible in the list |
| TC-08 | D-08 | Add a fuel supply entry | Entry saved and visible in fuel records |
| TC-09 | D-09 | Add an extra service fee to a client booking, then open the invoice and receipt | Fee appears as a line item; totals are correct |
| TC-10 | D-10 | Enter invalid phone numbers (letters, wrong length) | Submission rejected with a clear message |
| TC-11 | D-11 | Enter invalid email formats | Submission rejected with a clear message |
| TC-12 | D-12 | Select different currencies and open dashboards | Correct symbol shown beside every amount |

### 6.2 Regression, Landing Page and UAT Cases

| ID | Area | Test Case | Expected Result |
| --- | --- | --- | --- |
| TC-13 | Regression | Re-run TC-01 – TC-12 after Phase 3 UI changes | All pass |
| TC-14 | Workflow | Dispatcher completes booking from start to invoice | No duplicate actions; invoice accurate |
| TC-15 | Workflow | Administrator manages users end to end | No forced deactivation; clear feedback |
| TC-16 | Workflow | Crew member registers and signs in | Registration succeeds with feedback |
| TC-17 | Operations | Log maintenance and fuel for an aircraft | Both records saved and retrievable |
| TC-18 | Billing | Booking with multiple add-on fees in a non-default currency | Invoice shows all fees with the correct symbol |
| TC-19 | Landing page | Open the Qair page on desktop, tablet and mobile | Layout responsive; branding correct; portal link works |
| TC-20 | Landing page | Open the Viva Jets page on desktop, tablet and mobile | Layout responsive; branding correct; portal link works |
| TC-21 | Demo | Run the end-to-end demo journey in the sandbox | Journey completes without errors |

---

# Part B – UAT Report

## 7. UAT Summary

| Item | Detail |
| --- | --- |
| UAT window | February 16 – February 20, 2026 (Phase 6) |
| Environment | Production-equivalent, using the sandbox prepared for demonstration |
| Testers | Sadiq Ilu, Morenikeji Bankole (execution); David and Ahmad (landing pages and UI support); Abubakar Suleiman (fix support) |
| Accepting authority | Maryam Abubakar (Project Lead) |
| **Overall result** | **Passed** |

## 8. Results

| Test Group | Scope | Result |
| --- | --- | --- |
| Defect verification (TC-01 – TC-12) | One case for each of the 12 logged defects | Passed |
| Regression (TC-13) | Re-run of defect cases after UI changes | Passed |
| Workflow and operations (TC-14 – TC-17) | Dispatcher, administrator, crew, maintenance and fuel journeys | Passed |
| Billing and currency (TC-18) | Add-on fees and currency symbols on invoices | Passed |
| Landing pages (TC-19, TC-20) | Qair and Viva Jets pages across devices | Passed |
| Demo journey (TC-21) | End-to-end demonstration path in the sandbox | Passed |

**Overall:** every planned test group passed.

## 9. Defects Found During UAT

No P0 or P1 defects were open at sign-off. Any minor observations were handled through the normal ClickUp triage process.

## 10. Acceptance Decision

All exit criteria were met: all critical journeys passed and no P0/P1 defect was open. The Project Lead accepted the system as ready for commercial demonstration, and the commercial demo was held within the Phase 6 window.

| Role | Name | Decision |
| --- | --- | --- |
| Project Lead | Maryam Abubakar | Accepted |
| Project Manager | Morenikeji Bankole | Recommended for acceptance |
| QA | Sadiq Ilu | Test evidence confirmed |

## 11. Related Documents

- [Defect Log Summary](07-defect-log-summary.md)
- [Deployment & Release Plan](10-deployment-release-plan.md)
- [Project Closure Report](12-project-closure-report.md)
