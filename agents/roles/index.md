---
created: 2026-06-27
---

# Roles

이 문서는 `agents/roles/`에 있는 장기적으로 유지되는 AI 역할 문서의 진입점입니다.

## Purpose

Role documents define durable responsibilities, authority, inputs, outputs, knowledge sources, and boundaries.
They describe how a role fits into the workspace.

## Documents

- [template](template.md): canonical self-contained role template
- [external-design-partner](external-design-partner.md): external architectural collaborator
- [planner](planner.md): defines planning responsibility and decision-shaping scope
- [explorer](explorer.md): defines discovery and context-gathering responsibility
- [worker](worker.md): defines implementation and record-updating responsibility

## Boundaries

- Do not use role documents as a place for one-off session instructions.
- Do not use role documents for operational practice.
- Keep operational prompting in the agent bootstrap flow.
- Keep architectural decisions in decision records.
