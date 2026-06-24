# AGENTS

New AI agents should onboard by reading source documents directly.

## Read In Order

1. `README.md`
2. `PHILOSOPHY.md`
3. `index.md`

## Source Of Truth

- `README.md` = what this repository is
- `PHILOSOPHY.md` = why this repository is designed this way
- `index.md` = where to go
- `records/*/*.md` = actual record documents
- `records/*/index.md` = what each record collection does
- `records/*/template.md`, `indexes/template.md` = local guide docs for their own record or index type
- When creating a new record, inspect the local `template.md` first and copy only the template block.

## Guidelines

- Prefer existing structures over introducing new ones.
- Avoid duplicating information across documents.
- Keep the system minimal.
