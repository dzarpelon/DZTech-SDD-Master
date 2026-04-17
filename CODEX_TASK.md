# CODEX TASK — DZTech SDD Master

## Objective

Create and maintain a reproducible, file-driven foundation for the repository "DZTech SDD Master", both locally and on GitHub.

This repository MUST be executable and evolvable from its files, with repository files serving as the source of truth.

---

## Task System

Repository operational tasks are defined as files in `/tasks/`.

Available tasks:

- `bootstrap-repo.md`
- `reconcile-repo.md`
- `validate-repo.md`

For an existing repository, the default task is `reconcile-repo.md`.

---

## Inputs

You MUST read and follow:

- `master-spec/dztech-sdd-master-spec-v1.md`
- `master-spec/dztech-sdd-master-operational-workflow-spec-v1.md`
- `AGENTS.md`
- the selected task file in `/tasks/`

---

## Task Selection Rules

- Use `/tasks/bootstrap-repo.md` only for initial repository creation
- Use `/tasks/reconcile-repo.md` to update an existing repository so it matches the source-of-truth files
- Use `/tasks/validate-repo.md` for audit-only validation with no file changes

If repository state already exists, do not recreate it. Execute the selected task from `/tasks/` instead.

---

## Constraints

- Do not use prompts as system logic
- Do not duplicate full task bodies in this controller file
- Keep repository behavior reproducible from repository files

---

## Final Step

Execute the selected task file and stop when that task's defined completion point is reached.
