---
created: 2026-06-16
related_template: "[index.md](index.md)"
---

# Index Schema

## Role

Index documents group content under a shared perspective.

## Relationships

- An index may group any document type when it supports the perspective.
- An index may point back to grouped documents when bidirectional linking is useful.

## Frontmatter Fields

### created (required)

Meaning:

- Creation date.

Applicability:

- Use for every index document.

Format:

- `YYYY-MM-DD`

### scope (optional)

Meaning:

- A short summary of the perspective or boundary that the index covers.

Applicability:

- Use when the title alone does not make the perspective clear.

Format:

- Short description.

### owner (optional)

Meaning:

- Human or AI responsible for maintaining the index.

Applicability:

- Use when ownership improves coordination or upkeep.

Format:

- Short name, handle, or agent label.

## Body Sections

### <Perspective or topic> (repeatable)

Behavior:

- Group documents under a shared perspective.
- Choose section names that match the perspective.
- Link directly to the source documents.
- Mix document types when that makes the grouping useful.

## Extensible Fields

- tags

## Conventions

- Keep indexes focused on a clear perspective or boundary.
- Let the section names carry the meaning of the grouping.
- Do not treat an index as a substitute for the source documents.
- Add links only when the grouping is useful.
- Avoid hardcoded object-type buckets.

## Notes

- Index documents are perspective-based navigation objects.
