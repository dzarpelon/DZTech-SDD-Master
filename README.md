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

- `ideas/`: idea-stage artifacts managed before spec drafting
- `specs/`: specification-stage artifacts
- `projects/`: project records created from validated specs
- `framework/`: framework-level workflow, traceability, and version references
- `.github/workflows/`: repository CI validation

## Governing Specifications

- `dztech-sdd-master-spec-v1.md`
- `dztech-sdd-master-operational-workflow-spec-v1.md`
- `AGENTS.md`
- `CODEX_TASK.md`
