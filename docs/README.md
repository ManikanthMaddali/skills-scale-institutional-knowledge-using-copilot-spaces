# OctoAcme Project Management Docs

This repository contains standardized, living documentation of OctoAcme project management processes.

## Overview: OctoAcme Project Management Processes

### Core Principles & Lifecycle
OctoAcme operates with a structured, iterative project management approach centered on five core principles: **customer-first prioritization**, **incremental delivery**, **clear ownership**, **data-informed decisions**, and **psychological safety**. The organization applies a consistent lifecycle across all cross-functional projects, progressing through five distinct phases:

1. **Initiation** — Problem validation and stakeholder alignment
2. **Planning** — Scope definition and backlog creation
3. **Execution** — Build-test-review cycles with daily standups
4. **Release** — Deployment, verification, and announcement
5. **Retrospective & Continuous Improvement** — Learning capture and process refinement

This standardized framework ensures predictable delivery while maintaining flexibility for iteration.

### Defined Roles & Responsibilities
OctoAcme maintains clear role definition with dedicated ownership:

- **Project Managers (PM)** — Coordinate delivery, manage schedules, risks, and communications to enable on-time, on-scope delivery
- **Product Managers (PdM)** — Define outcomes, prioritize backlogs, and measure success through data-informed decisions
- **Developers** — Implement features with quality standards, participate in design reviews, and help identify technical risks
- **QA/Testing** — Validate quality and acceptance criteria through unit, integration, and end-to-end tests
- **Stakeholders** — Provide inputs, approvals, and business context

### Workflows & Communication Cadence

**Execution Rhythm:**
- Daily standups (15 min) — Focus on progress, blockers, and dependencies
- Weekly delivery syncs — Show progress and flagged risks
- Sprint-based demos and reviews — Demonstrate incremental value
- Monthly stakeholder updates — Keep leadership informed

**Backlog & PR Discipline:**
- GitHub Projects board with standardized columns: Backlog, Ready, In Progress, In Review, QA, Done
- Pull requests follow a discipline of small increments (≤400 lines when possible)
- All PRs include issue links and acceptance criteria
- Automated tests and linting run in CI before review
- Require at least one approval before merge

**Risk & Dependency Management:**
- Capture risks in a Risk Register (ID, description, impact, probability, owner, mitigation)
- Mark cross-team dependencies in the project board
- Escalate through three-tier path: team-level triage → PM to Product Lead → sponsor-level for business-impacting issues

### Quality Assurance Practices

OctoAcme maintains rigorous quality standards:
- **Unit tests** for new logic
- **Integration tests** where applicable
- **End-to-end smoke tests** before release
- **Automated security scanning** in CI
- **Manual QA** for feature acceptance when needed

All code runs automated tests and linting checks before review, establishing a quality gate. Releases require pre-release verification: acceptance criteria met, CI/security scans passing, release notes drafted, and rollback plans documented.

### Continuous Learning & Improvement

Retrospectives are held after each sprint, release, or milestone to capture learnings and drive iterative improvement:
- Timebox: 45–75 minutes
- Focus: What went well, what could improve, actionable next steps
- Prioritize: 2–3 top action items to avoid overload
- Track: Action items as issues in the backlog with clear owners and due dates
- Review: Outstanding actions in weekly PM syncs

This emphasis on retrospectives and blameless incident reviews reinforces a culture of learning and psychological safety.

---

## Process Docs Index

Each of these documents provides detailed guidance for specific phases and aspects of project delivery:

- **[Project Management Overview](./octoacme-project-management-overview.md)** — Concise introduction to OctoAcme's approach, roles, and key artifacts
- **[Project Initiation Guide](./octoacme-project-initiation.md)** — Steps to validate business need, align stakeholders, and authorize work
- **[Project Planning](./octoacme-project-planning.md)** — Breaking work into shippable increments with clear dependencies and timelines
- **[Execution & Tracking](./octoacme-execution-and-tracking.md)** — Day-to-day execution, team rhythm, quality, and progress tracking
- **[Risk Management & Communication](./octoacme-risks-and-communication.md)** — Identifying, assessing, and communicating risks and dependencies
- **[Release & Deployment Guide](./octoacme-release-and-deployment.md)** — Standardizing releases to reduce risk and improve observability
- **[Retrospective & Continuous Improvement](./octoacme-retrospective-and-continuous-improvement.md)** — Capturing learnings and converting them to actionable improvements
- **[Roles & Personas](./octoacme-roles-and-personas.md)** — Detailed role definitions and responsibilities for project participants

---

## Getting Started

**New team members:** Start with the [Project Management Overview](./octoacme-project-management-overview.md) to understand our approach, then dive into docs relevant to your role.

**Existing teams:** Use these docs as a reference during project phases. Keep the Project Charter updated in your project repo and link to the relevant docs as needed.

**Process improvements:** Found a gap or want to refine a process? Open an issue using the "[Add Content to Project Management Process Docs](../.github/ISSUE_TEMPLATE/add-update-content-to-process-docs.yml)" template.
