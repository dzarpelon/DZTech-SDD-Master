# TASK — materialize-project-repo

## Purpose

Create a minimal in-repo project scaffold from a validated specification.

This is the first real deliverable task for v1:

- `validated spec`
- `project record`
- `minimal project scaffold`
- human can inspect and test the result

This task does not create a remote repository or implement downstream automation.

---

## Inputs

You MUST read and follow:

- `master-spec/dztech-sdd-master-spec-v1.md`
- `master-spec/dztech-sdd-master-operational-workflow-spec-v1.md`
- `framework/manifest.md`
- `framework/workflow-state-model.md`
- `templates/spec-template.md`
- `templates/project-record-template.md`
- `project-registry/project-record-template.md`
- `AGENTS.md`

The runtime inputs are:

- one validated spec file
- the matching project record in `project-registry/projects/`

---

## Deterministic Location

Materialize the project scaffold at:

- `project-registry/projects/<project_id>/`

Use the existing project record stem or the source spec basename without the file extension as `<project_id>`.

---

## Execution Model

You MUST:

1. Read the validated spec file
2. Read the matching project record
3. Read `framework/manifest.md` and use its `framework_version`
4. Create the scaffold directory at `project-registry/projects/<project_id>/`
5. Create `README.md`
6. Create `project-spec.md` as a copied or derived project spec from the validated specification
7. Create `project-metadata.md`

---

## Deterministic Rules

- Use the validated spec as the source for scaffold content
- Use the existing project record as the source for `project_id`, `project_name`, and registry alignment
- Use `framework/manifest.md` as the only version source
- The scaffold README must identify the source spec and the matching project record
- The metadata file must include:
  - `project_id`
  - `project_name`
  - `framework_version`
  - `source_spec`
  - `project_record`
  - `materialized_at`
- If the project record does not exist, stop and use `tasks/create-project-from-spec.md` first

---

## Constraints

You MUST NOT:

- Create a remote GitHub repository
- Generate backlog or task systems
- Implement automation pipelines
- Invent architecture beyond the source-of-truth files
- Expand scope beyond a minimal inspectable and testable scaffold

---

## Success Criteria

This task is complete when:

- one scaffold exists at `project-registry/projects/<project_id>/`
- the scaffold contains:
  - `README.md`
  - `project-spec.md`
  - `project-metadata.md`
- the scaffold aligns with the validated spec, the project record, and `framework/manifest.md`
- a human can inspect and test the generated result inside the master repository
