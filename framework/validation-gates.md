# Validation Gates

## Mandatory Human Gates

- Gate 1: Idea Approval
- Gate 2: Spec Approval
- Gate 3: Critical PR Review when applicable
- Gate 4: Product Validation

## Gate Rules

- Human gates cannot be auto-approved by the AI Agent
- A transition blocked by a gate cannot continue until the required actor approves it
- Human validation must happen on real outputs, not only on framework correctness

## Feature-First Validation

- Framework work is only valid when it unlocks a testable deliverable
- Each feature cycle should end with a result a human can inspect or test
- After each feature, test the output, observe failures, and refine framework, specs, or tasks only when needed

## V1 Testing Target

- `validated spec`
- `project record`
- `minimal project scaffold`
- human can inspect and test the result
