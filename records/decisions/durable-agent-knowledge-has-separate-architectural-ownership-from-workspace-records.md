---
updated: 2026-06-28
---

# Durable agent knowledge has separate architectural ownership from workspace records

This decision defines where durable agent knowledge belongs in the architecture.

## 결정

Durable agent knowledge has its own architectural ownership, separate from workspace records.
Roles and playbooks belong together as agent knowledge because roles define durable responsibility boundaries and playbooks define durable operating practices.

## 이유

- Workspace records had been carrying both workspace memory and durable agent knowledge.
- Roles and playbooks serve different responsibilities than workspace records.
- Prompt reduction and repeatable onboarding require durable agent knowledge to have a clear home of its own.

## 영향

- Workspace memory remains separate from agent knowledge.
- Onboarding can recover more durable knowledge from the workspace.
- Prompts can stay narrower and more session-specific.
- Future agent-specific knowledge has a clear architectural owner.
- This complements `PRINCIPLES.md` and aligns with the decisions on canonical templates and self-contained templates.
