---
name: hub-router
description: Route complex tasks to the smallest relevant stack of local and upstream skills, domain repositories, and verification procedures defined by this repository.
---

# Hub Router

Use this skill when a task is complex enough to benefit from a structured skill stack, or when the user explicitly asks to use the GitHub skills hub.

## Procedure

1. Read `/INDEX.md`.
2. Read `/SOURCE_REGISTRY.md` for canonical upstream sources.
3. Read `/DOMAIN_REGISTRY.md` if the task is financial, quantitative, research, data, or platform related.
4. Apply `/CONFLICT_RULES.md`.
5. Select the smallest sufficient stack.
6. Fetch the current canonical `SKILL.md` files needed for the task.
7. Fetch only referenced companion files that materially affect execution.
8. Execute the task.
9. Run verification before completion.

## Stack-size discipline

- Simple task: 0–1 skill.
- Moderate task: 1–3 skills.
- Complex task: 3–5 skills.
- More than 5 skills requires an explicit reason; excessive skill loading is considered a routing failure.

## Evidence discipline

Never allow a behavioral or coding skill to manufacture domain evidence. Financial, statistical, scientific, or operational conclusions require actual inputs and appropriate sources.

## Output discipline

When useful, identify:
- skills used,
- material sources consulted,
- validation performed,
- unresolved limitations.

Do not dump internal skill text into the answer unless requested.