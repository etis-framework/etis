# Repository Starter Kit Setup Guide

**Classification:** ETIS Educational Ecosystem Asset  
**Category:** Workflow  
**Origin:** Loyola University Chicago COMP 330 — Software Engineering  
**Authoritative Format:** Markdown  
**Typical Repository Location:** Course starter kit documentation

## Purpose

This guide provides step-by-step setup instructions for using an ETIS-aligned student repository starter kit professionally.

The team repository should be created once, organized correctly, and used as the authoritative engineering evidence system for the project.

Do not treat GitHub as file storage only.

For broader GitHub workflow, CI/CD, pull request, issue, and AI-assisted development guidance, also use the GitHub repository setup guidance and repository structure guidance.

---

## Before You Begin

- One student should serve as initial repository creator, but the repository belongs to the team.
- Use the official course starter kit file provided by the instructor.
- Use a clear repository name, such as `comp330-f26-teamX-projectname`.
- Create a public repository unless instructed otherwise.
- Do not upload private data, secrets, API keys, tokens, or peer reviews.

---

## Recommended Professional Setup Path

This is the cleanest Day-1 workflow for most teams.

1. Download the official starter kit archive from the course site.
2. Create a new empty GitHub repository using the team naming convention.
3. Clone the empty repository to your computer.
4. Extract the starter kit into the cloned repository folder.
5. Review `README.md` and update the project name, team number, members, and repository URL.
6. After the starter structure is committed, use the repository structure and README guidance to keep the README, `/docs` folders, templates, and evidence locations current throughout the semester.
7. Commit the starter structure with a meaningful message.
8. Push the initial commit to GitHub.
9. Invite all team members as collaborators.
10. Confirm every team member can clone, pull, create a branch, and open a pull request.

---

## Command-Line Setup

```bash
# 1. Clone the empty team repository
git clone https://github.com/<owner>/comp330-f26-teamX-projectname.git
cd comp330-f26-teamX-projectname

# 2. Extract starter kit outside or inside a temporary folder
tar -xzvf ~/Downloads/comp330-f26-starter-kit.tar.gz

# 3. Copy starter contents into the repository root if needed
cp -R comp330-f26-starter-kit/. .

# 4. Confirm structure
ls -la

# 5. Stage, commit, and push
git add .
git commit -m "Initialize engineering repository starter structure"
git push origin main
```

---

## Alternative Setup Path: Upload Through GitHub Web UI

This path is acceptable for students who are still learning Git, but the team should move to branch/PR workflow quickly.

1. Create a new GitHub repository using the naming convention.
2. Extract the starter kit locally.
3. Use GitHub web upload to upload the starter kit files and folders.
4. Commit the uploaded structure with a clear message.
5. Clone the repository locally afterward so team members can work through Git normally.
6. Begin all meaningful work through issues, branches, pull requests, reviews, and checks.

---

## Repository Settings Recommended for Teams

| Setting | Recommendation | Reason |
|---|---|---|
| Visibility | Public unless instructed otherwise | Allows instructor review and avoids access friction. |
| Default branch | `main` | Standard branch name and clean workflow target. |
| Issues | Enabled | Issues are the operational work queue. |
| Actions | Enabled | Actions provide CI/CD, validation, and release-readiness evidence. |
| Projects | Optional | Useful for teams that want visual task tracking. |
| Wiki | Avoid as primary evidence store | Course evidence should live in versioned `/docs` files. |
| Branch protection | Recommended once team workflow stabilizes | Protects `main` from unreviewed changes. |

---

## Professional Workflow After Setup

- Create an issue for meaningful work.
- Create a branch tied to the issue, requirement, task, or evidence purpose.
- Commit changes with meaningful messages.
- Open a pull request before merging into `main`.
- Use the pull request template to document purpose, tests, risks, and AI use.
- Have another team member review meaningful changes.
- Resolve CI/check failures before merge or clearly explain why they do not apply.
- Update evidence files when changes affect requirements, architecture, testing, release notes, or AI-use records.
- Use release tags, versions, or equivalent release markers when preparing major presentation or release evidence.

---

## Common Student Mistakes to Avoid

- Uploading all files through the web UI every time instead of learning branch/PR workflow.
- Editing directly on `main` for meaningful changes.
- Treating `README.md` as a placeholder instead of the repository front door.
- Leaving starter files blank or stale after the project matures.
- Putting peer reviews or private data in the public repository.
- Committing AI-generated code or documentation that the team cannot explain and verify.
- Waiting until the deadline to create evidence instead of maintaining it continuously.
- Creating empty folders or stale template files only to look complete instead of maintaining real engineering evidence.

---

## Day-1 Success Test

By the end of setup, every team member should be able to:

- Open the repository.
- Understand the project purpose.
- Find the main evidence folders.
- Create an issue.
- Create a branch.
- Make a small change.
- Open a pull request.
- Explain the workflow.

The team should also be able to explain why the repository structure supports evidence, review, traceability, AI governance, and release readiness.

---

## Final Takeaway

The starter kit is not a file dump.

It is the first engineering environment the team will use to create visible, reviewable, traceable, AI-accountable, and release-defensible work.
