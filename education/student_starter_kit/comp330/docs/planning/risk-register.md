<!--
COMP 330 Instructional Example Artifact

This Markdown file is an instructional example showing professional engineering evidence patterns, workflow visibility, repository organization, and planning/governance expectations.

Teams should adapt this structure to their actual project, repository evidence, risks, workflow, and operational maturity. Do not preserve the example entries unchanged.

The authoritative operational version of this artifact belongs inside the team GitHub repository and should evolve throughout the semester.
-->

# Risk Register Example

**Purpose:** Tracks risks that could affect scope, schedule, quality, security, governance, operational maturity, or release readiness.

**Typical repository location:** `/docs/planning/risk-register.md`

## Engineering Guidance

Risks should remain visible, actionable, and connected to engineering evidence, release decisions, workflow maturity, and operational understanding.

Significant risks should remain traceable through issues, pull requests, ADRs, release notes, postmortems, or operational evidence when appropriate.

Some risks may justify scope reduction, release delay, additional review, or operational mitigation before release approval.

## Risk Register

| Risk ID | Risk | Category | Probability | Impact | Trigger | Mitigation | Owner | Status |
|---|---|---|---|---|---|---|---|---|
| R-001 | Team underestimates integration work | Schedule / Technical | Medium | High | API and UI do not connect by checkpoint | Build early integration slice | Example: Development Lead | Open |
| R-002 | AI-generated code is accepted without understanding | AI / Quality | Medium | High | PR includes code no one can explain | Require review, validation, and AI-use log | Example: Review Lead | Open |
| R-003 | AI category suggestion lacks governance boundary | AI / Governance | Medium | High | Feature is added without human approval workflow | Defer until validation and approval boundary are documented | Example: Architecture Lead | Open |
| R-004 | Runtime failures are difficult to diagnose | Operational / Observability | Medium | Medium | Errors cannot be reproduced or explained | Improve logging and operational evidence | Example: QA Lead | Open |
| R-005 | Scope expands beyond review capacity | Planning / Release | Medium | High | New features added without estimates or evidence plan | Require scope review and re-estimation | Example: Planning Lead | Open |

## Risk Review Notes

| Date | What Changed? | New Action Needed? | Owner |
|---|---|---|---|
| YYYY-MM-DD | AI category suggestion moved to deferred candidates | Update scope and AI-use expectations | Example: Architecture Lead |
| YYYY-MM-DD | Basic logging gap found during testing | Add operational evidence task | Example: QA Lead |

## Release-Readiness Impact

| Risk ID | Release Impact | Release Decision / Mitigation |
|---|---|---|
| R-002 | AI-assisted behavior cannot be defended if no one understands it | Require human explanation and validation before merge |
| R-004 | Failures may be hard to diagnose during demo or review | Add logs and known limitation note before release |
| R-005 | Team may present unsupported claims | Reduce scope and tie claims to evidence |

## Reviewability Check

Another engineering team should be able to inspect the risk evidence and understand major engineering, governance, operational, and release concerns.
