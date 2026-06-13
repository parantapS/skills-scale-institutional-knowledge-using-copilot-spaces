# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

---

## Core Roles

### Developers

#### Role Summary
Developers design, build, test, and deliver software components. They collaborate with product and project leads to implement features that meet acceptance criteria and quality standards.

#### Responsibilities
- Implement features and fixes to meet acceptance criteria
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Help identify technical risks and propose mitigations

#### Goals
- Deliver reliable, maintainable code
- Reduce cycle time from idea to production
- Maintain high test coverage and observability

#### Typical Communication
- Daily standups and sprint planning
- PR descriptions and code review comments
- Technical design docs when needed

#### Interactions
- Works with Engineering Manager on technical direction and capacity allocation
- Collaborates with QA Lead and Test Engineers on acceptance criteria and test coverage
- Partners with Release Manager on deployment readiness
- Supports Security Lead on secure design and threat modeling

---

### Product Managers

#### Role Summary
Product Managers define what should be built to deliver customer and business value. They own the product vision, prioritize the backlog, and measure outcomes.

#### Responsibilities
- Define problem statements and success metrics
- Prioritize the roadmap and backlog
- Collaborate with stakeholders and engineering on trade-offs
- Validate solutions through user research and metrics

#### Goals
- Maximize customer value and impact
- Make clear, data-driven prioritization decisions
- Ensure product-market fit and usability

#### Typical Communication
- Weekly alignment with PM and engineering leads
- Roadmap updates and stakeholder briefings
- Acceptance criteria and feature specs

#### Interactions
- Partners with Project Manager on timeline and resource planning
- Collaborates with Data Analyst on success metrics and measurement
- Works with UX Researcher on user needs and design validation
- Receives escalations from QA Lead on quality risks
- Coordinates with Support Liaison on customer feedback and operational issues

---

### Project Managers

#### Role Summary
Project Managers coordinate delivery activities, manage schedules, risks, and communications. They enable the team to deliver on commitments efficiently.

#### Responsibilities
- Create and maintain project plans and timelines
- Manage risks, dependencies, and resource constraints
- Facilitate meetings (kickoff, planning, retrospectives)
- Ensure consistent project documentation and status reporting
- Coordinate cross-team and stakeholder communication

#### Goals
- Deliver projects on time and within scope
- Minimize unplanned work and escalations
- Maintain transparency and alignment across stakeholders

#### Typical Communication
- Weekly status updates and stakeholder reports
- Risk registers and decision logs
- Coordination via project boards and meeting facilitation

#### Interactions
- Partners with Product Manager on priority and roadmap alignment
- Works with Delivery Lead on sprint planning and dependency tracking
- Escalates blockers to Engineering Manager and product leadership
- Coordinates release timing with Release Manager
- Collects status updates from all functional leads

---

## Expanded Roles

### Delivery Lead

#### Role Summary
Delivery Leads coordinate sprint commitments and track progress against team capacity and cross-team dependencies. They ensure the team stays focused on priorities and escalates blockers.

#### Responsibilities
- Coordinate sprint commitments and capacity planning
- Manage cross-team dependencies and integration points
- Track delivery risks and progress daily
- Escalate blockers and resource constraints to Project Manager
- Facilitate sprint planning, standups, and reviews

#### Goals
- Ensure predictable, on-time delivery
- Minimize context-switching and unplanned work
- Improve cross-team collaboration and handoff clarity

#### Typical Communication
- Daily standups with engineering and QA teams
- Weekly dependency sync with other delivery leads
- Risk escalation to Project Manager when needed

#### Interactions
- Works closely with Project Manager (PM) and Product Manager (PdM) to translate roadmap priorities into committed work
- Coordinates with Engineering Manager on team capacity and resource allocation
- Partners with QA Lead on test planning and release readiness
- Escalates technical risks to Engineering Manager

---

### Engineering Manager

#### Role Summary
Engineering Managers provide technical leadership, manage engineering team capacity, and guide technical direction. They support developers in overcoming technical challenges and mitigating technical debt.

#### Responsibilities
- People management and career development
- Define technical architecture and design standards
- Allocate engineering capacity across initiatives
- Identify and mitigate technical debt and risks
- Support developers in implementation and problem-solving
- Participate in capacity and estimation planning

#### Goals
- Build a high-performing, engaged engineering team
- Maintain code quality and system reliability
- Balance feature delivery with technical health

#### Typical Communication
- 1-on-1s with engineers and career development discussions
- Architecture reviews and design discussions
- Capacity planning with Delivery Lead and Project Manager

#### Interactions
- Collaborates with Delivery Lead on capacity estimates and sprint planning
- Works with Project Manager on resource constraints and tradeoffs
- Supports Developers on technical implementation and risk identification
- Partners with QA Lead and Security Lead on quality and security standards

---

### QA Lead / Test Engineer

#### Role Summary
QA Leads define testing strategy, own test plans for releases, coordinate automated and manual QA, and provide quality sign-off. They escalate quality risks to Product Manager.

#### Responsibilities
- Define testing strategy and test coverage targets
- Create and maintain test plans for each release
- Coordinate automated and manual QA activities
- Identify and escalate quality risks and defects
- Sign off on acceptance criteria before release
- Participate in Definition of Done and acceptance criteria definition

#### Goals
- Ensure features meet quality and acceptance standards
- Reduce escaped defects in production
- Improve test coverage and automation

#### Typical Communication
- Sprint planning and test planning meetings
- Daily QA status in standups
- Quality escalations to Product Manager

#### Interactions
- Works with Developers and Delivery Lead to ensure test coverage and quality
- Coordinates with Release Manager on staging verification
- Escalates quality risks to Product Manager
- Partners with Security Lead on security testing
- Collaborates with UX Researcher on usability acceptance criteria

---

### Release Manager / Platform Engineer

#### Role Summary
Release Managers own release procedures, maintain CI/CD pipeline health, and automate deployment processes. They coordinate with developers and QA to ensure smooth, safe releases.

#### Responsibilities
- Design and maintain release procedures and checklists
- Manage CI/CD pipeline health and reliability
- Automate deployment processes and reduce manual steps
- Create and test rollback plans
- Coordinate staging verification with developers and QA
- Monitor post-deployment health and alerts

#### Goals
- Enable fast, safe, reliable releases
- Minimize deployment failures and rollbacks
- Reduce time-to-recovery for production issues

#### Typical Communication
- Pre-release coordination meetings
- Deployment windows and status updates
- Post-incident reviews and rollback decisions

#### Interactions
- Coordinates with Developers and QA Lead for staging verification
- Works with Project Manager on release windows and scheduling
- Collaborates with Security Lead on security scanning in CI/CD
- Participates in incident response and rollback decisions

---

### Security Lead

#### Role Summary
Security Leads lead threat modeling, manage security scans and triage, and define minimum security acceptance criteria. They ensure security is built in throughout the project lifecycle.

#### Responsibilities
- Lead threat modeling and security design reviews
- Manage security scanning tools and triage results
- Define minimum security acceptance criteria
- Audit and approve secure coding practices
- Escalate security risks to Product Manager
- Participate in incident response for security issues

#### Goals
- Prevent security vulnerabilities in production
- Build security awareness across the team
- Ensure compliance with security standards

#### Typical Communication
- Security design reviews with developers
- Security scan triage meetings
- Escalations to Product Manager on remediation priorities

#### Interactions
- Collaborates with Developers and Product Manager on secure design and threat modeling
- Works with QA Lead on security testing
- Partners with Release Manager on security scanning in CI/CD pipelines
- Coordinates with Engineering Manager on secure coding standards
- Escalates critical vulnerabilities to Product Manager

---

### UX Researcher / Designer

#### Role Summary
UX Researchers and Designers validate user needs, provide research inputs to acceptance criteria, and review designs for usability. They ensure features solve real customer problems in an intuitive way.

#### Responsibilities
- Conduct user research and validate customer needs
- Define user acceptance criteria based on user feedback
- Create wireframes, prototypes, and design specifications
- Review implementations for usability and design consistency
- Test features with users before release

#### Goals
- Ensure features solve real customer problems
- Maximize usability and user satisfaction
- Reduce support burden through intuitive design

#### Typical Communication
- User research findings and synthesis
- Design reviews and feedback to developers
- Usability testing results and recommendations

#### Interactions
- Works with Product Manager to shape requirements and validate user needs
- Collaborates with Developers during implementation reviews
- Partners with QA Lead on usability acceptance criteria
- Provides user feedback to Product Manager for prioritization

---

### Data Analyst / Measurement Owner

#### Role Summary
Data Analysts define and instrument success metrics, create dashboards, and analyze release impact. They ensure OctoAcme is measuring what matters and learning from data.

#### Responsibilities
- Define success metrics aligned with business objectives
- Instrument code and processes to collect measurement data
- Create dashboards and reports for project and product teams
- Analyze feature impact and user adoption
- Provide data-driven insights to Product Manager

#### Goals
- Ensure data-driven decision-making
- Measure and demonstrate impact of features
- Identify opportunities for improvement through data

#### Typical Communication
- Weekly metrics reviews and dashboard updates
- Post-release analysis and impact reports
- Data insights and recommendations to Product Manager

#### Interactions
- Partners with Product Manager to define success criteria
- Works with Developers on measurement instrumentation
- Provides analytics to inform prioritization and roadmap decisions
- Shares learnings from feature launches with the broader team

---

### Support / Operations Liaison

#### Role Summary
Support Liaisons surface production issues, prioritize operational fixes, and participate in incident retrospectives. They represent the voice of the customer and operations team in project planning.

#### Responsibilities
- Track and escalate production issues and customer problems
- Prioritize operational fixes and hotfixes
- Participate in incident response and post-incident retrospectives
- Provide customer feedback to Product Manager
- Identify patterns in customer issues that should inform the roadmap

#### Goals
- Reduce customer-impacting production issues
- Improve time-to-recovery for incidents
- Feed customer feedback into product planning

#### Typical Communication
- Daily issue triage and escalation
- Incident notifications and status updates
- Customer feedback and trends to Product Manager

#### Interactions
- Feeds real-world customer-impacting issues to Product Manager and Developers
- Collaborates with Developers on root cause analysis and fixes
- Participates in post-incident action items and retrospectives
- Escalates critical issues to Project Manager
- Provides customer context to inform prioritization

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
- Reference the "Interactions" sections to understand handoffs and dependencies between roles.
