# Project Charter: CharterOps ERP System Revamp & SaaS Readiness

| Field | Detail |
| --- | --- |
| **Project** | CharterOps ERP System |
| **Document** | Project Charter |
| **Version** | 1.0 |
| **Status** | Approved for Execution |
| **Project Lead / Sponsor** | Maryam Abubakar |
| **Project Manager** | Morenikeji Bankole |

---

## 1. Project Overview & Metadata

| Project Detail | Information |
| --- | --- |
| **Project Name** | CharterOps ERP System |
| **Project Type** | ERP Product Revamp, Bug Remediation & SaaS Replication Readiness |
| **Project Lead / Sponsor** | Maryam Abubakar (Project Lead) |
| **Project Manager** | Morenikeji Bankole (Project Manager) |
| **Methodology** | Hybrid (Agile + Waterfall): Agile sprint execution with phase-based approvals |
| **Project Window** | January 5, 2026 – March 31, 2026 |
| **Primary System Link** | <https://charter-ops.vercel.app/> |
| **Document Status** | Approved for Execution |

## 2. Business Case & Executive Summary

CharterOps is an enterprise resource planning (ERP) system dedicated to executive aviation and charter flight operations. To position CharterOps for client acquisition, commercial demonstrations and multi-operator SaaS replication, the current platform requires a comprehensive stabilization and usability overhaul.

This project addresses critical operational bugs across flight booking, aircraft maintenance, fuel logging and invoicing, while modernizing the core user interface and establishing branded landing pages for target partner operators (including Qair and Viva Jets). Completing this project delivers an enterprise-grade, dependable and scalable operational platform ready for commercial release.

## 3. Project Objectives & Success Criteria

- **System Usability & Modernization:** Enhance core operational UI flows to eliminate duplicate actions, streamline data input and provide an intuitive user experience for dispatchers, flight crew and administrators.
- **Zero-Defect Core Workflows:** Resolve all high-priority (P0/P1) operational defects affecting authentication, bookings, passenger data consistency, maintenance records and fuel supply logs.
- **Financial & Configuration Accuracy:** Ensure exact billing calculations, guaranteeing that dynamic service fees reflect correctly on client invoices and receipts and that multi-currency symbols display accurately.
- **Commercial Demo & Replication Readiness:** Prepare a reliable, production-grade staging/production environment tailored for prospective enterprise buyers by **Q1 2026**.

## 4. Project Scope

### In Scope

- **Authentication & Access Control:** Admin and partner user management without mandatory deactivation; crew registration validation and feedback loops.
- **Flight & Aircraft Operations:** Flight booking submission reliability, elimination of redundant submission actions and passenger record de-duplication.
- **Maintenance & Resource Modules:** Resolution of API error codes in aircraft maintenance creation; fuel supply entry and tracking stabilization.
- **System Configuration & Billing:** Strict phone/email input validation; accurate propagation of auxiliary service fees to invoices; proper currency symbol rendering across dashboards.
- **Branding & Landing Pages:** Re-designed brand assets and client-facing landing pages for operator portals (Qair & Viva Jets).

### Out of Scope

- Complete database engine migration or backend architecture replacement.
- Custom on-premise hardware integrations with aircraft avionics.
- Third-party payment gateway renegotiations outside existing API scope.

## 5. High-Level Project Timeline & Milestones

| Phase | Milestone / Key Focus | Duration | Target Window |
| --- | --- | --- | --- |
| **Phase 1** | **Project Initiation, Planning & Team Onboarding**: scope walk-through, requirements gathering, roadmap and kick-off approval | 1 Week | Jan 5 – Jan 9, 2026 |
| **Phase 2** | **Defect Remediation & Stabilization**: fix P1 bugs across Auth, Flight Booking, Maintenance, Fuel and Invoicing | 2 Weeks | Jan 12 – Jan 23, 2026 |
| **Phase 3** | **UI/UX Enhancement & Feature Optimization**: workflow optimizations, form validations and user flow enhancements | 2 Weeks | Jan 26 – Feb 2, 2026 |
| **Phase 4** | **Production Deployment (Internal App)**: core system staging cutover and production release | 1–2 Days | Feb 4 – Feb 5, 2026 |
| **Phase 5** | **Landing Page Development & Partner Branding**: portal interfaces for Qair and Viva Jets | 1 Week | Feb 9 – Feb 13, 2026 |
| **Phase 6** | **Final Testing, Commercial Demo Readiness & Project Close**: user acceptance testing, demo preparation and project sign-off | 1 Week | Feb 16 – Feb 20, 2026 |

*Buffer and post-launch stabilization remain active through **March 31, 2026**.*

## 6. Project Governance & Key Stakeholders

| Role | Name | Responsibilities |
| --- | --- | --- |
| **Project Lead** | Maryam Abubakar | Strategic direction, stage-gate design approvals, resource allocation and final acceptance |
| **Project Manager** | Morenikeji Bankole | Scope control, sprint coordination, cross-functional communication, risk management and schedule delivery |
| **Full Stack Lead Developer** | Abubakar Suleiman | Core backend and frontend engineering, API defect resolution, database logic and deployment |
| **Technical Support / QA** | Sadiq Ilu | Test verification, secondary technical review, defect validation and deployment support |
| **Engineering Contributors** | David, Ahmad | Frontend UI development, landing page builds and QA testing |

## 7. Key Deliverables

- **Documented Project Plan & Roadmap:** Approved work breakdown, schedule and team alignment matrix.
- **Hardened Core ERP Application:** Tested and deployed CharterOps system with zero unresolved P0/P1 blocking issues.
- **Validated Financial Engine:** Accurate invoice generator reflecting itemized add-on fees and configured currency formatting.
- **Partner Landing Pages:** Responsive marketing and portal access pages for partner operators.
- **Demonstration Artifacts:** End-to-end user journeys and sandbox environments ready for prospective buyers.

## 8. Key Assumptions, Constraints & Risks

**Key Assumptions**

- Development and staging environments remain stable with continuous CI/CD availability.
- Access credentials and API documentation for ClickUp, Vercel and internal servers remain current.

**Constraints**

- Fixed delivery window requiring Phase 4 production readiness by early February.
- Compact cross-functional team requiring disciplined prioritization of P0/P1 issues over new features.

**Top Risks & Mitigation**

- *Hidden Backend Dependencies:* isolated API failures in maintenance/fuel may reveal deeper service issues. *Mitigation:* early code inspection by the Full Stack Developer during Phase 2.
- *Scope Creep:* requests for bespoke operator configurations during defect remediation. *Mitigation:* strict gatekeeping by the Project Manager using the hybrid change-control process.

## 9. Charter Approval & Sign-Off

| Stakeholder Role | Name | Signature | Date |
| --- | --- | --- | --- |
| Project Lead | Maryam Abubakar | _________________________ | _____ / _____ / 2026 |
| Project Manager | Morenikeji Bankole | _________________________ | _____ / _____ / 2026 |
