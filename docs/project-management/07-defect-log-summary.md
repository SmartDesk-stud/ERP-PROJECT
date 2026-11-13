# Defect Log Summary

| Field | Detail |
| --- | --- |
| **Project** | CharterOps ERP System |
| **Document** | Defect Log Summary |
| **Version** | 1.0 |
| **Date** | February 20, 2026 (final status) |
| **Status** | Final – All P0/P1 Defects Resolved |
| **Author** | Morenikeji Bankole (Project Manager) |
| **Approver** | Maryam Abubakar (Project Lead) |

---

## 1. Purpose

This document summarizes the defects identified in the CharterOps ERP System before remediation began, how they were prioritized and how each was resolved and verified. Each defect was raised as a bug task in ClickUp and assigned to the Full Stack Lead Developer, with Sadiq Ilu as the supporting verifier. The charter objective "Zero-Defect Core Workflows" is measured against this log.

## 2. Priority Definitions

| Priority | Definition | Target |
| --- | --- | --- |
| **P0** | System unusable or data loss; blocks all work | Fix immediately |
| **P1** | Core operational workflow broken or financially inaccurate | Fix in Phase 2 (Jan 12 – Jan 23, 2026) |
| **P2** | Workaround exists; usability or cosmetic issue | Schedule after P0/P1 |

## 3. Defect Dashboard

| Metric | Value |
| --- | --- |
| Total defects logged | 12 |
| P0 | 0 |
| P1 | 12 |
| Resolved and verified | 12 |
| Open at project close | 0 |
| Reopened after verification | 0 |
| Modules affected | 6 |

### 3.1 By Module

| Module | Defects | Share |
| --- | :-: | :-: |
| Authentication & Access | 3 | 25% |
| Flight & Aircraft Management (Flight Booking) | 3 | 25% |
| System Configuration | 3 | 25% |
| Aircraft Maintenance | 1 | 8% |
| Fuel Management | 1 | 8% |
| Payment & Transaction | 1 | 8% |

### 3.2 By Type

| Type | Defects | Defect IDs |
| --- | :-: | --- |
| Account management restriction | 2 | D-01, D-02 |
| Missing feedback on failure | 1 | D-03 |
| Data integrity (retrieval and duplication) | 2 | D-04, D-06 |
| Duplicate UI action | 1 | D-05 |
| Backend / API failure | 2 | D-07, D-08 |
| Financial accuracy | 1 | D-09 |
| Input validation | 2 | D-10, D-11 |
| Display / formatting | 1 | D-12 |

## 4. Defect Register

| ID | Module | Sub-area | Summary | Description (as reported) | Priority | Assignee | Verifier | Sprint | Status |
| --- | --- | --- | --- | --- | :-: | --- | --- | :-: | --- |
| D-01 | Authentication & Access | Admin user creation | Admin account cannot be edited without deactivation | An admin profile was created successfully, but after creation the account could not be edited or updated unless it was first deactivated, limiting administrative control | P1 | Abubakar Suleiman | Sadiq Ilu | 1 | Resolved – Verified |
| D-02 | Authentication & Access | Admin user creation | Partner account cannot be edited without deactivation | Post-creation account management of partner accounts was restricted | P1 | Abubakar Suleiman | Sadiq Ilu | 1 | Resolved – Verified |
| D-03 | Authentication & Access | Crew registration | Crew account creation fails with no feedback | Crew account creation did not complete after submission, with no confirmation or error message | P1 | Abubakar Suleiman | Sadiq Ilu | 1 | Resolved – Verified |
| D-04 | Flight & Aircraft Management | Flight booking | Booking not found after submission | A submitted booking did not appear after completion | P1 | Abubakar Suleiman | Sadiq Ilu | 1 | Resolved – Verified |
| D-05 | Flight & Aircraft Management | Flight booking | Duplicated "Finish" buttons | At final submission both "Finish & Save" and "Finish" appeared | P1 | Abubakar Suleiman | Sadiq Ilu | 1 | Resolved – Verified |
| D-06 | Flight & Aircraft Management | Flight booking | Passenger data duplicated | Adding passengers after booking duplicated passenger records | P1 | Abubakar Suleiman | Sadiq Ilu | 1 | Resolved – Verified |
| D-07 | Aircraft Maintenance | Add maintenance | Maintenance record cannot be created | The action failed with a "failed with status code" response, indicating a backend or API issue | P1 | Abubakar Suleiman | Sadiq Ilu | 2 | Resolved – Verified |
| D-08 | Fuel Management | Add fuel | Fuel supply cannot be added | The request failed with a "Failed Request" message | P1 | Abubakar Suleiman | Sadiq Ilu | 2 | Resolved – Verified |
| D-09 | System Configuration | Additional services | Extra service fees missing from receipt and invoice | Extra fees added to a client's booking did not reflect on the client's invoice | P1 | Abubakar Suleiman | Sadiq Ilu | 2 | Resolved – Verified |
| D-10 | System Configuration | Phone number | Invalid phone numbers accepted | Phone number validation was not effective | P1 | Abubakar Suleiman | Sadiq Ilu | 2 | Resolved – Verified |
| D-11 | System Configuration | Email | Invalid emails accepted | Email validation was not effective | P1 | Abubakar Suleiman | Sadiq Ilu | 2 | Resolved – Verified |
| D-12 | Payment & Transaction | Currency display | Selected currency symbol missing on dashboard | Amounts were shown without the selected currency symbol | P1 | Abubakar Suleiman | Sadiq Ilu | 2 | Resolved – Verified |

> Sprint numbers refer to the [Sprint Plan & Reports](08-sprint-plan-and-reports.md). D-07 and D-08 were investigated from Sprint 1 under change request CR-002 and closed in Sprint 2.

## 5. Resolution Workflow

1. Defect raised as a ClickUp bug task with priority, module and description.
2. Full Stack Lead reproduces, fixes and moves the task to review.
3. Sadiq Ilu verifies in staging against the test case in the [Test Plan](09-test-plan-and-uat-report.md); failed verification returns the task to the developer.
4. Verified fix is regression tested after Phase 3 and again in UAT.
5. Task closed only after verification evidence is attached.

## 6. Analysis

- **Hardest category:** the backend / API failures (D-07, D-08). Unlike the front-end defects, they pointed to dependencies beyond the screens where they appeared, which is the hidden backend dependency risk (R-01) described in the [Risk Register](04-risk-register.md).
- **Highest business exposure:** D-09 (extra fees missing from invoices) because it affected the accuracy of client billing; it received dedicated invoice test cases.
- **Cluster pattern:** three of the twelve defects were in Authentication and three in Flight Booking, which is why those two modules received the first sprint.
- **Reopened defects:** none.

## 7. Related Documents

- [Test Plan & UAT Report](09-test-plan-and-uat-report.md)
- [Risk Register](04-risk-register.md)
- [Project Closure Report](12-project-closure-report.md)
