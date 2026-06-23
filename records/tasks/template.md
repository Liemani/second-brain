---
status: <Now / Backlog / Done / Canceled>
updated: YYYY-MM-DD
related_work_logs:
  - "[<work log title>](../work_logs/<work log file>)"
related_decisions:
  - "[<decision title>](../decisions/<decision file>)"
---

# <작업 제목>

<Short role description>

## Checklist

- [ ] <아직 하지 않은 실행 항목> (YYYY-MM-DD)
- [~] <진행 중인 실행 항목> (YYYY-MM-DD)
- [x] <완료한 실행 항목> (YYYY-MM-DD)
- [-] <취소한 실행 항목> (YYYY-MM-DD)

## Notes

- <작업의 목적>
- <진행 중 참고할 사항>

---

# Template Guide

## Role

The task is the main execution container in the system.

## Frontmatter Fields

### status (required)

Meaning:

- Current state of the task.

Allowed values:

- `Backlog`
- `Now`
- `Done`
- `Canceled`

### updated (required)

Meaning:

- Last meaningful update date.

Format:

- `YYYY-MM-DD`

### related_work_logs (optional)

Meaning:

- Markdown links to work logs that record execution for this task.

Condition:

- When execution has been recorded in a work log.

Format:

- `"[Work Log Title](../work_logs/work_log_file.md)"`

### related_decisions (optional)

Meaning:

- Markdown links to decisions influenced by this task.

Condition:

- When the task leads to or depends on a decision.

Format:

- `"[Decision Title](../decisions/decision_file.md)"`

## Body Sections

### Checklist (required)

Behavior:

- Represent executable actions.
- Progress through checklist states.
- Include a date on each item.
- The date is the item's last status change date.

Allowed states:

- `[ ]`
- `[~]`
- `[x]`
- `[-]`

Checklist items should include dates.

### Notes (optional)

Behavior:

- Record extra context, constraints, or reminders.
- Keep it separate from executable checklist items.

## Relationships

- `idea` can become a task when it is ready for execution.
- `work_log` can record task execution.
- `decision` can be linked when work leads to a stable choice.

## Conventions

- Keep the task narrow enough to execute.
- Put actual execution items in `Checklist`.
- Include dates in checklist items.
