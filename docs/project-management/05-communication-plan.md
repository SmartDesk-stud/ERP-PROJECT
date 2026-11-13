# Communication Plan

| Field | Detail |
| --- | --- |
| **Project** | CharterOps ERP System |
| **Document** | Communication Plan |
| **Version** | 1.0 |
| **Date** | January 9, 2026 |
| **Status** | Approved for Execution |
| **Author** | Morenikeji Bankole (Project Manager) |
| **Approver** | Maryam Abubakar (Project Lead) |

---

## 1. Purpose

This plan defines who receives which project information, how often, through which channel and who is responsible for sending it. The team is small and cross-functional, so the plan favors short, regular, written updates with a single place for task truth (ClickUp).

## 2. Communication Principles

- **One source of truth for work:** every task, defect and status lives in ClickUp. Chat is for coordination, not for decisions of record.
- **Decisions are written down:** scope, priority and design decisions are recorded in the [Change Control Log](06-change-control-log.md) or the [Risk Register](04-risk-register.md).
- **Bad news travels early:** any threat to a P0/P1 target or a phase gate is escalated the same day.
- **Right-sized meetings:** short and frequent for the delivery team, formal only at phase gates.

## 3. Channels and Tools

| Channel | Purpose | Owner |
| --- | --- | --- |
| ClickUp | Task and defect tracking, assignments, priorities, status | Morenikeji Bankole |
| Team group chat | Day-to-day coordination, quick questions, sharing design options (such as logo candidates) | All |
| Cloud-hosted project documents | Project review report, roadmap, plan, reports | Morenikeji Bankole |
| Project plan spreadsheet | Phases, timelines, dependencies, milestones | Morenikeji Bankole |
| Email | Formal approvals, partner and buyer communication | Maryam Abubakar, Morenikeji Bankole |
| Vercel | Deployment status and preview/production builds | Abubakar Suleiman |

## 4. Communication Matrix

| ID | Communication | Audience | Purpose | Frequency | Format / Channel | Owner |
| --- | --- | --- | --- | --- | --- | --- |
| C-01 | Project kick-off | Whole team, Project Lead | Align on scope, roles, timeline | Once (Phase 1) | Meeting + approval record | Morenikeji Bankole |
| C-02 | Daily stand-up | Delivery team | Progress, blockers, today's focus | Daily (15 minutes) | Short call or written update in group chat | Morenikeji Bankole |
| C-03 | Sprint planning | Delivery team | Commit sprint scope from ClickUp | Start of each sprint | Meeting | Morenikeji Bankole |
| C-04 | Sprint review | Delivery team, Project Lead | Demonstrate completed work, accept items | End of each sprint | Meeting + sprint report | Morenikeji Bankole |
| C-05 | Weekly status report | Project Lead, team | Schedule, scope, risks, next steps | Weekly (Fridays) | Written report (see [Status Reports](11-status-reports.md)) | Morenikeji Bankole |
| C-06 | Defect notification | Full Stack Lead, QA | New or reopened defects with priority | As raised | ClickUp task | Morenikeji Bankole, Sadiq Ilu |
| C-07 | Defect verification result | Project Manager, Project Lead | Pass / fail on each fix | As completed | ClickUp status update | Sadiq Ilu |
| C-08 | Design review and approval | Project Lead, UI contributors | Stage-gate approval of UI and landing page designs | Per design milestone | Review session + recorded approval | Maryam Abubakar |
| C-09 | Change request notice | Project Lead, affected owners | Decision on scope or schedule change | As raised | Change request entry | Morenikeji Bankole |
| C-10 | Risk review | Project Lead, risk owners | Update scores and mitigations | Weekly, inside the status report | Risk register | Morenikeji Bankole |
| C-11 | Phase gate review | Project Lead, project team | Approve moving to next phase | End of each phase | Formal review | Maryam Abubakar |
| C-12 | Release notice | Team, Project Lead, business stakeholders | Announce production release and known limitations | Per release (Feb 5, Feb 13) | Written release note | Abubakar Suleiman, Morenikeji Bankole |
| C-13 | Partner portal preview | Qair and Viva Jets contacts | Confirm branding and portal access before launch | Once per partner (Phase 5) | Email with link | Maryam Abubakar |
| C-14 | Demo to prospective buyers | Prospective enterprise buyers | Show end-to-end user journeys | Phase 6 | Live demonstration | Maryam Abubakar |
| C-15 | Closure report | Project Lead, stakeholders | Outcomes, lessons learned, handover | Once (project close) | Written report | Morenikeji Bankole |

## 5. Escalation Rules

| Level | Trigger | Escalate To | Response Time |
| --- | --- | --- | --- |
| 1 | Task blocked for more than one working day | Project Manager | Same day |
| 2 | A P0/P1 target, sprint goal or phase gate at risk | Project Lead | Within one working day |
| 3 | A decision that changes scope, schedule or the production release date | Project Lead (decision) via the change control process | Before work continues on the affected item |

## 6. Reporting Calendar

| Date (2026) | Event |
| --- | --- |
| Jan 5 – 9 | Kick-off, roadmap and plan review; status report #1 on Jan 9 |
| Jan 12 – 23 | Sprints 1 and 2; status reports on Jan 16 and Jan 23 |
| Jan 26 – Feb 2 | Sprint 3 and design review; status report on Feb 2 |
| Feb 4 – 5 | Release readiness review and production release; release notice |
| Feb 9 – 13 | Landing page sprint; partner previews; status report on Feb 13 |
| Feb 16 – 20 | UAT, demo and sign-off; final status report on Feb 20 |
| Feb 23 – Mar 31 | Post-launch stabilization; closure report on Mar 31 |

## 7. Related Documents

- [Stakeholder Register & RACI](03-stakeholder-register-and-raci.md)
- [Status Reports](11-status-reports.md)
