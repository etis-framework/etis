---
hide:
  - toc
---

# ETIS Engineering Review Center

**Instructor-facing formal phase-gate review grounded in repository evidence**

The ETIS Engineering Review Center is the formal review component of the [ETIS Engineering Education Suite](Engineering_Education_Suite.md).

It gives instructors a structured environment for conducting detailed, phase-aware engineering reviews across multiple student teams while preserving evidence lineage and instructor authority.

The Review Center is the public-facing name for the instructor review environment previously described as the **Instructor Engineering Workbench**.

---

## Formal Phase-Gate Evidence Boundary

Developmental work can change continuously. Formal engineering review needs a stable evidence boundary.

In the flagship implementation, the course-designated Git tag identifies the evidence submitted for the phase gate. The Review Center takes the formal snapshot from that tagged repository state and performs the gate-specific analysis against that evidence.

The tagged submission establishes what the team presented for review.

---

## What the Review Center Provides

The Review Center supports instructors with evidence-centered analysis such as:

- phase-gate-aware repository review;
- rubric-aligned evidence;
- reviewer findings and summaries;
- confidence associated with analysis;
- evidence lineage showing where supporting information came from;
- cross-team review visibility;
- longitudinal awareness of prior phase-gate analysis;
- identification of evidence gaps, contradictions, risk, and areas requiring instructor attention;
- review continuity across the semester.

The purpose is not to produce an opaque AI score.

The purpose is to make the evidence, reasoning, confidence, and provenance behind the review visible enough for an instructor to exercise informed academic judgment.

---

## Same Engineering Review Board, Different Mandate

Engineering Studio and the Review Center use the same controlled engineering reviewer perspectives so that the meaning of strong engineering evidence remains coherent across the course.

In [Engineering Studio](Engineering_Studio.md), those reviewers act as mentors, coaches, and challengers helping students develop judgment.

In the Review Center, they act as formal engineering review-board members analyzing the evidence submitted at the gate.

The standards remain coherent. The review purpose and authority change.

---

## Developmental History Does Not Become Formal Evidence

An instructor may have visibility into Studio reviews and student/reviewer dialogue. That can help the instructor understand how students are learning and where teams are struggling.

The formal gate remains evidence-centered.

Studio conversations are not silently folded into the Review Center's formal phase-gate evidence. The formal review analyzes the tagged submission presented for that gate.

This mirrors professional engineering review practice: coaching before the review can improve the work, but the evidence presented at the review must be defensible on its own.

---

## Phase-Gate and Longitudinal Awareness

The Review Center is aware of the current phase gate and prior phase-gate analysis.

This matters because the same evidence should not be interpreted identically at project launch, architecture formation, release readiness, and operational enhancement.

The formal review can therefore evaluate the current submission in the context of the engineering maturity expected at that stage while retaining continuity with earlier program decisions and findings.

---

## Instructor Authority

The Review Center assists the instructor; it does not become the instructor.

The system can organize evidence, surface findings, provide confidence, summarize reviewer analysis, and preserve lineage.

The instructor remains responsible for:

- evaluating the meaning and sufficiency of the evidence;
- resolving ambiguity;
- considering course context;
- applying the rubric;
- exercising academic judgment;
- determining the educational outcome of the phase gate.

This boundary is central to ETIS.

> **AI-assisted review may strengthen visibility and consistency. It does not transfer educational authority to the model.**

---

## Relationship to Preflight and Engineering Studio

The three suite components answer different questions.

**[ETIS Preflight](Preflight.md)** helps the team determine whether expected evidence is present and basically review-ready.

**[ETIS Engineering Studio](Engineering_Studio.md)** gives students a developmental environment for repeated evidence-grounded mini-reviews, questions, challenge, and engineering judgment practice.

**Engineering Review Center** performs the instructor-facing formal analysis of the tagged phase-gate evidence.

Together they support readiness, learning, and evaluation without collapsing those responsibilities into one opaque system.

---

## Adoption Boundary

The Review Center is intended for instructors and educational stewards, not for public self-service use.

An adopting institution determines its phase-gate model, rubrics, repositories, access controls, reviewer configuration, course policies, and instructor responsibilities.

The COMP 330/474 implementation provides a reference model, not a requirement that another institution reproduce the course unchanged.

[Explore Institutional Adoption →](Institutional_Adoption.md)

[Study the COMP 330/474 Flagship Implementation →](Flagship_Implementation.md)

---

## Bottom Line

The ETIS Engineering Review Center turns a formal phase gate into an evidence-centered engineering review rather than an opaque automated assessment.

It shows the instructor what the reviewers found, how confident the analysis is, and where the supporting evidence came from—while keeping the instructor responsible for the final academic judgment.
