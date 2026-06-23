---
updated: YYYY-MM-DD
---

# <결정 제목>

<Short role description>

## 결정

<무엇을 결정했는지>

## 이유

- <왜 이런 결정을 내렸는지>
- <어떤 판단 근거가 있었는지>

## 영향

- <이 결정이 이후 작업에 주는 영향>
- <무엇이 바뀌는지>

---

# Template Guide

## Role

Decisions capture the stable outcome of reasoning so later work can follow the chosen direction.

## Frontmatter Fields

### updated (required)

Meaning:

- Last meaningful update date.

Format:

- `YYYY-MM-DD`

## Body Sections

### 결정 (required)

Behavior:

- State what was decided.
- Keep the decision separate from the reasoning.

### 이유 (required)

Behavior:

- Record the evidence, reasoning, or comparison that led to the decision.
- Keep it separate from the decision itself.

### 영향 (optional)

Behavior:

- Describe what changes because of this decision.
- Record downstream consequences or constraints.

## Relationships

- `work_log` can provide the evidence that led to a decision.

## Conventions

- State the decision plainly in the `결정` section.
- Link to the work log that motivated the choice when possible.
- Keep the reason and impact separate from the decision itself.

## Notes

- Do not turn this into a generic analysis note.
