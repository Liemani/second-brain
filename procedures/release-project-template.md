---
updated: 2026-06-30
---

# Release Project Template

Prepare the Project Template Release artifact, currently implemented at `projects/template/`, for new project creation.

## Purpose

- Keep the Project Template Release artifact reusable for starting a new project.
- Compare the workspace with the release artifact to separate source material from released material.
- Keep the release artifact minimal and internally consistent.

## When to Use

- After relevant workspace or template changes that may affect the next project template release.
- Before using the Project Template Release artifact to instantiate a new project.

## Inputs

- The current workspace, including `README.md`, `PRINCIPLES.md`, `AGENTS.md`, `records/`, `agents/`, `procedures/`, `indexes/`, and relevant decisions.
- `projects/template/` as the current implementation location for the release artifact.

## Procedure

1. Inspect the current workspace as the source material for the release.
2. Compare the workspace with the Project Template Release artifact to identify release scope.
3. Determine the approved release scope.
4. Apply only the approved release scope to the release artifact in `projects/template/`.
5. Review the release artifact in `projects/template/`, not as a continuously synchronized mirror.
6. Confirm that the release is ready to instantiate a new project and does not imply changes to already created projects.

## Checks

- The workspace source material and the Project Template Release artifact are clearly distinguished.
- The release artifact reads as a release-ready starter, not as a finished project.
- The release remains an explicit packaging decision, not an automatic synchronization step.
- The release artifact can be used to create a new project without extra cleanup.

## Output

- A reusable Project Template Release artifact ready to instantiate a new project.
