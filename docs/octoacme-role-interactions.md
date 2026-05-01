# OctoAcme — Role Interactions & RACI-lite

This document provides a lightweight responsibility matrix showing how OctoAcme roles collaborate across the project lifecycle and who owns key artifacts.

See also: [Roles & Personas](octoacme-roles-and-personas.md)

---

## Legend

| Symbol | Meaning |
|--------|---------|
| **O** | Owner / DRI — ultimately accountable; drives creation or decision |
| **C** | Contributor — actively participates in creating or executing |
| **R** | Reviewer / Consulted — provides input, feedback, or approval |
| **I** | Informed — kept up to date on outcomes |
| _(blank)_ | Not typically involved |

---

## Lifecycle Phase Matrix

| Phase | Project Manager | Product Manager | Developer | UI/UX Designer | Data Analyst | DevOps Engineer | Technical Writer | Customer Support Lead |
|---|---|---|---|---|---|---|---|---|
| **Initiation** | O | C | R | R | I | I | I | R |
| **Planning** | O | C | C | C | C | C | C | R |
| **Execution** | C | R | O | C | C | C | C | I |
| **Release** | C | R | C | I | I | O | C | R |
| **Retrospective** | O | C | C | C | C | C | C | C |

---

## Artifact Ownership Matrix

| Artifact | Owner / DRI | Contributors | Reviewers | Informed |
|---|---|---|---|---|
| **Project One-pager / Charter** | Project Manager | Product Manager | Developers, Customer Support Lead | All team members |
| **Prioritized Backlog** | Product Manager | Developers, UI/UX Designer | Project Manager, Data Analyst | All team members |
| **Risk Register** | Project Manager | All roles | Product Manager, Sponsor | Stakeholders |
| **Definition of Done** | Project Manager | Developers, QA | Product Manager | All team members |
| **Sprint / Iteration Plan** | Project Manager | Developers, Product Manager | UI/UX Designer, DevOps Engineer | All team members |
| **Design Prototypes** | UI/UX Designer | Product Manager | Developers, Customer Support Lead | Project Manager |
| **CI/CD Pipeline & Runbooks** | DevOps Engineer | Developers | Project Manager, Technical Writer | All team members |
| **Release Notes** | Technical Writer | Developers, Product Manager | Customer Support Lead | Stakeholders |
| **Metrics Dashboard** | Data Analyst | Developers (instrumentation) | Product Manager | Project Manager, Customer Support Lead |
| **Retrospective Action Items** | Project Manager | All roles | Product Manager | Stakeholders |
| **Support FAQs / Help Content** | Customer Support Lead | Technical Writer | Product Manager | All team members |
| **Process Documentation** | Technical Writer | All roles | Project Manager | All team members |

---

## Key Cross-Role Handoffs

### Initiation → Planning
- **Product Manager → Project Manager**: approved one-pager and initial backlog.
- **UI/UX Designer → Developers**: design briefs or discovery findings.
- **Customer Support Lead → Product Manager**: support-driven requirements or known pain points.

### Planning → Execution
- **Project Manager → All**: finalized project plan, sprint backlog, and DoD.
- **DevOps Engineer → Developers**: environment access, CI pipeline, and branching strategy.
- **Technical Writer → Project Manager**: documentation deliverables added to the milestone.

### Execution → Release
- **Developers → DevOps Engineer**: feature-complete builds ready for staging deployment.
- **Technical Writer → Product Manager**: draft release notes for review.
- **Customer Support Lead → Project Manager**: support-readiness assessment completed.
- **Data Analyst → Product Manager**: baseline metrics captured before release.

### Release → Retrospective
- **DevOps Engineer → Project Manager**: post-release health summary.
- **Customer Support Lead → All**: early support signal report (first 24–72 h after release).
- **Data Analyst → Product Manager**: initial outcome metrics vs. success criteria.

---

## Escalation Paths

| Situation | First Contact | Escalation |
|---|---|---|
| Scope change request | Product Manager | Project Manager → Sponsor |
| Delivery blocker | Project Manager | Product Manager → Sponsor |
| Critical production incident | DevOps Engineer | Project Manager → Sponsor |
| Design/UX conflict | UI/UX Designer | Product Manager |
| Documentation gap pre-release | Technical Writer | Project Manager |
| Surge in support tickets | Customer Support Lead | Product Manager → Project Manager |

---

*For individual role descriptions and responsibilities, see [Roles & Personas](octoacme-roles-and-personas.md).*
*For templates and checklists supporting these interactions, see [templates/](templates/).*
