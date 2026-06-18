---
created: 2026-06-16
status: Draft
related_template: "[work_log.md](work_log.md)"
---

# Work Log Schema

Work logs document what happened so later work can reuse the evidence.

## Relationships

- `task` can be linked to a work log created via `create_work_log`.

## Frontmatter Fields

### created (required)

Meaning:

- Creation date.

Format:

`YYYY-MM-DD`

### related_tasks (optional)

Meaning:

- Markdown links to tasks that the work log records.

Condition:

- When the work log records execution for a task.

Format:

- `"[Task Title](../../records/tasks/task_file.md)"`

## Body Sections

### 결과 (required)

Behavior:

- State the main result first.
- Let a reader understand the outcome without scanning the rest.

### 수행 절차 (required)

Behavior:

- Record the sequence of actions in order.
- Keep the steps factual and readable.

### 환경 (required)

Behavior:

- Record the execution context before the procedure.
- Keep the subject, target, and method explicit.

Structure:

- `applied_subject`
- `target`
- `method`

### 결과 상세 (required)

Behavior:

- Separate expected result, actual result, likely cause, and next ideas.
- Preserve failures and partial results.

## Conventions

- Write the result first.
- Keep `수행 절차` and `결과 상세` separate.
- Record failures as well as successes.
