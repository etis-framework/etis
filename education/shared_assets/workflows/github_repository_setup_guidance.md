# GitHub Repository Setup Guidance

**Classification:** ETIS Educational Ecosystem Asset  
**Category:** Workflow  
**Origin:** Loyola University Chicago COMP 330 — Software Engineering  
**Authoritative Format:** Markdown

---

## Core Idea

Your team GitHub repository is the project control center.

It is where the team creates the authoritative evidence trail for work, review, testing, AI use, and release readiness.

This document explains how to create and connect the repository. The separate repository structure and README guidance explains what must live inside it.

---

## 1. Purpose of This Guidance

Each COMP 330 team must create a GitHub repository early in the semester. The repository should be created as one of the first team formation actions by Week 2, before serious project work begins.

The purpose is not simply file storage. The repository is the shared engineering workspace where lifecycle-traceable evidence is created through issues, branches, pull requests, reviews, testing, and releases.

This document focuses on repository setup. It does not define the required folder structure, README contents, or detailed artifact layout. Those expectations are covered in the separate Repository Structure and README Guidance document.

Use this document first to create the repository correctly. Then use the structure document to organize the repository professionally.

The two documents should be used together:

- This document explains how to establish and operate the repository.
- The Repository Structure and README Guidance document defines the professional engineering layout and evidence organization expected throughout the semester.

---

## 2. Required Repository Setup Decision

Each team must create one public GitHub repository for the semester project unless the instructor explicitly approves a different arrangement.

Public repositories make evidence easier to inspect during phase-gate reviews and reduce access problems during grading.

The repository should be created by the team lead or another agreed owner during team launch.

All team members must be added as collaborators or given appropriate access through the repository or organization.

The repository URL must be submitted in assignments and used for phase-gate reviews.

The repository must not contain:

- Real private data
- Credentials
- Secrets
- Tokens
- Student records
- Grades
- Live university information

Use synthetic data for examples, demos, tests, and screenshots.

---

## 3. Standard Repository Naming Convention

Use a predictable repository name so the instructor can identify teams quickly and so repositories remain professional.

Use lowercase letters, numbers, and hyphens only.

| Item | Required Convention |
|---|---|
| Recommended format | `comp330-f26-teamNN-project-name` |
| Example default project | `comp330-f26-team03-campusconnect` |
| Example alternative project | `comp330-f26-team07-soccer-player-analysis` |

If team numbers are not assigned yet, use a temporary descriptive name and rename the repository after team numbers are assigned.

Do not use joke names, ambiguous names, or personal account names as the project identity.

---

## 4. Create the Repository on GitHub

1. Sign in to GitHub using an account you can reliably access throughout the semester.
2. Create a new repository using the standard naming convention above.
3. Set visibility to **Public** unless the instructor approves a private repository.
4. Initialize the repository with a README if GitHub offers that option. The README can be replaced later using the repository structure guidance.
5. The repository README should become the professional front door to the project and link to major engineering evidence, release artifacts, and operational resources.
6. Add a `.gitignore` appropriate for the technology stack if the team already knows the stack. If unsure, add it later after the architecture and development plan are clearer.
7. Do not add real credentials, API keys, secrets, or private data to the repository.
8. After creation, copy the repository HTTPS clone URL ending in `.git` and record it in the team launch evidence.

---

## 5. Repository URL Required for Assignments and Phase-Gate Reviews

Assignments act as phase-gate reviews and require the repository URL.

The preferred URL for setup and cloning is the HTTPS clone URL ending in `.git`.

GitHub remote URLs are commonly HTTPS URLs such as:

```text
https://github.com/user/repo.git
```

or SSH URLs such as:

```text
git@github.com:user/repo.git
```

### How to Find the `.git` URL

1. Open the team repository in GitHub.
2. Click the green **Code** button.
3. Select **HTTPS** unless the team is intentionally using SSH.
4. Copy the URL that ends with `.git`.
5. Paste that URL into the team launch document, Assignment 1 submission, and repository evidence index as required.

| URL Type | Example |
|---|---|
| HTTPS clone URL | `https://github.com/loyola-comp330/comp330-fall2026-team03-campusconnect.git` |
| SSH clone URL | `git@github.com:loyola-comp330/comp330-fall2026-team03-campusconnect.git` |

---

## 6. Add Team Members and Establish Access

Every team member must be able to:

- Clone the repository
- Create branches
- Push branches
- Open pull requests
- Review pull requests
- Update evidence artifacts

At least two people should have administrative or maintainer access so the team is not blocked if one person is unavailable.

Do not share GitHub passwords, personal tokens, or SSH private keys.

If a student cannot access the repository, the team should treat that as a project blocker and resolve it immediately.

---

## 7. Recommended GitHub Tool Ecosystem

Students may use any reasonable workflow that produces visible repository evidence.

The course does not require one specific tool interface, but teams should be familiar with the common GitHub ecosystem.

| Tool or Surface | What It Is Useful For | Course Expectation |
|---|---|---|
| GitHub website | Repository creation, issues, pull requests, reviews, Actions, settings, and evidence inspection. | Required. Students must be comfortable navigating the repository in the browser. |
| GitHub Desktop | Visual cloning, branching, committing, pulling, pushing, and pull request support for students less comfortable with command line. | Allowed and recommended for students who want a visual Git workflow. |
| Command-line Git | Direct professional workflow for clone, branch, commit, push, pull, merge, and troubleshooting. | Strongly recommended. Appendix B provides a basic workflow. |
| Visual Studio Code | Editing source code and documentation, integrated terminal, Git view, extensions, and GitHub Pull Requests extension. | Allowed. Do not rely on extensions the team cannot explain or maintain. |
| GitHub Issues and Projects | Task tracking, defects, enhancements, backlog, assignment, and traceability. | Expected for meaningful work tracking, ownership visibility, defect management, and engineering traceability. |
| GitHub Actions | Basic automated build/test validation supporting controlled integration, release confidence, and operational readiness. | Introduced during construction and integration; expected to support visible build/test evidence during release readiness and maturity reviews. |
| GitHub Copilot / AI tools | Code suggestions, explanations, review support, test ideas, documentation drafts, pull request exploration, and implementation assistance. | Allowed when disclosed, reviewed, verified, and owned by the team. |
| Logs, CI artifacts, and runtime evidence | Observability, debugging, runtime validation, failure investigation, and release confidence. | Introduced progressively as the system matures through Cycle 2 operational readiness. |

---

## 8. Optional Microsoft Teams Integration

Teams may coordinate in Microsoft Teams, Zoom, Discord, text chat, or another agreed channel, but GitHub remains the authoritative engineering record.

Microsoft Teams integration with GitHub is optional, not required.

If a team uses Microsoft Teams, GitHub integration can help surface repository activity in a Teams channel. Teams may use notifications for issues, pull requests, commits, code reviews, and Actions workflow events.

Recommended use:

- Receive notifications about new issues
- Receive notifications about pull requests
- Receive notifications about reviews
- Receive notifications about CI/CD failures

Not recommended:

- Treating Teams chat as the only place where engineering decisions live

Course rule:

> Decisions made in chat must be reflected in GitHub issues, pull requests, decision records, or other repository evidence.

---

## 9. GitHub and AI Integration Points

GitHub is increasingly an AI-assisted engineering environment.

Teams may use GitHub Copilot or other approved AI tools, but AI output must remain subject to human engineering judgment.

GitHub Copilot can assist with:

- Coding
- Code explanation
- Pull request understanding
- Code review workflows
- Test ideas
- Documentation drafts

Teams may use AI to draft, explain, critique, test, and review work.

Teams must not allow AI to become an unreviewed author of project truth.

Meaningful AI assistance must be disclosed in the AI-use log.

AI-generated code should be reviewed more carefully, not less carefully.

Teams remain responsible for the long-term maintainability, security, correctness, and operational consequences of AI-assisted work.

Never commit secrets, private data, or sensitive student information into AI prompts or the repository.

---

## 10. Minimum Setup Checklist

- [ ] Public GitHub repository created using the course naming convention.
- [ ] All team members have access and can clone the repository.
- [ ] Repository HTTPS clone URL ending in `.git` has been copied and recorded.
- [ ] Initial README exists, even if it is temporary.
- [ ] README links to major engineering evidence locations as the repository matures.
- [ ] No real private data, credentials, secrets, or live university data is stored in the repository.
- [ ] Team has agreed whether to use GitHub Desktop, command-line Git, Visual Studio Code, or a mixed workflow.
- [ ] Initial issue tracker use has begun for team setup tasks.
- [ ] Team knows that the separate Repository Structure and README Guidance document controls the required folder and artifact layout.
- [ ] Assignment 1 launch evidence points to the repository URL and authoritative evidence locations.

---

## 11. Common Setup Mistakes to Avoid

| Mistake | Why It Hurts the Team |
|---|---|
| Creating the repository late | The team loses early evidence and starts the project without a shared control system. |
| Making the repository private without approval | The instructor may not be able to inspect evidence during phase-gate reviews. |
| Using inconsistent or unclear naming | Repositories become harder to identify and manage. |
| Only one person has access | The team is blocked when that person is unavailable. |
| Uploading files manually without learning Git workflow | The team misses the professional issue-branch-pull request-review-traceability-evidence model used to control engineering change. |
| Putting decisions only in chat | Important engineering decisions become invisible and unreviewable. |
| Committing secrets or real data | Creates unnecessary privacy, security, and governance risk. |

---

## Appendix A: Git and GitHub for Students New to the Tools

Git and GitHub are related, but they are not the same thing.

| Concept | Plain-English Explanation |
|---|---|
| Git | The version control tool. It tracks changes, branches, commits, merges, and history. |
| GitHub | A cloud platform that hosts Git repositories and adds collaboration features such as issues, pull requests, reviews, Actions, permissions, and project visibility. |
| Local repository | The copy of the project on your computer. |
| Remote repository | The shared copy hosted on GitHub. The default remote is usually named `origin`. |

A simple mental model:

> Git tracks the work. GitHub hosts the shared project and makes teamwork visible.

---

## Appendix B: Command-Line Git Workflow for Beginners

Students may use GitHub Desktop or Visual Studio Code, but every software engineer should understand the command-line workflow.

The sequence below is intentionally basic.

### 1. Confirm Git Is Installed

```bash
git --version
```

### 2. Configure Your Name and Email Once

```bash
git config --global user.name "Your Name"
git config --global user.email "your-luc-email@luc.edu"
```

### 3. Clone the Team Repository Locally

```bash
git clone https://github.com/OWNER/REPOSITORY.git
cd REPOSITORY
```

### 4. Start from the Trusted Main Branch

```bash
git checkout main
git pull origin main
```

### 5. Create a Branch Tied to an Issue

```bash
git checkout -b issue-12-add-request-form
```

### 6. Inspect Changed Files Before Committing

```bash
git status
git diff
```

### 7. Stage and Commit Your Work

```bash
git add .
git commit -m "Add request form for issue #12"
```

### 8. Push Your Branch to GitHub

```bash
git push -u origin issue-12-add-request-form
```

### 9. Open a Pull Request on GitHub

Open GitHub in the browser, compare your branch to `main`, and create a pull request.

Link the issue using text such as:

```text
Closes #12
```

### 10. After Review and Merge, Update Local Main

```bash
git checkout main
git pull origin main
```

### 11. Delete the Local Branch After Merge

```bash
git branch -d issue-12-add-request-form
```

---

## Appendix C: Pull Request Basics

A pull request is the review gate between individual work and team-owned work.

Before a change enters `main`, the team should be able to answer:

- What changed?
- Why did it change?
- Who reviewed it?
- What evidence proves it works?
- Where is that evidence stored?

Engineering evidence associated with pull requests should be reviewable without requiring verbal clarification from the original author.

Open a pull request for meaningful code, documentation, testing, configuration, or evidence changes.

Link the pull request to the issue or task that explains why the change exists.

Keep pull requests small enough to review honestly.

Include test evidence, screenshots, or documentation links when relevant.

Disclose AI assistance when AI helped produce code, tests, documents, diagrams, or review notes.

Do not merge your own work without review unless the instructor explicitly permits an exception.

Pull requests should explain not only what changed, but also why the change was safe enough to merge.

---

## Appendix D: How This Setup Connects to Course Evidence

The repository setup supports the course traceability model.

The core rule is:

```text
No issue → no branch → no pull request → no review → no merge.
```

The workflow exists to create visible engineering traceability showing:

- Why work was performed
- How it was reviewed
- What changed
- What risks were identified
- Why the change was accepted

Issues capture tasks, defects, enhancements, and questions.

Branches isolate unfinished work.

Pull requests create the review gate.

Reviews challenge correctness, scope, security, maintainability, AI use, and evidence.

Merges move approved work into the shared version of truth.

Releases and repository tags identify the specific repository state associated with major demonstrations, presentations, and release reviews.

Documentation and test evidence show that the team can defend the change later.

---

## Appendix E: Useful Official References

These official GitHub resources may help students who want more detail beyond this course setup guidance.

- GitHub Docs: Cloning a repository
- GitHub Docs: About remote repositories and remote URLs
- GitHub Docs: GitHub Desktop documentation
- GitHub Docs: Integrating GitHub with Microsoft Teams
- GitHub Docs: GitHub Copilot documentation and Copilot code review

---

## Final Takeaway

Create the repository early.

Make it public unless instructed otherwise.

Name it consistently.

Add the whole team.

Copy the `.git` clone URL.

Treat GitHub as the engineering control system for the semester.

The repository is where the team proves, reviews, governs, and operationally defends its engineering work.
