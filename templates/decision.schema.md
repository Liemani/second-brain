---
created: 2026-06-16
status: Draft
related_template: "[decision.md](decision.md)"
---

# Decision Schema

## Role

Decisions capture the stable outcome of reasoning so later work can follow the chosen direction.

## Relationships

- `work_log` can provide the evidence behind a decision.
- `task` can reference a decision when execution should follow a chosen direction.

## Frontmatter Fields

### created (required)

Meaning:

- Creation date.

Format:

`YYYY-MM-DD`

### related_work_logs (optional)

Meaning:

- Markdown links to work logs that support the decision.

Condition:

- When evidence exists in work logs.

Format:

- `"[Work Log Title](../work_logs/work_log_file.md)"`

### related_tasks (optional)

Meaning:

- Markdown links to tasks that follow from the decision.

Condition:

- When execution follows from the decision.

Format:

- `"[Task Title](../tasks/task_file.md)"`

## Body Sections

### 결정 (required)

Behavior:

- State what was decided.
- Keep the decision separate from the reasoning.

### 이유 (required)

Behavior:

- Record the evidence, reasoning, or comparison that led to the decision.
- Keep it separate from the decision itself.

### 영향 (optional)

Behavior:

- Describe what changes because of this decision.
- Record downstream consequences or constraints.

## Extensible Fields

- tags
- source

## Conventions

- State the decision plainly in the `결정` section.
- Link to the work log that motivated the choice when possible.
- Keep the reason and impact separate from the decision itself.

## Notes

- Do not turn this into a generic analysis note.
