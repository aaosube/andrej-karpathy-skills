# Skills Routing Index

Use this file as the first routing layer. Select the smallest sufficient stack; do not load every source.

## 1. Software development / platform building

### New system, feature, or major redesign
1. `obra/superpowers` → `brainstorming`
2. `obra/superpowers` → `writing-plans`
3. `obra/superpowers` → `test-driven-development`
4. `obra/superpowers` → `requesting-code-review`
5. `obra/superpowers` → `verification-before-completion`

### Existing implementation plan
- `obra/superpowers` → `executing-plans`
- For separable work: `dispatching-parallel-agents`
- For task-by-task agent execution: `subagent-driven-development`

### Bug / unexplained failure
1. `obra/superpowers` → `systematic-debugging`
2. `obra/superpowers` → `test-driven-development`
3. `obra/superpowers` → `verification-before-completion`

### Code review / review response
- `requesting-code-review`
- `receiving-code-review`

### Git isolation / branch completion
- `using-git-worktrees`
- `finishing-a-development-branch`

### Creating or improving a skill
- `writing-skills`
- local Karpathy guidelines as behavioral constraint

## 2. Skill discovery and agent architecture

### Find a specialized existing skill
Search `github/awesome-copilot` first, especially its Agent Skills catalog.

### Evaluate / assemble a skill stack
Prefer `github/awesome-copilot` → `agent-skill-stack` when relevant.

### Agent evaluation / governance / security
Look in `github/awesome-copilot` for:
- `agentic-eval`
- `agent-governance`
- `agent-owasp-compliance`
- `agent-supply-chain`

### Plugin / Codex-compatible packaging
Use `openai/plugins` as the structural reference for plugin manifests, skills, agents, commands, hooks, assets, and MCP configuration.

## 3. Baseline behavioral rules

Use the local `skills/karpathy-guidelines/SKILL.md` for:
- surfacing assumptions,
- simplicity,
- surgical changes,
- goal-driven execution,
- avoiding speculative complexity.

These rules supplement domain methods; they do not replace them.

## 4. Research / quantitative / finance work

Consult `DOMAIN_REGISTRY.md` to identify relevant user-owned repositories. Do not infer a repository's correctness from its name. Inspect its current documentation/code/data before use.

Default analytical sequence:
1. Define the question and success criteria.
2. Identify required observed inputs.
3. Validate data integrity and timestamps.
4. Retrieve domain-specific references/code.
5. Apply statistical/quantitative method.
6. Run adversarial/alternative explanation check.
7. Report uncertainty and invalidation conditions.
8. Verify calculations/results.

## 5. Conflict handling

Always apply `CONFLICT_RULES.md`.

## 6. Source locations

Canonical repositories and paths are defined in `SOURCE_REGISTRY.md`.