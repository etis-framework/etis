# ETIS Repository Expectations Guidance

The **ETIS Repository Expectations Guidance** document provides reusable syllabus language and governance principles for teaching repository-centered engineering within ETIS-based courses.

This document helps instructors establish the repository as the authoritative engineering record rather than a location for storing code and assignment submissions.

The repository is one of the defining characteristics of ETIS education.

Students should understand from the beginning of the course that repositories preserve engineering intent, decisions, evidence, accountability, and engineering memory.

---

# Purpose

The purpose of this document is to help instructors establish consistent repository expectations across ETIS implementations.

Repository expectations should answer a simple question:

> If another engineer examined this repository six months from now, would they understand what happened?

ETIS treats repositories as professional engineering systems rather than technical storage systems.

Students should learn how repositories support:

* engineering intent,
* engineering evidence,
* reviewability,
* accountability,
* transparency,
* operational thinking,
* and long-term stewardship.

---

# Educational Philosophy

ETIS teaches repository-centered engineering.

The repository is not where engineering ends.

The repository is where engineering becomes visible.

Students should understand that repositories preserve evidence of:

* what was intended,
* what decisions were made,
* what work was performed,
* what was reviewed,
* what was tested,
* what AI contributed,
* what risks remain,
* and why engineering decisions were accepted.

A repository should help future engineers understand both the system and the engineering that created the system.

---

# Core Repository Principle

The following principle should remain visible throughout ETIS implementations.

> The learning management system tells students what to do. The repository proves what the team actually did.

Assignments may be submitted through institutional systems.

Engineering evidence should live in the repository.

---

# Recommended Syllabus Statement

The following language may be used directly in a syllabus.

## Standard Repository Statement

This course uses repository-centered engineering. The repository serves as the authoritative engineering record for the team and system throughout the semester.

Students are expected to preserve evidence of engineering intent, requirements, plans, architecture decisions, implementation activities, reviews, testing, AI use, release readiness, operational considerations, and final engineering accountability.

The repository is not a code submission mechanism. It is an engineering evidence system.

Students should assume that another engineer, reviewer, or future maintainer may eventually inspect the repository to understand the work that was performed.

---

# Short Repository Statement

The following language may be used in abbreviated syllabi.

This course uses repository-centered engineering. The repository serves as the authoritative engineering record and should preserve evidence of decisions, reviews, testing, AI use, risks, and engineering accountability.

---

# First-Day Student Statement

The following language may be used during course introductions.

You are not building a collection of assignments.

You are building an engineering system.

The repository is where that system becomes visible.

Your repository should help another engineer answer questions such as:

* What problem were you solving?
* What decisions did you make?
* Why did you make them?
* What changed over time?
* What did you review?
* What did you test?
* How did AI help?
* What risks remain?
* Why is this release defensible?

The repository should answer those questions without requiring you to stand next to it and explain everything.

---

# Repository Responsibilities

Students should understand that repositories support multiple engineering responsibilities.

These include:

## Responsibility 1 — Preserve Intent

The repository should preserve why work is being performed.

Examples:

* problem statements,
* requirements,
* assumptions,
* goals,
* scope boundaries.

---

## Responsibility 2 — Preserve Decisions

The repository should preserve important engineering decisions.

Examples:

* architecture decisions,
* tradeoffs,
* alternatives considered,
* rationale.

---

## Responsibility 3 — Preserve Evidence

The repository should preserve evidence that supports engineering claims.

Examples:

* test evidence,
* validation records,
* review artifacts,
* release evidence.

---

## Responsibility 4 — Preserve Accountability

The repository should make engineering participation visible.

Examples:

* pull requests,
* reviews,
* AI disclosures,
* ownership records.

---

## Responsibility 5 — Preserve Operational Thinking

The repository should demonstrate that students considered life after implementation.

Examples:

* risks,
* observability,
* runbooks,
* postmortems,
* release readiness.

---

## Responsibility 6 — Preserve Engineering Memory

The repository should help future engineers understand the engineering history of the system.

---

# Repository Evidence Categories

A strong ETIS repository often contains evidence categories such as:

```text id="jef0go"
/docs
  /requirements
  /planning
  /architecture
  /decisions
  /reviews
  /testing
  /quality
  /release
  /operations
  /observability
  /security
  /governance
  /ai
  /postmortems
  /presentations

/src

/tests

/.github
```

This is an example.

Exact structures may vary by implementation.

The evidence expectations should remain stable.

---

# Repository Design Principles

Students should learn these principles.

## Principle 1 — Repositories Are Evidence Systems

Repositories should explain engineering work.

Not merely store engineering work.

---

## Principle 2 — Repositories Should Support Review

A reviewer should be able to navigate the repository efficiently.

Organization matters.

---

## Principle 3 — Repositories Should Explain Decisions

Engineering decisions should remain visible.

---

## Principle 4 — Repositories Should Support Accountability

Contributions and reviews should be traceable.

---

## Principle 5 — Repositories Should Support Future Engineers

Repositories should outlive the semester.

---

# Repository Quality Characteristics

Students should strive to make repositories:

* understandable,
* navigable,
* reviewable,
* maintainable,
* transparent,
* evidence-driven,
* accountable,
* and trustworthy.

These qualities are often more important than aesthetic perfection.

---

# Repository Review Questions

Students should periodically ask:

* Could another engineer understand this repository?
* Could another engineer find important information quickly?
* Are engineering decisions visible?
* Is AI use transparent?
* Are risks documented?
* Are reviews preserved?
* Is evidence connected to claims?
* Could this repository survive team turnover?

If the answer is no, the repository should improve.

---

# AI And Repositories

Repositories should preserve meaningful AI use.

Examples include:

* AI-use logs,
* architecture critiques,
* review notes,
* verification activities,
* lessons learned.

AI contributions should remain visible.

Transparency strengthens trust.

---

# Repository Expectations For Teams

Teams should establish shared repository habits.

Teams should:

* agree on organization,
* review work regularly,
* communicate changes,
* preserve evidence continuously,
* maintain documentation,
* and improve repository quality over time.

Repository stewardship is a team responsibility.

---

# Repository Expectations For Instructors

Instructors should evaluate repositories as engineering systems.

Evaluation should extend beyond code quality.

Instructors should look for evidence of:

* engineering intent,
* planning,
* decision making,
* reviews,
* testing,
* AI governance,
* release readiness,
* operational thinking,
* and accountability.

---

# Common Student Misconceptions

## Misconception 1 — The Repository Is A Submission Folder

It is an engineering record.

---

## Misconception 2 — Only Code Matters

Engineering evidence matters.

---

## Misconception 3 — Documentation Is Separate From Engineering

Documentation is part of engineering.

---

## Misconception 4 — AI Use Does Not Need To Be Visible

Transparency matters.

---

## Misconception 5 — Repositories End At Deployment

Repositories should support operation and future change.

---

# Common Instructor Mistakes

## Mistake 1 — Grading Only Code

Evaluate evidence.

---

## Mistake 2 — Waiting Until The End Of The Semester To Inspect Repositories

Repository quality should be evaluated continuously.

---

## Mistake 3 — Treating Documentation As Administrative Overhead

Documentation preserves engineering memory.

---

## Mistake 4 — Over-Prescribing Folder Structures

Teach responsibilities first.

Structures are secondary.

---

## Mistake 5 — Disconnecting Repositories From Assessments

Repository evidence should directly support assessment activities.

---

# Adaptation Rules

Institutions may adapt repository structures.

However, adaptations should preserve these principles:

* repositories preserve engineering intent,
* repositories preserve evidence,
* repositories preserve accountability,
* repositories support review,
* repositories support operations,
* repositories preserve engineering memory.

These principles should remain visible.

---

# Guiding Standard

Students should be able to answer these questions.

* What problem were we solving?
* What decisions did we make?
* What evidence supports our claims?
* What did AI help produce?
* What did humans verify?
* What risks remain?
* Why is this release defensible?
* Could another engineer understand our repository?

If those answers are difficult to find, the repository needs improvement.

---

# Core Commitment

ETIS repositories are not assignment containers.

They are professional engineering systems.

Students should leave ETIS understanding that repositories preserve engineering memory.

Code may eventually change.

Teams may eventually disappear.

Technologies may eventually evolve.

Engineering memory should remain.

That is one of the foundations of trustworthy intelligent systems.
