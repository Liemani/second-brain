# AGENTS

New AI agents should begin by reading the source documents first.

## Read In Order

1. `README.md`
2. `PRINCIPLES.md`
3. `agents/index.md`
4. `agents/roles/<matching-role>.md`

## Source Of Truth

- `README.md` = what this workspace is and how to navigate it
- `PRINCIPLES.md` = why this workspace is designed this way
- `projects/*` = managed project documents and workspace material
- `procedures/*` = workspace-owned repeatable operations invoked explicitly
- `records/*/*.md` = actual record documents
- `records/*/index.md` = what each record collection does
- `records/*/template.md`, `indexes/template.md`, `procedures/template.md` = local guide docs for their own record, index, or procedure type
- `agents/index.md` = overview of durable agent knowledge
- `agents/roles/*` = long-lived agent role documents
- `agents/playbooks/*` = durable operational knowledge for roles
- When creating a new record or procedure, inspect the local `template.md` first and copy only the template block.

## Role Docs

- Read the role document that matches your assigned role next.
- Role documents define durable responsibilities and boundaries, not session procedures.
- Procedures are not part of ordinary role operating knowledge; consult them only when explicitly requested or referenced.

## Guidelines

- Prefer existing structures over introducing new ones.
- Avoid duplicating information across documents.
- Keep the system minimal.
