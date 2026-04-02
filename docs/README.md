# OctoAcme Project Management Docs

## Overview

OctoAcme runs projects through a structured, repeatable lifecycle — **Initiation → Planning → Execution → Release → Close/Retro** — designed to deliver high-quality outcomes with clear ownership and continuous learning. Every project begins with a Project One-pager that captures the problem statement, measurable goals, and success metrics before any work is prioritized. Stakeholders are mapped early, communication plans are set, and a decision gate ensures the team only advances when business needs are clear, priorities are agreed upon, and resources are confirmed.

Planning and execution emphasize small, testable increments managed through a visual project board (Backlog → Ready → In Progress → In Review → QA → Done). Work items follow a consistent backlog template — description, acceptance criteria, priority, estimates, owner, and related docs — and a shared Definition of Done keeps quality expectations unambiguous. During execution, short-lived pull requests follow a PR workflow that requires CI to pass before review and at least one approval before merge. Fixed team cadences (daily standups, weekly delivery syncs, per-sprint demos) surface blockers and dependencies early and keep feedback loops tight.

Roles are clearly separated: the **Project Manager (PM)** owns delivery coordination, schedules, risk, and communications; the **Product Manager (PdM)** defines outcomes, prioritizes the backlog, and measures impact; **Developers** design, implement, test, and maintain code while participating in estimation and review; **QA/Testing** validates quality and acceptance criteria; and **Stakeholders** provide requirements and approvals. Communication follows a layered escalation model — blockers are resolved at the team standup (Level 1), escalated by the PM to the Product Lead or dependency team (Level 2), or raised to the Sponsor (Level 3) — with a single source of truth (project README/status document) and weekly status report templates (progress, next steps, risks/blockers, decisions needed) maintaining consistent, transparent updates.

Quality assurance and release readiness are enforced at every stage. New logic requires unit tests and, where necessary, integration tests; critical flows require end-to-end smoke tests before any release. CI pipelines run automated tests, lint checks, and security scans on every pull request. A release gate confirms that all acceptance criteria are met, CI and security scans pass, release notes are ready, and a rollback/mitigation plan is in place before deploying to staging and then production. Failed or incident-causing deployments trigger the incident notification process and a rollback to the last stable version. Each project closes with a Retrospective that produces a small set of actionable improvement items (owner, due date, success criteria) fed back into the backlog, completing the continuous-improvement loop.

---

## Table of Contents

| Document | Description |
|---|---|
| [OctoAcme Project Management Overview](octoacme-project-management-overview.md) | High-level introduction to OctoAcme's project management approach, principles, roles, and lifecycle |
| [OctoAcme — Project Initiation Guide](octoacme-project-initiation.md) | How to kick off a project: one-pager, stakeholders, timeline, risk inventory, and decision gates |
| [OctoAcme — Project Planning](octoacme-project-planning.md) | Scope, milestones, backlog creation, kickoff template, and Definition of Done |
| [OctoAcme — Execution & Tracking](octoacme-execution-and-tracking.md) | Sprint workflow, PR practices, project board, team cadences, and status reporting |
| [OctoAcme — Risk Management & Communication](octoacme-risks-and-communication.md) | Risk register, escalation levels, communication cadences, and stakeholder update templates |
| [OctoAcme — Release & Deployment Guide](octoacme-release-and-deployment.md) | Release checklist, deployment process, post-deploy verification, and incident/rollback handling |
| [OctoAcme — Retrospective & Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md) | Retrospective format, action-item tracking, and feeding learnings back into the backlog |
| [OctoAcme Personas](octoacme-roles-and-personas.md) | Detailed role definitions for Developers, Product Managers, Project Managers, QA, and Stakeholders |
