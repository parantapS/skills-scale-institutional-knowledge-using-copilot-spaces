# OctoAcme — Dependency & Handoff Management

## Purpose

Provide guidance for identifying, tracking, and managing cross-team dependencies and handoffs to reduce delays and improve coordination.

## Types of Dependencies

### Technical Dependencies
- One feature/service depends on another being available or modified
- Data integration points between systems
- Shared infrastructure or platform changes required
- API or contract dependencies between teams

### Resource Dependencies
- Multiple initiatives competing for same engineering resources
- Subject matter expert (SME) availability
- Infrastructure, security, or ops team capacity
- External vendor or third-party dependencies

### Release/Timeline Dependencies
- Feature A must ship before Feature B
- Integration testing requires both features deployed together
- Coordinated release across multiple systems
- Data migration or database schema changes

### Organizational Dependencies
- Cross-team product alignment
- Stakeholder sign-off or approval required
- Legal, compliance, or security review needed
- Customer or partner feedback loop

---

## Dependency Identification

### When to Identify
- During project planning (kickoff meeting)
- During backlog refinement (before sprint planning)
- During sprint planning (as stories are pulled)
- Continuously during execution (ad-hoc)

### How to Identify

**Ask these questions during planning:**

1. Does this work require input or output from another team?
2. Does this depend on infrastructure, tools, or platforms maintained by others?
3. Is there shared expertise or resources needed?
4. Does this integrate with or modify shared systems?
5. Does this require customer or stakeholder feedback?
6. Does this depend on external libraries, vendors, or services?
7. Does release timing depend on other work being complete?

### Documentation

For each identified dependency, document:

```
Dependency ID: [unique identifier]
Type: [Technical / Resource / Timeline / Organizational]
From: [our initiative]
To: [dependent team/system]
Description: [what is the dependency]
Owner (Them): [contact on dependent team]
Owner (Us): [owner on our team]
Critical Path: [Yes/No - is this on critical path to launch?]
Target Date: [when do we need this resolved?]
Status: [Open / In Progress / Resolved / Blocked]
Risk: [High / Medium / Low]
```

---

## Dependency Tracking

### Dependency Register

Maintain a simple dependency register (spreadsheet or project board) with:

| ID | Description | Type | To Team | Owner (Them) | Target Date | Status | Risk | Notes |
|----|-------------|------|---------|--------------|-------------|--------|------|-------|
| DEP-001 | API contract for user service | Technical | Platform | john@... | 2026-06-20 | In Progress | High | Blocking dev start |
| DEP-002 | Capacity for security review | Resource | Security | jane@... | 2026-06-15 | Open | Medium | No review scheduled |
| DEP-003 | Data migration script | Technical | Data Eng | bob@... | 2026-06-25 | Blocked | High | Waiting on schema approval |

### Review Cadence

- **Weekly**: Review dependency status in delivery sync
- **Daily**: Escalate high-risk or blocked dependencies in standups
- **Monthly**: Stakeholder update includes dependency status

---

## Dependency Escalation

### Level 1: Dependency Coordination (Delivery Team)

**When**: Dependency identified but not urgent  
**Action**:
1. Document in dependency register
2. Direct contact between team owners
3. Schedule coordination sync if needed
4. Agree on target completion date
5. Track in weekly sync

**Owner**: Delivery Lead, Project Manager

### Level 2: Escalation to Team Leads (Management)

**When**: Dependency at risk, timeline slipping, or misalignment between teams  
**Action**:
1. Alert Engineering Manager and other team's lead
2. Highlight business impact and timeline risk
3. Request priority adjustment or resource reallocation
4. Agree on mitigation plan
5. Document decision and next steps

**Owner**: Project Manager, Product Manager

### Level 3: Executive Escalation (Leadership)

**When**: Dependency blocks release, impacts multiple teams, or requires scope/timeline tradeoff  
**Action**:
1. Escalate to Product Lead and Engineering Leadership
2. Present impact analysis and business risk
3. Request executive decision on tradeoffs
4. Execute approved mitigation plan
5. Document decision for retrospective

**Owner**: Product Manager, Project Sponsor

---

## Dependency Mitigation Strategies

### Strategy 1: Break the Dependency
- Refactor architecture to remove dependency
- Use mocks/stubs instead of real dependencies
- Split feature into phased deliveries
- Use feature flags to decouple releases

### Strategy 2: Parallelize Work
- Work on dependent features in parallel
- Use contracts or APIs to define boundaries
- Agree on interfaces upfront
- Integrate incrementally

### Strategy 3: Add Buffer / Contingency
- Identify critical-path dependencies
- Add time buffer for dependent work
- Have backup plan if dependency slips
- Plan for phased rollout

### Strategy 4: Accept the Risk
- Document dependency and timeline risk
- Plan for aggressive schedule (contingency for slippage)
- Prepare escalation plan if slips
- Communicate risk to stakeholders

### Strategy 5: De-prioritize or Defer
- Move dependent feature to later release
- Cut scope from this release
- Reduce feature complexity
- Communicate tradeoff to stakeholders

---

## Handoff Management

### Planning Handoffs

When handing off work between teams (e.g., dev to QA, QA to ops):

**Preparation**:
- [ ] Clear acceptance criteria documented
- [ ] Definition of "ready" agreed between teams
- [ ] Artifacts prepared (code, test data, runbooks)
- [ ] Questions answered by sending team

**Handoff Meeting**:
- [ ] Walkthrough of work and acceptance criteria
- [ ] Receiving team asks clarifying questions
- [ ] Known issues or limitations discussed
- [ ] Timeline and dependencies confirmed
- [ ] Next steps and escalation path agreed

**Follow-up**:
- [ ] Sending team available for questions
- [ ] Status updated in shared project board
- [ ] Issues logged and prioritized
- [ ] Escalation path clear if problems found

### Communication Template for Handoffs

```
Handoff: [Feature/Component Name]
From: [Team/Person Name]
To: [Team/Person Name]
Date: [Handoff Date]

## What is being handed off?
[Brief description]

## Acceptance Criteria
- [ ] Criterion 1
- [ ] Criterion 2
- [ ] Criterion 3

## Artifacts Provided
- [ ] Code/documentation at [location]
- [ ] Test data at [location]
- [ ] Deployment runbook at [location]
- [ ] Other: ____

## Known Issues / Limitations
- Issue 1: [description]
- Issue 2: [description]

## Questions / Clarifications
- Q1: ___?
- Q2: ___?

## Timeline
- Handoff date: [date]
- Expected completion: [date]
- Critical path item: [Yes/No]

## Escalation Path
If blockers arise, escalate to: [Name, title]
```

---

## Dependency Health Metrics

**Track these metrics in retrospectives:**

- Number of dependencies identified in planning
- Number of dependencies completed on time
- Number of dependencies that slipped
- Impact of slipped dependencies (days of delay)
- Number of escalations due to dependencies
- Most common dependency types
- Effectiveness of mitigation strategies used

**Use metrics to identify patterns and improve planning.**

---

## Best Practices

1. **Identify dependencies early**: Preferably during planning, not during execution
2. **Document everything**: Use a shared register accessible to all teams
3. **Communicate frequently**: Weekly reviews at minimum, daily if high-risk
4. **Set clear ownership**: Each dependency should have clear owners on both sides
5. **Build in buffers**: Add time buffer for critical-path dependencies
6. **Have escalation paths**: Make clear who to escalate to and when
7. **Mitigate proactively**: Don't wait for dependencies to slip to take action
8. **Learn from failures**: Review slipped dependencies in retrospectives
9. **Break dependencies when possible**: During planning, consider architecture changes to remove dependencies
10. **Over-communicate**: Explicit, frequent communication prevents surprises
