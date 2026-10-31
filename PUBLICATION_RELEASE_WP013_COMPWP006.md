# ETIS Companion Publications — Release and Validation

## Scope

- New canonical publication pages: WP-013 and COMP-WP-006.
- Authoritative PDFs and editable Word masters in existing series asset directories.
- Updates to publication overview, both series indexes, reading paths, citations, Library, What’s New, and discovery pages.
- No changes to existing publications or book edition content.

## Publication governance

- Proposed permanent IDs: WP-013 and COMP-WP-006. Confirm against the authoritative publication registry before merge.
- Canonical pages describe version **1.0**, October 2026. Existing manuscript cover labels may differ; harmonize in a later controlled source revision if required.
- PDFs are the authoritative public editions; Word masters are stored alongside them as non-authoritative source documents. The website does not link to DOCX downloads.

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
