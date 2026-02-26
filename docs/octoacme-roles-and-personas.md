# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises. For a full mapping of who is Responsible, Accountable, Consulted, and Informed for each activity, see [octoacme-roles-and-raci.md](./octoacme-roles-and-raci.md).

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

### Interactions
- **Planning**: collaborate with Product Manager on acceptance criteria and estimates.
- **Execution**: partner with QA Lead on test coverage; work with DevOps Engineer on CI/CD pipelines and environment issues.
- **Release**: hand off deployment packages to DevOps Engineer; address defects surfaced by QA Lead.
- **Retrospective**: share technical learnings and propose engineering improvements.

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

### Interactions
- **Initiation**: partner with Executive Sponsor to define goals and secure resources.
- **Planning**: work with UX Designer on user flows; align with Project Manager on scope and milestones.
- **Execution**: review UX prototypes; consult Customer/User Representative for feedback.
- **Release**: collaborate with Technical Writer on user-facing documentation; brief Support Lead on new features.
- **Retrospective**: review metrics with Customer/User Representative; align roadmap adjustments with Executive Sponsor.

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

### Interactions
- **Initiation**: align with Executive Sponsor on goals, budget, and governance; onboard all team roles.
- **Planning**: coordinate with all roles on estimates and dependencies; confirm QA approach with QA Lead and deployment strategy with DevOps Engineer.
- **Execution**: track QA gates and CI/CD status; escalate blockers involving DevOps or Support Lead.
- **Release**: confirm readiness across QA Lead, DevOps Engineer, Technical Writer, and Support Lead before release.
- **Retrospective**: facilitate session with all roles; capture action items from every team area.

---

## UX Designer

### Role Summary
UX Designers research user needs, design interaction flows, and create prototypes and design specifications. They ensure the product is usable, accessible, and aligned with customer expectations.

### Responsibilities
- Conduct user research and synthesize findings
- Create wireframes, prototypes, and high-fidelity designs
- Define and document interaction patterns and accessibility requirements
- Collaborate with developers on design implementation and quality
- Participate in usability testing and incorporate feedback

### Goals
- Deliver intuitive, accessible user experiences
- Reduce design-implementation rework through clear specifications
- Advocate for user needs throughout the project lifecycle

### Typical Communication
- Design review sessions with Product Manager and Developers
- Prototype walkthroughs and usability test reports
- Design specs and annotated mockups shared via design tool or docs

### Interactions
- **Initiation**: provide user research insights to inform the Project One-pager and success metrics.
- **Planning**: define user flows and design requirements alongside Product Manager; flag UX dependencies for Developers.
- **Execution**: work closely with Developers on implementation fidelity; review built features against designs; partner with QA Lead on usability checks.
- **Release**: review final UI with QA Lead; provide screenshots or design notes to Technical Writer for user documentation.
- **Retrospective**: share usability observations and propose design improvements.

---

## Technical Writer

### Role Summary
Technical Writers create and maintain user-facing and internal documentation. They ensure information is accurate, consistent, and accessible to the intended audience.

### Responsibilities
- Author and maintain user guides, API docs, release notes, and changelogs
- Collaborate with Developers and QA Lead to verify technical accuracy
- Work with UX Designer to document UI flows and features
- Ensure documentation is complete before release
- Update internal process docs as workflows evolve

### Goals
- Ensure users and support staff have the information needed to use and support the product
- Reduce support tickets by providing clear, discoverable documentation
- Keep all project documentation accurate and up-to-date

### Typical Communication
- Documentation review cycles with Developers and Product Manager
- Release notes drafts shared with Product Manager and Support Lead
- Coordination with UX Designer on UI walkthroughs

### Interactions
- **Planning**: review backlog to identify documentation needs; align with Product Manager on scope of user-facing docs.
- **Execution**: interview Developers and UX Designer to document new features; collaborate with QA Lead to confirm documented behavior matches tested behavior.
- **Release**: finalize and publish release notes and user-facing docs before deployment (see [octoacme-release-and-deployment.md](./octoacme-release-and-deployment.md)); hand off to Support Lead.
- **Retrospective**: assess documentation gaps and propose improvements.

---

## QA Lead

### Role Summary
The QA Lead owns the testing strategy and quality gates across the project lifecycle. They ensure that features meet acceptance criteria and that defects are identified and resolved before release.

### Responsibilities
- Define and maintain the test plan and test strategy
- Manage manual and automated test execution
- Own the QA column on the project board and triage incoming defects
- Enforce quality gates before features move to Done or to release
- Collaborate with Developers on test coverage and CI integration
- Validate release readiness and sign off on pre-release smoke tests

### Goals
- Prevent defects from reaching production
- Build confidence in release readiness through systematic testing
- Continuously improve test automation and coverage

### Typical Communication
- Daily standups and defect triage sessions
- Test reports and quality dashboards shared with Project Manager and Product Manager
- Pre-release sign-off confirmation to DevOps Engineer and Project Manager

### Interactions
- **Planning**: contribute to Definition of Done; draft test plan aligned with scope (see [octoacme-project-planning.md](./octoacme-project-planning.md)).
- **Execution**: manage the QA column on the project board; work with Developers on test fixes; ensure CI quality checks pass (see [octoacme-execution-and-tracking.md](./octoacme-execution-and-tracking.md)).
- **Release**: execute pre-release smoke tests; provide formal sign-off before deployment (see [octoacme-release-and-deployment.md](./octoacme-release-and-deployment.md)).
- **Retrospective**: report on defect trends and propose quality improvements.

---

## DevOps Engineer

### Role Summary
DevOps Engineers own the CI/CD pipelines, infrastructure, environments, and deployment processes. They enable reliable, repeatable, and observable software delivery.

### Responsibilities
- Design and maintain CI/CD pipelines and automation
- Manage environments (development, staging, production)
- Own the deployment runbook and rollback procedures
- Integrate security, performance, and quality scanning into the pipeline
- Monitor system health and observability tooling post-deployment
- Coordinate deployment windows and change management

### Goals
- Enable fast, safe, and repeatable deployments
- Minimize deployment risk through automation and testing
- Provide observability and quick incident recovery

### Typical Communication
- Deployment readiness notifications to Project Manager and QA Lead
- Incident alerts and post-mortems
- Infrastructure and pipeline documentation

### Interactions
- **Planning**: advise on infrastructure requirements and deployment feasibility; flag DevOps dependencies.
- **Execution**: maintain CI/CD pipelines; unblock Developers on environment issues; ensure quality gates run in CI (see [octoacme-execution-and-tracking.md](./octoacme-execution-and-tracking.md)).
- **Release**: execute or oversee deployment per the deployment checklist; coordinate with QA Lead on smoke tests; provide rollback plan (see [octoacme-release-and-deployment.md](./octoacme-release-and-deployment.md)).
- **Retrospective**: review deployment metrics, incident trends, and propose pipeline improvements.

---

## Stakeholders

Stakeholders are people or groups with a direct interest in project outcomes. OctoAcme recognizes three primary stakeholder subtypes:

### Customer / User Representative

#### Role Summary
Customer/User Representatives bring the voice of the end user into the project. They provide feedback, validate prototypes, and help confirm that delivered features meet real needs.

#### Responsibilities
- Represent end-user needs and priorities in planning and review sessions
- Provide timely feedback on prototypes, demos, and early releases
- Validate acceptance criteria from a user perspective
- Escalate user-facing issues to the Product Manager

#### Goals
- Ensure the product solves real user problems
- Reduce time to value for end users

#### Typical Communication
- Sprint demos and user testing sessions
- Ad-hoc feedback via Product Manager or designated channel

#### Interactions
- **Initiation**: interviewed by Product Manager to validate problem statement.
- **Execution**: attend sprint demos; provide feedback to Product Manager and UX Designer.
- **Release**: participate in user acceptance testing (UAT) where applicable.
- **Retrospective**: share user sentiment and satisfaction observations.

---

### Executive Sponsor

#### Role Summary
The Executive Sponsor champions the project at the organizational level. They provide strategic direction, authorize resources, and remove executive-level blockers.

#### Responsibilities
- Approve the project charter and major scope changes
- Allocate budget and resources
- Remove organizational blockers and facilitate cross-department alignment
- Receive and act on escalations from the Project Manager

#### Goals
- Ensure the project delivers strategic business value
- Keep the initiative resourced and unblocked

#### Typical Communication
- Monthly or milestone-based status updates from Project Manager
- Escalation notifications for high-impact risks and decisions
- Post-project value review

#### Interactions
- **Initiation**: approve go/no-go and authorize resources (see [octoacme-project-initiation.md](./octoacme-project-initiation.md)).
- **Planning**: review and approve high-level scope, timeline, and budget.
- **Execution**: receive escalations for Level 3 blockers (see [octoacme-risks-and-communication.md](./octoacme-risks-and-communication.md)).
- **Release**: receive release announcement and high-level outcome summary.
- **Retrospective**: review business impact and strategic learnings.

---

### Support Lead

#### Role Summary
The Support Lead represents the customer support function. They ensure support teams are prepared to handle questions and issues related to new releases, and they feed operational insights back to the product team.

#### Responsibilities
- Review release notes and user documentation before release
- Brief and train support staff on new features and known issues
- Define and document support runbooks for new functionality
- Escalate recurring customer issues as product feedback
- Coordinate incident communication with the DevOps Engineer during production issues

#### Goals
- Minimize customer-impacting incidents and time-to-resolution
- Ensure support teams are release-ready
- Close the feedback loop between customers and the product team

#### Typical Communication
- Pre-release documentation review with Technical Writer
- Support runbooks and FAQs for new releases
- Escalation paths during incidents with DevOps Engineer

#### Interactions
- **Planning**: flag known supportability concerns to Product Manager.
- **Execution**: stay informed of upcoming features to prepare support materials.
- **Release**: confirm support readiness before deployment; receive final release notes from Technical Writer (see [octoacme-release-and-deployment.md](./octoacme-release-and-deployment.md)).
- **Retrospective**: report on support ticket trends and customer pain points.

---

## How these roles interact

The table below summarizes key touchpoints across the project lifecycle. See individual role **Interactions** sections above for more detail, and the [RACI matrix](./octoacme-roles-and-raci.md) for accountability assignments.

| Lifecycle Phase | Key Interactions |
|---|---|
| **Initiation** | Executive Sponsor approves charter. Product Manager + UX Designer align on user needs. Project Manager onboards all roles. Customer/User Rep validates problem statement. |
| **Planning** | Product Manager + UX Designer define flows. QA Lead drafts test plan. DevOps Engineer advises on infrastructure. Project Manager aligns everyone on scope, milestones, and Definition of Done. |
| **Execution** | Developers + UX Designer ensure design fidelity. QA Lead owns quality gates; works with Developers on CI. DevOps Engineer maintains pipelines. Technical Writer documents features as they land. |
| **Release** | DevOps Engineer deploys; QA Lead signs off on smoke tests. Technical Writer publishes docs. Support Lead confirms support readiness. Project Manager confirms release go/no-go. |
| **Retrospective** | Project Manager facilitates. All roles contribute learnings. Customer/User Rep and Support Lead share user feedback. Executive Sponsor reviews business outcomes. |

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

