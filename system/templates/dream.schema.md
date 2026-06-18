---
created: 2026-06-16
status: Draft
related_template: "[dream.md](dream.md)"
---

# Dream Schema

Dreams are separate from thoughts and act as a dedicated capture surface for sleep narratives.

## Relationships

- `thought` can be linked when a dream leads to interpretation.
- `idea` can be linked when a dream suggests a useful direction or concept.

## Frontmatter Fields

### created (required)

Meaning:

- Creation date.

Format:

`YYYY-MM-DD`

### related_thoughts (optional)

Meaning:

- Markdown links to related thoughts or interpretations.

Condition:

- When the dream leads to interpretation.

Format:

- `"[Thought Title](../thoughts/thought_file.md)"`

### related_ideas (optional)

Meaning:

- Markdown links to ideas suggested by the dream.

Condition:

- When the dream suggests a useful direction.

Format:

- `"[Idea Title](../ideas/idea_file.md)"`

## Body Sections

### Notes (required)

Behavior:

- Record raw dream content first.
- Preserve remembered scenes, feelings, and sequence.
- Keep interpretation separate if added later.

## Conventions

- Record the dream as soon as possible after waking.
- Keep the sequence of events, scenes, and emotions intact.
- Separate interpretation from raw recall.
