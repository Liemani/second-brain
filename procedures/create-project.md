---
updated: 2026-06-30
---

# Create Project

Create a new project as the one-time transition from a released Project Template artifact to an independent project. If no suitable release exists, invoke `Release Project Template` first and continue from the resulting artifact.

## Purpose

- Turn a released Project Template artifact into a new project.
- Establish the project as independent from the moment it is created.
- Keep later workspace or template releases separate from the created project unless a deliberate migration happens later.
- Depend on `Release Project Template` for the release artifact that creation consumes.

## When to Use

- When a new project should begin from a released Project Template artifact.
- When no suitable release artifact exists yet and the release procedure must run first.
- When the project identity and destination are ready to be established.

## Inputs

- The selected Project Template Release artifact.
- Whether a suitable Project Template Release artifact already exists.
- The destination for the new project.
- The project identity and any project-specific starting information.

## Procedure

1. Check whether a suitable Project Template Release artifact already exists.
2. If no suitable release exists, invoke `Release Project Template` and wait for the resulting artifact.
3. Select the Project Template Release artifact.
4. Choose the destination and project identity.
5. Instantiate the new project from the release artifact.
6. Initialize project-specific information.
7. Verify the project is ready for independent evolution.

## Checks

- The new project begins from a released Project Template artifact.
- The release artifact is a prerequisite, not an optional shortcut.
- Project creation is treated as a one-time lifecycle transition.
- The new project is independent immediately after creation.
- Later workspace or template releases do not automatically affect the project.

## Output

- A new independent project ready for later work.
