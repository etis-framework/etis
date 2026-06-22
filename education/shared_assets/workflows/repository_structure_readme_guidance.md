# Repository Structure and README Guidance

**Classification:** ETIS Educational Ecosystem Asset  
**Category:** Workflow  
**Origin:** Loyola University Chicago COMP 330 — Software Engineering  
**Authoritative Format:** Markdown

---

Repository-Centered Engineering for Trustworthy Intelligent Systems

| Core idea<br>The GitHub repository is the project’s engineering control center. The README is the front door. The folder structure, issues, pull requests, reviews, tests, AI-use evidence, observability artifacts, release notes, and governance records should allow another engineer to understand what the team is building, why it matters, how work is controlled, what risks remain, and where proof lives. |
| --- |


## 1. Purpose of This Guidance

This document explains the expected repository structure and README content for COMP 330 team projects. It does not replace the GitHub repository setup guidance. That separate setup document explains how to create the repository, name it, make it public, clone it, invite teammates, and connect tools. This document explains what should live inside the repository after setup and how students should make the repository professionally reviewable.

The goal is not paperwork. The goal is to build an evidence trail that makes the team’s engineering work visible, inspectable, and defensible throughout Cycle 1 and Cycle 2. The repository should become the team’s engineering memory, governance record, operational evidence source, and release witness.

| Professional framing<br>A professional repository is not a code dump. It is the visible control system for trustworthy engineering: intent, work, review, evidence, release judgment, and operational learning. |
| --- |


## 2. Repository-Centered Engineering Doctrine

Repository-Centered Engineering is the practice of treating the repository as the authoritative system of record for engineering work. In this course, the repository should show not only source code, but also requirements, design decisions, review evidence, tests, defects, risks, AI-use verification, release readiness, observability, and governance controls.

| Principle | Meaning |
| --- | --- |
| Everything important leaves evidence | Important engineering claims should point to inspectable repository evidence. |
| The README is the front door | A reviewer should know where to begin and where proof lives. |
| No traceability, no merge | Meaningful changes should connect intent, work, review, tests, and evidence. |
| AI proposes; engineers verify | AI-generated or AI-assisted artifacts must be disclosed, reviewed, and verified. |
| A demo is not operational proof | Working once is not the same as being reviewable, testable, governable, observable, or supportable. |
| Honest evidence beats polished claims | Known limitations, failed checks, deferred work, and residual risks should be visible. |


## 3. Repository Ownership Principle

| Important rule<br>Any team member may update repository artifacts. However, each major artifact area must have a primary owner and a backup. The owner is responsible for making sure the artifact is current, accurate, reviewable, and ready at the appropriate point in the course cycle. |
| --- |

Every student is a developer and engineering contributor first. Operational roles create accountability visibility, not isolated ownership silos. Operational roles exist to make ownership visible, not to prevent others from contributing. The repository should show evidence of team participation through issues, commits, pull requests, reviews, documents, tests, and release artifacts.

A team should never rely on one person silently holding project knowledge outside the repository. If the team cannot explain the project without private chat messages or one person’s memory, the repository is not yet doing its job.


## 4. Repository Maturity Progression

The repository should mature as the system matures. Teams do not need every folder or artifact on day one. They should add evidence when the corresponding engineering work becomes real.

| Maturity Stage | What It Contains | Review Question |
| --- | --- | --- |
| Stage 1: Functional Repository | Contains code, README, early requirements, and basic project files. | Can the team build something and explain the basic project purpose? |
| Stage 2: Structured Engineering Repository | Adds planning, traceability, architecture, ADRs, reviews, tests, CI/CD, and issue-linked work. | Can another engineer inspect intent, design, work, review, and verification? |
| Stage 3: Operational Repository | Adds release evidence, known limitations, defect review, observability, runtime evidence, and supportability documentation. | Can the team diagnose, explain, observe, recover from, and defend operational behavior? |
| Stage 4: Trustworthy Engineering Repository | Adds governance artifacts, AI oversight evidence, operational readiness, postmortems, release maturity, and residual risk ownership. | Can the system be responsibly governed, operated, recovered, and evolved? |


## 5. Complete Repository Structure

The structure below is the recommended complete structure by the end of the course. It preserves the course repository model while making the operational-trust, AI-governance, observability, review, and release-evidence expectations more explicit. Teams should not create empty folders just to look complete. Create folders and files when the evidence is real. Repository structure should support engineering work, not create the appearance of maturity without operational evidence.

The repository structure evolves throughout the semester and should be expanded incrementally as new engineering workflows, artifacts, and operational needs are introduced during the development cycles. Teams should add structure intentionally when it becomes relevant to the project lifecycle rather than creating empty placeholder artifacts upfront.

comp330-f26-teamX-projectname/

README.md

.gitignore

LICENSE or NOTICE.md, if applicable

.github/

pull_request_template.md

ISSUE_TEMPLATE/

feature_request.md

defect_report.md

task.md

workflows/

ci.yml

docs/

team/
 team-charter.md

roles.md

working-agreements.md

requirements/

README.md

requirements.md

acceptance-criteria.md

assumptions-open-questions.md

planning/

README.md

scope.md

traceability.md

task-plan.md

estimates.md

risk-register.md

schedule.md

re-estimation.md

architecture/

README.md

architecture.md

architecture-diagram.png

component-responsibilities.md

api-contracts.md

data-context.md

governance-and-approvals.md

workflows.md

decisions/
 adr/

adr-0001-decision-title.md

reviews/

architecture-review.md

code-review-example.md

ai-code-review-example.md

security-review.md

assignment4-review-package.md

release-readiness-review.md

operational-readiness-review.md

governance-review.md

ai-oversight-review.md

testing/

README.md

test-strategy.md

test-plan.md

test-cases.md

ci-evidence.md

final-test-evidence.md

quality/

defect-log.md

defect-review.md

ai/

ai-policy.md

ai-use-log.md

ai-verification-notes.md

release/

assignment5-release-package.md

release-notes.md

known-limitations.md

changed-files-since-a4.md

traceability-summary.md

presentation-index.md

demo-script.md

assignment6-final-release-package.md

final-release-notes.md

changed-files-since-a5.md

observability/

observability-plan.md

runtime-evidence.md

sample-logs.md

metrics-notes.md

security/

security-governance-checklist.md

data-handling-notes.md

permission-boundaries.md

operations/

runbook.md

incident-response-notes.md

postmortem-template.md

postmortem-YYYY-MM-DD.md

src/

application source code

tests/

automated tests

test-evidence/

manual test evidence, screenshots, logs, or evaluation outputs when useful

scripts/

build, setup, seed-data, or utility scripts when useful

data/

synthetic sample data only, if needed


## 6. What the Structure Is Designed to Prove

| Area | Primary Purpose | Reviewer Question |
| --- | --- | --- |
| /docs/requirements | Intent and acceptance criteria | What is the system supposed to do, and how will the team know it is acceptable? |
| /docs/planning | Scope, work, estimates, risks, schedule, and traceability | Can the team plan realistically under uncertainty? |
| /docs/architecture | Boundaries, workflows, components, APIs, data/context, governance, approvals | Can another engineer understand how the system is structured and controlled? |
| /docs/decisions | ADRs and important engineering decisions | Can the team explain tradeoffs and consequences over time? |
| /docs/reviews | Architecture, code, AI, security, governance, operational, and release reviews | Can engineering claims survive disciplined review? |
| /docs/testing and /tests | Test strategy, test cases, CI evidence, automated tests | Can behavior be verified repeatedly? |
| /docs/quality | Defect log and defect review | Does the team understand defects, severity, disposition, and trends? |
| /docs/ai | AI policy, AI-use log, AI verification notes | Can the team show what AI helped produce and how humans verified it? |
| /docs/release | Release notes, known limitations, demo script, final evidence index | Can the team defend release readiness honestly? |
| /docs/observability | Runtime evidence, logs, metrics, operational signals | Can the team understand runtime behavior and failure? |
| /docs/security | Permission boundaries, data handling, governance checklist | Can the team show how unsafe actions and data exposure are controlled? |
| /docs/operations | Runbooks, incident response, postmortems | Can the team operate, recover, and learn from failure? |
| /.github | PR templates, issue templates, workflows | Can the repository enforce repeatable workflow discipline? |
| /test-evidence | Manual evidence, screenshots, logs, evaluation outputs | Can claims be supported when automated tests are not enough? |


## 7. Structure by Assignment and Role Ownership

The table below shows when each major repository area becomes important, what it proves, and which team role normally owns readiness. Roles may be combined on smaller teams. Each area should also have a backup owner.

| Course Point | Repository Areas Introduced or Emphasized | What This Evidence Proves | Typical Owner(s) |
| --- | --- | --- | --- |
| A1: Project Launch | README.md, /docs/team-charter.md, /docs/roles.md, /docs/working-agreements.md, /docs/ai/ai-policy.md, initial /docs/requirements/ | Team is formed, repository exists, roles are visible, AI policy is established, and the team is ready to operate. | Team Lead; Operations & Evidence Lead |
| A2: Planning and Estimation | /docs/planning/, updated /docs/requirements/, /docs/ai/ai-use-log.md | Cycle 1 scope, tasks, estimates, risks, schedule, commitments, and traceability are visible. | Planning & Process Lead |
| A3: Architecture and Review | /docs/architecture/, /docs/decisions/, /docs/reviews/architecture-review.md, /docs/testing/test-strategy.md | The team can explain components, interfaces, data ownership, AI/tool boundaries, governance points, risks, and review questions before construction accelerates. | Architecture & Development Lead; Quality & Review Lead |
| A4: Construction and Review | /src, /tests, /.github/, /docs/reviews/, /docs/testing/, /docs/ai/ai-use-log.md | Implementation is controlled through issues, branches, pull requests, reviews, CI/CD checks, tests, and AI-use evidence. | Architecture & Development Lead; Quality & Review Lead |
| A5: Cycle 1 Release | /docs/release/, /docs/testing/, /docs/quality/, /docs/planning/traceability.md, /docs/ai/ai-use-log.md | The team can present a working Cycle 1 release with release notes, known limitations, test evidence, defect status, and peer accountability. | Operations & Evidence Lead; Quality & Review Lead |
| A6: Final Release and Maturity | /docs/release/, /docs/observability/, /docs/security/, /docs/operations/, /docs/planning/, /docs/ai/ | Cycle 2 improvements, observability, security/governance, operational readiness, final risks, AI-use reflection, and final release judgment are visible. | Operations & Evidence Lead; Team Lead |


## 8. README.md: The Repository Front Door

The README.md file sits at the root of the repository and should be the first file a reviewer reads. It should not be a random placeholder. It should tell the instructor, teammates, and outside reviewers what the project is, what works, how to run or inspect it, where the engineering evidence lives, and how the team controls trustworthy change.

| README principle<br>The README is the operational front door to engineering trust. It should orient a reviewer to product purpose, current maturity, run/test instructions, evidence locations, AI-use disclosure, risks, and workflow discipline.<br><br>A reviewer should not need to search the repository blindly to determine project maturity, operational status, or evidence location. | README principle<br>The README is the operational front door to engineering trust. It should orient a reviewer to product purpose, current maturity, run/test instructions, evidence locations, AI-use disclosure, risks, and workflow discipline.<br><br>A reviewer should not need to search the repository blindly to determine project maturity, operational status, or evidence location. | README principle<br>The README is the operational front door to engineering trust. It should orient a reviewer to product purpose, current maturity, run/test instructions, evidence locations, AI-use disclosure, risks, and workflow discipline.<br><br>A reviewer should not need to search the repository blindly to determine project maturity, operational status, or evidence location. |
| --- | --- | --- |
| README Section | README Section | What It Should Contain |
| Project title and team identity | Project title and team identity | Project name, team number, team members, course, semester, repository URL. |
| Project purpose | Project purpose | Short explanation of the problem, intended users, and what workflow or need the system supports. |
| Current release status | Current release status | What currently works, what is incomplete, what cycle/release the team is in, and known limitations. |
| How to run or inspect the project | How to run or inspect the project | Setup, dependencies, run commands, test commands, and known setup limitations. |
| Demo path | Demo path | The main user path the team can demonstrate and the evidence that supports it. |
| Evidence index | Evidence index | Direct links to requirements, planning, architecture, reviews, tests, AI-use log, release notes, known limitations, observability, security/governance, and operations artifacts. |
| Team roles and responsibilities | Team roles and responsibilities | Primary role owners and backups, with a reminder that all students contribute to implementation, review, testing, and evidence. |
| AI-use statement | AI-use statement | Short summary of how AI is used and where the detailed AI-use log lives. |
| Known limitations and risks | Known limitations and risks | Current limits, deferred work, residual risks, mitigations, and links to release notes or risk register. |
| Repository workflow | Repository workflow | Brief note that work should flow through issues, branches, pull requests, reviews, checks, and evidence updates. |

Sample README Skeleton

# Project Name

Team Number: Team X

Repository: https://github.com/<owner>/comp330-f26-teamX-projectname

## Project Purpose

Briefly describe the problem, users, and workflow the system supports.

## Current Status

- Current cycle: Cycle 1 / Cycle 2

- Current release: v0.1 / v1.0 / other

- What works now:

- What is intentionally out of scope:

- Known limitations:

- Residual risks:

## How to Run or Inspect


## 1. Clone the repository.


## 2. Install dependencies.


## 3. Run the application.


## 4. Run tests.

## Demo Path

Describe the primary workflow the team will demonstrate.

## Engineering Evidence Index

- Requirements: /docs/requirements/

- Planning: /docs/planning/

- Architecture: /docs/architecture/

- Decisions: /docs/decisions/

- Reviews: /docs/reviews/

- Testing: /docs/testing/ and /tests

- Quality / defects: /docs/quality/

- AI use: /docs/ai/ai-use-log.md

- Release evidence: /docs/release/

- Observability: /docs/observability/

- Security / Governance: /docs/security/

- Operations / Runbook: /docs/operations/

## Team Roles

List primary owners and backup owners for major role areas.

## Repository Workflow

Issues -> Branches -> Pull Requests -> Review -> Checks -> Merge -> Evidence Updated

## AI Use

Summarize allowed AI use and link to /docs/ai/ai-use-log.md.

## Known Limitations and Risks

Summarize current limits and link to release notes and risk register.


## 9. Non-Folder GitHub Areas Students Must Use

Important project evidence also lives in GitHub features outside the folder tree. The repository is more than files.

| GitHub Area | How It Should Be Used | Typical Owner |
| --- | --- | --- |
| Issues tab | Tracks tasks, defects, enhancements, questions, and follow-up work. Issues are the operational work queue, not a replacement for requirements or planning documents. | Planning & Process Lead |
| Pull Requests tab | Shows proposed changes, review comments, status checks, AI disclosure notes, and merge decisions. Pull requests are the main review gate. | Quality & Review Lead |
| Actions tab | Shows CI/CD workflow runs, build results, test results, and failed checks. This supports release and quality evidence. | Quality & Review Lead |
| Projects board, optional | Can help teams manage issue status visually. Optional, but useful for teams that want a board view. | Planning & Process Lead |
| Wiki, usually avoid | Avoid using the Wiki as the primary evidence store unless approved. Course evidence should normally live in versioned repository files under /docs. | Operations & Evidence Lead |
| Releases, optional | Can be used for formal tagged releases and version markers associated with major demonstrations, presentations, and operational review points. | Operations & Evidence Lead |


## 10. Professional Workflow Rule: From Issue to Merge

| Simple rule<br>No issue -> no branch -> no pull request -> no review -> no merge. |
| --- |

Professional GitHub workflow is not bureaucracy. It is the control system that makes team work visible, reviewable, traceable, and safe to merge into the shared codebase.

| Step | Meaning |
| --- | --- |
| Issue | Every meaningful change should begin with a GitHub Issue or documented task that explains why the work exists. |
| Branch | Work should happen on a branch tied to the issue or purpose, not directly on main. |
| Pull Request | A pull request should make the proposed change visible to the team before it is merged. |
| Review | Another team member should review scope, correctness, tests, architecture fit, risk, and AI disclosure when applicable. |
| Checks | Builds, tests, or other CI/CD checks should run when appropriate and be visible. |
| Merge | After approval and successful checks, the change may be merged into main and the related evidence should be updated. Pull requests should clearly explain why the change exists, what engineering evidence supports it, what risks were considered, and what related artifacts were updated. |

This rule does not mean every spelling correction needs a heavyweight process. It does mean that every meaningful code, requirement, design, test, release, AI-use, observability, security/governance, or phase-gate artifact change should be traceable and reviewable.


## 11. Review Boards and Engineering Gates

The repository should support recurring engineering gates. These reviews are not ceremony. They are professional safety mechanisms that test whether engineering claims can survive disciplined review and evidence evaluation.

| Review Gate | Evidence Location | What It Evaluates |
| --- | --- | --- |
| Architecture Review | /docs/reviews/architecture-review.md | Boundaries, responsibilities, interfaces, dependencies, data/context ownership, AI/tool boundaries, governance points. |
| Code / PR Review | GitHub PRs; /docs/reviews/code-review-example.md | Correctness, maintainability, tests, architecture fit, security, dependencies, and evidence. |
| AI Oversight Review | /docs/reviews/ai-oversight-review.md; /docs/ai/ | What AI produced, what humans accepted/rejected/modified, and how the result was verified. |
| Security / Governance Review | /docs/reviews/security-review.md; /docs/security/ | Permissions, approvals, sensitive data, audit expectations, and residual risk ownership. |
| Release Readiness Review | /docs/reviews/release-readiness-review.md; /docs/release/ | What shipped, what was tested, what risks remain, what mitigations exist, and why release is defensible. |
| Operational Readiness Review | /docs/reviews/operational-readiness-review.md; /docs/observability/; /docs/operations/ | Runtime evidence, logs, runbook, failure diagnosis, incident response, and supportability. |


## 12. AI-Use Evidence and Verification Expectations

AI assistance is allowed. Undisclosed or unverified AI work is not professional. If AI produces or substantially transforms code, tests, documentation, architecture ideas, diagrams, release notes, review comments, or planning artifacts, the team must disclose the use and verify the result.

| AI-use log field | Question it answers |
| --- | --- |
| Tool / date | What tool or model was used and when? |
| Task | What was the AI asked to do? |
| Accepted output | What was accepted into the project after human review? |
| Rejected output | What was rejected and why? |
| Human edits | What did the team change before accepting the output? |
| Verification | What tests, reviews, comparisons, or evidence support the accepted artifact? |
| Risk / limitation | What AI-related uncertainty remains? |
| AI rule<br>Generated output is proposed engineering material, not verified engineering truth. The team owns the result even if AI helped produce it. | AI rule<br>Generated output is proposed engineering material, not verified engineering truth. The team owns the result even if AI helped produce it. |


## 13. Evidence Quality Standards

| Standard | Meaning |
| --- | --- |
| Specific | Avoid vague claims such as “tests passed” without naming what was tested or where the evidence lives. |
| Current | Old documents that do not reflect the current system create confusion and weaken trust. |
| Linked | Requirements should connect to tasks, pull requests, tests, defects, release notes, or known limitations. |
| Reviewable | Another engineering team should be able to inspect, understand, review, and operationally support the project without interviewing the original team. |
| Honest | Known limitations, failed checks, unresolved defects, deferred work, and residual risks should be visible. |
| Actionable | Evidence should help the team decide what to fix, defer, mitigate, release, or monitor. |


## 14. What Not to Put in the Repository

Do not store real student records, grades, private university data, credentials, secrets, API keys, passwords, tokens, or personal data.

Do not store private peer reviews in the public team repository. Peer reviews are submitted privately in Sakai.

Do not commit large generated folders, temporary files, dependency folders, build output, or local environment files unless there is a documented reason.

Do not use the repository as a dumping ground for unrelated screenshots, old drafts, or files that cannot be traced to project evidence.

Do not hide major project decisions in chat messages. Decisions that affect the system should be captured in /docs/decisions/ or the appropriate evidence file.

Do not merge AI-generated or AI-assisted work that the team cannot explain, test, review, and maintain.


## 15. Recommended .gitignore and Housekeeping

Teams should create a .gitignore file appropriate to their technology stack. The exact contents depend on the language and framework, but the principle is simple: commit source and evidence; do not commit local clutter, secrets, or generated build artifacts.

Use a .gitignore template appropriate to the selected language or framework.

Keep README.md current after major changes.

Keep /docs/release/ and /docs/testing/ current near presentations and phase gates.

Keep /docs/observability/, /docs/security/, and /docs/operations/ current during Cycle 2 maturity work.

Use synthetic sample data only.

If AI produces or substantially modifies a file, disclose that work in the AI-use log and review it before merge.


## 16. Repository Review Checklist

README explains the project, current status, run/test instructions, and evidence locations.

Repository has a clear /docs structure aligned with current assignment expectations.

Issues show current and completed work.

Pull requests show meaningful review and merge decisions.

Tests or validation evidence support important claims.

AI-use log is current and honest.

Known limitations and risks are visible.

Defects are recorded, triaged, and linked to disposition or regression evidence when appropriate.

Observability evidence shows runtime behavior, logs, metrics, or operating assumptions when relevant.

Security/governance evidence shows permissions, data rules, approvals, and residual risk ownership when relevant.

No secrets, private data, peer reviews, or unsafe files are stored in the repository.

Role owners and backup owners are documented.

The repository could be reviewed by another team without a private explanation.

Appendix A - Folder Purpose Quick Reference

| Folder or Area | Purpose |
| --- | --- |
| /docs | Engineering evidence and project memory. |
| /docs/requirements | Requirements, user stories, acceptance criteria, assumptions, and open questions. |
| /docs/planning | Scope, tasks, estimates, risks, schedule, commitments, re-estimation, and traceability. |
| /docs/architecture | Architecture overview, diagrams, components, interfaces, data/context rules, governance, and workflows. |
| /docs/decisions | Architecture Decision Records and other important engineering decisions. |
| /docs/reviews | Architecture review, code review, AI-code review, security review, governance review, operational readiness review, and phase-gate evidence. |
| /docs/testing | Test strategy, test plan, test cases, CI evidence, and final validation summaries. |
| /docs/quality | Defect logs and defect review summaries. |
| /docs/ai | AI policy, AI-use log, and AI verification notes. |
| /docs/release | Release notes, known limitations, demo script, presentation index, traceability summary, and final release evidence. |
| /docs/observability | Logs, metrics, runtime behavior evidence, cost awareness, and operational assumptions. |
| /docs/security | Security and governance checklist, approval rules, data rules, permission boundaries, and residual risk ownership. |
| /docs/operations | Runbooks, incident response notes, postmortems, and recovery guidance. |
| /src | Source code. |
| /tests | Automated tests. |
| /test-evidence | Manual test results, screenshots, logs, or evaluation evidence when useful. |
| /scripts | Setup, build, seed data, or utility scripts. |
| /data | Synthetic sample data only, if needed. |
| /.github | Pull request templates, issue templates, and GitHub Actions workflows. |

Appendix B - Markdown Basics for README and Evidence Files

Most repository evidence should be written in Markdown files using the .md extension. Markdown is simple, readable in GitHub, and easy to review in pull requests.

# Heading 1

## Heading 2

### Heading 3

- Bullet item

- Another bullet item


## 1. Numbered item


## 2. Numbered item

**Bold text**

*Italic text*

[Link text](https://example.com)

| Column A | Column B |

|---|---|

| Value 1 | Value 2 |

```text

Use fenced code blocks for commands or examples.

```


## Final Takeaway

| Bottom line<br>A professional repository is not merely a place where code is stored. It is a visible engineering control system. It should show what the team planned, what changed, who reviewed it, what evidence supports it, how AI was used, what risks remain, how the system can be observed and operated, and why the system is ready for the next phase gate. |
| --- |
