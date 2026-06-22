# Release Notes Template

**Classification:** ETIS Educational Ecosystem Asset  
**Category:** Template  
**Origin:** Loyola University Chicago COMP 330 — Software Engineering  
**Authoritative Format:** Markdown  
**Typical Repository Location:** `/docs/release/release-notes.md`

## Purpose

Release notes explain what shipped, what changed, what remains limited, what is operationally risky, what was deferred, and what is intentionally constrained.

They are not marketing copy.

They are engineering communication supported by repository evidence.

Release notes should support engineering review, operational understanding, and release decisions. They should not merely create presentation polish.

---

## Engineering Guidance

- Keep this file concise, evidence-based, and updated for each release.
- Link to GitHub Issues, Pull Requests, tests, defects, risk records, AI-use logs, demo notes, release tags, and operational evidence when available.
- Repository tags, release versions, or equivalent release identifiers should align with the repository state demonstrated during presentation or review.
- Adapt the sample structures to actual release evidence, risks, and operational maturity.

---

## 1. Release Information

| Item | Team Entry |
|---|---|
| Team Number / Team Name | |
| Repository URL | |
| Release Name / Version | Cycle 1 Release / Final Release / v0.1 / v1.0 |
| Release Date | |
| Release Owner | |
| Evidence Owner | |
| Primary Demo Path | |
| Repository Tag / Commit | |

---

## 2. Executive Release Summary

Write 3-5 sentences explaining:

- What this release does
- Who it serves
- What is ready to demonstrate
- What evidence supports the release
- What major limitations or risks remain

---

## 3. What Shipped

Claims listed here should remain defensible through repository evidence, tests, reviews, and release artifacts.

| Feature / Capability | Status | Evidence Link or Repo Path |
|---|---|---|
| Student can submit a support request | Complete | Issue #__; PR #__; `/docs/testing/final-test-evidence.md` |
| Reviewer can update request status | Complete | Issue #__; PR #__; demo step |
| Request category suggestions | Deferred | `/docs/release/known-limitations.md` |
| | | |

---

## 4. What Did Not Ship / Deferred Scope

| Deferred Item | Reason Deferred | Impact | Next Action / Owner |
|---|---|---|---|
| Email notification workflow | Out of Cycle 1 scope | Users must check status manually | Evaluate for Cycle 2 — Planning Lead |
| Role-based admin dashboard | Not needed for first vertical slice | No admin summary view yet | Reassess after postmortem |
| | | | |

---

## 5. Testing and Validation Evidence

| Test Area | Evidence Completed | Result | Evidence Link or Repo Path |
|---|---|---|---|
| Unit tests | Request validation tests | Pass | `/tests/...` |
| Integration tests | Submit and update request workflow | Pass | `/docs/testing/final-test-evidence.md` |
| Manual demo path | Submit request → review → update status | Pass with known limitation | `/docs/release/demo-script.md` |
| AI validation, if applicable | Category suggestions reviewed by human | Not applicable / Pass / Needs work | `/docs/ai/ai-use-log.md` |
| Operational / observability validation | Logging, runtime diagnostics, recovery expectations, or postmortem review | Pass / Needs work | `/docs/observability/`; `/docs/operations/` |
| | | | |

---

## 6. Known Limitations and Residual Risks

Honest limitation visibility is a professional engineering strength, not a weakness.

| Limitation / Risk | Severity | User Impact | Mitigation / Disposition | Owner |
|---|---|---|---|---|
| No real university login integration | Medium | Demo uses simulated users only | Documented constraint; do not use real student data | Architecture Lead |
| Limited error handling for invalid request edits | Low | Reviewer may see basic error message | Add validation refinement in Cycle 2 | Quality Lead |
| AI suggestion service unavailable | Medium | Manual category selection required | Human workflow fallback documented | Architecture Lead |
| | | | | |

---

## 7. Defects Fixed, Open, or Accepted

| Defect ID / Issue | Disposition | Evidence | Notes |
|---|---|---|---|
| Issue #__ — status update bug | Fixed | PR #__; regression test added | |
| Issue #__ — empty category display | Deferred | `/docs/release/known-limitations.md` | Low severity; Cycle 2 candidate |
| | | | |

---

## 8. AI Use and Verification Summary

Summarize how AI was used for the release, such as requirements review, code generation, test brainstorming, debugging, documentation, presentation preparation, or review.

State what humans accepted, rejected, modified, and verified.

AI-assisted outputs should remain explainable, reviewable, governable, and traceable through repository evidence.

| AI Use Area | Accepted / Modified / Rejected | Verification Evidence |
|---|---|---|
| Test-case brainstorming | Modified | Human review; final tests in `/tests` |
| Release notes draft wording | Modified | Team reviewed for accuracy against repository evidence |
| | | |

---

## 9. Traceability and Evidence Index

Another engineering team should be able to inspect the linked evidence and understand the release state without relying on private explanation from the original team.

| Claim | Evidence Location |
|---|---|
| Requirements covered by this release | `/docs/planning/traceability.md` |
| Final test evidence | `/docs/testing/final-test-evidence.md` |
| Known limitations | `/docs/release/known-limitations.md` |
| AI-use log | `/docs/ai/ai-use-log.md` |
| Demo script / presentation evidence | `/docs/release/demo-script.md`; `/docs/release/presentation-index.md` |
| | |

---

## 10. Release Readiness Judgment

**Release judgment:** Ready for Cycle 1 presentation / Ready for final presentation / Ready with limitations / Not ready

**Rationale:**  
State why the team believes this release is defensible based on engineering evidence, operational understanding, residual risk visibility, and engineering judgment.

The team should be able to explain why this release was considered safe enough, reviewable enough, governable enough, and operationally understandable for the current release scope.

---

## 11. Quick Checklist Before Submission

- [ ] Release notes state what shipped and what did not ship.
- [ ] Known limitations and residual risks are honest and specific.
- [ ] Testing and validation evidence is linked from the release notes.
- [ ] AI assistance is disclosed and human verification is described.
- [ ] Defects are classified as fixed, deferred, accepted, mitigated, or removed from scope.
- [ ] The team can explain every major claim in the release using repository evidence.
- [ ] The release notes clearly separate verified behavior from planned future capability.
- [ ] The repository state associated with the release is identified by tag, version, commit, or equivalent marker.

---

## Final Takeaway

A release note is a professional engineering artifact.

It should help another engineer understand what changed, what evidence supports the release, what risks remain, and why the team believes the current release judgment is defensible.
