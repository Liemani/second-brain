---
updated: YYYY-MM-DD
related_template: "[<template file>](<template file>)"
status: <Draft / Stable / Deprecated>
---

# <Template Name> Template Guide

<Short role description>

## Relationships

- <how this template relates to other templates>

## Frontmatter Fields

### <field name> (required)

Meaning:

- <meaning>

Applicability:

- <when it should be used>

Format:

- <format>

### <field name> (optional)

Meaning:

- <meaning>

Applicability:

- <when it should be used>

Format:

- <format>

## Body Sections

### <section name> (required)

Behavior:

- <what this section does>
- <how it should behave>

### <section name> (optional)

Behavior:

- <what this section does>
- <how it should behave>

## Conventions

- Keep frontmatter fields explicit and template-specific.
- Keep body sections separate from frontmatter fields.
- Use this template to define how a template guide should be written.

## Notes

- <additional considerations>

---

# Template Guide

## Role

Template guides describe how templates should be written and interpreted.

## Frontmatter Fields

### updated (required)

Meaning:

- Last meaningful update date.

Applicability:

- Use for template guides that need update traceability.

Format:

- `YYYY-MM-DD`

### related_template (required)

Meaning:

- The template this guide describes.

Applicability:

- Use on template guides tied to a specific template.

Format:

- Relative link to the related template file.

### status (optional)

Meaning:

- Lifecycle state of the template guide.

Applicability:

- Use when the guide itself needs to track review or maturity.

Allowed values:

- `Draft`
- `Stable`
- `Deprecated`

## Body Sections

### Relationships (required)

Behavior:

- Describe how this template relates to other templates.

### Frontmatter Fields (required)

Behavior:

- Define the frontmatter fields that belong to the related template.
- Keep the definitions explicit and template-specific.

### Body Sections (required)

Behavior:

- Define the markdown body sections that belong to the related template.
- Describe how each section should be used.

### Conventions (optional)

Behavior:

- State writing conventions that make the guide easier to use consistently.

### Notes (optional)

Behavior:

- Record additional considerations, cautions, or implementation notes.

## Conventions

- Keep the guide specific to the related template.
- Do not treat this file as inherited defaults for every template.
- `updated`, `related_template`, and `status` are common template-guide fields, not automatic template fields.
- Update `updated` whenever the file changes.

## Notes

- Template guides are templates for writing template guides.
