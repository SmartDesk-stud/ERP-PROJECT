# Change Control Process & Log

| Field | Detail |
| --- | --- |
| **Project** | CharterOps ERP System |
| **Document** | Change Control Process & Log |
| **Version** | 2.0 (process v1.0 issued January 9, 2026) |
| **Date** | March 31, 2026 (final update) |
| **Status** | Final – Project Closed |
| **Author** | Morenikeji Bankole (Project Manager) |
| **Approver** | Maryam Abubakar (Project Lead) |

---

## 1. Purpose

The project runs a hybrid model: agile sprint execution with phase-based approvals. Change control is the mechanism that lets the team stay flexible inside a sprint without letting scope, schedule or the production date drift. The charter names scope creep as a top risk (see R-02 in the [Risk Register](04-risk-register.md)); this process is its primary mitigation.

## 2. What Counts as a Change

| Type | Example | Handling |
| --- | --- | --- |
| **In-scope clarification** | Better wording of a defect that is already in scope | Project Manager updates the ClickUp task; no formal request |
| **Scope change** | New feature, bespoke operator configuration, new module | Formal change request |
| **Schedule change** | Moving a phase gate, milestone or release date | Formal change request |
| **Priority or sequencing change** | Re-ordering work inside a phase | Lightweight request, Project Lead approval |
| **Baseline change to out-of-scope items** | Database engine migration, avionics integration, payment gateway renegotiation | Rejected by default (listed as out of scope in the charter) |

## 3. Change Control Process

1. **Raise.** Anyone on the team or a stakeholder submits the request to the Project Manager with a short description and reason.
2. **Log.** The Project Manager assigns a CR number and records it in the log below within one working day.
3. **Assess.** The Project Manager, with the Full Stack Lead and QA, assesses impact on scope, schedule, quality, risk and the P0/P1 defect commitment.
4. **Decide.** The Project Lead decides: **Approve**, **Approve in part**, **Defer** (to a backlog) or **Reject**. Decisions that touch a phase gate are taken at the gate review.
5. **Implement.** Approved items become ClickUp tasks and are placed in a sprint; the WBS and plan are updated.
6. **Close.** The Project Manager confirms completion or deferral and updates the log.

**Decision rules**

- P0/P1 defects are never displaced by a new feature request.
- A change that would move the Phase 4 production date requires explicit Project Lead approval.
- Deferred items go to the SaaS replication backlog, not to the current sprint.

## 4. Change Request Template

| Field | Entry |
| --- | --- |
| CR number | |
| Date raised / Raised by | |
| Description | |
| Reason / benefit | |
| Impact on scope / schedule / quality / risk | |
| Recommendation (Project Manager) | |
| Decision (Project Lead) | Approve / Approve in part / Defer / Reject |
| Decision date | |
| Resulting action | |

## 5. Change Log

| CR | Date Raised | Raised By | Description | Impact Assessment | Decision | Decided By | Outcome |
| --- | --- | --- | --- | --- | --- | --- | --- |
| CR-001 | January 2026 (Phase 2) | Operator-side stakeholders, via the team | Requests for bespoke operator-specific configuration while defect remediation was under way (risk R-02) | Would compete with P0/P1 defect work and add unplanned scope to a small team | **Approved in part / Deferred** | Maryam Abubakar | Branding-related items absorbed into Phase 5 landing pages (WBS 5.1 – 5.3); remaining configuration requests moved to the SaaS replication backlog. No change to the production date. |
| CR-002 | January 2026 (Phase 2, Sprint 1) | Abubakar Suleiman | Re-sequence the maintenance (D-07) and fuel (D-08) defects earlier in Phase 2 so the backend investigation starts in Sprint 1 (risk R-01) | No change to scope; moves two defects from Sprint 2 to an earlier start; supports the early code inspection mitigation | **Approved** | Maryam Abubakar | Investigation began in Sprint 1; both defects fixed and verified within Phase 2. |

## 6. Change Summary

| Metric | Count |
| --- | --- |
| Change requests logged | 2 |
| Approved or approved in part | 2 |
| Rejected | 0 |
| Changes that moved the production release date | 0 |
| Changes that moved a charter phase date | 0 |

## 7. Related Documents

- [Risk Register](04-risk-register.md)
- [Work Breakdown Structure](02-work-breakdown-structure.md)
- [Project Closure Report](12-project-closure-report.md)
