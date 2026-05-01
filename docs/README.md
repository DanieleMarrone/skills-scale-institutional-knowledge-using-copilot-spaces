# OctoAcme Project Management Docs

This folder contains the process documentation for OctoAcme's project management practices. Its purpose is to centralize PM knowledge, convert tacit team insights into versioned, discoverable artifacts, and enable consistent execution across projects and contributors. Whether you are onboarding to OctoAcme for the first time or looking for a quick reference on a specific workflow, this folder is your single entry point.

## Overview of OctoAcme Project Management Processes

OctoAcme follows a lightweight, repeatable lifecycle that moves work from idea to delivery with clear ownership and measurable outcomes. Every project begins with an **initiation** phase: the team validates the business need, defines success criteria and metrics, identifies stakeholders, and reaches an explicit go/no-go decision before investing in detailed planning. Minimum expected artifacts include a project one-pager (problem, objective, success metrics), a stakeholder and communication plan, a high-level timeline with milestones, an initial risk register, and an outline of resource needs. Once approved, **planning** turns the initiative into an actionable backlog and release plan: the team runs a kickoff, decomposes scope into shippable increments with explicit acceptance criteria, estimates effort (T-shirt sizing or story points), and documents a shared Definition of Done. Risks and cross-team dependencies are captured with impact/likelihood ratings, owners, mitigations, and statuses, then revisited routinely—with escalation paths running from team triage through product leadership to sponsors when needed.

Roles are clearly defined to support each phase of the lifecycle. The **Project Manager** owns the overall plan, risk register, status reporting, and stakeholder communication cadence. The **Product Manager** maintains the prioritised backlog and acceptance criteria. **Developers** own implementation, unit tests, and PR hygiene (targeting ≤ 400 lines per PR, linking every PR to its underlying issue). **QA/Testing** validates acceptance criteria through integration, end-to-end, and smoke tests. **Stakeholders** participate in demos and provide timely sign-off. Communication follows a regular cadence—daily standups for blockers and dependencies, weekly delivery syncs for progress and risk flags, and sprint or milestone demos to keep stakeholders aligned.

**Execution** emphasises delivery hygiene and transparent tracking via a project board that flows through Backlog → Ready → In Progress → In Review → QA → Done. Quality assurance is built into the process: new logic is expected to include unit tests, CI pipelines enforce linting, automated testing, and security scanning before review or merge, and critical flows require integration and smoke tests. **Release & deployment** follows a checklist requiring acceptance criteria completion, passing CI and security checks, prepared release notes, and a documented rollback or mitigation plan. Deployments proceed through staging with smoke tests and post-deploy verification, followed by stakeholder announcements. After every sprint, release, or incident, **retrospectives** convert learnings into a small number of owned, time-bound action items that are tracked in the backlog and reviewed in ongoing PM syncs—closing the loop and driving continuous improvement.

## Process Documents

| Document | Description |
|---|---|
| [Project Management Overview](octoacme-project-management-overview.md) | High-level summary of OctoAcme's PM philosophy, lifecycle phases, and guiding principles. |
| [Project Initiation](octoacme-project-initiation.md) | Steps and artifacts for validating a business need and reaching a go/no-go decision. |
| [Project Planning](octoacme-project-planning.md) | Backlog decomposition, estimation, Definition of Done, and release-plan guidance. |
| [Execution & Tracking](octoacme-execution-and-tracking.md) | Board workflow, PR conventions, daily standups, weekly syncs, and demo cadence. |
| [Risks & Communication](octoacme-risks-and-communication.md) | Risk register format, escalation levels, and stakeholder communication strategies. |
| [Release & Deployment](octoacme-release-and-deployment.md) | Release checklist, staging process, smoke tests, rollback playbook, and announcements. |
| [Retrospective & Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md) | Retro formats, action-item tracking, and feedback loops for ongoing improvement. |
| [Roles & Personas](octoacme-roles-and-personas.md) | Detailed descriptions of all team roles including UI/UX Designer, Data Analyst, DevOps Engineer, Technical Writer, and Customer Support Lead. |
| [Role Interactions & RACI-lite](octoacme-role-interactions.md) | Cross-functional responsibility matrix for lifecycle phases, key artifacts, handoff paths, and escalation guidance. |

## Templates & Checklists

| Template | Description |
|---|---|
| [Kickoff Checklist](templates/octoacme-kickoff-checklist.md) | Pre-kickoff prep, meeting agenda, post-kickoff actions, and role-readiness checks. |
| [Weekly Status Update Template](templates/octoacme-weekly-status-update-template.md) | Structured template for weekly project health communication to stakeholders. |
| [Role Handoff Checklist](templates/octoacme-role-handoff-checklist.md) | Checklists for key inter-role handoffs (Design→Dev, Dev→DevOps, Product→Support, etc.). |
