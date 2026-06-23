---
status: <Open / Linked / Archived>
updated: YYYY-MM-DD
related_ideas:
  - "[<idea title>](../ideas/<idea file>)"
related_issues:
  - "[<issue title>](../issues/<issue file>)"
---

# <생각 제목>

<Short role description>

## Notes

- <생각 내용>
- <왜 떠올랐는지>
- <나중에 idea나 issue로 이어질 수 있는지>

---

# Template Guide

## Role

Thoughts are the earliest reusable unit of the knowledge system.

## Frontmatter Fields

### status (required)

Meaning:

- Current state of the thought.

Allowed values:

- `Open`
- `Linked`
- `Archived`

### updated (required)

Meaning:

- Last meaningful update date.

Format:

- `YYYY-MM-DD`

### related_ideas (optional)

Meaning:

- Markdown links to ideas that were derived from this thought.

Applicability:

- Use when the thought becomes more concrete.

Format:

- `"[Idea Title](../ideas/idea_file.md)"`

### related_issues (optional)

Meaning:

- Markdown links to issues that were derived from this thought.

Applicability:

- Use when the thought identifies a problem.

Format:

- `"[Issue Title](../issues/issue_file.md)"`

## Body Sections

### Notes (required)

Behavior:

- Preserve the raw thought first.
- Record why it arose and what it may connect to later.
- Keep the note short enough to revisit.

## Relationships

- `idea` can grow out of a thought when the thought becomes actionable or coherent.
- `issue` can grow out of a thought when the thought identifies a problem.

## Conventions

- Preserve the raw observation or hunch.
- Keep the note short enough to revisit later.
- Promote the thought only when it becomes more specific.
