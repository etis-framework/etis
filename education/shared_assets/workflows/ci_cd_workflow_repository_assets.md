# CI/CD Workflow Repository Assets

**Classification:** ETIS Educational Ecosystem Asset  
**Category:** Workflow  
**Origin:** Loyola University Chicago COMP 330 — Software Engineering  
**Authoritative Format:** Markdown  
**Typical Repository Location:** `/.github/workflows/`

## Purpose

This guide provides example repository assets teams may adapt to introduce basic Continuous Integration and Continuous Delivery evidence into a student engineering repository.

CI/CD is not used because it is trendy. It is used because professional teams need repeatable evidence that the project still builds, tests still run, documentation remains reviewable, and engineering change is controlled through visible validation.

These examples are starter patterns, not mandatory one-size-fits-all solutions. Teams should adapt the pattern to their actual technology stack rather than forcing an inappropriate workflow.

---

## What CI/CD Means in This Course

| Concept | Plain-English Meaning | Evidence Value |
|---|---|---|
| Continuous Integration | Every proposed change is automatically checked when pushed or opened as a pull request. | Shows the team did not rely only on manual confidence. |
| Build Check | The project can be installed and prepared from a clean checkout. | Supports repeatable demo, operational confidence, and release readiness. |
| Test Automation | Automated tests run without someone clicking through manually. | Connects requirements and defects to evidence. |
| Linting / Formatting | Basic style or documentation quality checks run consistently. | Reduces avoidable review noise and improves maintainability. |
| Dependency Scan | Known dependency risks are surfaced early. | Supports security and governance awareness. |
| Pull Request Gate | Checks run before merge into main. | Turns GitHub into an engineering control system. |

---

## Minimum Recommended Workflow

Teams do not need sophisticated deployment automation.

A simple CI workflow is enough if it produces visible evidence on pull requests.

Minimum expectations:

- Run on pull requests and pushes to `main`.
- Install project dependencies.
- Run tests or at least a smoke check.
- Optionally lint Markdown or source files.
- Keep the workflow simple enough that the team can explain it.
- Document failed, skipped, or intentionally limited checks in release evidence.

---

## Generic CI Workflow

Use this when the team wants a simple placeholder workflow that proves the repository can run a basic check.

Replace the placeholder commands with project-specific build and test commands.

```yaml
# File: .github/workflows/ci.yml
name: CI

on:
  pull_request:
  push:
    branches: [ main ]

jobs:
  basic-checks:
    runs-on: ubuntu-latest

    steps:
      - name: Check out repository
        uses: actions/checkout@v4

      - name: Show repository contents
        run: ls -la

      - name: Confirm required folders exist
        run: |
          test -f README.md
          test -d docs
          test -d src || echo "src folder not created yet"
          test -d tests || echo "tests folder not created yet"

      - name: Project-specific build or test command
        run: |
          echo "Replace this with your real build/test commands."
```

---

## Node / JavaScript CI Workflow

Use this pattern if the team uses a Node-based frontend, backend, or full-stack project.

```yaml
# File: .github/workflows/node-ci.yml
name: Node CI

on:
  pull_request:
  push:
    branches: [ main ]

jobs:
  build-test:
    runs-on: ubuntu-latest

    steps:
      - uses: actions/checkout@v4

      - name: Set up Node
        uses: actions/setup-node@v4
        with:
          node-version: '20'
          cache: 'npm'

      - name: Install dependencies
        run: npm ci

      - name: Run tests
        run: npm test -- --watch=false

      - name: Build project
        run: npm run build --if-present
```

---

## Python CI Workflow

Use this pattern if the project uses Python, Flask, FastAPI, scripts, or Python-based tests.

```yaml
# File: .github/workflows/python-ci.yml
name: Python CI

on:
  pull_request:
  push:
    branches: [ main ]

jobs:
  test:
    runs-on: ubuntu-latest

    steps:
      - uses: actions/checkout@v4

      - name: Set up Python
        uses: actions/setup-python@v5
        with:
          python-version: '3.12'

      - name: Install dependencies
        run: |
          python -m pip install --upgrade pip
          if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
          pip install pytest

      - name: Run tests
        run: pytest -q
```

---

## Markdown Documentation Check

Use this if the team wants documentation quality checks for repository evidence files.

This is helpful because much of the course evidence lives in Markdown.

```yaml
# File: .github/workflows/markdown-check.yml
name: Markdown Check

on:
  pull_request:
  push:
    branches: [ main ]

jobs:
  markdown:
    runs-on: ubuntu-latest

    steps:
      - uses: actions/checkout@v4

      - name: Install markdownlint-cli
        run: npm install -g markdownlint-cli

      - name: Lint Markdown files
        run: markdownlint "**/*.md" || true
```

The `|| true` keeps the workflow informational. Remove it if the team wants Markdown lint failures to block the pull request.

---

## Dependency Review

Use this to introduce supply-chain awareness when teams add external packages.

```yaml
# File: .github/workflows/dependency-review.yml
name: Dependency Review

on:
  pull_request:

jobs:
  dependency-review:
    runs-on: ubuntu-latest

    steps:
      - uses: actions/checkout@v4

      - name: Dependency Review
        uses: actions/dependency-review-action@v4
```

If dependency review is too much for the project, teams may instead document dependency decisions in an ADR or security review note.

---

## Pull Request Evidence Expectations

A workflow only helps if the team uses the results.

Pull request authors and reviewers should treat CI/CD output as part of the lifecycle-traceable engineering evidence trail.

| Pull Request Question | Expected Evidence |
|---|---|
| Did the workflow run? | Link or screenshot of GitHub Actions / pull request checks. |
| Did it pass? | Passing check, or clear explanation of failure and correction. |
| What did it prove? | Build succeeded, tests ran, docs checked, dependency scan completed, or limitations stated. |
| What remains manual? | Manual test notes, demo checks, known limitations, or deferred validation. |
| Did AI help create the workflow? | AI-use log entry and human verification notes if applicable. |

---

## Common Mistakes to Avoid

- Copying a workflow the team cannot explain.
- Adding CI/CD after the release instead of using it during development.
- Ignoring failed checks because the demo still works.
- Letting generated workflow files access secrets or deploy systems without review.
- Treating green checks as complete proof of quality.
- Using CI/CD as decoration instead of connecting it to pull requests, tests, and release notes.

Passing automation does not eliminate the need for engineering judgment, review, threat awareness, or operational reasoning.

---

## Suggested Starter Path

1. Start with the generic CI workflow.
2. Replace the placeholder command with the project’s real build or test command.
3. Add Node or Python workflow only if it fits the actual stack.
4. Add Markdown checking if the team wants cleaner repository evidence.
5. Add dependency review when the project introduces third-party packages.
6. Reference CI/CD results in construction, release, and final readiness evidence.

---

## Final Takeaway

CI/CD is not about impressing anyone with automation.

It is about making quality checks visible, repeatable, reviewable, and operationally defensible.

In ETIS-aligned engineering education, the repository is the proof source. CI/CD helps the repository prove that the team is controlling change professionally.
