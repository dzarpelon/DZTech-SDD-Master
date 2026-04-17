# Ideation To Spec Method

## Purpose

Define the minimal method for turning an idea into a validated specification and then into a first testable project output.

## Flow

1. Store the initial concept in `ideation/`
2. Human Operator approves the idea state
3. AI Agent drafts the specification using the framework rules
4. Human Operator validates the specification
5. AI Agent creates the project record from the validated specification
6. AI Agent materializes a minimal project scaffold for inspection and testing
7. Human Operator validates the real output, not only the framework or specification structure

## Required State Sequence

- `idea`
- `approved_idea`
- `spec_draft`
- `validated_spec`

No intermediate state may be skipped.

## V1 Testing Target

The first working feature for v1 is:

- `validated spec`
- `project record`
- `minimal project scaffold`
- human can inspect and test the result
