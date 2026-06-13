# OctoAcme — Quality Assurance Gate Checklist

Use this checklist at key quality gates during development to ensure features meet acceptance standards before proceeding to the next phase.

## Definition of Ready (Pre-Development)

**Purpose**: Ensure work is well-defined before developers start.

- [ ] User story or acceptance criteria clearly written
- [ ] Acceptance criteria are measurable and testable
- [ ] Dependencies identified and documented
- [ ] QA Lead has reviewed and approved acceptance criteria
- [ ] Design or technical spec (if needed) is complete
- [ ] No blockers or unknowns remain

**Gate Owner**: Product Manager / Delivery Lead  
**Action**: If not ready, return to backlog for refinement

---

## In-Development QA Checks

**Purpose**: Maintain quality throughout development.

- [ ] Developer has written unit tests (target: >80% code coverage)
- [ ] Code follows team's coding standards and best practices
- [ ] Code review completed and approved by at least one peer
- [ ] No linting or formatting errors
- [ ] Security scanning passed in CI pipeline
- [ ] No integration conflicts with other work

**Gate Owner**: Engineering Manager / Lead Developer  
**Action**: If not passed, address issues before moving to QA

---

## QA Testing Gate (Feature Testing)

**Purpose**: Verify features meet acceptance criteria and quality standards.

- [ ] Feature deployed to QA/staging environment
- [ ] QA Lead has created and executed test plan
- [ ] All acceptance criteria verified and passing
- [ ] Happy path testing passed (main user workflows)
- [ ] Edge cases and error scenarios tested
- [ ] Regression testing completed for related features
- [ ] Performance testing passed (if applicable)
- [ ] Accessibility testing passed (if applicable)
- [ ] No critical or high-priority bugs remain
- [ ] All defects documented and prioritized

**Gate Owner**: QA Lead / Test Engineer  
**Action**: If issues found, create bugs and assign to developers for fixes

---

## Security & Compliance Gate

**Purpose**: Ensure security and compliance standards are met.

- [ ] Security scanning passed in CI pipeline
- [ ] No high-severity vulnerabilities identified
- [ ] Threat modeling completed (if applicable)
- [ ] Secure coding practices followed
- [ ] Authentication/authorization properly implemented
- [ ] Data handling meets privacy requirements
- [ ] Compliance requirements verified (GDPR, HIPAA, etc. if applicable)
- [ ] Security Lead has approved for release

**Gate Owner**: Security Lead  
**Action**: If issues found, escalate to Product Manager for prioritization

---

## Integration & Release Readiness Gate

**Purpose**: Ensure features are ready for staging/production deployment.

- [ ] All features deployed to staging environment
- [ ] End-to-end (E2E) smoke tests passing
- [ ] All components integrated successfully
- [ ] No data migration issues identified
- [ ] Feature flags or rollout plan in place (if needed)
- [ ] Rollback plan documented
- [ ] Release notes drafted
- [ ] Documentation updated
- [ ] Post-deployment monitoring configured

**Gate Owner**: Release Manager / Delivery Lead  
**Action**: If issues found, resolve before proceeding to production deployment

---

## UAT / Stakeholder Acceptance Gate

**Purpose**: Validate features meet business requirements with key stakeholders.

- [ ] Staging environment available and stable
- [ ] UAT script or scenario provided to stakeholders
- [ ] Key stakeholders have tested features
- [ ] Business acceptance criteria met
- [ ] No blocking issues from stakeholders
- [ ] Sign-off obtained from Product Manager and key stakeholders

**Gate Owner**: Product Manager  
**Action**: If issues found, prioritize fixes. If critical, may defer to next release

---

## Pre-Production Deployment Gate

**Purpose**: Final verification before deploying to production.

- [ ] All QA gates passed
- [ ] Security scan passed
- [ ] Performance testing passed
- [ ] Staging smoke tests passed
- [ ] Rollback plan reviewed and tested
- [ ] On-call team notified and ready
- [ ] Deployment window scheduled
- [ ] Stakeholder notifications prepared
- [ ] Post-deployment monitoring dashboards ready

**Gate Owner**: Release Manager / Product Manager  
**Action**: If any gate not passed, delay deployment. Do NOT deploy if gates not met.

---

## Post-Deployment Verification Gate

**Purpose**: Verify production deployment is healthy.

- [ ] Deployment completed successfully
- [ ] Application is running and responsive
- [ ] No error spikes in monitoring
- [ ] Key user workflows functioning
- [ ] Customer-facing features working as expected
- [ ] Performance metrics normal
- [ ] Security alerts quiet (no suspicious activity)
- [ ] Support team reports no critical issues

**Gate Owner**: Release Manager / Operations  
**Action**: If issues detected, execute rollback plan immediately

---

## Release Sign-Off Gate

**Purpose**: Final approval before announcing release.

- [ ] Post-deployment verification passed
- [ ] No critical bugs or issues
- [ ] Performance impact acceptable
- [ ] Data integrity verified (if applicable)
- [ ] Release notes approved
- [ ] Stakeholders notified
- [ ] Feature is ready for general availability

**Gate Owner**: Product Manager  
**Action**: Release approved for general availability or rollback if needed

---

## Quality Metrics & Tracking

**Track these metrics for each release:**

- [ ] Total number of bugs found in QA: ____
- [ ] Number of critical/high bugs: ____
- [ ] Test coverage: ____% (Target: >80%)
- [ ] Time in QA phase: ____ days
- [ ] Number of test cycles: ____
- [ ] Defect escape rate (bugs found in production): ____
- [ ] Time to fix post-deployment issues: ____ hours

**Review these metrics in retrospective to identify process improvements.**
