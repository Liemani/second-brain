# Handover

This repository is a second brain. The current structure is role-based, not stage-based.

## Current Layout

- `README.md`: short repository overview.
- `index.md`: main entry point for the whole second brain.
- `protocols/`: shared action protocols for humans and AI.
- `areas/`: subject or project areas, each with its own `index.md` when needed.
- `dreams/`: dream diary documents.
- `thoughts/`: free-form thoughts.
- `ideas/`: ideas that are not yet tasks.
- `issues/`: unresolved problems or friction.
- `tasks/`: task documents; each task uses an internal checklist for execution items.
- `work_logs/`: execution records and outcomes.
- `decisions/`: decisions made after attempts or analysis.
- `indexes/`: perspective-based indexes, such as `indexes/ai.md`.
- `legacy/`: old material and previously reorganized content.
- `templates/`: reusable templates and template schemas for the document types above.

## Key Conventions

- `task` is the main work unit.
- `todo` files were removed; task checklists now hold execution items.
- `indexes/` is not tied to a single document type. Any document type can appear there when the perspective fits.
- Item documents use YAML frontmatter near the top for dates, links, and lifecycle fields when needed.
- `task` checklist items include a date in parentheses.
- `areas/` is separate from the operational docs. It is for domain/project material.
- `templates/*.schema.md` describe how templates should be interpreted and evolved through fields and sections.

## Important Files

- [index.md](index.md)
- [rules.md](rules.md)
- [dreams/index.md](dreams/index.md)
- [protocols/README.md](protocols/README.md)
- [protocols/index.md](protocols/index.md)
- [protocols/template.md](protocols/template.md)
- [indexes/index.md](indexes/index.md)
- [indexes/ai.md](indexes/ai.md)
- [areas/index.md](areas/index.md)
- [tasks/index.md](tasks/index.md)
- [ideas/index.md](ideas/index.md)
- [thoughts/index.md](thoughts/index.md)
- [decisions/index.md](decisions/index.md)
- [work_logs/index.md](work_logs/index.md)
- [templates/index.md](templates/index.md)
- [templates/index.schema.md](templates/index.schema.md)
- [templates/schema.md](templates/schema.md)
- [templates/schema.schema.md](templates/schema.schema.md)
- [templates/dream.md](templates/dream.md)

## Recent State

- `workflow/`, `0_inbox/`, `1_active/`, `2_stable/`, and `3_archive/` are no longer the active structure.
- `todo` documents were removed in favor of task checklists.
- `develop_custom_ai.md` was removed as a separate task and absorbed into `ideas/custom_ai.md`.
- `indexes/ai.md` currently groups AI-related content under a shared perspective.
- `dreams/` was added as a separate document type, distinct from `thoughts/`.
- Item documents across `tasks/`, `thoughts/`, `ideas/`, `issues/`, `dreams/`, `decisions/`, `work_logs/`, and `indexes/` now use shared YAML frontmatter.
- `protocols/` was added as a shared action layer between objects and rules.
- `templates/index.md` is now also used as the template for index objects.
- `templates/index.schema.md` describes how `templates/index.md` should be written.
- `schema.md` is the reusable template for schema documents.
- `schema.schema.md` describes how `schema.md` should be written.
- `templates/*.schema.md` describe how templates should be interpreted and evolved through fields and sections.

## Notes For The Next Agent

- Keep `index.md` as the top-level entry point for the entire second brain.
- When adding a new perspective-based index, place it in `indexes/` and link the relevant items both ways when useful.
- Use `apply_patch` for edits.
- There is a lingering Vim swap file in `tasks/.modify_haven_and_hearth_client.md.swp`; it is safe to ignore or delete if needed.
