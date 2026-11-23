# ETIS Companion Publications — Historical Release and Validation Record

> **Historical release checklist (October 2026).** This document records the initial publication workflow. For the current authoritative records, see the canonical WP-013 and COMP-WP-006 publication pages and `docs/publications/citations.md`. WP-013 is now **v1.1 (revised November 2026)**; COMP-WP-006 remains **v1.0 (October 2026)**. The website repository retains authoritative public PDFs; editable Word masters are maintained separately and are not part of this release.

## Scope

- New canonical publication pages: WP-013 and COMP-WP-006.
- Authoritative PDFs in the website publication asset directories; editable Word masters are maintained separately.
- Updates to publication overview, both series indexes, reading paths, citations, Library, What’s New, and discovery pages.
- No changes to existing publications or book edition content.

## Publication governance

- Permanent identifiers are **WP-013** and **COMP-WP-006**.
- WP-013 was originally published in October 2026 and is currently **v1.1 (November 2026)**. COMP-WP-006 remains **v1.0 (October 2026)**.
- PDFs are the authoritative public editions. Word masters are retained separately; the website does not link to DOCX downloads.

## Validate locally

```bash
python3 -m pip install -r requirements.txt
mkdocs build --strict
```

Check: `/publications/`, both new publication pages, both series indexes, reading paths, citations, ETIS Library, Student Resources, and What’s New. Confirm PDF downloads, mobile cards, and cross-links. Inspect all 15 PDF pages in each document at reading size.

## Git workflow

```bash
git switch -c feature/etis-companion-white-papers
git status --short
git diff --check
git add docs PUBLICATION_RELEASE_WP013_COMPWP006.md
git diff --cached --stat
git diff --cached --check
git commit -m "Publish ETIS agentic AI and engineering career companion papers"
git push -u origin feature/etis-companion-white-papers
```

Review the staged diff before committing. Open a PR and require build and link validation before merge. Do not force push to main.
