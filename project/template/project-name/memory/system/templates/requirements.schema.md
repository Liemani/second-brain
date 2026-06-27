---
created: 2026-06-18
status: Draft
related_template: "[requirements.md](requirements.md)"
---

# Requirements Schema

Requirements define what must be true before the work is considered complete.

## Frontmatter Fields

### created (required)

Meaning:

- Creation date.

Format:

- `YYYY-MM-DD`

### status (required)

Meaning:

- Lifecycle state of the requirement.

Allowed values:

- `Draft`
- `Approved`
- `Deprecated`

## Body Sections

### Requirement (required)

Behavior:

- State the requirement plainly.

### Acceptance Criteria (required)

Behavior:

- List the conditions that must be satisfied.

## Conventions

- Describe what must be true, not how to implement it.
- Keep each requirement narrow enough to evaluate.
