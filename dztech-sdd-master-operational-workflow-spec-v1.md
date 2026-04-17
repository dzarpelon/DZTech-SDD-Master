# DZTech SDD Master — Operational Workflow

## States
- idea
- approved_idea
- spec_draft
- validated_spec
- project_created
- backlog_generated
- in_execution
- pr_review
- product_validation
- released

## Transitions

- idea → approved_idea (Human Operator)
- approved_idea → spec_draft (AI Agent)
- spec_draft → validated_spec (Human Operator)
- validated_spec → project_created (Orchestrator)
- project_created → backlog_generated (AI Agent)
- backlog_generated → in_execution (AI Agent)
- in_execution → pr_review (AI Agent)
- pr_review → product_validation (Human Operator)
- product_validation → released (Human Operator)

## Rules

- No state skipping allowed
- Human gates are mandatory
- AI must STOP on ambiguity
- AI must NOT assume missing logic

## Validation Gates

### Gate 1 — Idea Approval
Actor: Human Operator

### Gate 2 — Spec Approval
Actor: Human Operator

### Gate 3 — Critical PR Review
Actor: Human Operator (conditional)

### Gate 4 — Product Validation
Actor: Human Operator