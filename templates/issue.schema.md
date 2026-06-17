---
created: 2026-06-16
status: Draft
related_template: "[issue.md](issue.md)"
---

# Issue Schema

## Role

Issues hold the problem statement before it becomes a task or a decision.

## Relationships

- `thought` can become an issue when an observation turns into a problem.
- `task` can address an issue.
- `decision` can resolve or redirect an issue.

## Frontmatter Fields

### status (required)

Meaning:

- Current state of the issue record.

Allowed values:

- `Open`
- `Promoted`
- `Closed`
- `Dropped`

### created (required)

Meaning:

- Creation date.

Format:

`YYYY-MM-DD`

### related_tasks (optional)

Meaning:

- Markdown links to tasks that address the issue.

Condition:

- When the issue has a concrete task response.

Format:

- `"[Task Title](../tasks/task_file.md)"`

### related_decisions (optional)

Meaning:

- Markdown links to decisions that resolve or redirect the issue.

Condition:

- When a decision redirects or closes the issue.

Format:

- `"[Decision Title](../decisions/decision_file.md)"`

## Body Sections

### Notes (required)

Behavior:

- State the problem directly.
- Record why it matters and what is known.
- Keep proposed solutions separate until they are chosen.

## Conventions

- Describe the problem first, not the fix.
- Keep the effect on the system visible.
