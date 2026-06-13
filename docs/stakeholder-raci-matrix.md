# OctoAcme — Stakeholder RACI Matrix

## Purpose

Define roles and responsibilities for key decisions and activities across the project lifecycle using the RACI model (Responsible, Accountable, Consulted, Informed).

## RACI Definitions

- **R — Responsible**: Does the work or makes the decision
- **A — Accountable**: Ultimately answerable for the outcome; has veto power
- **C — Consulted**: Provides input and feedback before decision
- **I — Informed**: Kept informed of decision but doesn't participate in decision-making

## Project Initiation

| Activity | PM | PdM | Sponsor | Stakeholders | Engineering Lead |
|----------|----|----|---------|--------------|------------------|
| Define problem statement | C | **A** | C | C | C |
| Set success metrics | C | **A** | C | I | C |
| Identify stakeholders | **R** | **A** | C | - | C |
| Get sponsor alignment | **R** | C | **A** | C | I |
| Go/no-go decision | C | C | **A** | I | C |

## Planning

| Activity | Delivery Lead | Engineering Lead | QA Lead | Security Lead | Product Manager | Sponsor |
|----------|--------------|------------------|---------|---------------|-----------------|----------|
| Define scope | **R** | C | C | C | **A** | I |
| Create backlog | **R** | C | - | - | **A** | I |
| Estimate work | **R** | **R** | C | C | C | I |
| Define DoD | **R** | C | **A** | C | C | - |
| Plan timeline | **R** | C | C | C | **A** | C |
| Identify risks | **R** | C | C | C | C | **A** |
| Plan releases | **R** | C | C | C | **A** | C |

## Execution

| Activity | Developers | Delivery Lead | QA Lead | Managers | Product Manager |
|----------|-----------|---------------|---------|----------|------------------|
| Implement features | **R** | I | - | I | - |
| Code review | **A** | I | - | C | - |
| Unit testing | **R** | - | C | - | - |
| Feature acceptance | C | C | **A** | - | C |
| Track progress | I | **R** | I | C | **A** |
| Escalate blockers | I | **R** | I | **A** | **A** |
| Update documentation | **R** | C | - | - | C |

## Testing & QA

| Activity | QA Lead | Developers | Delivery Lead | Security Lead | Product Manager |
|----------|---------|-----------|---------------|---------------|------------------|
| Create test plan | **R** | - | C | C | **A** |
| Execute tests | **R** | I | - | - | - |
| Log defects | **R** | - | C | - | I |
| Triage defects | **A** | **R** | C | C | C |
| Approve for release | **R** | I | C | C | **A** |
| Security testing | **A** | C | - | **R** | - |

## Release & Deployment

| Activity | Release Manager | Developers | QA Lead | Product Manager | Operations |
|----------|----------------|-----------|---------|-----------------|------------|
| Create deployment plan | **R** | C | C | C | **A** |
| Test in staging | C | I | **R** | - | C |
| Schedule release | **R** | - | - | **A** | C |
| Deploy to production | **R** | I | - | - | **A** |
| Monitor post-deploy | **A** | I | - | - | **R** |
| Rollback decision | C | I | C | **A** | **R** |
| Release announcement | - | - | - | **R** | **A** |

## Risks & Issues

| Activity | Project Manager | Delivery Lead | Sponsor | Affected Team |
|----------|-----------------|---------------|---------|----------------|
| Identify risks | **A** | **R** | I | **C** |
| Assess risk impact | **A** | **R** | C | C |
| Create mitigation plan | **R** | **C** | - | **A** |
| Escalate high risks | **A** | **R** | **A** | I |
| Monitor risk status | **R** | **C** | I | I |
| Implement mitigation | - | **A** | - | **R** |

## Retrospective & Improvements

| Activity | Project Manager | Delivery Lead | Team Lead | All Team | Sponsor |
|----------|-----------------|---------------|-----------|----------|----------|
| Schedule retrospective | **A** | **R** | C | I | I |
| Facilitate discussion | **R** | **C** | - | C | - |
| Document learnings | **R** | C | C | C | I |
| Create action items | **A** | **R** | **C** | C | I |
| Assign owners | **R** | **A** | - | - | I |
| Track action progress | **R** | C | - | - | I |

## Cross-Functional Decisions

| Decision | Product Manager | Engineering Lead | Design Lead | Security Lead | Sponsor |
|----------|-----------------|------------------|-------------|---------------|----------|
| Scope change | **A** | **C** | C | C | **C** |
| Timeline adjustment | **A** | **C** | - | - | **C** |
| Quality tradeoff | **A** | **C** | - | C | **C** |
| Technology choice | **C** | **A** | - | **C** | I |
| Security requirement | C | C | - | **A** | **C** |
| Resource reallocation | **C** | **A** | - | - | **C** |
| Release postponement | **A** | **C** | - | C | **A** |

## Key Principles

1. **Every activity has one Accountable owner** — usually a manager or lead
2. **Responsible parties report to Accountable owner** — clear escalation path
3. **Consult early and often** — before decisions are made
4. **Inform widely** — even if not consulted, stakeholders deserve to know
5. **Respect expertise** — Consult people with relevant knowledge
6. **Make decisions explicit** — Document who made what decision and when
7. **Escalate when unclear** — If RACI is ambiguous, clarify before executing

## Using This Matrix

### During Planning
1. Print or share this matrix with the team
2. Review and adjust roles based on your team composition
3. Add rows for activities specific to your project
4. Confirm all team members understand their role for each decision

### During Execution
1. Reference this matrix when decisions need to be made
2. Follow the escalation path defined by RACI
3. If conflicts arise, reference RACI to clarify decision rights
4. Update RACI if roles shift during project

### In Retrospectives
1. Review whether RACI was followed
2. Identify decision delays caused by unclear ownership
3. Note adjustments for future projects

## Template for Project-Specific RACI

Copy this template and customize for your project:

| Activity | Role 1 | Role 2 | Role 3 | Role 4 | Role 5 |
|----------|--------|--------|--------|--------|--------|
| Activity 1 | R/A/C/I | | | | |
| Activity 2 | R/A/C/I | | | | |
| Activity 3 | R/A/C/I | | | | |

**Tips**:
- Fill in your team's specific roles
- Add activities relevant to your project
- Ensure each row has at least one **A** (Accountable)
- Minimize the number of **R** roles per activity (one or two is ideal)
- Ensure everyone understands the matrix before starting
