# OctoAcme — Roles & RACI Matrix

## Purpose
Provide a lightweight RACI (Responsible, Accountable, Consulted, Informed) matrix that maps key project activities to OctoAcme roles and personas. Use this alongside [octoacme-roles-and-personas.md](./octoacme-roles-and-personas.md) to clarify ownership and reduce ambiguity.

## RACI Key
| Symbol | Meaning |
|---|---|
| **R** | Responsible — does the work |
| **A** | Accountable — owns the outcome; final decision maker |
| **C** | Consulted — provides input before/during |
| **I** | Informed — notified of outcomes/progress |

---

## RACI Matrix

| Activity | Project Manager | Product Manager | Developer | UX Designer | Technical Writer | QA Lead | DevOps Engineer | Customer/User Rep | Executive Sponsor | Support Lead |
|---|---|---|---|---|---|---|---|---|---|---|
| **Initiation** | | | | | | | | | | |
| Define project charter / one-pager | R | A | C | C | I | I | I | C | A | I |
| Stakeholder alignment & sign-off | A | R | I | I | I | I | I | C | A | I |
| Go/no-go decision | C | C | I | I | I | I | I | C | A | I |
| **Planning** | | | | | | | | | | |
| Backlog creation & prioritization | C | A | C | C | C | C | C | C | I | C |
| Define Definition of Done | A | C | R | C | C | R | C | I | I | C |
| Draft test plan & QA approach | C | C | C | I | I | A/R | C | I | I | I |
| Infrastructure & pipeline design | C | I | C | I | I | C | A/R | I | I | I |
| Documentation plan | C | C | I | C | A/R | C | I | I | I | C |
| **Execution** | | | | | | | | | | |
| Feature implementation | I | C | A/R | C | I | C | C | I | I | I |
| UX/design review | I | C | C | A/R | I | C | I | C | I | I |
| CI/CD pipeline maintenance | I | I | C | I | I | C | A/R | I | I | I |
| Test execution & defect triage | C | I | R | C | I | A/R | C | I | I | I |
| Documentation authoring | I | C | C | C | A/R | C | I | I | I | I |
| Risk register updates | A/R | C | C | I | I | C | C | I | I | I |
| **Release** | | | | | | | | | | |
| Pre-release checklist & readiness | A | C | C | C | C | C | C | I | I | C |
| QA sign-off / smoke testing | C | I | C | C | I | A/R | C | I | I | I |
| Deployment execution | C | I | C | I | I | C | A/R | I | I | I |
| Release notes & user documentation | I | C | C | C | A/R | C | I | I | I | C |
| Support briefing & runbook | C | C | I | I | C | I | I | I | I | A/R |
| Release announcement | A | R | I | I | C | I | I | I | I | C |
| **Retrospective** | | | | | | | | | | |
| Facilitate retrospective | A/R | C | C | C | C | C | C | C | I | C |
| Capture & publish action items | A/R | C | C | C | C | C | C | C | I | C |
| Business outcome review | C | R | I | I | I | I | I | C | A | I |

---

## Notes
- "A/R" in a single cell indicates a role that both owns the outcome and does the work. Separate A and R when possible on larger teams.
- Activities map to the lifecycle phases described in the [project management overview](./octoacme-project-management-overview.md).
- Consult the [execution and tracking guide](./octoacme-execution-and-tracking.md) for QA and CI/CD quality gate details.
- Consult the [release and deployment guide](./octoacme-release-and-deployment.md) for the pre-release readiness checklist and deployment responsibilities.
