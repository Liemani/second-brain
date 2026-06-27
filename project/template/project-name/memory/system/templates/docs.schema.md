---
created: 2026-06-18
status: Draft
related_template: "[docs.md](docs.md)"
---

# Docs Schema

Docs capture project-related explanatory material that is useful but not part of the core execution or decision trail.

## Frontmatter Fields

### created (required)

Meaning:

- Creation date.

Format:

- `YYYY-MM-DD`

### status (optional)

Meaning:

- Lifecycle state of the document.

Allowed values:

- `Draft`
- `Stable`
- `Deprecated`

## Body Sections

### Context (required)

Behavior:

- State what the document is for and why it exists.

### Content (required)

Behavior:

- Hold the main explanatory content.

## Conventions

- Keep docs focused on explanation, not execution.
- Prefer one clear purpose per document.
