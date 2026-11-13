# Sprint Plan & Sprint Reports

| Field | Detail |
| --- | --- |
| **Project** | CharterOps ERP System |
| **Document** | Sprint Plan & Sprint Reports |
| **Version** | 2.0 (plan v1.0 issued January 9, 2026) |
| **Date** | February 20, 2026 (final report) |
| **Status** | Final – All Sprints Closed |
| **Author** | Morenikeji Bankole (Project Manager) |
| **Approver** | Maryam Abubakar (Project Lead) |

---

## 1. Delivery Approach

The project uses a hybrid model: **Agile sprint execution inside Waterfall phase gates**. Each charter phase is delivered as one or more sprints; the Project Lead approves each phase at its gate. Sprints are one week long, planned in ClickUp, with a daily 15-minute stand-up, a sprint review and a short sprint report.

## 2. Sprint Calendar

| Sprint | Charter Phase | Dates (2026) | Sprint Goal |
| --- | --- | --- | --- |
| Sprint 0 | Phase 1 | Jan 5 – Jan 9 | Initiate, plan and onboard the team |
| Sprint 1 | Phase 2 | Jan 12 – Jan 16 | Fix Authentication and Flight Booking defects; begin backend investigation |
| Sprint 2 | Phase 2 | Jan 19 – Jan 23 | Fix Maintenance, Fuel, billing, validation and currency defects |
| Sprint 3 | Phase 3 | Jan 26 – Feb 2 | UI/UX enhancement, workflow optimization and form validation |
| Sprint 4 | Phase 4 | Feb 4 – Feb 5 | Production release of the internal app |
| Sprint 5 | Phase 5 | Feb 9 – Feb 13 | Qair and Viva Jets landing pages |
| Sprint 6 | Phase 6 | Feb 16 – Feb 20 | UAT, demo readiness and project sign-off |
| Stabilization | Buffer | Feb 23 – Mar 31 | Post-launch monitoring and fixes |

## 3. Sprint Plan (Planned Scope)

### Sprint 0 – Initiation and Planning (Jan 5 – Jan 9)

| Item | Owner |
| --- | --- |
| System walkthrough and scope confirmation | Maryam Abubakar |
| Project review report, roadmap, plan, WBS | Morenikeji Bankole |
| Kick-off approval request | Morenikeji Bankole |
| Logo options shared with the team | Maryam Abubakar |

### Sprint 1 – Defect Remediation, Part 1 (Jan 12 – Jan 16)

| Item | Defect | Owner |
| --- | --- | --- |
| Admin edits without deactivation | D-01 | Abubakar Suleiman |
| Partner edits without deactivation | D-02 | Abubakar Suleiman |
| Crew account creation feedback | D-03 | Abubakar Suleiman |
| Booking retrievable after submission | D-04 | Abubakar Suleiman |
| Remove duplicated Finish buttons | D-05 | Abubakar Suleiman |
| Passenger duplication | D-06 | Abubakar Suleiman |
| Begin backend investigation of maintenance and fuel failures | D-07, D-08 (investigation) | Abubakar Suleiman |
| Verification of each fix | D-01 – D-06 | Sadiq Ilu |

### Sprint 2 – Defect Remediation, Part 2 (Jan 19 – Jan 23)

| Item | Defect | Owner |
| --- | --- | --- |
| Maintenance creation API error | D-07 | Abubakar Suleiman |
| Fuel supply failed request | D-08 | Abubakar Suleiman |
| Additional service fees on invoice | D-09 | Abubakar Suleiman |
| Phone number validation | D-10 | Abubakar Suleiman |
| Email validation | D-11 | Abubakar Suleiman |
| Currency symbol on dashboards | D-12 | Abubakar Suleiman |
| Verification and Phase 2 regression | D-07 – D-12 | Sadiq Ilu |

### Sprint 3 – UI/UX Enhancement (Jan 26 – Feb 2)

| Item | Owner |
| --- | --- |
| Workflow optimization (remove duplicate actions, streamline steps) | Abubakar Suleiman |
| Form validation and user feedback across forms | Abubakar Suleiman, David, Ahmad |
| User flow enhancements for dispatchers, crew and administrators | David, Ahmad |
| Design review and approval | Maryam Abubakar |
| Regression test of Phase 2 fixes | Sadiq Ilu |
| Draft UAT scripts | Morenikeji Bankole, Sadiq Ilu |

### Sprint 4 – Production Release (Feb 4 – Feb 5)

| Item | Owner |
| --- | --- |
| Go / No-Go review | Morenikeji Bankole |
| Staging cutover and smoke test | Abubakar Suleiman |
| Production release on Vercel | Abubakar Suleiman |
| Production smoke test | Sadiq Ilu |

### Sprint 5 – Landing Pages (Feb 9 – Feb 13)

| Item | Owner |
| --- | --- |
| Final brand assets | Maryam Abubakar |
| Qair landing page | David, Ahmad |
| Viva Jets landing page | David, Ahmad |
| Cross-device and link testing | Sadiq Ilu |
| Publish pages | Abubakar Suleiman |

### Sprint 6 – UAT, Demo and Close (Feb 16 – Feb 20)

| Item | Owner |
| --- | --- |
| Execute UAT scripts | Sadiq Ilu, Morenikeji Bankole |
| Demo journeys and sandbox environment | Morenikeji Bankole, Abubakar Suleiman |
| Commercial demo | Maryam Abubakar |
| Project sign-off | Maryam Abubakar |

## 4. Sprint Reports

### Sprint 0 Report (closed Jan 9)

| Measure | Result |
| --- | --- |
| Goal met | Yes |
| Completed | System walkthrough, project review report, roadmap, plan, WBS, kick-off approval path, logo options shared |
| Carried over | None |
| Notes | Team knowledge-transfer task continues through the project |

### Sprint 1 Report (closed Jan 16)

| Measure | Result |
| --- | --- |
| Goal met | Yes |
| Planned defects | D-01 – D-06, plus investigation start for D-07 / D-08 |
| Resolved and verified | All planned defects |
| Carried over | None |
| Risks and issues | R-01 materialized: maintenance and fuel failures confirmed as backend-related; handled through CR-002 |
| Retrospective | Early code inspection made the later fixes predictable; keep verification inside the same sprint as the fix |

### Sprint 2 Report (closed Jan 23)

| Measure | Result |
| --- | --- |
| Goal met | Yes |
| Planned defects | D-07 – D-12 |
| Resolved and verified | All planned defects |
| Carried over | None |
| Phase 2 gate | All P1 defects resolved; gate approved by the Project Lead |
| Retrospective | Dedicated invoice and currency test cases caught formatting differences before verification |

### Sprint 3 Report (closed Feb 2)

| Measure | Result |
| --- | --- |
| Goal met | Yes |
| Completed | Workflow optimization, form validation, user flow enhancements, design review, regression test |
| Carried over | None |
| Risks and issues | R-02 active: operator configuration requests managed through CR-001 |
| Phase 3 gate | Approved |
| Retrospective | Written design approval from the Project Lead removed rework |

### Sprint 4 Report (closed Feb 5)

| Measure | Result |
| --- | --- |
| Goal met | Yes |
| Completed | Go / No-Go review, staging cutover, production release, production smoke test |
| Carried over | None |
| Phase 4 gate | Approved; see [Deployment & Release Plan](10-deployment-release-plan.md) |

### Sprint 5 Report (closed Feb 13)

| Measure | Result |
| --- | --- |
| Goal met | Yes |
| Completed | Qair and Viva Jets landing pages built, tested and published |
| Carried over | None |
| Phase 5 gate | Approved |

### Sprint 6 Report (closed Feb 20)

| Measure | Result |
| --- | --- |
| Goal met | Yes |
| Completed | UAT executed, demo held, sign-off obtained; see [Test Plan & UAT Report](09-test-plan-and-uat-report.md) |
| Carried over | None |
| Phase 6 gate | Approved; project moved to post-launch stabilization |

## 5. Delivery Summary

All planned work in every sprint was completed and no items were carried over. Every sprint goal was met, and each phase gate was approved by the Project Lead.

## 6. Related Documents

- [Defect Log Summary](07-defect-log-summary.md)
- [Status Reports](11-status-reports.md)
- [Work Breakdown Structure](02-work-breakdown-structure.md)
