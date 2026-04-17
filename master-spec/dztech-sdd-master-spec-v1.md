# DZTech SDD Master — Core Specification

## Identity
Name: DZTech SDD Master  
Type: Central Spec-Driven Development Repository  

## Objective
Provide a single source of truth for AI-first Spec-Driven Development.

## Actors
- Human Operator (final authority)
- AI Agent (executor)
- Orchestrator (n8n)
- GitHub (execution environment)

## Principles
- Spec-first
- Human final authority
- No assumptions
- Fast functional delivery
- Centralized method, distributed execution
- Upgrade by decision, not drift

## Core Flow
Idea → Approved Idea → Spec → Validated Spec → Project → Execution → Validation

## Responsibilities

### Human Operator
- Approves ideas
- Approves specs
- Validates product output

### AI Agent
- Generates specs
- Decomposes tasks
- Executes within defined constraints

### Orchestrator
- Moves workflow states
- Triggers automations

## Versioning
Framework versioned as a single unit (v1.0.0 initial)

## Outcome
System capable of generating structured project repositories from validated specs