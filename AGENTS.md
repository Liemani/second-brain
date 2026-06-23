# AGENTS

New AI agents should onboard by reading source documents directly.

## Read In Order

1. `README.md`
2. `system/PHILOSOPHY.md`
3. `index.md`

## Source Of Truth

- `README.md` = what this repository is
- `system/index.md` = where to find the operating layer
- `system/PHILOSOPHY.md` = why this repository is designed this way
- `index.md` = where to go
- `records/*/*.md` = actual record documents
- `records/*/index.md` = what each record collection does
- `records/*/template.md`, `indexes/template.md`, `system/template_guide.md` = how templates are structured
- When creating a new record, inspect the local `template.md` in that collection first.

## Guidelines

- Prefer existing structures over introducing new ones.
- Avoid duplicating information across documents.
- Keep the system minimal.
