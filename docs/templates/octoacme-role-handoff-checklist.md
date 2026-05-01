# OctoAcme — Role Handoff Checklist

Use this checklist whenever work passes from one role or team to another during the project lifecycle. Clear handoffs reduce dropped context and rework.

See also: [Role Interactions & RACI-lite](../octoacme-role-interactions.md) | [Roles & Personas](../octoacme-roles-and-personas.md)

---

## How to Use

1. The **outgoing role** completes the relevant section before handing off.
2. The **incoming role** confirms receipt and reviews completeness.
3. Any gaps are flagged and resolved before work begins.
4. The checklist (or a link to it) is attached to the relevant issue or PR.

---

## Design → Development Handoff (UI/UX Designer → Developer)

- [ ] Final design files linked in the issue/PR (Figma, Storybook, etc.)
- [ ] Component annotations and interaction specifications included
- [ ] Accessibility requirements called out (WCAG level, focus management, ARIA notes)
- [ ] Edge cases and empty/error states documented
- [ ] Design sign-off confirmed by Product Manager
- [ ] Questions from Developers answered or tracked as follow-up issues

---

## Development → QA / Review Handoff (Developer → Reviewer / QA)

- [ ] PR description includes: context, acceptance criteria link, testing steps
- [ ] Automated tests added for new logic (unit / integration)
- [ ] CI passing (build, lint, tests, security scan)
- [ ] Self-review completed by the author
- [ ] Known limitations or deferred items noted in PR description

---

## Development → DevOps / Release Handoff (Developer → DevOps Engineer)

- [ ] Feature branch merged to the target release branch
- [ ] Deployment notes or migration steps documented
- [ ] Feature flags configured (if applicable)
- [ ] Rollback instructions or considerations noted
- [ ] Monitoring / alerting requirements communicated

---

## Engineering → Technical Writer Handoff (Developer / Product Manager → Technical Writer)

- [ ] Summary of what changed and why provided
- [ ] API changes, config options, or user-facing changes enumerated
- [ ] Links to relevant PRs, issues, and design docs shared
- [ ] Review of draft documentation scheduled before release

---

## Product → Support Readiness Handoff (Product Manager → Customer Support Lead)

- [ ] Feature overview and expected user impact communicated
- [ ] Known limitations or deferred fixes disclosed
- [ ] FAQ or help-center content reviewed / updated
- [ ] Support team trained or briefed (if applicable)
- [ ] Escalation contact identified for post-release issues

---

## Post-Release Handoff (Project Manager → Retrospective)

- [ ] Release summary shared with team
- [ ] Action items from the release captured with owners
- [ ] Metrics baseline noted for comparison at retrospective
- [ ] Support signal review scheduled (first 24–72 h post-release)

---

*Related: [Kickoff Checklist](octoacme-kickoff-checklist.md) | [Weekly Status Update Template](octoacme-weekly-status-update-template.md)*
