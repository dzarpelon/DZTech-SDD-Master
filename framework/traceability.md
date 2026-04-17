# Traceability

This repository maintains traceability between workflow stages, actors, and repository locations.

This file is operationally used by reconciliation and validation work to map workflow intent to repository domains.

## Flow Mapping

- `idea`, `approved_idea` -> `ideation/`
- `spec_draft`, `validated_spec` -> `master-spec/`
- `project_created`, `backlog_generated`, `in_execution`, `pr_review`, `product_validation`, `released` -> `project-registry/`
- reusable scaffolds and repository blueprints -> `templates/`
- framework governance and method references -> `framework/`

## Source Of Truth Context

1. Operational Workflow Spec
2. Core Spec
3. Repository State
4. AI reasoning

## Governance

- Human Operator is the final authority
- AI Agent executes within approved constraints
- Orchestrator controls workflow movement
- GitHub is the execution environment
