# Traceability

This repository maintains traceability between workflow stages, actors, and repository locations.

## Flow Mapping

- `idea`, `approved_idea` -> `ideas/`
- `spec_draft`, `validated_spec` -> `specs/`
- `project_created`, `backlog_generated`, `in_execution`, `pr_review`, `product_validation`, `released` -> `projects/`
- framework governance and method references -> `framework/`

## Source of Truth Priority

1. Operational Workflow Spec
2. Core Spec
3. Repository State
4. AI reasoning

## Governance

- Human Operator is the final authority
- AI Agent executes within approved constraints
- Orchestrator controls workflow movement
- GitHub is the execution environment
