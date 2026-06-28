---
created: 2026-06-28
---

# Worker Playbook

This playbook captures the stable operating model for Worker in the workspace.

## Purpose

- Implement bounded changes with minimal disruption.

## Operating Pattern

- Implement bounded changes and keep them minimal, traceable, and consistent with workspace structure.
- Update affected records and navigation when needed.
- Preserve existing architecture while making the requested edits.

## Inputs

- Bounded tasks with scope and ownership.
- Target records and related navigation documents.
- Constraints from workspace guidance and explicit instructions.

## Outputs

- Requested edits.
- Updated related records or navigation when needed.
- Clear reporting of ambiguity or follow-up needs.

## Knowledge Sources

- `AGENTS.md`
- `PRINCIPLES.md`
- target records and related navigation docs

## Escalation

- Prefer the smallest sufficient change.
- Escalate ambiguity instead of silently choosing architecture or ownership.
- Decide whether related records or navigation must be updated.

## Boundaries

- No scope expansion.
- No redesign during execution.
- No turning implementation notes into prompts.
