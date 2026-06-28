---
created: 2026-06-27
---

# Role Template

This document contains a copyable template and guidance for creating long-lived role documents.
Copy only the fenced block under `## Template` when creating a new role document.

## Template

```md
---
created: YYYY-MM-DD
---

# <Role Name>

<One-line role summary>

## Purpose

- <purpose>

## Responsibilities

- <responsibility>

## Authority

- <authority>

## Expected Inputs

- <input>

## Expected Outputs

- <output>

## Knowledge Sources

- <source>

## Boundaries

- <boundary>
```

## Guide

### What this document is

Role documents define long-lived responsibilities for a durable workspace role.

### What this document is not

- A workflow.
- A session prompt.
- A place for operational behavior.
- A place to restate architectural rationale.

### Operational and architectural separation

- Operational behavior belongs in prompts.
- Architectural rationale belongs in decision records.
- Role docs should stay focused on stable responsibilities and boundaries.

### Template fields

- Use `created` for the document creation date.
- Keep the summary short and declarative.
- Use the sections in the template as the stable role shape.
