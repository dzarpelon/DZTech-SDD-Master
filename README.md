# DZTech SDD Master

DZTech SDD Master is the central repository for an AI-first Spec-Driven Development method.

## Purpose

This repository provides a single source of truth for:

- the core method specification
- the operational workflow specification
- the repository structure that supports the workflow

## Actors

- Human Operator: final authority
- AI Agent: executor within defined constraints
- Orchestrator: workflow controller
- GitHub: execution environment

## Repository Structure

- `ideation/`: idea-stage artifacts managed before spec drafting
- `master-spec/`: central specification artifacts for the master repository
- `project-registry/`: project records created from validated specs
- `templates/`: reusable repository templates and scaffolds
- `framework/`: framework-level workflow, traceability, and version references
- `tasks/`: file-driven operational tasks for bootstrap, reconcile, and validation
- `.github/workflows/`: repository CI validation

## Governing Specifications

- `master-spec/dztech-sdd-master-spec-v1.md`
- `master-spec/dztech-sdd-master-operational-workflow-spec-v1.md`
- `AGENTS.md`
- `CODEX_TASK.md`
