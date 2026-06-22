# Team Project Overview

## Provenance

Origin: Loyola University Chicago COMP 330 — Software Engineering  
Original Context: COMP 330 team software engineering project  
ETIS Category: Shared Asset — Playbook  
Authoritative Format: Markdown  

This guide originated as a COMP 330 course asset and has been normalized as an ETIS shared playbook. It preserves Loyola COMP 330 provenance while making the guidance reusable across ETIS-aligned educational implementations.

---

## Purpose

This document explains the purpose, structure, expectations, and evidence model for an ETIS-aligned team software engineering project.

The team project is not just a coding assignment.

It is a semester-long engineering evidence exercise.

Teams build a useful software system, but the gradeable professional skill is how well the team defines, plans, architects, reviews, tests, governs, releases, and explains that system.

---

## Core Idea

A professional team does not ask others to trust a demo.

A professional team shows the requirements, design, reviews, tests, risks, AI-use decisions, release notes, and maturity evidence that make the demo credible.

---

## Project Purpose

The team project gives students a realistic experience with modern software engineering.

Teams build a small but meaningful software system across two development cycles.

The system does not need to be large.

It does need to be:

* Understandable
* Reviewable
* Testable
* Governed
* Supported by evidence
* Explainable by the team

Artificial Intelligence tools are expected to be used throughout the lifecycle when they are helpful.

AI may assist with:

* Requirements
* Planning
* Architecture
* Implementation
* Testing
* Review
* Documentation
* Release preparation

AI assistance must be disclosed, reviewed, verified, and owned by the team.

---

## Two-Cycle Project Model

The project is organized around two development cycles.

### Cycle 1: Controlled Vertical Slice

Cycle 1 builds a controlled vertical slice.

The team proves it can launch, plan, architect, construct, review, test, and present a first release with evidence.

Cycle 1 asks:

```text
Can it work?
```

### Cycle 2: Maturity and Professional Readiness

Cycle 2 matures the system.

The team uses feedback, defects, estimates, risks, presentation evidence, and the Cycle 1 postmortem to decide what should be improved.

Cycle 2 is intentionally short, so teams must select realistic maturity scope rather than attempting every possible improvement.

Cycle 2 asks:

```text
Can it survive?
```

---

## Team Formation and Professional Expectations

Software engineering is a team discipline.

Individual technical skill matters, but professional software is delivered through coordination, communication, review, shared ownership, and disciplined evidence.

Each team should:

* Create a team charter
* Create a role matrix
* Establish working agreements
* Establish a communication rhythm
* Use GitHub as the authoritative engineering record
* Document AI use honestly
* Verify AI-assisted output before accepting it
* Participate in review, evidence creation, and release preparation

Every team member must own visible project work.

Every team member must be able to explain what the team built, why it was built, how it was tested, what risks remain, and what evidence supports release readiness.

---

## Default Project: CampusConnect Workflow System

The default project for COMP 330 is **CampusConnect**, a student support request and workflow system.

The project is intentionally university-centered, realistic, and expandable.

It gives teams enough structure to begin quickly while still leaving room for design decisions, feature choices, and professional engineering judgment.

CampusConnect helps students submit campus support requests and helps staff or peer support roles triage, track, update, and resolve those requests.

The system may start small, but it can grow toward broader university workflows such as:

* Tutoring referrals
* Academic support requests
* Club or event support
* Facility issue routing
* Advising intake
* Technology help requests

Teams should keep CampusConnect small enough to engineer well.

A narrow, well-evidenced workflow is stronger than a broad system with weak evidence.

---

## Default Problem Statement

Students often need help but may not know where to go, what information to provide, or how to track the status of a request.

Staff and support teams need enough information to route requests, prioritize work, communicate status, and maintain a record of what happened.

CampusConnect gives the class a realistic workflow problem without requiring access to real university systems or private student data.

---

## Required Design Constraint

Do not use real student records, private university data, or live institutional systems.

Use synthetic sample data and simulated roles.

If a team wants to connect to any external service, that decision must be approved by the instructor and documented as an architecture and security/governance decision.

---

## Suggested User Roles

### Student requester

Submits a request, views status, updates information, and sees resolution notes.

### Support reviewer

Reviews incoming requests, assigns category/status/owner, requests clarification, and records resolution.

### Team administrator

Manages categories, views summary information, and reviews workflow evidence.

### Optional AI assistant

Suggests categories, missing information, risk flags, or draft responses, but does not make final decisions without human review.

---

## Recommended Cycle Scope

The Cycle 2 items below are candidate maturity directions, not a checklist of required features.

Teams should use Cycle 1 evidence, defects, risks, feedback, estimates, and the postmortem to choose a small, defensible Cycle 2 scope.

A focused maturity improvement is stronger than an overcommitted feature expansion.

| Area | Cycle 1: Controlled Vertical Slice | Cycle 2: Maturity and Professional Readiness Candidates |
|---|---|---|
| Core workflow | Student submits a request; reviewer sees it; reviewer updates status; student can view status. | Improve workflow depth, edge cases, status history, search/filter, role handling, and cleaner release behavior. |
| Requirements | Small set of user stories with acceptance criteria and clear out-of-scope decisions. | Refined requirements based on Cycle 1 evidence, defects, risks, feedback, and postmortem findings. |
| Architecture | Simple client/server or modular application with clear data ownership and interfaces. | Improved boundaries, documented decisions, data/context rules, governance points, or simplified architecture based on observed pain. |
| AI use | AI may assist development, requirements, tests, review, and documentation; user-facing AI is optional. | If justified by evidence, add controlled AI assistance such as category suggestion, missing-information prompts, or draft response suggestions with human approval. |
| Testing | Basic unit, integration, or manual tests tied to acceptance criteria and demo path. | Regression tests, negative cases, validation evidence, and final release confidence tied to actual Cycle 1 risks. |
| Operations | Basic logging or evidence of runtime behavior. | Observability, error handling, known limitations, security/governance checklist, or release maturity evidence selected to reduce real project risk. |

---

## Alternative Team Project Option

Teams may propose a different project if the team has a serious interest in building a real system.

Alternative projects are encouraged when they are realistic, appropriately scoped, and suitable for software engineering evidence.

The instructor must approve alternative projects before the team commits to them.

---

## Alternative Project Approval Criteria

An alternative project should satisfy the following criteria.

* The project solves a real workflow, coordination, information, decision, or support problem.
* The project is small enough for a controlled Cycle 1 vertical slice and meaningful Cycle 2 maturity work.
* The project supports visible requirements, planning, architecture, GitHub workflow, testing, defects, release notes, and postmortem evidence.
* The project allows responsible AI use somewhere in the lifecycle, even if AI is not a user-facing feature.
* The project avoids unsafe use of private data, credentials, regulated records, or live production systems.
* The team can demo the system and defend its engineering evidence.

---

## Good Alternative Project Categories

Good alternative project directions include:

* Campus club event planning and approval workflow
* Study group matching and meeting coordination system
* Tutoring intake and scheduling support system
* Student project issue tracker or team health dashboard
* Equipment checkout or lab resource reservation system
* Simple incident or intake management system for a student organization
* Document review or request routing workflow with human approval

---

## Examples Inspired by Prior Student Projects

Prior teams have selected creative projects outside the default campus workflow.

These are examples of appropriately scoped directions, not required topics or endorsements of any product.

### Sports analytics dashboard

A small sports analytics dashboard inspired by sports data products may be appropriate if scoped narrowly.

A good version might focus on one sport, historical player analysis, simple comparisons, visual summaries, synthetic or permitted data, and clear limits on what the analysis claims.

### Music organization or discovery workflow

A small music organization or discovery workflow may be appropriate if scoped to personal music tracking, tagging, listening queues, notes, recommendations, or collection management using sample metadata.

Teams should avoid copying proprietary app behavior, copyrighted content, or private account data.

---

## Projects That Are Usually Too Risky or Too Large

Avoid projects such as:

* Full social networks
* Full learning management systems
* Full marketplaces
* Full university registration systems
* Projects requiring real student data, grades, private records, credentials, or production university integration
* Projects whose main value is only a chatbot with no workflow, evidence, controls, or system boundaries
* Projects that cannot be tested, reviewed, or explained within the course timeline

---

## Required Engineering Evidence Across the Semester

The project is assessed through both the working system and the engineering evidence that supports it.

The GitHub repository is the authoritative evidence source.

Written submissions should summarize and index repository evidence; they should not replace it.

Required evidence includes:

* Team charter, role matrix, working agreements, and AI-use policy
* Requirements package with acceptance criteria, assumptions, and open questions
* Planning package with scope, tasks, estimates, schedule, risks, and traceability
* Architecture package with components, interfaces, data/context ownership, workflows, and decision records
* Issues, branches, pull requests, reviews, build/test evidence, and AI-use disclosures
* Test plans, automated/manual testing evidence, defect tracking, and release notes
* Release/version evidence identifying the repository state associated with each presented release
* Cycle 1 presentation evidence, peer reviews, postmortem learning, and Cycle 2 maturity plan
* Final release evidence covering testing, observability, security/governance, AI-use reflection, risks, and next steps

---

## Assignment Alignment

| Course Stage | Primary Evidence Focus | Major Student Outcome | Typical GitHub Repository Evidence |
|---|---|---|---|
| Assignment 1: Project Launch | Team structure, repo setup, working agreements, AI-use policy | Team is operational before serious implementation begins. | `/docs/team/team-charter.md`, `/docs/team/roles.md`, `/docs/team/working-agreement.md`, `/docs/ai/ai-policy.md`, `/docs/requirements/` |
| Assignment 2: Planning and Estimation | Scope, tasks, estimates, risks, schedule, traceability | Cycle 1 work is visible, bounded, and owned. | `/docs/planning/`, `/docs/requirements/`, `/docs/ai/ai-use-log.md` |
| Assignment 3: Architecture and Intelligent Systems Review | Components, interfaces, data/context ownership, AI/tool boundaries, governance points | The team can explain and review the design before construction accelerates. | `/docs/architecture/`, `/docs/decisions/`, `/docs/reviews/architecture-review.md` |
| Assignment 4: Construction and Review | Pull requests, code review, CI/CD, tests, AI code review | Implementation is controlled, traceable, tested, and reviewed. | `/src`, `/tests`, GitHub issues/PRs, `/.github/`, `/docs/reviews/`, `/docs/testing/` |
| Assignment 5: Cycle 1 Release | Release notes, final test evidence, known limits, demo, peer review | The team presents a working release with honest evidence. | `/docs/release/`, `/docs/testing/`, `/docs/quality/`, `/docs/ai/` |
| Assignment 6: Final Release and Maturity | Cycle 2 improvements, observability, security/governance, final risk and AI-use reflection | The team proves engineering maturity, not just feature completion. | `/docs/release/`, `/docs/observability/`, `/docs/security/`, `/docs/planning/`, `/docs/ai/` |

---

## Minimum Product Expectations

By the end of Cycle 1, every team should have a working, demonstrable vertical slice.

By the end of Cycle 2, every team should have a more mature system with stronger engineering evidence.

### Cycle 1 Minimum

* One primary user workflow implemented
* Basic persistence or state management
* Clear roles
* Requirements traceability
* Tests or validation evidence
* Release notes
* Known limitations
* Controlled demo

### Cycle 2 Minimum

* Evidence-based improvements after Cycle 1
* Better tests
* Defect and risk disposition
* Observability or runtime evidence
* Security/governance review
* AI-use reflection
* Final release notes
* Professional final presentation

---

## AI Use Expectations

AI use is expected, but unmanaged AI use is not acceptable.

Teams should use AI as an engineering assistant, reviewer, critic, generator, explainer, and test-case brainstorming partner.

The team remains responsible for every accepted artifact and every submitted line of code, test, document, diagram, or decision.

Teams must:

* Disclose AI assistance in the AI-use log
* Record what the team accepted, rejected, modified, and verified
* Use AI to find gaps, risks, edge cases, weak requirements, and missing tests
* Avoid accepting generated code, architecture, or tests that the team cannot explain
* Avoid allowing AI to expand scope beyond the approved Cycle 1 or Cycle 2 plan
* Treat AI-generated output as draft material until reviewed by humans and supported by evidence

---

## What Teams Should Do First

Teams should begin by doing the following:

* Form the team and select a team name
* Confirm whether the team will use the default CampusConnect project or propose an alternative
* Identify the Cycle 1 vertical slice
* Create the GitHub repository and minimum folder structure
* Create a professional README that serves as the front door to the project and links to major engineering evidence
* Draft the team charter, role matrix, working agreements, and AI-use policy
* Create initial requirements, risks, assumptions, and open questions
* Decide what evidence must exist before the team starts serious implementation

---

## Final Takeaway

The project succeeds when the team can show both a useful system and the engineering evidence behind it.

A professional team does not ask others to trust a demo.

It shows the requirements, design, review, tests, risks, AI-use decisions, release notes, and maturity evidence that make the demo credible.
