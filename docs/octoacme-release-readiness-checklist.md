# OctoAcme — Release Readiness Checklist

## Purpose
Gate each release with a consistent set of checks before the Release Manager calls a go/no-go. This checklist supplements the Deployment Checklist in `octoacme-release-and-deployment.md` with role-specific sign-offs.

---

## Release Information

| Field | Value |
|---|---|
| Release name / version | |
| Planned deployment window | |
| Release Manager | |
| PM (Project Manager) | |
| PdM (Product Manager) | |
| QA lead | |
| On-call engineer | |

---

## Feature Completeness (PdM + BA)

- [ ] All planned features for this release are merged and deployed to staging
- [ ] Acceptance criteria for each feature verified by PdM or BA
- [ ] Scope changes since last release reviewed and approved
- [ ] Release notes drafted and reviewed by PdM

---

## Design & UX (UX Designer)

- [ ] UI changes reviewed against approved design specs
- [ ] Accessibility requirements verified (or deferred items documented)
- [ ] No critical UX regressions identified in staging

---

## Quality Assurance (QA / Testing)

- [ ] Full regression suite completed on staging
- [ ] All release-blocking defects resolved
- [ ] Non-blocking defects logged with agreed disposition
- [ ] Automated CI checks (unit, integration, security scan) passing
- [ ] End-to-end smoke tests passing on staging
- [ ] UAT completed and sign-off recorded (if applicable)

---

## Technical Readiness (Developers + Release Manager)

- [ ] All PRs merged; no outstanding code review blockers
- [ ] Database migrations tested and rollback scripts prepared (if applicable)
- [ ] Configuration / environment variable changes documented and applied to staging
- [ ] Rollback plan documented and verified
- [ ] On-call engineer briefed on the release and potential risks

---

## Stakeholder & Communication Readiness (PM + Release Manager)

- [ ] Deployment window confirmed with PM and communicated to stakeholders
- [ ] External Stakeholder / Sponsor approvals obtained (if required for this release)
- [ ] Support team briefed on changes and known issues
- [ ] Release announcement drafted (internal and/or external)

---

## Go / No-Go Decision

| Role | Sign-off | Date |
|---|---|---|
| Release Manager | ☐ Go  ☐ No-Go | |
| PdM (Product Manager) | ☐ Go  ☐ No-Go | |
| PM (Project Manager) | ☐ Go  ☐ No-Go | |
| QA Lead | ☐ Go  ☐ No-Go | |

**Decision:** ☐ Go — proceed with deployment  ☐ No-Go — document blockers below

**Blockers (if No-Go):**
- 

---

## Post-Release Verification (Release Manager)

- [ ] Production deployment completed successfully
- [ ] Post-deploy smoke tests passing
- [ ] Key metrics and error rates within normal bounds
- [ ] Release announcement sent to stakeholders
- [ ] Any incidents triggered during release logged in the risk register

---

## Related Documents
- [Roles & Personas](octoacme-roles-and-personas.md)
- [Role Handoff Checklist](octoacme-role-handoff-checklist.md)
- [Release & Deployment Guide](octoacme-release-and-deployment.md)
- [Risk Management & Communication](octoacme-risks-and-communication.md)
- [Execution & Tracking](octoacme-execution-and-tracking.md)
