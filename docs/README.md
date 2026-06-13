# OctoAcme Project Management Docs

This README provides a comprehensive summary of OctoAcme's project management processes and quick links to the detailed process documents maintained in the docs/ folder.

## Summary

OctoAcme follows a comprehensive, lifecycle-based approach to project management grounded in clear ownership, iterative delivery, and data-informed decision-making. The framework spans five core phases: **Initiation**, **Planning**, **Execution**, **Release**, and **Retrospective**. During initiation, teams validate business need and stakeholder alignment by developing a lightweight One-pager that captures the problem statement, success metrics, and initial timeline. Once approved, the planning phase transforms the initiative into an actionable backlog with prioritized, estimated items that include clear acceptance criteria and a Definition of Done. This structured approach ensures that all work moving into execution has been thoroughly vetted and that team capacity is understood upfront.

Execution and tracking are coordinated through a consistent team rhythm that includes daily standups (15 minutes), weekly delivery syncs, and sprint-based iterations managed on a project board. The team uses small pull requests (≤400 lines), automated CI/CD pipelines, and a requirement for at least one approval before merging to maintain quality. Quality assurance is woven throughout delivery via unit tests, integration tests, end-to-end smoke tests, and security scanning in CI, with manual QA applied for critical feature acceptance. Risk and blocker escalation follows a tiered model: team-level triage during standups, PM escalation to Product Leads and dependent teams, and sponsor-level involvement for business-impacting issues.

Three primary roles drive OctoAcme projects: **Project Managers** coordinate delivery, manage schedules and risks, and facilitate cross-team communication; **Product Managers** define outcomes, prioritize the backlog, and measure success through data; and **Developers** implement features, collaborate on design, and contribute to estimating and risk identification. Communication is structured through weekly syncs between PM and Product Manager, twice-weekly team standups, and monthly stakeholder updates using templates that highlight progress, next steps, risks, and decisions needed. Release and deployment follow standardized checklists that include pre-release verification, smoke testing on staging, post-deploy verification, and rollback procedures to minimize production risk.

Finally, OctoAcme embeds continuous improvement into its culture through retrospectives held after sprints, releases, or key milestones. Teams capture learnings (what went well, what could improve), generate 2–3 prioritized action items with clear owners and timelines, and track their impact in the project backlog. This closed-loop approach—from initiation through retrospective—ensures that processes are not static but evolve based on team experience and measurable outcomes.

## Documents

- **[Project Management Overview](octoacme-project-management-overview.md)** — High-level introduction to OctoAcme's approach, core roles, key artifacts, and lifecycle.
- **[Project Initiation Guide](octoacme-project-initiation.md)** — Steps to validate and authorize work, align stakeholders, and create a lightweight plan.
- **[Project Planning](octoacme-project-planning.md)** — Turn an approved initiative into an actionable plan and backlog for delivery.
- **[Execution & Tracking](octoacme-execution-and-tracking.md)** — Guidance for managing day-to-day execution and tracking progress toward project milestones.
- **[Release & Deployment Guide](octoacme-release-and-deployment.md)** — Standardize how OctoAcme releases features to production to reduce risk and improve observability.
- **[Risk Management & Communication](octoacme-risks-and-communication.md)** — Explain how to identify, manage, and communicate risks and dependencies.
- **[Retrospective & Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md)** — Capture learnings and convert them into actionable improvements.
- **[Roles & Personas](octoacme-roles-and-personas.md)** — Define typical roles and responsibilities used in OctoAcme project docs and exercises.

## How to Use

1. **New to OctoAcme?** Start with the [Project Management Overview](octoacme-project-management-overview.md) to understand roles and core artifacts.
2. **Starting a new project?** Follow the [Project Initiation Guide](octoacme-project-initiation.md) and use the one-pager template.
3. **Ready to plan?** Use [Project Planning](octoacme-project-planning.md) to create a backlog, estimate, and define milestones.
4. **In execution?** Follow the [Execution & Tracking](octoacme-execution-and-tracking.md) guidance for PR conventions, CI, and QA practices.
5. **Approaching release?** Review the [Release & Deployment Guide](octoacme-release-and-deployment.md) checklist and prepare rollback plans.
6. **After a sprint or release?** Run a [Retrospective](octoacme-retrospective-and-continuous-improvement.md) and convert action items into tracked issues.
7. **Managing risks?** Consult the [Risk Management & Communication](octoacme-risks-and-communication.md) guide for escalation paths and stakeholder updates.

## Contribution

To propose edits or add new process content, open an issue using the "[Add Content to Project Management Process Docs](.github/ISSUE_TEMPLATE/add-update-content-to-process-docs.yml)" template and select "new document" if creating a new file.
