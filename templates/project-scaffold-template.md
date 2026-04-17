# Project Scaffold Template

Use this template to define the minimal v1 scaffold for a materialized project.

## Required Files

- `README.md`
- `project-spec.md`
- `project-metadata.md`

## README.md

Purpose:

- identify the materialized project by `project_name`
- identify the validated spec path
- identify the matching project record path
- state that the scaffold is a minimal inspectable output of the DZTech SDD Master workflow

## project-spec.md

Purpose:

- identify `project_id`
- identify `project_name`
- identify `framework_version`
- identify `source_spec`
- restate the project objective in copied or derived form from the validated specification
- restate minimal acceptance criteria aligned with the validated specification and matching project record

## project-metadata.md

Purpose:

- identify `project_id`
- identify `project_name`
- identify `framework_version`
- identify `source_spec`
- identify `project_record`
- identify `materialized_at`

## Deterministic Rules

- derive scaffold content from the validated specification and matching project record
- use `framework/manifest.md` as the only `framework_version` source
- keep the scaffold minimal, readable, and inspectable by a human
