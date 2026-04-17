# TASK — reconcile-repo

## Purpose

Update an existing repository so it matches the source-of-truth files.

This is the default task for an existing repository.

---

## Inputs

You MUST read and follow:

- `master-spec/dztech-sdd-master-spec-v1.md`
- `master-spec/dztech-sdd-master-operational-workflow-spec-v1.md`
- `AGENTS.md`

---

## Execution Model

Treat the current repository state as an existing implementation.

You MUST:

1. Analyze the current repository files and structure
2. Compare the repository state against the governing specifications
3. Identify what is missing, incomplete, or inconsistent
4. Implement only the missing or incomplete required components
5. Validate the final repository state

---

## Requirements

You MUST:

- Maintain the repository locally and on GitHub without recreating it when it already exists
- Keep the repository structure aligned with the specifications
- Ensure required repository files exist and contain meaningful content
- Keep workflow representation in repository files
- Keep traceability represented in repository files
- Ensure GitHub Actions CI exists and is functional
- Replace placeholders with minimal functional implementations when required

---

## Constraints

You MUST NOT:

- Recreate the repository if it already exists
- Remove existing valid structure
- Duplicate repository structures
- Over-engineer the implementation
- Add features not defined by the specifications
- Rely on prompts as the source of truth

---

## Success Criteria

Repository state is valid when:

- Required structure exists and remains coherent
- Required files contain real content, not only scaffolding
- Workflow representation exists in repository files
- GitHub Actions CI is present and valid
- The repository is ready for human validation

---

## Final Step

Stop after completing the required repository updates and summarizing the changes for Human Operator validation.
