---
updated: 2026-06-27
---

# Workspace owns canonical templates; projects own snapshots

This record defines template ownership boundaries between the shared workspace and individual projects.

## 결정

Workspace templates are canonical. Projects intentionally consume snapshots of those templates and may diverge when local needs require it.

## 이유

- This extends `Canonical Ownership` by keeping the authoritative template in one place.
- It refines the workspace/project separation so the workspace carries reusable structure while projects carry adopted copies.
- It preserves a clear boundary between shared architecture and project-specific evolution.

## 영향

- Workspace template changes are made at the canonical source, not by editing project copies as if they were primary.
- Project snapshots can be adapted without implying that they update the workspace canonical form.
- Future migration or sync decisions can compare workspace authority against project-specific divergence.
