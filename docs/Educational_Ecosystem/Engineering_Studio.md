---
hide:
  - toc
---

# ETIS Engineering Studio

**Developing engineering judgment through evidence-grounded review**

AI can increasingly help students produce code, tests, documentation, and other project artifacts.

The harder educational question is:

> **If AI can help students produce software, how do we ensure they are still learning to be software engineers?**

ETIS Engineering Studio addresses that problem directly.

Engineering Studio is an **instructor-operated, browser-based learning environment for student engineering teams**. It uses controlled, evidence-grounded reviewer perspectives to help students examine their own project, defend engineering decisions, identify uncertainty, challenge findings, and learn how to reason from evidence.

The student remains the responsible engineer.

---

## What Engineering Studio Is For

Engineering Studio is not an AI coding assistant, an answer generator, or an automated grader.

It is designed to develop engineering judgment before formal phase-gate review.

Students use Studio to:

- examine the project holistically rather than artifact by artifact;
- conduct developmental mini-reviews before a formal gate;
- ask questions about facts and findings surfaced by reviewers;
- defend recommendations, tradeoffs, assumptions, risks, and unknowns with evidence;
- challenge a reviewer when the evidence supports a different conclusion;
- identify unresolved engineering decisions;
- understand where evidence is weak or missing;
- connect current project concerns to relevant ETIS guidance;
- improve the repository before the formal phase-gate submission.

A well-supported disagreement with a reviewer can demonstrate stronger engineering judgment than passive agreement.

“I don't know yet” is also a valid engineering position when the evidence gap is explicit and the next step is understood.

---

## Frozen Evidence Snapshots

A student team may start a Studio evidence snapshot whenever a developmental review would be useful.

Teams can create multiple snapshots as the project improves.

Once created, the snapshot freezes the repository evidence used for that review. This gives the students and reviewers a stable factual basis for discussion and preserves provenance.

Every student on the team sees the same snapshot evidence. Individual students can then interact independently with the reviewers against that shared evidence base.

This creates an important educational condition:

> **The facts remain shared while the reasoning remains individual.**

Snapshot evidence is immutable. Review interpretations may be corrected when contrary evidence proves a finding wrong, but the underlying frozen evidence is not rewritten.

---

## Six Controlled Reviewer Perspectives

The reference Engineering Studio uses a multidisciplinary engineering review board:

- **Chief Architect / Chair** — architecture coherence, consequential decisions, tradeoffs, and overall engineering reasoning;
- **Security Engineer** — security boundaries, threat considerations, sensitive data, trust assumptions, and risk;
- **Verification Lead** — test strategy, evidence quality, claims, defects, and verification sufficiency;
- **Operations Lead** — deployability, observability, recoverability, service behavior, and operational readiness;
- **Human Impact Reviewer** — users, stakeholders, usability, human consequences, oversight, and responsible operation;
- **Red Team** — weak assumptions, failure paths, contradictions, gaming, and adversarial challenge.

The reviewers are controlled agents with bounded roles and evidence scope.

They may challenge, question, compare evidence, and identify concerns. They must not fabricate evidence or become the student's decision authority.

---

## Reviewer as Mentor, Not Oracle

Studio reviewers are designed to coach and guide rather than give students the engineering answer.

A reviewer may ask why a decision was made, point out conflicting evidence, surface an overlooked risk, or direct the student toward the relevant engineering guidance.

The student must still decide what the evidence means and what action the team should take.

This is a deliberate educational boundary:

> **The reviewers help students learn how to reason about engineering. They do not solve the engineering problem for them.**

---

## Phase-Gate and History Awareness

Engineering Studio is phase-gate aware.

The current phase changes what the reviewers expect to find, which engineering concerns deserve attention, and what maturity is reasonable at that point in the semester.

Studio is also aware of prior phase-gate analysis. Review does not restart from zero at every checkpoint. Earlier decisions, findings, corrections, and engineering history provide context for later work.

This supports a longitudinal engineering experience rather than a sequence of disconnected assignments.

---

## Three Review Modes

Engineering Studio supports three complementary review purposes.

### Board Review

The normal multidisciplinary engineering review. The review board examines the current frozen snapshot using the concerns appropriate to the current phase gate.

### Focused Review

A student-selected review of a specific engineering concern such as an architecture decision, requirement, artifact, pull request, risk, AI use, verification issue, or other consequential choice.

### Review Findings

A focused environment for understanding, questioning, challenging, resolving, accepting, deferring, or providing contrary evidence for one or more existing findings.

Students may ask questions in any review mode. The mode defines the review purpose, not a rigid dialogue script.

---

## Connection to the Engineering Platform

Engineering Studio is linked to and aware of the [ETIS Engineering Platform](../Platform/Platform.md).

When a student needs additional guidance, Studio can direct the student to relevant resources that open separately, including:

- the appropriate ETIS Engineering Stage;
- Starter Kit templates and guidance;
- governance or evidence patterns;
- completed LMU/COICP reference examples.

The Platform supplies professional guidance and examples. The student's own team repository remains the authoritative project record.

The objective is contextual instructional scaffolding: help the student find the right engineering knowledge at the moment it becomes relevant without replacing the student's own reasoning.

---

## Relationship to Preflight and Formal Review

Engineering Studio is one part of the [ETIS Engineering Education Suite](Engineering_Education_Suite.md).

**[ETIS Preflight](Preflight.md)** is the phase-gate readiness capability. It checks whether expected evidence is present and has the basic shape needed before formal submission.

**Engineering Studio** is the developmental environment. A team may use it many times to improve its engineering understanding and evidence.

**[ETIS Engineering Review Center](Engineering_Review_Center.md)** is the instructor-facing formal review environment. Its evidence boundary is established by the course-designated phase-gate Git tag.

Studio review history may be visible to the instructor, but Studio conversations do not become hidden evidence in the formal phase-gate review. The tagged submission must stand on its own.

!!! important "Developmental review and formal review are intentionally separate"
    Engineering Studio is a coaching and engineering-judgment environment. The Engineering Review Center performs the formal phase-gate review against the evidence submitted at the designated Git tag. Students are not being trained against a hidden grading conversation, and prior Studio dialogue is not silently used as formal gate evidence.

---

## Instructor-Operated Course Environment

Engineering Studio is not currently a public self-service application.

Students do not independently create production Studio environments. The instructor or adopting institution provisions and configures the environment, establishes the course term and teams, controls authorization, and determines the repositories that may become trusted course evidence.

The reference implementation includes:

- institutional identity and course authorization;
- GitHub identity and exact-repository authorization;
- section and team context;
- frozen evidence snapshots;
- review sessions and findings;
- longitudinal Engineering Records;
- instructor cross-team visibility;
- setup → active → archived semester lifecycle;
- read-only historical preservation after archival.

---

## Built as an Operational Course Service

Engineering Studio has been engineered as a course service rather than a classroom prototype.

The production reference architecture uses managed Azure services and operational controls supporting reliability, availability, serviceability, and recoverability.

The reference deployment includes:

- Azure Container Apps;
- PostgreSQL Flexible Server;
- Microsoft Entra identity;
- GitHub OAuth and a GitHub App;
- Azure Key Vault and managed identity;
- Application Insights and Log Analytics;
- GitHub Actions with OIDC deployment;
- private database networking;
- database migration discipline;
- backup, point-in-time recovery, and rollback readiness.

The production reference implementation completed acceptance on August 21, 2026.

This architecture is a reference, not a requirement that another institution reproduce Loyola University's exact cloud configuration.

---

## Institutional Adoption

Engineering Studio was developed for use in the COMP 330/474 Software Engineering flagship implementation at Loyola University Chicago.

Other universities adopting ETIS may deploy Studio for their own courses, students, teams, institutional identities, GitHub organizations, and operating policies.

Each adopting institution should own its own:

- cloud environment;
- identity registration and authorization model;
- GitHub App and OAuth configuration;
- course, roster, and team authorization;
- domain and TLS configuration;
- database, backups, and recovery policy;
- secrets and managed identities;
- AI service and cost controls;
- monitoring and alerts;
- privacy, retention, and semester lifecycle policy.

[Explore Institutional Adoption →](Institutional_Adoption.md)

---

## Open-Source Reference Implementation

The Engineering Studio source is published as an open-source reference implementation under the Apache License 2.0.

**Repository:** [etis-framework/etis-engineering-studio ↗](https://github.com/etis-framework/etis-engineering-studio)  
**Reference release:** v0.16.0

The public repository supports inspection, institutional evaluation, and adoption. It should not be confused with a public student sign-up service: production use requires instructor or institutional deployment and configuration.

---

## Bottom Line

Engineering Studio exists to make engineering judgment observable and developable.

AI may help produce artifacts. The Studio asks students to explain what the evidence means, challenge weak conclusions, defend consequential decisions, recognize uncertainty, and remain responsible for the system they are building.

**AI can increasingly write code. ETIS Engineering Studio helps students learn to take responsibility for the engineering decisions around it.**
