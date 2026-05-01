# OctoAcme — Release & Deployment Guide

See also: [Role Interactions & RACI-lite](octoacme-role-interactions.md) | [Role Handoff Checklist](templates/octoacme-role-handoff-checklist.md)

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability.

## Release Types
- Patch: hotfixes addressing critical production issues
- Minor: incremental features and improvements
- Major: significant functionality or breaking changes

## Pre-release requirements
- All acceptance criteria met and PRs merged
- Passing CI and security scans
- Release notes drafted
- Rollback / mitigation plan documented
- Smoke tests prepared

## Deployment Checklist
- [ ] Deployment window scheduled (if needed)
- [ ] Backup or snapshot (if applicable)
- [ ] Deploy to staging and run smoke tests
- [ ] Deploy to production (automated pipeline preferred)
- [ ] Run post-deploy verifications
- [ ] Announce release to stakeholders and support

## Rollback & Incident Playbook
- If a deployment fails or causes a critical issue:
  - Trigger incident response and notify on-call
  - Rollback to last known-good release if necessary
  - Triage root cause and capture action items

## Release Notes Template
- Release name / number:
- Date:
- Summary:
- Notable changes:
- Migration steps (if any):
- Known issues:

---

## Support Readiness

Before announcing a release, confirm that customer-facing teams are prepared:

### Roles Involved
| Role | Responsibility |
|------|---------------|
| **Customer Support Lead** | Reviews release scope; updates FAQs and known-issues list; confirms support team is briefed |
| **Technical Writer** | Publishes or updates user-facing release notes and help content |
| **DevOps Engineer** | Provides deployment summary and monitors post-release health dashboards |

### Support Readiness Checklist
- [ ] Customer Support Lead has reviewed release scope and user impact
- [ ] FAQs and help-center content updated (Customer Support Lead + Technical Writer)
- [ ] Release notes published or queued (Technical Writer)
- [ ] On-call rotation confirmed for post-release monitoring (DevOps Engineer)
- [ ] Support escalation contact identified for critical post-release issues

> Use the [Role Handoff Checklist — Product → Support Readiness](templates/octoacme-role-handoff-checklist.md#product--support-readiness-handoff-product-manager--customer-support-lead) section to ensure a complete handoff.
