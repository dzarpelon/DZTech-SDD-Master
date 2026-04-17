# Workflow State Model

## States

- `idea`
- `approved_idea`
- `spec_draft`
- `validated_spec`
- `project_created`
- `backlog_generated`
- `in_execution`
- `pr_review`
- `product_validation`
- `released`

## Transitions

- `idea` -> `approved_idea` by Human Operator
- `approved_idea` -> `spec_draft` by AI Agent
- `spec_draft` -> `validated_spec` by Human Operator
- `validated_spec` -> `project_created` by Orchestrator
- `project_created` -> `backlog_generated` by AI Agent
- `backlog_generated` -> `in_execution` by AI Agent
- `in_execution` -> `pr_review` by AI Agent
- `pr_review` -> `product_validation` by Human Operator
- `product_validation` -> `released` by Human Operator

## Validation Gates

- Gate 1: Idea Approval by Human Operator
- Gate 2: Spec Approval by Human Operator
- Gate 3: Critical PR Review by Human Operator when applicable
- Gate 4: Product Validation by Human Operator

No state skipping is allowed.
