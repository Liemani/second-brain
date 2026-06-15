# Handover

This repository is a second brain. The current structure is role-based, not stage-based.

## Current Layout

- `README.md`: short repository overview.
- `index.md`: main entry point for the whole second brain.
- `areas/`: subject or project areas, each with its own `index.md` when needed.
- `dreams/`: dream diary documents.
- `thoughts/`: free-form thoughts.
- `ideas/`: ideas that are not yet tasks.
- `issues/`: unresolved problems or friction.
- `tasks/`: task documents; each task uses an internal checklist for execution items.
- `work_logs/`: execution records and outcomes.
- `decisions/`: decisions made after attempts or analysis.
- `indexes/`: thematic cross-cutting indexes, such as `indexes/ai.md`.
- `legacy/`: old material and previously reorganized content.
- `templates/`: reusable templates for the document types above.

## Key Conventions

- `task` is the main work unit.
- `todo` files were removed; task checklists now hold execution items.
- `indexes/` is not tied to a single document type. Any item type can appear there.
- Item documents use a `Meta` block near the top for status, dates, and links.
- `task` checklist items include a date in parentheses.
- `areas/` is separate from the operational docs. It is for domain/project material.

## Important Files

- [index.md](index.md)
- [rules.md](rules.md)
- [dreams/index.md](dreams/index.md)
- [indexes/index.md](indexes/index.md)
- [indexes/ai.md](indexes/ai.md)
- [areas/index.md](areas/index.md)
- [tasks/index.md](tasks/index.md)
- [ideas/index.md](ideas/index.md)
- [thoughts/index.md](thoughts/index.md)
- [decisions/index.md](decisions/index.md)
- [work_logs/index.md](work_logs/index.md)
- [templates/index.md](templates/index.md)
- [templates/dream.md](templates/dream.md)

## Recent State

- `workflow/`, `0_inbox/`, `1_active/`, `2_stable/`, and `3_archive/` are no longer the active structure.
- `todo` documents were removed in favor of task checklists.
- `develop_custom_ai.md` was removed as a separate task and absorbed into `ideas/custom_ai.md`.
- `indexes/ai.md` currently indexes AI-related thoughts and ideas.
- `dreams/` was added as a separate document type, distinct from `thoughts/`.
- Item documents across `tasks/`, `thoughts/`, `ideas/`, `issues/`, `dreams/`, `decisions/`, and `work_logs/` now use a shared `Meta` block style.

## Notes For The Next Agent

- Keep `index.md` as the top-level entry point for the entire second brain.
- When adding a new thematic index, place it in `indexes/` and link the relevant items both ways when useful.
- Use `apply_patch` for edits.
- There is a lingering Vim swap file in `tasks/.modify_haven_and_hearth_client.md.swp`; it is safe to ignore or delete if needed.
