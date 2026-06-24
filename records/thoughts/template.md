---
updated: 2026-06-24
---

# Thought Template

This document contains a copyable template and guidance for creating thought records.
Copy only the fenced block under `## Template` when creating a new record.

## Template

```md
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
```

## Guide

### What this record is

Thought records capture early observations, hunches, and problem signals before they become ideas or issues.

### Important fields

#### status

- Current state of the thought.

Allowed values:

- `Open`
- `Linked`
- `Archived`

#### updated

- Last meaningful update date. Use `YYYY-MM-DD`.

#### related_ideas

- Link ideas that came from this thought when useful.

#### related_issues

- Link issues that came from this thought when useful.

### Notes

- Preserve the raw thought first.
- Record why it arose and what it may connect to later.
- Keep the note short enough to revisit.

### Links

- `idea` can grow out of a thought when the thought becomes actionable or coherent.
- `issue` can grow out of a thought when the thought identifies a problem.
