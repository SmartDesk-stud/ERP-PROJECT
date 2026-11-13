# Stakeholder Register & RACI Matrix

| Field | Detail |
| --- | --- |
| **Project** | CharterOps ERP System |
| **Document** | Stakeholder Register & RACI Matrix |
| **Version** | 1.0 |
| **Date** | January 6, 2026 |
| **Status** | Approved for Execution |
| **Author** | Morenikeji Bankole (Project Manager) |
| **Approver** | Maryam Abubakar (Project Lead) |

---

## 1. Stakeholder Register

### 1.1 Core Project Team

| ID | Name | Role | Responsibilities | Influence | Interest | Engagement Approach |
| --- | --- | --- | --- | --- | --- | --- |
| S-01 | Maryam Abubakar | Project Lead / Sponsor | Strategic direction, stage-gate design approvals, resource allocation, final acceptance | High | High | Manage closely: weekly status report, phase-gate approvals |
| S-02 | Morenikeji Bankole | Project Manager | Scope control, sprint coordination, cross-functional communication, risk management, schedule delivery | High | High | Owns plan, reporting and change control |
| S-03 | Abubakar Suleiman | Full Stack Lead Developer | Backend and frontend engineering, API defect resolution, database logic, deployment | High | High | Daily stand-up, direct task assignment |
| S-04 | Sadiq Ilu | Technical Support / QA | Test verification, secondary technical review, defect validation, deployment support | Medium | High | Daily stand-up, verification gate on every defect |
| S-05 | David | Engineering Contributor | Frontend UI development, landing page builds, QA testing | Medium | High | Sprint tasks, design review feedback |
| S-06 | Ahmad | Engineering Contributor | Frontend UI development, landing page builds, QA testing | Medium | High | Sprint tasks, design review feedback |

### 1.2 External and Business Stakeholders

| ID | Stakeholder | Interest in the Project | Influence | Interest | Engagement Approach |
| --- | --- | --- | --- | --- | --- |
| S-07 | Qair (partner operator) | Branded landing page and portal access for its operations | Medium | High | Keep informed; review of landing page before release |
| S-08 | Viva Jets (partner operator) | Branded landing page and portal access for its operations | Medium | High | Keep informed; review of landing page before release |
| S-09 | Prospective enterprise buyers | Commercial demonstration of a dependable, multi-operator platform | High | Medium | Keep satisfied: demo-ready environment and user journeys |
| S-10 | Dispatchers, flight crew and administrators (end users) | Fewer errors, faster data entry, accurate invoices | Medium | High | Keep informed through release notes; feedback during UAT |

## 2. Stakeholder Power / Interest Grid

| | **Low Interest** | **High Interest** |
| --- | --- | --- |
| **High Power** | Prospective enterprise buyers (keep satisfied) | Maryam Abubakar, Morenikeji Bankole, Abubakar Suleiman (manage closely) |
| **Lower Power** | – | Sadiq Ilu, David, Ahmad, Qair, Viva Jets, end users (keep informed / involved) |

## 3. RACI Matrix

**R** = Responsible, **A** = Accountable, **C** = Consulted, **I** = Informed

| Activity | Maryam Abubakar | Morenikeji Bankole | Abubakar Suleiman | Sadiq Ilu | David | Ahmad |
| --- | :---: | :---: | :---: | :---: | :---: | :---: |
| Project charter and scope approval | A | R | C | C | I | I |
| Project plan, roadmap and WBS | A | R | C | C | I | I |
| Kick-off approval | A | R | I | I | I | I |
| Requirements and defect triage | A | R | C | C | I | I |
| Defect remediation (P1) | I | A | R | C | I | I |
| Defect verification and regression | I | A | C | R | C | C |
| Billing / invoice accuracy fixes | A | C | R | R | I | I |
| UI/UX enhancement and form validation | A | C | R | C | R | R |
| Design review and stage-gate approval | A / R | C | C | I | C | C |
| Landing pages (Qair, Viva Jets) | A | C | C | C | R | R |
| Logo and brand asset decision | A / R | C | I | I | C | C |
| Production deployment | A | C | R | R | I | I |
| Risk register maintenance | I | A / R | C | C | I | I |
| Change control decisions | A | R | C | C | I | I |
| Sprint planning and stand-ups | I | A / R | R | R | R | R |
| Status reporting | I | A / R | C | C | I | I |
| User acceptance testing | A | R | C | R | C | C |
| Demo preparation and delivery | A / R | R | R | C | C | C |
| Project sign-off and closure | A | R | C | C | I | I |

## 4. Escalation Path

1. Task owner raises the issue to the Project Manager (same day).
2. Project Manager escalates to the Project Lead if it threatens a phase gate, a P0/P1 target or the production release date.
3. Project Lead decides; the decision is recorded in the [Change Control Log](06-change-control-log.md) or [Risk Register](04-risk-register.md).

## 5. Related Documents

- [Communication Plan](05-communication-plan.md)
- [Work Breakdown Structure](02-work-breakdown-structure.md)
