# AI-Assisted Engineering Guidance

**Classification:** ETIS Educational Ecosystem Asset  
**Category:** AI Engineering  
**Origin:** Loyola University Chicago COMP 330 — Software Engineering  
**Implementation Provenance:** COMP330 Flagship Implementation  
**Authoritative Format:** Markdown  
**Purpose:** Student and team guidance for responsible AI-assisted engineering across the software development lifecycle

---

## Purpose

This guidance explains how students and engineering teams should use AI tools responsibly during ETIS-aligned software engineering work.

The original version of this asset was created for Loyola University Chicago COMP 330 — Software Engineering. It has been normalized as an ETIS AI Engineering shared asset while preserving COMP330 provenance.

The goal is not to restrict useful tools.

The goal is to make AI-assisted engineering visible, reviewable, verifiable, and accountable.

AI tools may help teams think, draft, code, review, test, document, and prepare releases. However, AI assistance must be disclosed, reviewed, verified, and owned by the team.

Students must be able to explain every submitted artifact, every accepted decision, and every line of submitted code.

---

## Core Policy

AI tools are encouraged throughout the software development lifecycle.

AI may assist with:

* Requirements
* Planning
* Architecture
* Implementation
* Testing
* Review
* Documentation
* Release preparation
* Reflection
* Operational analysis

However, AI-generated or AI-assisted output is proposed engineering material until humans review, validate, govern, and intentionally accept it.

The engineering team owns the outcome.

---

## Why This Guidance Exists

AI can accelerate engineering work.

It can also introduce hidden assumptions, hallucinated APIs, weak tests, insecure code, unexplained dependencies, poor architecture, and false confidence.

Professional teams use AI with discipline.

AI should improve engineering practice, not obscure responsibility.

Professional engineering evidence exists to support review, validation, governance, and operational understanding. It should not be used merely to create the appearance of maturity.

---

## Student Policy Summary

### AI use is encouraged.

Students may use AI across requirements, planning, architecture, implementation, testing, review, documentation, release preparation, and reflection.

### Disclosure is required.

Teams must record meaningful AI assistance in the AI-use log and in pull requests or artifact notes where appropriate.

### Human review is required.

AI-generated output is proposed engineering material until humans review, validate, govern, and intentionally accept it.

### The team owns the outcome.

The team is responsible for correctness, security, architecture fit, maintainability, testing, governance, and operational impact.

### Explanation is required.

Students must be able to explain the work they submit.

If the team cannot explain it, the team should not submit it.

### Evidence is required.

Repository evidence should remain organized and discoverable through the README, repository structure, pull requests, linked issues, and related engineering documentation.

---

## Allowed, Expected, and Not Acceptable

| Category | Meaning |
|---|---|
| Allowed and encouraged | Using AI to brainstorm requirements, find edge cases, critique plans, draft tests, explain errors, suggest refactoring, review code, draft documentation, or prepare release notes. |
| Expected professional behavior | Disclose meaningful AI use, review outputs carefully, verify with tests or inspection, reject weak suggestions, and record what the team accepted, modified, or rejected. |
| Not acceptable | Submitting AI-generated work the team cannot explain; hiding AI use; pasting full generated systems into main without review; using AI to bypass learning; exposing private data, credentials, real student records, or sensitive university information. |

---

## What Must Be Disclosed

Students do not need to log every spelling correction, grammar edit, or tiny autocomplete.

Teams should disclose meaningful AI assistance that affects engineering content, project decisions, code, tests, architecture, review, release evidence, or presentation claims.

Meaningful AI assistance includes:

* Generated or substantially revised code, tests, configuration, scripts, diagrams, documentation, or presentation content
* AI-assisted requirements, user stories, acceptance criteria, risks, estimates, scope decisions, or architecture decisions
* AI review of pull requests, security concerns, defects, test gaps, design tradeoffs, or release readiness
* AI-generated suggestions the team rejected when rejection materially affected scope, architecture, risk, or release decisions
* AI assistance used to interpret project evidence, summarize work, prepare release notes, or shape the final presentation

The test is simple:

```text
Did AI materially affect the engineering work, evidence, decision, or claim?
```

If yes, disclose it.

---

## Minimum AI-Use Log Entry

The AI-use log does not need to be long.

It needs to be honest, inspectable, and useful.

A typical location is:

```text
/docs/ai/ai-use-log.md
```

| Field | What to Record |
|---|---|
| Date | When the AI assistance occurred. |
| Tool | Tool used, such as GitHub Copilot, ChatGPT, Gemini Code Assist, Gemini CLI, Claude, Microsoft Copilot, or another approved tool. |
| Task | What the team asked AI to help with. |
| Artifact or location | Repository path, issue, pull request, test, or document affected. |
| Accepted / modified / rejected | What the team did with the output. |
| Verification | How the team checked it: review, test, comparison to requirements, security check, manual run, or team explanation. |
| Owner | Team member responsible for ensuring the entry is accurate. |

---

## AI Use Across the Software Development Lifecycle

| Lifecycle Area | Good AI Uses | Required Control |
|---|---|---|
| Requirements | Ask for missing stakeholders, edge cases, weak acceptance criteria, ambiguity, assumptions, and out-of-scope risks. | Do not let AI expand the project beyond approved scope. |
| Planning | Use AI to identify task breakdowns, risks, dependencies, estimate assumptions, and schedule threats. | AI estimates are not truth. Teams must adjust based on actual capacity and evidence. |
| Architecture | Use AI to critique boundaries, coupling, data ownership, API contracts, failure paths, permissions, and governance points. | Do not accept architecture the team cannot explain or maintain. |
| Construction | Use AI for scaffolding, code suggestions, debugging, refactoring ideas, and explaining unfamiliar APIs. | Generated code must be reviewed, tested, and connected to issues and pull requests. |
| Review | Use AI as an additional reviewer for correctness, maintainability, security, architecture fit, tests, and dependencies. | AI review does not replace human review. |
| Testing | Use AI to propose test cases, negative paths, edge cases, regression tests, and failure scenarios. | AI-generated tests often mirror assumptions; teams must challenge the implementation. |
| Operations / Observability | Use AI to help analyze logs, identify operational anomalies, summarize incidents, draft runbooks, propose recovery steps, or critique observability gaps. | AI operational suggestions must be validated against actual runtime evidence, recovery procedures, governance expectations, and release constraints. |
| Release and Presentation | Use AI to draft release notes, summarize changes, prepare demo scripts, and check clarity. | Release claims must be supported by repository evidence, not polished wording. |

---

## GitHub-First AI Workflow Expectations

ETIS-aligned student teams should use AI within a repository-centered engineering workflow.

Teams should:

* Use issues to define the work before asking AI to produce or revise artifacts.
* Use branches and pull requests so AI-assisted changes are visible and reviewable.
* Explain in pull requests why the AI-assisted change exists.
* Identify what evidence supports the change.
* Identify what risks were considered.
* Disclose meaningful AI assistance in the pull request description or linked AI-use log entry.
* Use AI review as an additional signal, not as the engineering approval authority or merge decision maker.
* Update requirements, tests, architecture notes, decisions, or release evidence when AI-assisted changes affect them.
* Maintain release or version evidence identifying the repository state associated with major demonstrations, presentations, and operational reviews.

A useful rule for student teams is:

```text
No issue, no branch, no pull request, no review, no merge.
```

---

## Privacy, Security, and Data Rules

Students and teams must not paste the following into AI tools:

* Real student records
* Grades
* Private university data
* Credentials
* Tokens
* API keys
* Passwords
* Personal information
* Confidential material
* Sensitive operational information

Use synthetic sample data unless the instructor explicitly approves another approach.

Do not connect AI tools to live production systems or real institutional workflows without instructor approval.

If an AI tool suggests a package, API, database, or integration, document the dependency and review license, security, and maintainability risks.

If AI-generated content affects user-facing behavior or system actions, document the human approval point and what evidence is logged.

---

## Tool Guidance

Tool availability, limits, and institutional access change quickly.

Students should use free or university-accessible tools when possible and should not pay for tools unless they personally choose to do so.

GitHub-centered tools are preferred when they fit the repository, issue, pull request, and evidence workflow used in the course.

Possible tool categories include:

| SDLC Slice | Suggested Tool Types | Course Use | Student Note |
|---|---|---|---|
| GitHub workflow | GitHub Copilot, GitHub code review features, repository assistants | Coding assistance, chat, command-line help, code review, pull request support, repository-centered development | Use within issues, branches, pull requests, and review discipline. |
| Coding in editor | GitHub Copilot in Visual Studio Code, Gemini Code Assist, or similar IDE tools | Inline suggestions, code explanation, debugging help, test ideas, and code generation | Do not accept code blindly. |
| Command-line / local workflow | GitHub Copilot CLI, Gemini CLI, or similar terminal tools | Explaining commands, generating scripts, exploring local files, debugging errors | Read commands before running them. Never paste secrets. |
| Requirements / planning / documentation | ChatGPT, Microsoft Copilot, Gemini, Claude, or similar tools | Brainstorming, critique, rewriting, finding gaps, summarizing decisions, drafting documentation | Treat output as draft analysis. Verify against project scope. |
| Team collaboration | GitHub integrations, Teams integrations, notification tools | Repository notifications, issue/PR visibility, discussion-to-action workflow | Optional. GitHub remains the authoritative engineering record. |
| Security / dependency awareness | Dependabot, code scanning, Snyk, SonarQube, or similar tools | Dependency vulnerability awareness, static analysis, code quality, security review | Tools identify risks. Teams must classify, mitigate, document, and explain them. |
| Observability / operations | GitHub Actions logs, logging tools, monitoring tools, observability assistants | Runtime diagnostics, operational troubleshooting, release investigation | Operational evidence must remain explainable and reviewable. |

This guidance intentionally avoids depending on one vendor or tool because AI tooling changes rapidly.

Use tools that support engineering discipline.

Do not let tools replace engineering discipline.

---

## Quick Student Checklist

Before accepting AI-assisted work, teams should ask:

* Did AI materially help produce or revise this artifact?
* Did the team disclose the assistance in the AI-use log or pull request?
* Can the team explain the output without reading the AI transcript?
* Did the team verify the result with review, tests, inspection, or evidence?
* Did the output stay within approved project scope?
* Did the team avoid private data, credentials, and unsafe integrations?
* Is the final artifact stored in GitHub where a reviewer can inspect it?
* Could another engineering team inspect the repository evidence and understand the AI-assisted engineering decisions without interviewing the original team?

---

## Reusable Team AI-Use Statement

Teams may adapt the following statement for their repository.

```text
This project may use AI tools for requirements analysis, planning, architecture critique, implementation assistance, testing ideas, review support, documentation, and presentation preparation. All AI-assisted output is reviewed, modified when needed, verified by the team, and disclosed in the project AI-use log. The team remains responsible for the correctness, security, maintainability, explainability, governance, operational behavior, and release readiness of all submitted work.
```

---

## Core Thesis

AI use is expected.

Blind trust is not.

Professional engineering teams use AI to accelerate engineering work while preserving human judgment, verification, review discipline, governance, operational accountability, and ownership.

The responsible question is never:

```text
Did AI generate this?
```

The responsible question is:

```text
Did humans review, verify, understand, disclose, and accept responsibility for this?
```
