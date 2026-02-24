# OctoAcme Project Management Docs

Welcome to the central documentation hub for OctoAcme's project management processes. This README provides a concise overview of OctoAcme's delivery methodology and links to all relevant process guides. It is intended as an entry point for new team members and a quick-reference for existing contributors. For the full high-level introduction, see the [Project Management Overview](octoacme-project-management-overview.md).

## Key Workflows

OctoAcme follows a customer-first, iterative, and data-informed delivery model. Projects move through five phases: **Initiation** (validate the business need, align stakeholders, and define success criteria — see [Project Initiation Guide](octoacme-project-initiation.md)); **Planning** (break work into shippable increments, estimate scope, and create a release milestone map — see [Project Planning](octoacme-project-planning.md)); **Execution & Tracking** (daily standups, weekly delivery syncs, project-board–driven workflow, and rigorous PR and testing standards — see [Execution & Tracking](octoacme-execution-and-tracking.md)); **Release & Deployment** (standardized pre-release checks, automated pipeline, post-deploy verifications, and rollback playbook — see [Release & Deployment Guide](octoacme-release-and-deployment.md)); and **Retrospective & Continuous Improvement** (structured sprint/milestone retrospectives converted into tracked action items — see [Retrospective & Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md)). Risk identification, assessment, and escalation run continuously across all phases (see [Risk Management & Communication](octoacme-risks-and-communication.md)).

## Personas & Roles

Four core roles collaborate on every project. The **Project Manager (PM)** owns delivery coordination, schedules, the risk register, and stakeholder communications. The **Product Manager (PdM) / Product Lead** defines the problem statement, owns the roadmap and backlog, and measures outcomes. **Developers** implement features, write and maintain tests, and participate in design and code reviews. **QA/Testing** validates acceptance criteria and coordinates manual and automated quality checks. **Stakeholders** (including sponsors, sales, and support) provide business context, approvals, and feedback. Full persona definitions — including goals, responsibilities, and typical communication patterns — are documented in [Roles & Personas](octoacme-roles-and-personas.md).

## Communication Strategies

OctoAcme maintains a predictable communication cadence: twice-weekly standups for the delivery team, a weekly PM + PdM sync, monthly stakeholder updates, and ad-hoc escalations as needed. A single source of truth (the project README or release doc) is kept current so all stakeholders share the same status view. Standardized templates — weekly status reports (progress, next steps, risks/blockers, decisions needed) and incident communication summaries — reduce ambiguity and speed up information sharing. Escalation follows a clear path: team-level triage → PM → Product Lead → Sponsor; security incidents are routed directly to the Security on-call team. See [Risk Management & Communication](octoacme-risks-and-communication.md) for templates and escalation details.

## Quality Assurance Practices

Code quality is enforced through a structured PR workflow: pull requests should be small (≤ 400 lines where possible), include an issue link and acceptance criteria in the description, and pass automated tests and linting in CI before a reviewer is assigned. At least one approval is required before merging. The testing strategy layers unit tests for new logic, integration tests where applicable, and end-to-end smoke tests for critical flows before each release. Security scanning runs in CI on every PR. Pre-release gates require all acceptance criteria to be met, CI and security scans to pass, release notes to be drafted, and a rollback plan to be documented. A full deployment checklist and release notes template are available in the [Release & Deployment Guide](octoacme-release-and-deployment.md); day-to-day QA workflow details are in [Execution & Tracking](octoacme-execution-and-tracking.md).

---

## Process Documents

| Document | Description |
|---|---|
| [Project Management Overview](octoacme-project-management-overview.md) | Principles, core roles, key artifacts, and lifecycle summary |
| [Project Initiation Guide](octoacme-project-initiation.md) | One-pager template, initiation checklist, and decision gate |
| [Project Planning](octoacme-project-planning.md) | Backlog creation, estimation, sprint planning, and planning checklist |
| [Execution & Tracking](octoacme-execution-and-tracking.md) | Team rhythm, PR workflow, quality & testing standards, escalation |
| [Risk Management & Communication](octoacme-risks-and-communication.md) | Risk register, communication templates, escalation paths |
| [Release & Deployment Guide](octoacme-release-and-deployment.md) | Pre-release checklist, deployment steps, rollback playbook, release notes template |
| [Retrospective & Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md) | Retro structure, action item tracking, continuous improvement culture |
| [Roles & Personas](octoacme-roles-and-personas.md) | Detailed persona definitions for PM, PdM, Developers, and QA |

For process improvements or suggestions, please open an issue using the **"Add Content to Project Management Process Docs"** template.
