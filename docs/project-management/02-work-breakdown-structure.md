# Work Breakdown Structure (WBS)

| Field | Detail |
| --- | --- |
| **Project** | CharterOps ERP System |
| **Document** | Work Breakdown Structure |
| **Version** | 1.0 |
| **Date** | January 9, 2026 |
| **Status** | Approved for Execution |
| **Author** | Morenikeji Bankole (Project Manager) |
| **Approver** | Maryam Abubakar (Project Lead) |

---

## 1. Purpose

This WBS decomposes the CharterOps ERP System Revamp & SaaS Readiness project into manageable work packages. It follows the scope in the [Project Charter](01-project-charter.md) and the phase plan (January 5 – March 31, 2026). Every work package maps to a charter phase, an owner and a ClickUp task, so progress can be tracked consistently across the hybrid (Agile + Waterfall) delivery model.

## 2. WBS Hierarchy

```
1.0  CharterOps ERP System Revamp & SaaS Readiness
├── 1.0  Project Initiation, Planning & Team Onboarding   (Phase 1)
├── 2.0  Defect Remediation & Stabilization               (Phase 2)
├── 3.0  UI/UX Enhancement & Feature Optimization         (Phase 3)
├── 4.0  Production Deployment (Internal App)             (Phase 4)
├── 5.0  Landing Page Development & Partner Branding      (Phase 5)
├── 6.0  Final Testing, Demo Readiness & Project Close    (Phase 6)
└── 7.0  Project Management (continuous)
```

## 3. WBS Dictionary

### 1.0 Project Initiation, Planning & Team Onboarding (Phase 1: Jan 5 – Jan 9, 2026)

| WBS ID | Work Package | Description | Owner | Deliverable |
| --- | --- | --- | --- | --- |
| 1.1 | System walkthrough / demo | Walk the team through the existing CharterOps ERP and agree scope | Maryam Abubakar | Shared understanding of system flow |
| 1.2 | Requirements gathering | Draft project review report and goal summary | Morenikeji Bankole | Project Review Report |
| 1.3 | Project roadmap | Design roadmap, SOPs and workflow | Morenikeji Bankole | Project Roadmap |
| 1.4 | Project plan | Task owners, timelines, dependencies | Morenikeji Bankole | Project Plan (ClickUp + spreadsheet) |
| 1.5 | Kick-off approval | Request and receive management approval to start | Morenikeji Bankole | Approved kick-off |
| 1.6 | Logo and brand direction | Team agrees on the new logo from the proposed options | Maryam Abubakar | Agreed logo direction |
| 1.7 | Team knowledge transfer | Team builds understanding of ERP flows as work progresses (runs to project end) | All | Team readiness |

### 2.0 Defect Remediation & Stabilization (Phase 2: Jan 12 – Jan 23, 2026)

| WBS ID | Module | Work Package | Defect Ref | Priority | Assignee / Supporter |
| --- | --- | --- | --- | --- | --- |
| 2.1 | Authentication & Access | Allow admin account edits without deactivation | D-01 | P1 | Abubakar Suleiman / Sadiq Ilu |
| 2.2 | Authentication & Access | Allow partner account edits without deactivation | D-02 | P1 | Abubakar Suleiman / Sadiq Ilu |
| 2.3 | Authentication & Access | Fix crew account creation (add confirmation and error feedback) | D-03 | P1 | Abubakar Suleiman / Sadiq Ilu |
| 2.4 | Flight Booking | Booking must be retrievable after submission | D-04 | P1 | Abubakar Suleiman / Sadiq Ilu |
| 2.5 | Flight Booking | Remove duplicated "Finish" buttons at final submission | D-05 | P1 | Abubakar Suleiman / Sadiq Ilu |
| 2.6 | Flight Booking | Stop passenger data duplication when adding passengers after booking | D-06 | P1 | Abubakar Suleiman / Sadiq Ilu |
| 2.7 | Aircraft Maintenance | Resolve API error when creating a maintenance record | D-07 | P1 | Abubakar Suleiman / Sadiq Ilu |
| 2.8 | Fuel Management | Resolve failed request when adding a fuel supply | D-08 | P1 | Abubakar Suleiman / Sadiq Ilu |
| 2.9 | System Configuration | Reflect additional service fees on receipts and invoices | D-09 | P1 | Abubakar Suleiman / Sadiq Ilu |
| 2.10 | System Configuration | Enforce valid phone number input | D-10 | P1 | Abubakar Suleiman / Sadiq Ilu |
| 2.11 | System Configuration | Enforce valid email input | D-11 | P1 | Abubakar Suleiman / Sadiq Ilu |
| 2.12 | Payment & Transaction | Display the selected currency symbol on dashboards | D-12 | P1 | Abubakar Suleiman / Sadiq Ilu |
| 2.13 | Verification | Defect validation and regression pass | – | P1 | Sadiq Ilu |

### 3.0 UI/UX Enhancement & Feature Optimization (Phase 3: Jan 26 – Feb 2, 2026)

| WBS ID | Work Package | Description | Owner |
| --- | --- | --- | --- |
| 3.1 | Workflow optimization | Remove duplicate actions and streamline multi-step flows | Abubakar Suleiman |
| 3.2 | Form validation | Consistent validation and user feedback across forms | Abubakar Suleiman, David, Ahmad |
| 3.3 | User flow enhancements | Improve navigation and data entry for dispatchers, crew and administrators | David, Ahmad |
| 3.4 | Design review | Stage-gate design review and approval | Maryam Abubakar |
| 3.5 | Regression testing | Re-test Phase 2 fixes against UI changes | Sadiq Ilu |

### 4.0 Production Deployment – Internal App (Phase 4: Feb 4 – Feb 5, 2026)

| WBS ID | Work Package | Description | Owner |
| --- | --- | --- | --- |
| 4.1 | Release readiness review | Go / No-Go checklist | Morenikeji Bankole |
| 4.2 | Staging cutover | Deploy release candidate to staging and smoke test | Abubakar Suleiman |
| 4.3 | Production release | Promote to production on Vercel | Abubakar Suleiman |
| 4.4 | Post-release verification | Production smoke test and monitoring | Sadiq Ilu |

### 5.0 Landing Page Development & Partner Branding (Phase 5: Feb 9 – Feb 13, 2026)

| WBS ID | Work Package | Description | Owner |
| --- | --- | --- | --- |
| 5.1 | Brand assets | Finalize logo and brand assets | Maryam Abubakar |
| 5.2 | Qair portal landing page | Responsive branded page and portal access | David, Ahmad |
| 5.3 | Viva Jets portal landing page | Responsive branded page and portal access | David, Ahmad |
| 5.4 | Landing page QA | Cross-device and link testing | Sadiq Ilu |
| 5.5 | Landing page release | Publish pages | Abubakar Suleiman |

### 6.0 Final Testing, Commercial Demo Readiness & Project Close (Phase 6: Feb 16 – Feb 20, 2026)

| WBS ID | Work Package | Description | Owner |
| --- | --- | --- | --- |
| 6.1 | User acceptance testing | Execute UAT scripts end to end | Sadiq Ilu, Morenikeji Bankole |
| 6.2 | Demo preparation | End-to-end user journeys and sandbox environment | Morenikeji Bankole, Abubakar Suleiman |
| 6.3 | Commercial demo | Demonstration to prospective buyers | Maryam Abubakar |
| 6.4 | Project sign-off | Final acceptance by the Project Lead | Maryam Abubakar |

### 7.0 Project Management (continuous, Jan 5 – Mar 31, 2026)

| WBS ID | Work Package | Description | Owner |
| --- | --- | --- | --- |
| 7.1 | Scope and change control | Gatekeeping of requests through the change process | Morenikeji Bankole |
| 7.2 | Sprint coordination | Planning, stand-ups, reviews | Morenikeji Bankole |
| 7.3 | Risk and issue management | Maintain the risk register | Morenikeji Bankole |
| 7.4 | Status reporting | Weekly status reports | Morenikeji Bankole |
| 7.5 | Post-launch stabilization (buffer) | Monitoring and fixes through March 31, 2026 | Abubakar Suleiman, Sadiq Ilu |
| 7.6 | Project closure | Closure report and lessons learned | Morenikeji Bankole |

## 4. Assumptions

- Work packages are tracked as ClickUp tasks and carry the priority shown in the project plan.
- All remediation items are P1 and are completed in Phase 2; new feature work does not displace P0/P1 defects.
- Database engine migration and avionics hardware integrations are out of scope (see charter section 4).

## 5. Related Documents

- [Stakeholder Register & RACI](03-stakeholder-register-and-raci.md)
- [Risk Register](04-risk-register.md)
- [Sprint Plan & Reports](08-sprint-plan-and-reports.md)
