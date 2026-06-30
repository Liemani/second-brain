---
updated: 2026-06-28
---

# Workspace, project templates, and projects evolve on separate lifecycles

This decision defines how workspace evolution relates to project creation and project stability.

## 결정

The workspace evolves continuously. Project templates are intentional releases of a canonical snapshot of the workspace's current architecture, conventions, and initialization structure. Projects are created from those snapshots and then diverge independently. Existing projects are never implicitly updated from later template changes, and any project migration or adoption is always an explicit architectural decision.

## 이유

- Project stability should be preserved after creation.
- Workspace improvement should not force downstream change.
- Ownership boundaries stay clear when the workspace, templates, and projects evolve by different rules.

## 영향

- The workspace, project templates, and projects evolve at different rates.
- Project templates package stable canonical starting points for new projects.
- Migration or adoption decisions remain explicit.
- This complements `PRINCIPLES.md` and extends `workspace owns canonical templates; projects own snapshots`.
