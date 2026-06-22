# Meeting Notes Template

**Classification:** ETIS Educational Ecosystem Shared Asset  
**Category:** Template  
**Origin:** Loyola University Chicago COMP 330 — Software Engineering  
**Authoritative Format:** Markdown  
**Typical Repository Location:** `/docs/team/meetings/meeting-YYYY-MM-DD.md` or `/docs/team/meetings/README.md`

## Purpose

Use this template to record concise team meeting evidence for status checks, planning meetings, engineering reviews, release preparation, and decision follow-up.

Weekly status checks should normally take 15-30 minutes, with a target closer to 15 minutes. The goal is not a long discussion. The goal is visibility, agreements, blockers, action items, and next checkpoints.

Meeting notes are engineering evidence. They should make team coordination, decisions, risks, blockers, release concerns, operational issues, and follow-up work visible to future reviewers.

---

## Engineering Guidance

Keep notes short, factual, and action-oriented.

Record decisions, blockers, risks, assignments, and follow-up evidence.

Do not use the status check as a long design meeting. Schedule a separate engineering meeting when deeper discussion is needed.

Link action items to GitHub Issues, Pull Requests, or repository artifacts when possible.

Any team member may take notes, but the Team Lead or Planning & Process Lead should ensure meeting evidence is current.

Meeting evidence should support engineering coordination, workflow visibility, release readiness, operational awareness, and accountable follow-through. It should not merely document that a meeting occurred.

Teams should prefer visible repository evidence, issues, pull requests, reviews, tests, and updated engineering artifacts over verbal status reporting alone.

Another engineering team should be able to inspect the meeting evidence and understand major decisions, blockers, status, release concerns, and next actions without relying on private explanation from the original team.

If AI-assisted work affects architecture, implementation, tests, governance, operational behavior, or release readiness, the meeting should identify what review, validation, or follow-up evidence is required.

---

## Meeting Information

| Item | Team Response |
|---|---|
| Team Name / Number |  |
| Meeting Date |  |
| Meeting Type | Weekly status check / planning / review / release / other |
| Meeting Format | Zoom / in-person / hybrid |
| Start - End Time |  |
| Facilitator |  |
| Note Taker |  |

---

## Attendees

| Name | Present? | Role / Responsibility | Notes |
|---|---|---|---|
|  |  |  |  |
|  |  |  |  |
|  |  |  |  |
|  |  |  |  |
|  |  |  |  |

---

## 1. Status Check

Each person should briefly state what they completed, what they are working on next, and whether they are blocked.

Teams should discuss whether current work remains stable, reviewable, and defensible enough for the next planned release checkpoint.

| Team Member | Completed Since Last Check | Next Work | Blockers / Help Needed | Related Issue / Evidence |
|---|---|---|---|---|
| Example: Mia | Drafted login requirement | Open issue and test plan | Needs API decision | `#12`; `/docs/requirements/` |
|  |  |  |  |  |
|  |  |  |  |  |
|  |  |  |  |  |
|  |  |  |  |  |

---

## 2. Decisions and Agreements

Decisions should remain concise, actionable, reviewable, and connected to repository evidence rather than hidden inside verbal discussion history.

| Decision / Agreement | Owner | Evidence Location | Follow-Up Needed? |
|---|---|---|---|
|  |  |  |  |
|  |  |  |  |
|  |  |  |  |

---

## 3. Risks, Blockers, and Open Questions

| Item | Type | Impact | Owner | Next Action |
|---|---|---|---|---|
| Example: database choice unresolved | Open question | May delay implementation | Architecture Lead | Create ADR draft |
| Example: logging gaps make failures difficult to diagnose | Operational / Observability | Weakens troubleshooting and release confidence | Operations & Evidence Lead | Add logging evidence |
|  |  |  |  |  |
|  |  |  |  |  |
|  |  |  |  |  |

---

## 4. Action Items Before Next Checkpoint

| Action Item | Owner | Backup | Due Date | Evidence / Link | Status |
|---|---|---|---|---|---|
| Example: create PR template | Sam | Lee | Sep 10 | `/.github/pull_request_template.md` | Open |
|  |  |  |  |  |  |
|  |  |  |  |  |  |
|  |  |  |  |  |  |

---

## 5. Next Meeting / Checkpoint

| Item | Team Response |
|---|---|
| Next Meeting Date / Time |  |
| Expected Focus | Status check / planning / review / release readiness / other |
| What Must Be Ready |  |
| Meeting Link or Location |  |

---

## Optional Section: Longer Engineering Meeting Notes

Use this section only when the meeting includes deeper design, architecture, review, debugging, or release-readiness discussion.

Longer engineering discussions should usually produce visible follow-up evidence such as ADRs, issues, pull requests, tests, release notes, architecture updates, or operational guidance.

### Topic Discussed

[Enter topic.]

### Options Considered

[Enter options.]

### Decision or Next Step

[Enter decision or next step.]

### Evidence or Artifact to Update

[Enter repository evidence or artifact.]

---

## Final Check

Before saving this meeting note, confirm:

- [ ] Major decisions are recorded.
- [ ] Blockers and risks are visible.
- [ ] Owners and next actions are clear.
- [ ] Follow-up evidence locations are identified.
- [ ] AI-assisted work requiring review or verification is captured.
- [ ] Release concerns or operational risks are visible when relevant.
- [ ] Another engineering team could understand current status without a private explanation.

---

## Bottom Line

A useful meeting note should make the team’s current status, engineering decisions, blockers, workflow priorities, release concerns, operational risks, owners, and next actions visible without becoming a long transcript or discussion archive.
