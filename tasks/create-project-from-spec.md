# TASK — create-project-from-spec

## Purpose

Create a project record from a validated specification.

This task implements the minimal project creation flow:

- `validated_spec` -> `project_created`

It does not create a repository or perform downstream execution.

---

## Inputs

You MUST read and follow:

- `master-spec/dztech-sdd-master-spec-v1.md`
- `master-spec/dztech-sdd-master-operational-workflow-spec-v1.md`
- `framework/manifest.md`
- `framework/workflow-state-model.md`
- `templates/spec-template.md`
- `templates/project-record-template.md`
- `AGENTS.md`

The runtime input is one validated spec file from `master-spec/` or a future project spec path.

---

## Execution Model

Treat the selected spec file as the source for one project record.

You MUST:

1. Read the selected spec file
2. Use `templates/spec-template.md` as the canonical field model for extracting spec information
3. Read `framework/manifest.md` and use its `framework_version`
4. Generate one project record using `templates/project-record-template.md`
5. Write the result to `project-registry/projects/<source-spec-stem>.project-record.md`
6. Set `status` to `project_created`

---

## Deterministic Rules

- Use the source spec path exactly in `source_spec`
- Use `framework/manifest.md` as the only version source
- Use the spec `Name:` value as `project_name` when present
- If no `Name:` value exists, use the source spec basename without the file extension as `project_name`
- Use the execution date in ISO format for `created_at`
- Do not invent `repo_url`, `variant`, or `source_idea` values when they are not present in the source-of-truth files

---

## Constraints

You MUST NOT:

- Create a Git repository
- Create a GitHub repository
- Invent architecture beyond the source-of-truth files
- Skip the `validated_spec` -> `project_created` workflow meaning
- Produce more than one project record from a single spec in one run

---

## Success Criteria

This task is complete when:

- One project record exists in `project-registry/projects/`
- The record contains:
  - `project_name`
  - `framework_version`
  - `source_spec`
  - `created_at`
  - `status`
- The record is derived from repository files only
