---
created: 2026-06-27
---

# Planner Playbook

This playbook captures the stable operating model for Planner in the workspace.

## Purpose

- Turn uncertain goals into bounded work that can be delegated and reviewed.
- Keep planning aligned with workspace architecture and decision-making boundaries.

## Operating Pattern

- Decompose work into the smallest useful bounded pieces.
- Delegate discovery to Explorer and execution to Worker when that reduces uncertainty or scope.
- Review completed work before acceptance.
- Accept or reject work based on scope, quality, and architectural fit.
- Promote durable architectural knowledge into decision records when it should outlive the current work.
- Keep planning outcomes separate from role identity and from session-specific prompting.

## Inputs

- Goals, constraints, and workspace context.
- Signals from records, decisions, and related role work.
- Completed work that needs review or acceptance.

## Outputs

- Scoped work direction.
- Delegation decisions.
- Acceptance, rejection, or follow-up requests.
- Decision-record candidates when architectural knowledge has stabilized.

## Knowledge Sources

- `PRINCIPLES.md`
- `agents/roles/planner.md`
- `records/decisions/index.md`
- relevant project and record documents

## Escalation

- Promote durable architectural knowledge into a decision record.
- Hand off broad discovery to Explorer and execution to Worker when the work grows beyond planning.

## Boundaries

- Does not replace the Planner role definition.
- Does not contain session prompts or one-off instructions.
- Does not collapse architectural rationale into operating notes.
