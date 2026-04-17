# TASK — reconcile-repo

## Purpose

Update an existing repository so it matches the source-of-truth files.

This is the default task for an existing repository and the main repository reconciliation task.

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
3. Produce an exact gap list before applying edits
4. Preserve valid existing work unless it conflicts with the source-of-truth files
5. Prefer moving or refactoring valid files instead of recreating them
6. Replace weak placeholders with minimal functional implementations only where required
7. Implement only the missing or incomplete required components
8. Validate the final repository state against the governing files

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
- Preserve valid existing work unless it conflicts with the source-of-truth files
- Prefer moving or refactoring valid files instead of recreating them
- Keep the reconciliation behavior deterministic and explicit
- Summarize exact gaps, applied changes, and remaining human review points using the required final summary sections

---

## Constraints

You MUST NOT:

- Recreate the repository if it already exists
- Remove existing valid structure
- Duplicate repository structures
- Over-engineer the implementation
- Add features not defined by the specifications
- Invent new architecture beyond the source-of-truth files
- Rely on prompts as the source of truth

---

## Success Criteria

Repository state is valid when:

- Required structure exists and remains coherent
- Required files contain real content, not only scaffolding
- Workflow representation exists in repository files
- GitHub Actions CI is present and valid
- The repository is ready for human validation

## Required Final Summary

The final reconciliation summary must include:

- `Gaps Found`: exact missing, incomplete, or inconsistent items found
- `Changes Applied`: exact repository changes made
- `Remaining Human Review Points`: decisions, risks, or confirmations still requiring human review

---

## Final Step

Stop after completing the required repository updates and summarizing the changes for Human Operator validation.
