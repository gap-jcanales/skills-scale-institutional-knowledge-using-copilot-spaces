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

---

```yaml
# OctoAcme Project Management Docs — LLM/MCP Metadata
purpose: >
  Central entry point and index for OctoAcme project management process documentation.
  Provides a concise overview of delivery methodology and links to all process guides
  for use by team members, onboarding engineers, and LLM/Copilot Spaces retrieval.
scope: >
  All cross-functional projects delivering product features, services, or integrations
  within OctoAcme.
workflows:
  - name: Initiation
    description: Validate business need, align stakeholders, define success criteria.
    artifact: Project Charter / One-pager
    doc: octoacme-project-initiation.md
  - name: Planning
    description: Break work into shippable increments, estimate scope, define milestones.
    artifact: Sprint/Iteration Backlog, Release Plan
    doc: octoacme-project-planning.md
  - name: Execution & Tracking
    description: Daily standups, weekly delivery syncs, project-board–driven workflow, PR and testing standards.
    artifact: Project Board, PR descriptions, Test reports
    doc: octoacme-execution-and-tracking.md
  - name: Release & Deployment
    description: Pre-release checks, automated pipeline, post-deploy verification, rollback playbook.
    artifact: Release Checklist, Release Notes, Rollback Plan
    doc: octoacme-release-and-deployment.md
  - name: Retrospective & Continuous Improvement
    description: Structured retrospectives converted into tracked action items.
    artifact: Retrospective Notes, Action Item Log
    doc: octoacme-retrospective-and-continuous-improvement.md
  - name: Risk Management (ongoing)
    description: Identify, assess, mitigate, and communicate risks across all phases.
    artifact: Risk Register
    doc: octoacme-risks-and-communication.md
roles:
  - name: Project Manager (PM)
    responsibilities: Delivery coordination, schedules, risk register, stakeholder communications.
  - name: Product Manager (PdM / Product Lead)
    responsibilities: Problem statement, roadmap ownership, backlog prioritization, outcome measurement.
  - name: Developers
    responsibilities: Feature implementation, tests, design and code reviews, estimation.
  - name: QA/Testing
    responsibilities: Acceptance criteria validation, manual and automated quality checks.
  - name: Stakeholders
    responsibilities: Business context, approvals, feedback, escalation sponsors.
cadence_events:
  - event: Standup
    frequency: Twice-weekly (delivery team)
  - event: PM + PdM Sync
    frequency: Weekly
  - event: Stakeholder Update
    frequency: Monthly
  - event: Retrospective
    frequency: Per sprint/milestone
  - event: Ad-hoc escalation
    frequency: As needed
artifacts:
  - Project Charter / One-pager
  - Roadmap and Release Plan
  - Sprint/Iteration Backlog
  - Acceptance Criteria & Definition of Done
  - Risk Register
  - Weekly Status Report
  - Retrospective Notes and Action Items
  - Release Notes
  - Rollback Plan
quality_gates:
  pr_workflow:
    - Small PRs (≤ 400 lines where possible)
    - Link issue and acceptance criteria in PR description
    - Automated tests and linting must pass in CI
    - At least one approval required before merge
  testing:
    - Unit tests for new logic
    - Integration tests where applicable
    - End-to-end smoke tests before each release
  security:
    - Security scanning runs in CI on every PR
  pre_release:
    - All acceptance criteria met
    - CI and security scans pass
    - Release notes drafted
    - Rollback plan documented
escalation_path:
  standard: Team-level triage → PM → Product Lead → Sponsor
  security: Security incident runbook → Security on-call team
doc_index:
  - file: octoacme-project-management-overview.md
    description: Principles, core roles, key artifacts, and lifecycle summary
  - file: octoacme-project-initiation.md
    description: One-pager template, initiation checklist, and decision gate
  - file: octoacme-project-planning.md
    description: Backlog creation, estimation, sprint planning, and planning checklist
  - file: octoacme-execution-and-tracking.md
    description: Team rhythm, PR workflow, quality & testing standards, escalation
  - file: octoacme-risks-and-communication.md
    description: Risk register, communication templates, escalation paths
  - file: octoacme-release-and-deployment.md
    description: Pre-release checklist, deployment steps, rollback playbook, release notes template
  - file: octoacme-retrospective-and-continuous-improvement.md
    description: Retro structure, action item tracking, continuous improvement culture
  - file: octoacme-roles-and-personas.md
    description: Detailed persona definitions for PM, PdM, Developers, and QA
```
