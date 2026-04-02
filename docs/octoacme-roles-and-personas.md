# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

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

---

## Business Analyst

### Role Summary
Business Analysts (BA) bridge business needs and technical implementation. They translate stakeholder requirements into clear, actionable specifications that developers and PdMs can act on.

### Responsibilities
- Elicit, document, and refine business and functional requirements
- Facilitate workshops and discovery sessions with stakeholders
- Create user stories, process flows, and acceptance criteria
- Validate that delivered features meet business outcomes
- Identify and resolve ambiguities between business intent and technical design

### Goals
- Ensure requirements are clear, complete, and testable before development begins
- Reduce re-work caused by misunderstood or incomplete requirements
- Improve traceability from business need to delivered feature

### Typical Communication
- Requirements reviews and sign-off sessions with PdMs and stakeholders
- Grooming sessions with developers to clarify story details
- Sprint demos to confirm acceptance criteria were met

### Interactions / Collaboration Map
| Touchpoint | Details |
|---|---|
| **PM (Project Manager)** | Align on scope, timeline, and delivery constraints; surface requirement changes that affect schedule |
| **PdM (Product Manager)** | Co-define acceptance criteria and success metrics; validate feature prioritisation against business goals |
| **Developers** | Walk through requirements; answer questions during development; review implementation against specs |
| **QA / Testing** | Share acceptance criteria and edge cases; review test plans to confirm coverage |
| **Stakeholders / Sponsors** | Facilitate requirements workshops; obtain sign-off on functional specs; communicate scope changes |

---

## UX Designer

### Role Summary
UX Designers ensure that user experience considerations are embedded throughout planning and development. They advocate for end users and translate research insights into designs that guide implementation.

### Responsibilities
- Conduct user research and usability studies
- Create wireframes, prototypes, and design specifications
- Define interaction patterns and accessibility requirements
- Participate in sprint planning to inform effort estimates for design work
- Review implemented features against design specs and flag deviations

### Goals
- Deliver intuitive, accessible, and consistent user experiences
- Reduce usability defects discovered late in delivery
- Align design decisions with product vision and technical feasibility

### Typical Communication
- Design reviews with PdMs and developers before implementation begins
- Usability feedback shared after QA testing or user testing sessions
- Async feedback via design tools (e.g., Figma comments) and PR reviews

### Interactions / Collaboration Map
| Touchpoint | Details |
|---|---|
| **PM (Project Manager)** | Coordinate design timelines and flag dependencies that affect sprint planning |
| **PdM (Product Manager)** | Align on product vision, user personas, and feature priorities; co-review research findings |
| **Developers** | Provide design specs and assets; clarify intent during implementation; review UI output before QA handoff |
| **QA / Testing** | Share interaction specs and edge-case flows; review QA test results for UX regressions |
| **Stakeholders / Sponsors** | Present design proposals and usability findings; collect feedback at key review gates |

---

## Release Manager

### Role Summary
Release Managers coordinate deployments and release communications. They own the release process end-to-end, ensuring technical readiness, stakeholder awareness, and smooth rollout.

### Responsibilities
- Own and maintain the release schedule and deployment calendar
- Drive the Release Readiness Checklist (see `octoacme-release-readiness-checklist.md`) before each deployment
- Coordinate go/no-go decisions with PM, PdM, and technical leads
- Communicate release plans and post-release status to stakeholders
- Lead incident response coordination if a deployment causes issues; trigger rollback when needed
- Maintain release notes and post-deploy verification records

### Goals
- Reduce deployment risk through consistent pre-release gating
- Keep stakeholders informed before, during, and after each release
- Shorten mean time to recovery (MTTR) when incidents occur

### Typical Communication
- Release planning meetings with PM and engineering leads
- Go/no-go calls before each deployment window
- Release announcements and incident updates to stakeholders
- Post-release retrospective notes captured in the risk register

### Interactions / Collaboration Map
| Touchpoint | Details |
|---|---|
| **PM (Project Manager)** | Align release windows with project schedule; co-manage blocker escalation (Level 2/3 per escalation path in `octoacme-execution-and-tracking.md`) |
| **PdM (Product Manager)** | Confirm feature completeness and acceptance before release; coordinate release note content |
| **Developers** | Verify technical readiness (CI passing, smoke tests, rollback plan); coordinate hotfix deployments |
| **QA / Testing** | Gate release on QA sign-off; review outstanding defects for release-blocking determination |
| **Stakeholders / Sponsors** | Communicate release schedule, scope, and post-release status; escalate business-impacting incidents per escalation path |

---

## External Stakeholder / Advisor

### Role Summary
External Stakeholders and Advisors represent outside perspectives, such as customers, compliance bodies, partner organisations, or advisory board members. They provide strategic input and approval at key project gates without involvement in day-to-day execution.

### Responsibilities
- Provide domain expertise, compliance guidance, or customer perspective on requirements
- Review and approve major scope changes or deliverables at defined checkpoints
- Raise concerns or constraints that may affect project direction
- Participate in milestone demos or steering committee reviews as agreed

### Goals
- Ensure the project meets external requirements, regulations, or customer expectations
- Provide timely feedback to avoid late-stage rework
- Maintain confidence in the project's direction and progress

### Typical Communication
- Scheduled milestone or steering committee reviews
- Requirements review sign-off documents
- Release announcements and status summaries (consumer view)

### Interactions / Collaboration Map
| Touchpoint | Details |
|---|---|
| **PM (Project Manager)** | Receive project status updates; raise schedule or scope concerns through the PM; included in Level 3 escalation path per `octoacme-execution-and-tracking.md` |
| **PdM (Product Manager)** | Validate requirements against external needs (compliance, customer advisory); contribute to prioritisation at key milestones |
| **Developers** | Attend demos at milestone reviews; provide feedback on delivered functionality (not day-to-day involvement) |
| **QA / Testing** | Review acceptance criteria for compliance or customer-specific requirements; may observe UAT sessions |
| **Stakeholders / Sponsors** | Coordinate with internal sponsors on approval gates; escalate blocking concerns through the sponsor if needed |

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

