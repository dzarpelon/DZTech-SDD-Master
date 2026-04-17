# CODEX TASK — DZTech SDD Master

## Objective

Create a FULLY FUNCTIONAL foundation for the repository "DZTech SDD Master"
both locally and on GitHub.

---

## Inputs

You MUST read:

- dztech-sdd-master-spec-v1.md
- dztech-sdd-master-operational-workflow-spec-v1.md
- AGENTS.md

---

## Requirements

You MUST:

### Repository Setup
1. Create local folder: DZTech-SDD-Master
2. Initialize git repository
3. Create GitHub repository: "DZTech SDD Master"
4. Connect local repo to remote
5. Push initial commit

---

### Repository Structure

Create structure:

- /ideas
- /specs
- /projects
- /framework
- /.github/workflows

---

### Required Files

Create:

- README.md (describe purpose of repo)
- AGENTS.md (already provided)
- Spec files (already provided)

---

### GitHub Actions (MANDATORY)

Create a working CI pipeline:

File:
.github/workflows/ci.yml

Must include:

- Trigger on push and PR
- Basic job with:
  - checkout repo
  - echo validation step

Example behavior:
- Job name: "Validate Repository"
- Step: "Repository structure validation placeholder"

This MUST be a valid GitHub Actions file (not placeholder text).

---

### Validation

Ensure:

- Repo builds in GitHub Actions
- Workflow executes successfully
- Structure matches specs

---

## Constraints

You MUST NOT:

- Skip CI setup
- Leave workflows as empty placeholders
- Create advanced automation beyond CI
- Add features not defined

---

## Success Criteria

Repository is valid when:

- Exists locally and on GitHub
- Has structure + real files (not only .gitkeep)
- Has working GitHub Actions pipeline
- CI runs successfully

---

## Final Step

STOP execution after:

- Repo is pushed
- CI is configured and valid

Wait for Human Operator validation.