---
updated: 2026-06-30
---

# Procedure Template

이 문서는 workspace가 소유하는, 명시적으로 호출되는 반복 가능한 procedure를 만들 때 복사할 템플릿과 짧은 안내를 제공합니다.

## Template

```md
---
updated: YYYY-MM-DD
---

# <Procedure Title>

<Short purpose>

## Purpose

- <why this procedure exists>

## When to Use

- <trigger>

## Inputs

- <required input>

## Procedure

1. <step>
2. <step>
3. <step>

## Checks

- <verification>

## Output

- <result>
```

## Guide

### What this document is

Procedure documents define repeatable workspace operations that should be easy to invoke and execute by a human or an AI agent.
They are consulted when a human or another procedure explicitly invokes them, not as part of a role's ordinary operating knowledge.

### What this document is not

- A role definition.
- A role playbook.
- Ordinary role operating knowledge.
- A record of what already happened.

### Template fields

- Use `updated` for the last meaningful update date.
- Keep the purpose short and direct.
- Make the procedure executable without extra hidden context.
- Lifecycle procedures are examples of procedures, not the definition of the document type.
