# Deployment & Release Plan

| Field | Detail |
| --- | --- |
| **Project** | CharterOps ERP System |
| **Document** | Deployment & Release Plan |
| **Version** | 1.0 |
| **Date** | February 2, 2026 |
| **Status** | Approved for Execution |
| **Author** | Morenikeji Bankole (Project Manager) |
| **Approver** | Maryam Abubakar (Project Lead) |

---

## 1. Purpose

This plan governs how the hardened CharterOps ERP application moves from staging to production (Phase 4, February 4 – 5, 2026) and how the partner landing pages are released at the end of Phase 5 (February 13, 2026). It also records the release outcomes.

## 2. Release Summary

| Release | Content | Target Window | Owner |
| --- | --- | --- | --- |
| **Release 1.0 – Internal app** | All 12 defect fixes, UI/UX enhancements and form validations | Feb 4 – Feb 5, 2026 | Abubakar Suleiman |
| **Release 1.1 – Landing pages** | Qair and Viva Jets landing pages and portal access | Feb 13, 2026 | Abubakar Suleiman |

Primary system: <https://charter-ops.vercel.app/>

## 3. Environments

| Environment | Purpose | Notes |
| --- | --- | --- |
| Local / preview | Developer checks and preview builds | Vercel preview deployments per change |
| Staging | Verification, regression, release candidate | Must mirror production configuration |
| Production | Live internal app and commercial demo | Hosted on Vercel with CI/CD |

Database engine migration and backend architecture replacement are out of scope; the release deploys application changes only.

## 4. Roles

| Role | Name | Release Responsibility |
| --- | --- | --- |
| Release approver | Maryam Abubakar | Go / No-Go decision |
| Release coordinator | Morenikeji Bankole | Checklist, communication, release record |
| Release engineer | Abubakar Suleiman | Staging cutover, production release, rollback if needed |
| Verification | Sadiq Ilu | Smoke tests before and after release |

## 5. Pre-Release Checklist (complete by Feb 3, 2026)

| # | Item | Owner | Status |
| --- | --- | --- | --- |
| 1 | All Phase 2 defects D-01 – D-12 verified | Sadiq Ilu | Complete |
| 2 | Phase 3 UI/UX work approved at design review | Maryam Abubakar | Complete |
| 3 | Regression pass on staging with no open P0/P1 | Sadiq Ilu | Complete |
| 4 | CI/CD pipeline green on the release branch | Abubakar Suleiman | Complete |
| 5 | Vercel and server credentials confirmed valid (risk R-05) | Morenikeji Bankole | Complete |
| 6 | Rollback path confirmed (previous production deployment retained) | Abubakar Suleiman | Complete |
| 7 | Release note drafted | Morenikeji Bankole | Complete |
| 8 | Team informed of the release window | Morenikeji Bankole | Complete |

## 6. Go / No-Go Criteria

**Go** only if all are true:

- No open P0/P1 defects.
- Regression passed on staging.
- CI/CD build is successful.
- Rollback path is confirmed.
- Project Lead has approved.

Any failed criterion is a **No-Go**; the release moves within the Phase 4 window only with Project Lead approval through change control.

## 7. Deployment Steps

### Day 1 – February 4, 2026: Staging Cutover

1. Freeze changes to the release branch.
2. Deploy the release candidate to staging.
3. Sadiq Ilu runs the smoke test: sign-in, user management, booking, maintenance, fuel, invoice with extra fees, currency display.
4. Record the result; Go / No-Go review with the Project Lead.

### Day 2 – February 5, 2026: Production Release

1. Promote the verified build to production on Vercel.
2. Sadiq Ilu repeats the smoke test on production.
3. Abubakar Suleiman monitors build and runtime logs for errors.
4. Morenikeji Bankole sends the release note to the team and the Project Lead.

### Release 1.1 – February 13, 2026: Landing Pages

1. Complete cross-device and link testing on preview.
2. Obtain the Project Lead's approval of the final pages.
3. Publish the Qair and Viva Jets pages to production.
4. Verify the portal access links and issue the release note.

## 8. Rollback Plan

| Trigger | Action | Decision Maker |
| --- | --- | --- |
| Smoke test failure on production | Re-promote the previous production deployment on Vercel | Abubakar Suleiman, informing the Project Lead |
| Critical error found after release (P0) | Roll back, then diagnose on staging | Project Lead |
| Landing page defect after publish | Revert the page deployment; republish after fix | Abubakar Suleiman |

Rollback target time: under 30 minutes from decision.

## 9. Post-Release Support and Stabilization

- Daily review of errors and user reports from February 6.
- Stabilization continues in the buffer period through March 31, 2026.
- Any production issue is logged in ClickUp and triaged using the P0/P1/P2 definitions.

## 10. Release Record (Actuals)

| Release | Planned | Actual | Outcome |
| --- | --- | --- | --- |
| Release 1.0 – staging cutover | Feb 4 | Feb 4 | Smoke test passed; Go decision |
| Release 1.0 – production | Feb 5 | Feb 5 | Released; production smoke test passed; no rollback |
| Release 1.1 – landing pages | Feb 13 | Feb 13 | Qair and Viva Jets pages live; portal links verified |

## 11. Related Documents

- [Test Plan & UAT Report](09-test-plan-and-uat-report.md)
- [Risk Register](04-risk-register.md)
- [Status Reports](11-status-reports.md)
