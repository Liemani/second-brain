---
updated: 2026-06-30
---

# Apply Project Template

Apply a released Project Template artifact to an existing project as an adopted template structure.

## Purpose

- Apply the Project Template Release to an existing project without recreating it.
- Preserve the existing project's source files and git history.
- Keep later workspace or template releases separate unless a deliberate migration happens later.

## When to Use

- When an existing project should adopt the current Project Template Release.
- When the project identity and release scope are ready to be aligned.

## Inputs

- The current Project Template Release artifact, after it has been explicitly released from the current workspace.
- The existing project.
- The project-specific information needed for adoption.

## Preconditions

- Confirm that the Project Template Release reflects the current workspace architecture, conventions, and initialization structure intended for this adoption.
- If the Project Template Release is outdated, explicitly run the `Release Project Template` procedure before continuing.
- Do not apply an outdated Project Template Release to an existing project.

## Procedure

1. Confirm that the Project Template Release has been explicitly released from the current workspace.
2. Inspect the existing project.
3. Identify conflicts between the project and the template.
4. Apply the project template structure to the existing project.
5. Set the project-specific memory and identity.
6. Verify that the existing project remains intact.
7. Confirm that the project now evolves independently.

## Checks

- The procedure applies to an existing project, not a recreated one.
- Existing source files and git history are preserved.
- The Project Template Release is applied as an adopted structure.
- The Project Template Release was not used while outdated relative to the intended workspace release state.
- Later workspace or template releases do not automatically affect the project.

## Output

- An existing project that incorporates the Project Template Release and remains independently owned.
