# Engineering Repository Structure Guide

**Classification:** ETIS Educational Ecosystem Asset  
**Category:** Workflow  
**Origin:** Loyola University Chicago COMP 330 — Software Engineering  
**Authoritative Format:** Markdown  
**Typical Repository Location:** Repository root and `/docs/`

## Purpose

This guide explains the standard engineering repository structure used in an ETIS-aligned student software engineering project.

Many students have used GitHub only as a place to store code. In this model, GitHub is treated as an engineering evidence system.

The repository contains not only code, but also requirements, planning, architecture, reviews, testing evidence, AI-use documentation, release records, and operational maturity artifacts.

---

## Core Idea

The GitHub repository is the project's engineering control center.

The README is the front door.

The repository should make intent, work, review, evidence, release judgment, and operational learning visible to another engineer.

---

## Repository-Centered Engineering Doctrine

| Principle | Meaning |
|---|---|
| Everything important leaves evidence | Important engineering claims should point to inspectable repository evidence. |
| The README is the front door | A reviewer should know where to begin and where proof lives. |
| No traceability, no merge | Meaningful changes should connect intent, work, review, tests, and evidence. |
| Merges require engineering judgment | Pull requests should explain why changes were considered safe enough to merge into the operational system. |
| AI proposes; engineers verify | AI-generated or AI-assisted artifacts must be disclosed, reviewed, and verified. |
| A demo is not operational proof | Working once is not the same as being reviewable, testable, governable, observable, or supportable. |
| Honest evidence beats polished claims | Known limitations, failed checks, deferred work, and residual risks should be visible. |

---

## Starter Kit Structure

The starter kit provides the Day-1 repository scaffold.

Students should not treat it as busywork.

Each folder has a purpose, and each Markdown file is a starting point for engineering evidence.

Repository structure should support real engineering work and reviewability, not create the appearance of maturity without supporting evidence.

```text
comp330-f26-teamX-projectname/
  README.md
  .gitignore

  .github/
    ISSUE_TEMPLATE/
    pull_request_template.md
    workflows/
      ci.yml

  docs/
    team/
    requirements/
    planning/
    architecture/
    reviews/
    testing/
    quality/
    ai/
    release/
    observability/
    security/
    operations/

  src/
  tests/
  test-evidence/
  scripts/
  data/
```

---

## Folder Purpose Quick Reference

| Folder or Area | Purpose |
|---|---|
| `/docs/team` | Team charter, roles, working agreements, ownership, and coordination rules. |
| `/docs/requirements` | Requirements, acceptance criteria, assumptions, and open questions. |
| `/docs/planning` | Scope, task plan, estimates, schedule, risk register, and traceability. |
| `/docs/architecture` | Architecture overview, interfaces, component responsibilities, diagrams, boundaries, ADRs, and major engineering decisions. |
| `/docs/reviews` | Architecture, code, AI-code, release readiness, and operational review evidence. |
| `/docs/testing` | Test strategy, test plan, test cases, CI evidence, and validation summaries. |
| `/docs/quality` | Defect logs and defect review summaries. |
| `/docs/ai` | AI policy, AI-use log, and AI verification notes. |
| `/docs/release` | Release notes, known limitations, demo script, and release traceability. |
| `/docs/observability` | Runtime evidence, logs, metrics, and operational assumptions. |
| `/docs/security` | Security/governance checklist, data handling, and permission boundaries. |
| `/docs/operations` | Runbooks, incident response notes, postmortems, and recovery guidance. |
| `/src` | Source code. |
| `/tests` | Automated tests. |
| `/test-evidence` | Manual testing evidence, screenshots, logs, or evaluation outputs. |
| `/.github` | Issue templates, pull request template, and GitHub Actions workflows. |

---

## Assignment Progression

| Assignment | Repository Areas Emphasized | What This Proves |
|---|---|---|
| A1: Repository Launch | `README.md`, `/docs/team`, `/docs/requirements`, `/docs/ai`, `/.github` | Team is formed, roles are visible, AI policy exists, and the repository is ready to operate. |
| A2: Planning and Estimation | `/docs/planning`, `/docs/requirements`, Issues, Milestones | Scope, tasks, estimates, risks, schedule, commitments, and traceability are visible. |
| A3: Architecture and Review | `/docs/architecture`, `/docs/reviews`, `/docs/security` | Components, boundaries, interfaces, AI/tool boundaries, governance points, and risks are reviewable. |
| A4: Construction and Integration | `/src`, `/tests`, `/.github/workflows`, `/docs/testing`, `/docs/ai` | Implementation is controlled through issues, branches, PRs, reviews, CI/CD, tests, and AI-use evidence. |
| A5: Cycle 1 Release | `/docs/release`, `/docs/testing`, `/test-evidence`, `/docs/quality` | Cycle 1 release claims are supported by test evidence, defects, known limitations, release notes, and release/version evidence. |
| A6: Final Release and Maturity | `/docs/operations`, `/docs/observability`, `/docs/security`, `/docs/release` | Operational readiness, governance, observability, recovery expectations, and release maturity are visible. |

---

## README Expectations

The root README should include:

- Project title, team identity, course, semester, and repository URL.
- Project purpose, intended users, and supported workflow.
- Current release status: what works, what is incomplete, and known limitations.
- How to run or inspect the system, including setup and test commands.
- Evidence index linking directly to requirements, planning, architecture, testing, AI-use, release, security, observability, and operations artifacts.
- Operational expectations, observability assumptions, or recovery guidance when appropriate to the system maturity level.
- Repository workflow expectations: issues → branches → pull requests → review → validation checks → merge → evidence updated.

Repository evidence should remain reviewable without requiring verbal clarification from the original team.

---

## What Not to Put in the Repository

Do not store:

- Real student records, grades, private university data, credentials, secrets, API keys, passwords, or tokens.
- Private peer reviews.
- Large generated folders, dependency folders, build output, temporary files, or local environment files unless explicitly justified.
- Unrelated screenshots, old drafts, or files that cannot be traced to project evidence.
- AI-generated or AI-assisted work that the team cannot explain, test, review, and maintain.

---

## Repository Review Checklist

- [ ] README explains project purpose, current status, run/test instructions, and evidence locations.
- [ ] Repository structure aligns with current assignment expectations.
- [ ] Issues and pull requests show current and completed work.
- [ ] Tests or validation evidence support important claims.
- [ ] AI-use log is current and honest.
- [ ] Known limitations, defects, and risks are visible.
- [ ] No secrets, private data, peer reviews, or unsafe files are stored in the repository.
- [ ] Another engineering team could inspect, review, and operationally understand the repository without relying on private explanations.

---

## Final Takeaway

A professional repository is not merely a code dump.

It is the visible engineering control system for planning, review, testing, governance, release readiness, and operational learning.
