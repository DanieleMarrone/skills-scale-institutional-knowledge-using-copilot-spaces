# OctoAcme — Roles & Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

See also: [Role Interactions & RACI-lite](octoacme-role-interactions.md)

---

## Developers

### Role Summary
Developers design, build, test, and deliver software components. They collaborate with product and project leads to implement features that meet acceptance criteria and quality standards.

### Responsibilities
- Implement features and fixes to meet acceptance criteria
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Help identify technical risks and propose mitigations

### Goals
- Deliver reliable, maintainable code
- Reduce cycle time from idea to production
- Maintain high test coverage and observability

### Typical Communication
- Daily standups and sprint planning
- PR descriptions and code review comments
- Technical design docs when needed

### Interaction Model
- **Product Managers**: receive feature specs and acceptance criteria; flag technical trade-offs.
- **Project Managers**: report progress, surface blockers, and update estimates.
- **UI/UX Designers**: collaborate on component implementation and flag feasibility constraints.
- **DevOps Engineers**: coordinate deployment pipelines and environment provisioning.
- **Technical Writers**: provide context for documentation of APIs and new features.

---

## Product Managers

### Role Summary
Product Managers define what should be built to deliver customer and business value. They own the product vision, prioritize the backlog, and measure outcomes.

### Responsibilities
- Define problem statements and success metrics
- Prioritize the roadmap and backlog
- Collaborate with stakeholders and engineering on trade-offs
- Validate solutions through user research and metrics

### Goals
- Maximize customer value and impact
- Make clear, data-driven prioritization decisions
- Ensure product-market fit and usability

### Typical Communication
- Weekly alignment with PM and engineering leads
- Roadmap updates and stakeholder briefings
- Acceptance criteria and feature specs

### Interaction Model
- **Developers**: provide prioritized backlog items with acceptance criteria; review demos.
- **Project Managers**: align on scope, milestones, and risk trade-offs.
- **UI/UX Designers**: co-define user journeys and review design prototypes.
- **Data Analysts**: consume usage and outcome metrics to guide prioritization.
- **Customer Support Lead**: receive user feedback signals to inform roadmap decisions.

---

## Project Managers

### Role Summary
Project Managers coordinate delivery activities, manage schedules, risks, and communications. They enable the team to deliver on commitments efficiently.

### Responsibilities
- Create and maintain project plans and timelines
- Manage risks, dependencies, and resource constraints
- Facilitate meetings (kickoff, planning, retrospectives)
- Ensure consistent project documentation and status reporting
- Coordinate cross-team and stakeholder communication

### Goals
- Deliver projects on time and within scope
- Minimize unplanned work and escalations
- Maintain transparency and alignment across stakeholders

### Typical Communication
- Weekly status updates and stakeholder reports
- Risk registers and decision logs
- Coordination via project boards and meeting facilitation

### Interaction Model
- **Developers**: track sprint progress; help remove blockers through escalation.
- **Product Managers**: align on scope changes and priority shifts.
- **DevOps Engineers**: coordinate release windows and deployment schedules.
- **Technical Writers**: ensure documentation milestones are included in the plan.
- **Customer Support Lead**: loop in for support-readiness assessments before releases.

---

## UI/UX Designer

### Role Summary
UI/UX Designers craft intuitive, accessible user interfaces and experiences. They translate product requirements into concrete designs that developers can implement and users can navigate confidently.

### Responsibilities
- Create wireframes, prototypes, and high-fidelity designs
- Conduct or synthesize user research and usability testing
- Maintain and evolve the design system and component library
- Ensure designs meet accessibility standards (WCAG)
- Iterate based on feedback from stakeholders, developers, and users

### Typical Communication
- Design reviews with Product and Engineering at key milestones
- Prototype links shared via project board or PR descriptions
- Async feedback on Figma/design tool comments

### Interaction Model
- **Developers**: hand off designs with annotated specs; answer implementation questions.
- **Product Managers**: receive problem framing and user stories; present design options for prioritization decisions.
- **Project Managers**: flag design scope changes or discovery work that may affect the timeline.
- **Data Analysts**: use analytics and heatmap data to validate design hypotheses.
- **Customer Support Lead**: incorporate usability pain points surfaced from support tickets.

---

## Data Analyst

### Role Summary
Data Analysts collect, analyze, and visualize project and product data to support evidence-based decisions across the team.

### Responsibilities
- Define and track key product and process metrics
- Build dashboards and reports for stakeholders
- Analyze usage trends, quality signals, and experiment results
- Surface actionable insights from data to Product and Project Managers
- Partner on instrumentation and data collection with Developers

### Typical Communication
- Regular metrics reviews in weekly syncs or dedicated data reviews
- Dashboard links and summary reports in project status updates
- Ad-hoc analysis requests from Product or Project Managers

### Interaction Model
- **Product Managers**: provide metric baselines and outcome data to validate roadmap bets.
- **Project Managers**: highlight velocity trends or quality signals that could affect delivery timelines.
- **Developers**: partner on instrumentation, event tracking, and data schema decisions.
- **UI/UX Designers**: share behavioral analytics to inform design iterations.
- **Customer Support Lead**: correlate support-ticket volume with product changes.

---

## DevOps Engineer

### Role Summary
DevOps Engineers own the CI/CD pipelines, infrastructure automation, and operational health of project environments. They enable teams to ship reliably and recover quickly from incidents.

### Responsibilities
- Design and maintain CI/CD pipelines (build, test, deploy, rollback)
- Provision and manage infrastructure (cloud resources, containers, environments)
- Implement observability: logging, metrics, alerting, tracing
- Coordinate deployment windows and release automation
- Lead incident triage and post-mortem action items for infrastructure issues

### Typical Communication
- Release coordination meetings with PM and engineering leads
- On-call and incident channels
- Infrastructure change notifications and runbooks

### Interaction Model
- **Developers**: review pipeline configs and provide deployment runbooks; help debug CI failures.
- **Project Managers**: communicate deployment schedules and environment readiness.
- **Product Managers**: advise on operational risk for new features (feature flags, rollout strategies).
- **Technical Writers**: collaborate on runbooks and operational documentation.
- **Customer Support Lead**: provide incident status updates that may affect end users.

---

## Technical Writer

### Role Summary
Technical Writers author, organize, and maintain clear documentation—covering processes, APIs, onboarding guides, and user-facing help content—so that all contributors and users can operate effectively.

### Responsibilities
- Write and maintain process docs, API references, user guides, and release notes
- Ensure documentation accuracy by reviewing with subject-matter experts
- Manage the documentation lifecycle (create, review, publish, deprecate)
- Bridge communication between technical contributors and non-technical readers
- Identify and fill gaps in existing documentation coverage

### Typical Communication
- Documentation reviews with Developers and Product Managers
- Release note drafts circulated before deployment
- Async comments and reviews on PRs that touch docs

### Interaction Model
- **Developers**: review technical accuracy of API and implementation docs; receive code context.
- **Product Managers**: align on user-facing messaging and feature announcements.
- **Project Managers**: track documentation deliverables as part of the release milestone.
- **DevOps Engineers**: collaborate on runbooks, deployment guides, and incident playbooks.
- **Customer Support Lead**: incorporate FAQ content and known-issue documentation based on support feedback.

---

## Customer Support Lead

### Role Summary
Customer Support Leads represent the voice of the customer within the delivery team. They surface recurring issues, coach support staff, and ensure teams ship with sufficient documentation and readiness.

### Responsibilities
- Aggregate and prioritize user-reported issues and feature requests
- Evaluate support-readiness before product releases
- Create or review customer-facing FAQs, known-issues lists, and help content
- Facilitate feedback loops between customers and Product/Engineering
- Track support ticket trends to identify recurring quality or usability problems

### Typical Communication
- Pre-release readiness reviews with PM and Product Manager
- Support ticket trend summaries in stakeholder updates
- Async updates to FAQ and help-center content

### Interaction Model
- **Product Managers**: surface customer pain points to influence roadmap prioritization.
- **Project Managers**: flag support-readiness risks ahead of planned releases.
- **Technical Writers**: co-author or review customer-facing help documentation.
- **Developers**: escalate reproduction steps for high-priority bugs.
- **Data Analysts**: collaborate on correlating support volume with product changes.

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
- See [Role Interactions & RACI-lite](octoacme-role-interactions.md) for a cross-functional responsibility matrix.

