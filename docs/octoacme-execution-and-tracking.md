# OctoAcme — Execution & Tracking

## Purpose
Guidance for managing day-to-day execution and tracking progress toward project milestones.

## Team Rhythm
- Daily standups (15 min) — focus on progress, blockers, dependencies
- Weekly delivery sync — show progress, updates, and flagged risks
- Demo/Review at the end of each sprint or milestone

## Workflows
- Use the project board (e.g., GitHub Projects) with columns: Backlog, Ready, In Progress, In Review, QA, Done
  - The **QA column** is owned by the QA Lead. Items move to QA after code review is complete and CI passes.
  - The **DevOps Engineer** is responsible for CI/CD pipeline health; coordinate with them on environment or pipeline blockers.
- Pull Request workflow:
  - Small PRs (<= 400 lines when possible)
  - Include issue link and acceptance criteria in PR description
  - Run automated tests and linting in CI before requesting review
  - Require at least one approval before merging (or team-defined policy)

## Quality & Testing
- Unit tests for new logic
- Integration tests where applicable
- End-to-end smoke tests for critical flows before release
- Security scanning in CI
- Manual QA for feature acceptance when needed
- **QA Lead** owns the test plan and quality gates; provides sign-off before items move to Done or to release. See [octoacme-roles-and-personas.md](./octoacme-roles-and-personas.md) for the full QA Lead role description.
- **DevOps Engineer** integrates security, performance, and quality scanning into the CI/CD pipeline. See [octoacme-roles-and-raci.md](./octoacme-roles-and-raci.md) for accountability assignments.
- Quality gate: no feature moves from QA to Done without QA Lead sign-off.

## Reporting & Metrics
- Track velocity and burndown
- Monitor success metrics identified in the Project One-pager
- Use dashboards for key signals (errors, latency, usage)

## Blocker Escalation
- Level 1: Team-level triage in daily standup
- Level 2: PM escalates to Product Lead and dependent teams
- Level 3: Sponsor-level escalation for business-impacting issues

## Execution Checklist
- [ ] Branching and PR conventions documented in repo
- [ ] CI configured for tests and lint
- [ ] Regular demos scheduled
- [ ] Risk register updated weekly
