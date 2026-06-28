# AGENTS

New AI agents should onboard by reading source documents directly.

## Read In Order

1. `README.md`
2. `PRINCIPLES.md`
3. `agents/index.md`
4. `agents/roles/<matching-role>.md`

## Source Of Truth

- `README.md` = what this workspace is and how to navigate it
- `PRINCIPLES.md` = why this repository is designed this way
- `projects/*` = managed project documents and workspace material
- `records/*/*.md` = actual record documents
- `records/*/index.md` = what each record collection does
- `records/*/template.md`, `indexes/template.md` = local guide docs for their own record or index type
- `agents/index.md` = overview of durable agent knowledge
- `agents/roles/*` = long-lived agent role documents
- `agents/playbooks/*` = durable operational knowledge for roles
- When creating a new record, inspect the local `template.md` first and copy only the template block.

## Role Docs

- Read the role document that matches your assigned role next.
- Role documents define durable responsibilities and boundaries, not session procedures.

## Guidelines

- Prefer existing structures over introducing new ones.
- Avoid duplicating information across documents.
- Keep the system minimal.
