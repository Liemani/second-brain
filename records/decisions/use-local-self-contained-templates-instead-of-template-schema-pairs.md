---
updated: 2026-06-27
---

# Use local self-contained templates instead of template-schema pairs

This record defines the canonical form of template documents in the workspace.

## 결정

Template documents should be local and self-contained. The older template-plus-schema pairing is no longer the preferred form for the workspace.

## 이유

- This extends `Templates` by keeping the template itself responsible for the authoring guidance it needs.
- It extends `Minimal Useful Structure` by removing a redundant split that adds maintenance cost without improving clarity.
- It replaces the older template/schema pattern with a simpler unit that is easier to read, copy, and keep current.

## 영향

- New templates should include their own usage guidance instead of depending on a parallel schema file.
- Indexes can still point to templates, but template placement remains separate from navigation structure.
- Existing or future template families can stay consistent without reintroducing a template/schema split.
