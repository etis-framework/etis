---
hide:
  - toc
title: "Engineering Agentic AI Systems | ETIS Professional Computing Series"
description: "Build, secure, verify, and operate trustworthy AI agents: 36 chapters, enterprise architecture, and six progressive Python reference builds."
---

<div style="text-align:center; margin-bottom:1.5rem;">
  <img src="/assets/etis-logo.svg" alt="ETIS" style="width:320px; max-width:60%; height:auto;">
</div>

# Engineering Agentic AI Systems

**ETIS Professional Computing Series · Featured Title**

*Build, Secure, Verify, and Operate Trustworthy AI Agents*

**William T. O’Connell, Ph.D.**

<div style="text-align:center; margin:1.25rem 0 1.75rem 0;">
  <img src="/assets/books/agentic-ai/front-cover.png"
       alt="Front cover of Engineering Agentic AI Systems"
       style="width:360px; max-width:100%; height:auto; border:1px solid #d9d9d9; box-shadow:0 12px 32px rgba(0,0,0,.14); border-radius:.25rem;">
</div>

<div style="margin:0 0 1rem 0;">
  <a class="md-button md-button--primary"
     href="/downloads/books/Engineering_Agentic_AI_Systems_First_Edition_2026.pdf"
     download>
     Download Free PDF
  </a>
  <a class="md-button"
     href="https://www.amazon.com/dp/B0HSKLJPT7">
     View on Amazon ↗
  </a>
  <a class="md-button" href="/Books/agentic-ai/companion-resources/">Companion Resources</a>
  <a class="md-button" href="/Books/agentic-ai/updates-and-errata/">Updates &amp; Errata</a>
</div>

!!! note "Publication status"
    **Publication date:** November 26, 2026 · First Edition<br>
    **PDF edition:** Available here as a free ETIS website download.<br>
    **Amazon:** [Paperback and hardcover listings ↗](https://www.amazon.com/dp/B0HSKLJPT7)<br>
    **Paperback ISBN:** 979-8-9966760-6-4<br>
    **Hardcover ISBN:** 979-8-9966760-7-1

---

## About the Book

An agent demonstration is not an independently verified engineering system. Agentic systems must be designed so that model suggestions are separated from trusted consequential execution, and every authority-bearing action can be justified, constrained, observed, and recovered.

*Engineering Agentic AI Systems* develops a vendor-neutral approach to building enterprise agentic AI applications that are governable in production, not merely impressive in a prototype. It shows how to define trust boundaries, establish system contracts, control delegation, authorize effects independently, and verify behavior with executable evidence.

**AI proposes; engineers verify. Governance is architecture. Context is control.**

---

## From AI Models to Trustworthy Agentic Systems

Traditional AI applications often generate an answer for a person to interpret. **Agentic AI systems** can go further: pursuing goals across multiple steps, selecting tools, coordinating agents, and proposing operations that affect enterprise workflows. More autonomy and integration create more potential for consequential mistakes.

<div style="display:grid; grid-template-columns:repeat(auto-fit,minmax(min(100%,220px),1fr)); gap:.85rem; margin:1.35rem 0 1rem; align-items:stretch;" role="group" aria-label="Three-stage conceptual architecture from agentic proposals through independent authorization to enterprise effects">
  <div style="border:1px solid var(--md-default-fg-color--lightest); border-top:4px solid #456c92; border-radius:.45rem; padding:1.1rem; background:var(--md-default-bg-color); box-shadow:0 4px 16px rgba(20,35,50,.07);">
    <div style="font-size:.75rem; font-weight:700; letter-spacing:.06em; text-transform:uppercase; color:var(--md-default-fg-color--light);">01 · Propose</div>
    <div style="font-weight:700; font-size:1.07rem; margin:.5rem 0;">Models &amp; agents</div>
    <p style="margin:0; line-height:1.55;">Reason, plan, coordinate, and request tools. Their outputs are proposals, not permission to act.</p>
  </div>
  <div style="border:2px solid #bd9137; border-top:5px solid #bd9137; border-radius:.45rem; padding:1.1rem; background:var(--md-default-bg-color); box-shadow:0 6px 22px rgba(113,82,20,.14);">
    <div style="font-size:.75rem; font-weight:700; letter-spacing:.06em; text-transform:uppercase; color:#a47b24;">02 · Independently authorize</div>
    <div style="font-weight:700; font-size:1.07rem; margin:.5rem 0;">Trusted execution boundary</div>
    <p style="margin:0; line-height:1.55;">Enforce identity, policy, approval, and transaction constraints outside model-controlled instructions.</p>
  </div>
  <div style="border:1px solid var(--md-default-fg-color--lightest); border-top:4px solid #456c92; border-radius:.45rem; padding:1.1rem; background:var(--md-default-bg-color); box-shadow:0 4px 16px rgba(20,35,50,.07);">
    <div style="font-size:.75rem; font-weight:700; letter-spacing:.06em; text-transform:uppercase; color:var(--md-default-fg-color--light);">03 · Execute &amp; verify</div>
    <div style="font-weight:700; font-size:1.07rem; margin:.5rem 0;">Enterprise systems</div>
    <p style="margin:0; line-height:1.55;">Carry out authorized effects with durable state, evidence, observability, and recovery.</p>
  </div>
</div>

<p style="text-align:center; font-weight:650; margin:.15rem 0 1.2rem;">Agentic coordination proposes · Trusted controls authorize · Enterprise systems execute</p>

**Why the boundary matters.** A model or agent may make a factual error, follow a malicious instruction embedded in retrieved material, optimize an objective in an unintended way, or attempt an unauthorized action. More adversarial behaviors can include **reward hacking, deceptive behavior, and unauthorized coordination**. These are risks to assess and test, not claims that every model or agent will exhibit them. Neither convincing reasoning nor a valid agent access token substitutes for independent authorization.

The book addresses these problems at **two different levels**: evaluating and constraining model/agent behavior, and engineering trusted system controls that limit consequential effects even when that behavior fails. See the [Chapter 29 discussion of adversarial agent behavior](https://github.com/etis-framework/etis-agentic-ai-book/blob/main/manuscript/part-05-reliability-security/ch29-security-and-adversarial-agent-behavior/index.md) and the [companion security exercises](https://github.com/etis-framework/etis-agentic-ai-book/tree/main/examples/refund-reference-system/security).

---

## What Readers Will Learn

- **Architect** bounded agent workflows with an explicit enterprise reference architecture and responsibility boundaries E1–E9 and contracts C01–C09.
- **Secure** identity, context, credentials, integration, and consequential actions through trusted enforcement outside model-generated instructions.
- **Integrate** tools and delegated agents while distinguishing MCP interoperability, A2A delegation, and actual authorization.
- **Build** durable workflows, approvals, provider reconciliation, retries, and recovery under real operational failure.
- **Verify** both intended behavior and adversarial failure modes with tests, logs, independent checks, and defensible evidence.
- **Operate** services with reliability controls, observability, incident response, and lifecycle governance.

---

## The Seven-Part Learning Journey

The 36 chapters span seven parts: foundational concepts; reference architecture and trust boundaries; engineering patterns; a progressive executable refund-system case; distributed failures, security, reliability, and verification; operational governance; and reference contracts.

The running example, **CASE-204**, concerns a $500 refund. Readers follow the system as progressively more capability is introduced without allowing the model to become the source of authority.

## Six Progressive Python Builds

The public executable companion contains **Builds 0–5**, progressing from deterministic controls to bounded agentic assistance, scoped identity and context, independent authorization, provider reconciliation, and coordinated recovery. Each build includes source code, a source-module architecture diagram, executable tests, and documented engineering limitations.

Readers can use **native Python or Docker**, with optional VS Code Dev Container integration for interactive development and debugging. Docker does not require Python on the host; the original textbook commands remain available to native Python users. No paid AI APIs, payment-provider credentials, or third-party Python packages are required for the standard exercises.

The purpose is to run, inspect, test, and critically evaluate the implementations—not to treat a successful demonstration as proof of production readiness.

**New to the reference implementation?** [Start with Build 0](companion-resources.md#reference-implementation-builds-05) and progress through the six builds with their tests and engineering evidence.

[View Companion Resources →](companion-resources.md){ .md-button .md-button--primary }
[Explore the Executable Companion ↗](https://github.com/etis-framework/etis-agentic-ai-book/releases/tag/v1.1.0){ .md-button }

---

## Who This Book Is For

Software engineers, enterprise architects, technical leaders, platform and security teams, reliability engineers, advanced students, and instructors who need to design, review, or operate consequential agentic applications. The book is not a prompt-engineering quick start or a product-specific agent tutorial. Readers benefit from working knowledge of software engineering, APIs, testing, and distributed-system fundamentals; the progressive builds make the design choices concrete for advanced students and working practitioners.

## Relationship to ETIS

The [ETIS Framework Reference Work](../ETIS_Framework_Reference.md) establishes full-lifecycle engineering discipline. This Professional Computing Series volume applies and extends that discipline to the concrete engineering of trustworthy agentic AI systems. The ETIS website is the canonical publication and reader-navigation home; the [public book repository](https://github.com/etis-framework/etis-agentic-ai-book) remains authoritative for manuscript source, code, build diagrams, tests, and implementation documentation.

[Explore the Professional Computing Series →](../ETIS_Professional_Computing_Series.md){ .md-button }
[View Updates & Errata →](updates-and-errata.md){ .md-button }
