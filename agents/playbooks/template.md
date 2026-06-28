---
created: 2026-06-27
---

# Playbook Template

This document contains a copyable template and guidance for creating durable operational playbooks.
Copy only the fenced block under `## Template` when creating a new playbook document.

## Template

```md
---
created: YYYY-MM-DD
---

# <Playbook Title>

<One-line summary>

## Operating Pattern

- <stable practice>

## Inputs

- <signal or condition>

## Outputs

- <resulting artifact or decision>

## Escalation

- <when this should become a role or decision concern>

## Knowledge Sources

- <source>

## Boundaries

- <boundary>
```

## Guide

### What this document is

Playbooks define durable operational knowledge for a role.

### What this document is not

- A role definition.
- A workflow.
- A session prompt.
- A place for architectural rationale.

### Operational and architectural separation

- Durable operational patterns belong in playbooks.
- Session-specific instructions belong in prompts.
- Architectural rationale belongs in decision records.
- Role identity belongs in role documents.

### Template fields

- Use `created` for the document creation date.
- Keep the summary short and declarative.
- Describe the stable operating pattern, not a one-time procedure.
