---
created: 2026-06-16
status: Draft
related_template: "[thought.md](thought.md)"
---

# Thought Schema

## Role

Thoughts are the earliest reusable unit of the knowledge system.

## Relationships

- `idea` can grow out of a thought when the thought becomes actionable or coherent.
- `issue` can grow out of a thought when the thought identifies a problem.

## Frontmatter Fields

### status (required)

Meaning:

- Current state of the thought record.

Allowed values:

- `Open`
- `Linked`
- `Archived`

### created (required)

Meaning:

- Creation date.

Format:

`YYYY-MM-DD`

### related_ideas (optional)

Meaning:

- Markdown links to ideas that were derived from this thought.

Condition:

- When the thought becomes more concrete.

Format:

- `"[Idea Title](../ideas/idea_file.md)"`

### related_issues (optional)

Meaning:

- Markdown links to issues that were derived from this thought.

Condition:

- When the thought identifies a problem.

Format:

- `"[Issue Title](../issues/issue_file.md)"`

## Body Sections

### Notes (required)

Behavior:

- Preserve the raw thought first.
- Record why it arose and what it may connect to later.
- Keep the note short enough to revisit.

## Conventions

- Preserve the raw observation or hunch.
- Keep the note short enough to revisit later.
- Promote the thought only when it becomes more specific.
