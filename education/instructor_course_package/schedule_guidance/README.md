# ETIS Schedule Guidance

The **ETIS Schedule Guidance** directory provides reusable sequencing models that help instructors organize ETIS-based learning experiences over time.

This directory does not provide fixed calendars.

It provides engineering maturity sequencing models that instructors may adapt to their own educational environments.

ETIS intentionally teaches engineering progression rather than chapter progression.

The objective is to help students progressively assume greater engineering responsibility throughout a course.

---

## Purpose

The purpose of this directory is to help instructors sequence ETIS learning experiences without rebuilding course structures from scratch.

This directory helps instructors answer questions such as:

* In what order should engineering capabilities be introduced?
* How should students progressively mature throughout a course?
* How should assignments be sequenced?
* How should phase gates be organized?
* How should ETIS chapters be mapped into a course?
* How should different academic calendars be supported?
* How should accelerated offerings be adapted?
* How should professional training environments consume ETIS?

The objective is to sequence engineering maturity rather than simply distribute content across weeks.

---

## Educational Philosophy

Traditional course schedules often organize learning around topics.

ETIS organizes learning around engineering maturity.

Traditional sequencing may look like this:

```text id="yo6lme"
Week 1 - Chapter 1

Week 2 - Chapter 2

Week 3 - Chapter 3
```

ETIS sequencing looks more like this:

```text id="f0mww5"
Engineering Foundations

        ↓

Engineering Construction

        ↓

Engineering Validation

        ↓

Engineering Operations

        ↓

Engineering Defense
```

Chapters support maturity.

Maturity does not serve chapters.

This distinction is one of the defining characteristics of ETIS education.

---

## Guiding Principle

ETIS schedules should answer one question:

> In what order should engineering responsibilities be learned?

Students should progressively learn how to:

* define intent,
* engineer context,
* bound authority,
* verify behavior,
* operate reality,
* explain decisions,
* and own outcomes.

Educational sequencing should support this progression.

---

## Relationship To The Educational Ecosystem

This directory is one component of the Instructor Course Package.

```text id="pgp4yv"
ETIS Book
        ↓
Educational Architecture
        ↓
Shared Assets
        ↓
Instructor Course Package
        ↓
Schedule Guidance
        ↓
Course Implementations
```

The ETIS book remains authoritative.

Schedule Guidance helps instructors translate ETIS doctrine into teachable sequences.

---

## Directory Contents

```text id="fq4iv7"
schedule_guidance/

README.md

schedule_models_library.md

semester_sequence_guidance.md

quarter_sequence_guidance.md

module_sequence_guidance.md

professional_training_sequence_guidance.md

book_mapping_guidance.md

phase_gate_sequencing_guidance.md

schedule_adaptation_guide.md
```

---

## schedule_models_library.md

Provides reusable educational sequencing models.

Examples include:

* 15-week semester
* 16-week semester
* 10-week quarter
* 8-week accelerated offerings
* 6-week modules
* professional training programs

These models provide structure without becoming institution-specific implementations.

---

## semester_sequence_guidance.md

Provides sequencing guidance for traditional semester-based environments.

Examples may include:

* 14-week semesters
* 15-week semesters
* 16-week semesters

The emphasis remains engineering progression rather than week-by-week chapter assignments.

---

## quarter_sequence_guidance.md

Provides sequencing guidance for quarter-based and accelerated academic calendars.

Examples may include:

* 10-week quarters
* 12-week quarters
* compressed offerings

Adaptations should preserve ETIS doctrine while adjusting pacing.

---

## module_sequence_guidance.md

Provides sequencing guidance for smaller ETIS educational experiences.

Examples include:

* AI Governance modules
* Software Architecture modules
* Release Readiness modules
* Operational Readiness modules

Modules should remain focused and intentionally bounded.

---

## professional_training_sequence_guidance.md

Provides sequencing guidance for organizational and professional learning environments.

Examples include:

* workshops,
* professional cohorts,
* leadership programs,
* and workforce development initiatives.

---

## book_mapping_guidance.md

Provides guidance for mapping ETIS chapters into educational experiences.

The emphasis is on capability groupings rather than sequential chapter coverage.

Not every implementation should teach all 39 chapters equally.

---

## phase_gate_sequencing_guidance.md

Provides guidance for organizing assignments as engineering maturity gates.

Students should experience increasing accountability over time.

Assignments should function as professional progression rather than isolated submissions.

---

## schedule_adaptation_guide.md

Provides guidance for adapting schedules to local institutional constraints without disrupting ETIS educational philosophy.

Adaptations should remain intentional and documented.

---

## Engineering Maturity Sequencing Model

ETIS educational experiences generally progress through stages.

```text id="z3kjr0"
Engineering Foundations

        ↓

Engineering Construction

        ↓

Engineering Validation

        ↓

Engineering Operations

        ↓

Engineering Defense
```

Each stage increases engineering responsibility.

Students should feel this progression throughout the course.

---

## Relationship To Syllabus Guidance

The `syllabus_guidance` directory and `schedule_guidance` directory serve different purposes.

```text id="ib6yfi"
syllabus_guidance/
```

Answers:

> What will students experience?

```text id="vwx59q"
schedule_guidance/
```

Answers:

> In what order will students mature?

Both are required.

Neither replaces the other.

---

## What Does Not Belong Here

This directory should remain reusable and implementation-agnostic.

The following artifacts should not be placed here:

* semester-specific calendars,
* instructor-specific schedules,
* yearly schedules,
* institution-specific schedules,
* COMP330 schedules,
* holiday calendars,
* grading schedules,
* or local administrative information.

Those artifacts belong inside adoption examples.

For example:

```text id="mgylw5"
education/
└── adoption_examples/
    └── loyola_comp330/
```

---

## Adaptation Philosophy

Different institutions have different constraints.

Examples include:

* semester length,
* quarter systems,
* enrollment size,
* student maturity,
* meeting frequency,
* institutional requirements,
* and available instructional time.

These constraints may alter pacing.

They should not alter ETIS doctrine.

Adaptations should preserve educational purpose.

---

## Stewardship Rules

Future maintainers should preserve these rules.

* Do not create week-by-week chapter schedules.
* Do not create institution-specific schedules.
* Do not duplicate COMP330 materials.
* Do not sequence content without educational purpose.
* Do not prioritize logistics over engineering maturity.
* Do not disconnect schedules from ETIS doctrine.

This directory should remain reusable, adaptable, and maintainable.

---

## Guiding Standard

Every file in this directory should answer at least one of these questions:

* In what order should engineering capabilities be taught?
* In what order should engineering maturity develop?
* How should ETIS chapters be grouped?
* How should assignments become phase gates?
* How should schedules adapt to different environments?
* How should ETIS remain teachable across institutions?

If a file cannot answer one of those questions, it probably does not belong in this directory.

---

## Core Commitment

The purpose of ETIS Schedule Guidance is not to create better calendars.

The purpose is to help instructors intentionally sequence the formation of trustworthy engineers.

Students should progressively learn how to define intent, engineer context, bound authority, verify behavior, operate reality, explain decisions, and own outcomes.

Educational sequencing should make that progression visible.

That progression is one of the foundations of ETIS education.
