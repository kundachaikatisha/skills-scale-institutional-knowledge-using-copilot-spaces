# OctoAcme Project Management Docs

This folder contains OctoAcme's process documentation for project management. It is the single source of truth for how cross-functional projects are initiated, planned, executed, released, and continuously improved. Whether you are onboarding to the team or looking for a quick reference, start here.

## Overview

OctoAcme follows a structured project lifecycle to deliver customer value reliably and iteratively. The lifecycle moves through five key stages: **Initiation → Planning → Execution & Tracking → Release & Deployment → Close & Retrospective**. Each stage has defined goals, artifacts, and decision gates to keep teams aligned and work moving forward. A lightweight Project One-pager kicks off every initiative, ensuring a clear problem statement, SMART objectives, success metrics, and stakeholder alignment before any planning work begins.

Multiple roles collaborate throughout the lifecycle. The **Project Manager (PM)** coordinates delivery, schedules, risks, and cross-team communications. The **Product Manager (PdM / Product Lead)** owns the product vision, prioritizes the backlog, and measures outcomes against success metrics. **Developers** design, build, and test features to meet acceptance criteria while maintaining high code quality. **QA/Testing** validates that acceptance criteria are met and quality standards are upheld. **Stakeholders** provide inputs, approve key decisions, and receive regular updates on progress and risk.

Communication is structured to maintain transparency without overhead. The PM and PdM hold a **weekly sync**; the delivery team runs **twice-weekly standups**; and stakeholders receive **monthly updates** (or milestone-based reports). A standardized weekly status template—covering progress, next steps, risks/blockers, and decisions needed—keeps all updates consistent. The project README or release document serves as the single source of truth for current status, and escalation paths are clearly defined (Team → PM → Product Lead → Sponsor) to resolve blockers quickly.

Quality is built into every stage. During execution, pull requests are kept small (≤ 400 lines where possible), linked to issues, and require at least one approval after automated CI checks (tests, linting, and security scanning) pass. End-to-end smoke tests cover critical flows before each release. Pre-release requirements include passing CI, security scans, documented rollback plans, and drafted release notes. After every sprint or major release, a blameless retrospective captures what went well, what can improve, and produces 2–3 prioritized action items tracked through the backlog.

## What's in this folder

| Document | Description |
|---|---|
| [octoacme-project-management-overview.md](octoacme-project-management-overview.md) | High-level overview: principles, roles, lifecycle, and communication cadence |
| [octoacme-project-initiation.md](octoacme-project-initiation.md) | Initiation guide: one-pager template, stakeholder alignment, decision gate |
| [octoacme-project-planning.md](octoacme-project-planning.md) | Planning guide: backlog creation, sprint planning, risk & dependency management |
| [octoacme-execution-and-tracking.md](octoacme-execution-and-tracking.md) | Execution guide: team rhythm, PR workflow, quality & testing, escalation |
| [octoacme-risks-and-communication.md](octoacme-risks-and-communication.md) | Risk management: risk register, communication templates, escalation paths |
| [octoacme-release-and-deployment.md](octoacme-release-and-deployment.md) | Release guide: release types, deployment checklist, rollback playbook |
| [octoacme-retrospective-and-continuous-improvement.md](octoacme-retrospective-and-continuous-improvement.md) | Retrospective guide: structure, action item tracking, continuous improvement culture |
| [octoacme-roles-and-personas.md](octoacme-roles-and-personas.md) | Personas: detailed responsibilities and communication patterns for each role |
