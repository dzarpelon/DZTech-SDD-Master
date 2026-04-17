# TASK — validate-repo

## Purpose

Audit the repository against the source-of-truth files without changing repository contents.

Use this task for validation-only work.

---

## Inputs

You MUST read and follow:

- `master-spec/dztech-sdd-master-spec-v1.md`
- `master-spec/dztech-sdd-master-operational-workflow-spec-v1.md`
- `AGENTS.md`

---

## Execution Model

Treat the repository as an existing implementation under audit.

You MUST:

1. Analyze the current repository files and structure
2. Compare repository state against the governing specifications
3. Identify missing, incomplete, or inconsistent components
4. Report the gap list clearly
5. Validate the current repository state without making changes

---

## Constraints

You MUST NOT:

- Modify files
- Create files
- Delete files
- Recreate repository state
- Invent missing behavior

---

## Success Criteria

Validation is complete when:

- A clear list of gaps or confirmations is produced
- No repository files are changed
- The repository is ready for Human Operator review
