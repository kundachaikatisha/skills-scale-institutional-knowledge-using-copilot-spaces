# OctoAcme — Release & Deployment Guide

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability.

## Release Types
- Patch: hotfixes addressing critical production issues
- Minor: incremental features and improvements
- Major: significant functionality or breaking changes

## Release Roles & Responsibilities
The following roles have explicit responsibilities during release. See the [RACI matrix](./octoacme-roles-and-raci.md) for a full accountability breakdown.

- **DevOps Engineer**: owns the deployment pipeline and execution; prepares the deployment runbook and rollback plan; monitors system health post-deployment.
- **QA Lead**: executes pre-release smoke tests and provides formal sign-off before deployment proceeds.
- **Technical Writer**: finalizes and publishes release notes and user-facing documentation before deployment.
- **Support Lead**: confirms support team readiness; reviews release notes and prepares support runbooks for new features.
- **Project Manager**: final go/no-go authority; confirms all readiness criteria are met before authorizing deployment.

## Pre-release requirements
- All acceptance criteria met and PRs merged
- Passing CI and security scans
- **QA Lead sign-off** on smoke tests and acceptance criteria
- Release notes drafted and reviewed by Technical Writer
- Support Lead notified and support runbooks prepared
- Rollback / mitigation plan documented by DevOps Engineer
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
