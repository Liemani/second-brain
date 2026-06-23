---
updated: YYYY-MM-DD
related_tasks:
  - "[<task title>](../tasks/<task file>)"
---

# <작업 기록 제목>

<Short role description>

## 결과

<가장 핵심적인 결과 한 줄>

## 환경

- 적용 대상: <예: 서버 `hermes` 계정>
- 대상: <예: 조직, 계정, 시스템, 서비스>
- 방식: <예: 인증 방식, 적용 방식>

## 수행 절차

### 1. <첫 번째 단계>

1. <실행 순서>
2. <실행 순서>
3. <실행 순서>

### 2. <두 번째 단계>

1. <실행 순서>
2. <실행 순서>
3. <실행 순서>

## 결과 상세

- 기대한 결과: <무엇을 기대했는지>
- 실제 결과: <실제로 어떻게 되었는지>
- 문제 또는 실패 원인 후보: <확인된 문제나 추정 원인>
- 다음 시도 아이디어: <다음에 무엇을 바꿔볼지>

---

# Template Guide

## Role

Work logs document what happened so later work can reuse the evidence.

## Frontmatter Fields

### updated (required)

Meaning:

- Last meaningful update date.

Format:

- `YYYY-MM-DD`

### related_tasks (optional)

Meaning:

- Markdown links to tasks that the work log records.

Applicability:

- Use when the work log records execution for a task.

Format:

- `"[Task Title](../tasks/task_file.md)"`

## Body Sections

### 결과 (required)

Behavior:

- State the main result first.
- Let a reader understand the outcome without scanning the rest.

### 환경 (required)

Behavior:

- Record the execution context before the procedure.
- Keep the subject, target, and method explicit.

Structure:

- `applied_subject`
- `target`
- `method`

### 수행 절차 (required)

Behavior:

- Record the sequence of actions in order.
- Keep the steps factual and readable.

### 결과 상세 (required)

Behavior:

- Separate expected result, actual result, likely cause, and next ideas.
- Preserve failures and partial results.

## Relationships

- `task` can be linked to a work log when task execution is recorded.

## Conventions

- Write the result first.
- Keep `수행 절차` and `결과 상세` separate.
- Record failures as well as successes.
