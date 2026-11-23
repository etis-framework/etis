# ETIS publication landing-page profile standard

**Scope:** The 13 ETIS white papers, five executive briefs, and six education papers. This standard applies to the canonical website records only; it does **not** amend the authoritative PDFs or Word masters.

## Required reader information

1. Existing series, identifier, publication date, version/edition, page count, depth, and status metadata remain authoritative as stated on each canonical page.
2. **Reading time:** A clearly approximate range, not a guarantee. Existing series ranges are retained. WP-013 and COMP-WP-006 use page-count-based estimates until a verified body-text count is available. Do not describe these ranges as exact PDF-derived word-count measurements.
3. **Primary focus:** One short, source-grounded sentence immediately after the metadata block. It should describe the specific contribution, not repeat the full abstract or invent a new technical claim.
4. **Intended audience:** Use each page's existing audience section and role tags; do not duplicate it in a new profile card.
5. **Learning takeaways:** Use each page's existing `Why Read This...` / `What You Will Take Away` section; do not add competing outcomes lists.
6. **Related reading:** Preserve existing links and reading paths, and verify destinations during release QA.

## Editorial and technical boundaries

- The publication PDF remains the citable edition; website metadata is a discovery aid.
- Do not change the meaning, date, version, title, subtitle, or technical claims of a paper through reader-facing metadata.
- Keep executive briefs oriented to decisions, white papers to engineering reasoning, and education papers to learning and professional practice.
- Preserve distinct treatment of advisory model output versus trusted authorization; neither MCP nor A2A grants authority.
- Keep new focus descriptions concise; do not add a redundant new `Reader profile` box.

## Acceptance checks

- All 24 canonical records have exactly one primary-focus statement, one reading-time field, one audience section (`Intended Audience` or `Who Should Read`), and one learning-takeaway section (`Why Read This` or `What You Will Take Away`).
- Confirm all 24 PDFs remain unchanged; no DOC/DOCX edits.
- Verify canonical publication identifiers and version records, especially WP-013 v1.1 and COMP-WP-006 v1.0.
- Run `python -m mkdocs build --clean --strict` and the repository link validation workflow.
- Review the publication metadata layout at mobile and desktop widths.
- Before publishing a **new repository release**, update `CITATION.cff` version/date/artifact URL together to the intended new tag, review `CHANGELOG.md` and `README.md`, merge, tag the exact verified commit, and publish the release. Do not move historical tags.
