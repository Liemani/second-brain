---
status: <Open / Promoted / Closed / Dropped>
updated: YYYY-MM-DD
---

# <이슈 제목>

<Short role description>

## Notes

- <무슨 문제인지>
- <왜 문제인지>
- <영향 범위 또는 불편>
- <task로 올릴 조건 또는 해결 방향>

---

# Template Guide

## Role

Issues hold the problem statement before it becomes a task or a decision.

## Frontmatter Fields

### status (required)

Meaning:

- Current state of the issue.

Allowed values:

- `Open`
- `Promoted`
- `Closed`
- `Dropped`

### updated (required)

Meaning:

- Last meaningful update date.

Format:

- `YYYY-MM-DD`

## Body Sections

### Notes (required)

Behavior:

- State the problem directly.
- Record why it matters and what is known.
- Keep proposed solutions separate until they are chosen.

## Relationships

- `thought` can become an issue when an observation turns into a problem.

## Conventions

- Describe the problem first, not the fix.
- Keep the effect on the system visible.
