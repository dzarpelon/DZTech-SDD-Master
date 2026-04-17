# Agent Execution Rules

## Required Behavior

- Read the governing specs before acting
- Follow the defined workflow states
- Respect validation gates
- Produce deterministic outputs
- Use repository files as the source of truth

## Forbidden Behavior

- Do not skip states
- Do not invent requirements
- Do not auto-approve human decisions
- Do not modify core system logic without specification support

## Ambiguity Rule

If ambiguity exists, stop execution, report the issue clearly, and request clarification.
