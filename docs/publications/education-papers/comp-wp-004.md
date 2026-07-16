---
hide:
  - toc
---

<div style="text-align:center; margin-bottom:1.5rem;">
  <img src="../../../assets/etis-logo.svg"
       alt="ETIS"
       style="width:320px; max-width:60%; height:auto;">
</div>

<div class="publication-header publication-header--education">
  <div class="publication-series">COMP 330 PROFESSIONAL PAPER SERIES</div>
  <div class="publication-id">COMP-WP-004</div>
  <h1 class="publication-title">Using AI Professionally</h1>
  <p class="publication-subtitle">From Fast Output to Responsible Engineering Judgment</p>
  <p class="publication-byline">William T. O’Connell, Ph.D.</p>
</div>

<div class="publication-metadata" aria-label="Publication at a glance">
  <div class="publication-metadata-item"><span class="publication-metadata-label">Series</span><span class="publication-metadata-value">COMP 330 Professional Paper Series</span></div>
  <div class="publication-metadata-item"><span class="publication-metadata-label">Identifier</span><span class="publication-metadata-value">COMP-WP-004</span></div>
  <div class="publication-metadata-item"><span class="publication-metadata-label">Published</span><span class="publication-metadata-value">Fall 2026</span></div>
  <div class="publication-metadata-item"><span class="publication-metadata-label">Version</span><span class="publication-metadata-value">1.0</span></div>
  <div class="publication-metadata-item"><span class="publication-metadata-label">Length</span><span class="publication-metadata-value">11 pages</span></div>
  <div class="publication-metadata-item"><span class="publication-metadata-label">Reading time</span><span class="publication-metadata-value">25–35 minutes</span></div>
  <div class="publication-metadata-item"><span class="publication-metadata-label">Depth</span><span class="publication-metadata-value">Student and professional development</span></div>
  <div class="publication-metadata-item"><span class="publication-metadata-label">Status</span><span class="publication-status publication-status--current">Current</span></div>
</div>

<div class="publication-actions publication-actions--primary">
  <a class="md-button md-button--primary" href="/assets/publications/education-papers/COMP_WP-004_Using_AI_Professionally.pdf" download>Download PDF</a>
  <a class="md-button" href="/assets/publications/education-papers/COMP_WP-004_Using_AI_Professionally.pdf" target="_blank" rel="noopener">Open PDF</a>
  <a class="md-button" href="#citation">Cite This Paper</a>
  <a class="md-button" href="../../reading-paths/">Reading Path</a>
</div>

<div class="publication-core-thesis">
  <div class="publication-core-thesis-label">Core Thesis</div>
  <p>Professional AI use is not measured by how much work a tool produces. It is measured by whether the engineer can define the task, control the context, evaluate the result, preserve provenance, manage authority, and remain accountable for the outcome.</p>
</div>

## Executive Summary

Artificial intelligence has moved from optional assistance to a normal part of software engineering. Developers use AI to explore unfamiliar code, draft requirements, generate implementations, create tests, review changes, investigate defects, write documentation, and increasingly delegate bounded tasks to coding agents.

The professional question is therefore no longer whether engineers should use AI. It is whether they can use it without surrendering understanding, quality, security, or accountability. AI can accelerate generation while creating a verification tax: time saved during creation may be re-spent auditing work that engineers do not fully trust.

COMP-WP-004 presents a professional operating model for AI-assisted engineering. It treats AI use as a lifecycle decision rather than a prompting technique. The model begins with task classification and risk, continues through intent, context, bounded authority, small-batch execution, independent verification, disclosure, review, and release, and ends with operational observation and learning.

The paper distinguishes assistance from delegation, fluent output from evidence, and disclosure from confession. It explains why generation is not verification, why context is a controlled engineering asset, why large AI-generated changes are difficult to review, and why the same reasoning path cannot serve as both producer and proof.

For COMP 330 students, the standard is direct: AI tools are encouraged, but their work must remain attributable, reviewable, testable, and owned by the team. Students should use AI to increase the scope and quality of engineering—not to conceal the absence of understanding.

The strongest AI user is not the person who accepts the most generated work. It is the person who can determine where AI adds value, where it should not be trusted, what evidence is needed, and how the result fits the complete system.

## Why Read This Paper?

COMP-WP-004 establishes the professional AI-use standard for COMP 330 and provides a durable model for responsible AI-assisted engineering.

After reading it, you should be able to:

- explain why AI is now part of the engineering environment;
- distinguish assist, coordinate, execute, and operate modes;
- begin with an engineering task rather than a prompt;
- treat context as a controlled, versioned, permission-aware asset;
- explain why generation is not verification;
- work in small batches to preserve reviewability and learning;
- disclose AI use as provenance rather than confession;
- manage security, privacy, licensing, and intellectual-property boundaries;
- use AI for critique and learning without outsourcing decisions;
- apply the COMP 330 AI-assisted engineering workflow.

## Key Topics

<div class="publication-key-topics">
  <span class="publication-tag">Professional AI Use</span>
  <span class="publication-tag">AI-Assisted Engineering</span>
  <span class="publication-tag">Bounded Delegation</span>
  <span class="publication-tag">Task Framing</span>
  <span class="publication-tag">Context Engineering</span>
  <span class="publication-tag">Independent Verification</span>
  <span class="publication-tag">Small-Batch Work</span>
  <span class="publication-tag">AI Provenance</span>
  <span class="publication-tag">Security and Privacy</span>
  <span class="publication-tag">Human Accountability</span>
  <span class="publication-tag">Engineering Judgment</span>
  <span class="publication-tag">COMP 330</span>
</div>

## Intended Audience

<div class="publication-audience">
  <span class="publication-audience-tag">COMP 330 Students</span>
  <span class="publication-audience-tag">Computer Science Students</span>
  <span class="publication-audience-tag">Software Engineering Students</span>
  <span class="publication-audience-tag">Early-Career Engineers</span>
  <span class="publication-audience-tag">Software Engineering Instructors</span>
  <span class="publication-audience-tag">Engineering Team Leads</span>
  <span class="publication-audience-tag">AI Governance Leads</span>
  <span class="publication-audience-tag">Engineering Mentors</span>
</div>

## What the Paper Examines

1. AI as a normal part of the engineering environment.
2. Four modes of AI participation: assist, coordinate, execute, and operate.
3. Why professional use begins with the engineering task, not the prompt.
4. Context as a controlled engineering asset.
5. Why generation is not verification.
6. Small-batch work as a control for AI-assisted change.
7. Disclosure as provenance rather than confession.
8. Security, privacy, intellectual property, and authorization boundaries.
9. AI as reviewer, critic, and tutor—but not decision owner.
10. Failure patterns, the COMP 330 workflow, and professional capability.

## Relationship to ETIS

<div class="publication-related">
  <section class="publication-related-card">
    <h3>ETIS Framework</h3>
    <p>COMP-WP-004 operationalizes the ETIS doctrines that AI proposes and engineers verify, context is control, everything important leaves evidence, and accountable humans remain responsible.</p>
    <a href="/Framework/ETIS_Framework/">Explore the ETIS Framework →</a>
  </section>

  <section class="publication-related-card">
    <h3>Engineering Agentic Software Systems</h3>
    <p>WP-004 provides the broader engineering treatment of bounded autonomy, authority, context, identity, tools, behavioral evaluation, human oversight, and runtime governance.</p>
    <a href="../../white-papers/wp-004/">Read WP-004 →</a>
  </section>

  <section class="publication-related-card">
    <h3>Engineering Platform</h3>
    <p>The ETIS Engineering Platform provides the lifecycle stages, governance, evidence, review, release, operations, and stewardship structure for responsible AI-assisted work.</p>
    <a href="https://platform.etisframework.org">Open the Engineering Platform →</a>
  </section>

  <section class="publication-related-card">
    <h3>Engineering Platform Starter Kit</h3>
    <p>The Starter Kit supplies AI-use records, authority boundaries, review artifacts, provenance, verification evidence, release controls, and operational templates.</p>
    <a href="/Resources/Repository_Ecosystem/">Explore the Repository Ecosystem →</a>
  </section>
</div>

### Related Publications

- [WP-001 — Engineering Trustworthy Software in the AI Era](../white-papers/wp-001.md)
- [WP-003 — Engineering Evidence](../white-papers/wp-003.md)
- [WP-004 — Engineering Agentic Software Systems](../white-papers/wp-004.md)
- [WP-005 — Engineering Education in the AI Era](../white-papers/wp-005.md)
- [WP-009 — Context Engineering](../white-papers/wp-009.md)
- [WP-010 — Engineering Digital Colleagues](../white-papers/wp-010.md)
- [WP-012 — The ETIS Manifesto](../white-papers/wp-012.md)
- [COMP-WP-001 — Why Software Engineering Matters More in the AI Era](comp-wp-001.md)
- [COMP-WP-002 — Building a Professional Engineering Portfolio](comp-wp-002.md)
- [COMP-WP-003 — Working Effectively on an Engineering Team](comp-wp-003.md)
- [COMP-WP-005 — Engineering Career Lessons](comp-wp-005.md)

<section id="citation" class="publication-citation" aria-labelledby="citation-heading">
  <h2 id="citation-heading">Citation</h2>

  <h3>IEEE</h3>
  <pre><code>W. T. O’Connell, “Using AI Professionally: From Fast Output to Responsible Engineering Judgment,” COMP 330 Professional Paper Series, COMP-WP-004, ver. 1.0, Fall 2026.</code></pre>

  <h3>APA 7th Edition</h3>
  <pre><code>O’Connell, W. T. (2026). Using AI professionally: From fast output to responsible engineering judgment (COMP-WP-004, Version 1.0). Engineering Trustworthy Intelligent Systems.</code></pre>

  <h3>Chicago</h3>
  <pre><code>O’Connell, William T. “Using AI Professionally: From Fast Output to Responsible Engineering Judgment.” COMP 330 Professional Paper Series, COMP-WP-004, version 1.0. Fall 2026.</code></pre>

  <h3>BibTeX</h3>
  <pre><code>@techreport{oconnell2026usingaiprofessionally,
  author      = {William T. O'Connell},
  title       = {Using AI Professionally: From Fast Output to Responsible Engineering Judgment},
  institution = {Engineering Trustworthy Intelligent Systems},
  type        = {COMP 330 Professional Paper},
  number      = {COMP-WP-004},
  year        = {2026},
  note        = {Version 1.0, Fall 2026},
  url         = {https://etisframework.org/publications/education-papers/comp-wp-004/}
}</code></pre>
</section>

<section class="publication-version" aria-labelledby="version-history-heading">
  <h2 id="version-history-heading">Version History</h2>

  <div class="publication-version-table-wrapper">
    <table class="publication-version-table">
      <thead>
        <tr>
          <th scope="col">Version</th>
          <th scope="col">Date</th>
          <th scope="col">Status</th>
          <th scope="col">Notes</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>1.0</td>
          <td>Fall 2026</td>
          <td><span class="publication-status publication-status--current">Current</span></td>
          <td>Initial publication.</td>
        </tr>
      </tbody>
    </table>
  </div>
</section>

<div class="publication-navigation publication-navigation--cards" aria-label="Publication navigation">
  <a class="publication-navigation-item publication-navigation-item--previous" href="../comp-wp-003/">
    <span class="publication-navigation-label">← Previous</span>
    <span class="publication-navigation-title">COMP-WP-003 — Working Effectively on an Engineering Team</span>
  </a>

  <a class="publication-navigation-item publication-navigation-item--center" href="../../">
    <span class="publication-navigation-label">Publications</span>
    <span class="publication-navigation-title">Publications Overview</span>
  </a>

  <a class="publication-navigation-item publication-navigation-item--next" href="../comp-wp-005/">
    <span class="publication-navigation-label">Next →</span>
    <span class="publication-navigation-title">COMP-WP-005 — Engineering Career Lessons</span>
  </a>
</div>
