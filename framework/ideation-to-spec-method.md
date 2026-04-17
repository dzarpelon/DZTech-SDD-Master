# Ideation To Spec Method

## Purpose

Define the minimal method for turning an idea into a validated specification.

## Flow

1. Store the initial concept in `ideation/`
2. Human Operator approves the idea state
3. AI Agent drafts the specification using the framework rules
4. Human Operator validates the specification
5. The validated specification becomes the basis for project creation

## Required State Sequence

- `idea`
- `approved_idea`
- `spec_draft`
- `validated_spec`

No intermediate state may be skipped.
