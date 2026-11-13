# Risk Register

| Field | Detail |
| --- | --- |
| **Project** | CharterOps ERP System |
| **Document** | Risk Register (with actual outcomes) |
| **Version** | 2.0 (v1.0 issued January 9, 2026) |
| **Date** | March 31, 2026 (final update) |
| **Status** | Final – Project Closed |
| **Author** | Morenikeji Bankole (Project Manager) |
| **Approver** | Maryam Abubakar (Project Lead) |

---

## 1. Purpose and Method

This register was opened in Phase 1 and reviewed weekly through the project. Each risk was scored for **probability (P)** and **impact (I)** on a 1–3 scale (1 = low, 3 = high); **score = P × I**. Scores of 6–9 are High, 3–4 Medium, 1–2 Low. The *Planned Response* columns record what was agreed at the time; the *Outcome* columns record what actually happened and how it was resolved.

## 2. Risk Summary

| Metric | Count |
| --- | --- |
| Risks identified | 8 |
| Risks that occurred | 2 |
| Risks that did not occur (closed) | 6 |
| Open risks at closure | 0 |

## 3. Risk Register

### 3.1 Planned (as at January 9, 2026)

| ID | Risk | Category | P | I | Score | Rating | Owner | Planned Mitigation |
| --- | --- | --- | :-: | :-: | :-: | --- | --- | --- |
| R-01 | **Hidden backend dependencies.** Isolated API failures in maintenance and fuel modules may reveal deeper service issues. | Technical | 3 | 3 | 9 | High | Abubakar Suleiman | Early code inspection by the Full Stack Lead Developer during Phase 2 |
| R-02 | **Scope creep.** Requests for bespoke operator configurations during defect remediation. | Scope | 3 | 2 | 6 | High | Morenikeji Bankole | Strict gatekeeping by the Project Manager through the hybrid change-control process |
| R-03 | **Small-team capacity.** A compact cross-functional team and a single full stack lead create a key-person dependency. | Resource | 2 | 3 | 6 | High | Morenikeji Bankole | Prioritize P0/P1 over new features; Sadiq Ilu as secondary technical reviewer |
| R-04 | **Environment instability.** Development or staging environments or CI/CD become unavailable. | Technical | 2 | 3 | 6 | High | Abubakar Suleiman | Verify staging before each sprint review; keep a rollback path on Vercel |
| R-05 | **Expired access or credentials.** ClickUp, Vercel or internal server credentials and API documentation become stale. | Access | 2 | 2 | 4 | Medium | Morenikeji Bankole | Credential check at kick-off and before Phase 4 |
| R-06 | **Billing regression.** Fixing fee propagation breaks invoice totals or currency formatting. | Quality | 2 | 3 | 6 | High | Sadiq Ilu | Dedicated invoice and currency test cases; regression pass after Phase 3 |
| R-07 | **Brand decision delay.** Logo and brand direction not agreed in time for landing pages. | Schedule | 2 | 2 | 4 | Medium | Maryam Abubakar | Agree logo in Phase 1; brand freeze before Phase 5 |
| R-08 | **Compressed demo readiness.** Phase 6 slips because UAT, demo prep and sign-off share one week. | Schedule | 2 | 3 | 6 | High | Morenikeji Bankole | Pre-write UAT scripts in Phase 3; use the buffer through March 31 for stabilization |

### 3.2 Outcomes (as at March 31, 2026)

| ID | Occurred? | What Happened | How It Was Resolved | Residual Status |
| --- | --- | --- | --- | --- |
| R-01 | **Yes** | The maintenance creation error (D-07) and fuel supply failure (D-08) were API-level failures that were not isolated to the screens reporting them; they needed backend investigation beyond a front-end fix. | The Full Stack Lead inspected the code early in Phase 2, as planned, and the investigation of D-07 and D-08 was moved forward in the sprint plan (see CR-002). Both defects were fixed and verified by Sadiq Ilu within Phase 2. | Closed |
| R-02 | **Yes** | Requests for operator-specific configuration surfaced while defect remediation was under way. | Each request was logged and assessed through change control (see CR-001). Branding-related items were absorbed into Phase 5 landing pages; the remaining configuration requests were deferred to the SaaS replication backlog. P0/P1 defect work was not displaced. | Closed |
| R-03 | No | Team capacity held; P0/P1 defects were prioritized ahead of new features. | n/a | Closed |
| R-04 | No | No loss of staging or CI/CD that affected a milestone. | n/a | Closed |
| R-05 | No | Credentials and access were confirmed before Phase 4 and remained valid. | n/a | Closed |
| R-06 | No | Invoice and currency test cases passed in verification, UAT and regression. | n/a | Closed |
| R-07 | No | Logo direction was agreed in Phase 1 and brand assets were ready for Phase 5. | n/a | Closed |
| R-08 | No | UAT, demo preparation and sign-off were completed within February 16 – 20, 2026. The buffer was used for post-launch stabilization only. | n/a | Closed |

## 4. Issues Raised During the Project

| ID | Issue | Linked Risk | Resolution |
| --- | --- | --- | --- |
| I-01 | Maintenance and fuel API failures required deeper backend investigation | R-01 | Resolved in Phase 2 (D-07, D-08) |
| I-02 | Operator-specific configuration requests arrived during remediation | R-02 | Logged and decided through change control (CR-001) |

## 5. Lessons From Risk Management

- The two risks the charter flagged as top risks were the two that occurred, so naming them early and assigning a mitigation owner paid off.
- Early code inspection turned an unknown backend dependency into a scheduled piece of work.
- A written change-control path let the team say "not now" to configuration requests without delaying P0/P1 work.

## 6. Related Documents

- [Change Control Log](06-change-control-log.md)
- [Defect Log Summary](07-defect-log-summary.md)
- [Project Closure Report](12-project-closure-report.md)
