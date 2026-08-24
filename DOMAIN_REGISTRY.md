# Domain Repository Registry

This registry connects the skills hub to user-owned domain repositories. These repositories are sources of skills, code, research patterns, and examples. They are not automatically trusted as current market truth.

## Tier A — Directly useful skill / agent sources

### aaosube/finance-skills
Role: primary financial Agent Skills library.

Use for:
- company valuation,
- earnings analysis,
- estimate analysis,
- ETF premium/discount analysis,
- options payoff analysis,
- stock correlation,
- stock liquidity,
- financial data-provider patterns,
- TradingView read-only integration patterns,
- creating and evaluating finance skills.

Important rule: fetch the specific `SKILL.md` under `plugins/*/skills/*` required by the task; do not load the whole repository.

### aaosube/tradingagents
Role: multi-agent financial research architecture reference.

Use for:
- analyst/researcher/trader/risk-manager decomposition,
- bull vs bear structured debate,
- portfolio-manager gating,
- persistent decision logs and reflection patterns,
- checkpoint/resume design,
- data-access contracts and multi-provider architecture.

Do not use its generated trade decision as evidence by itself.

## Tier A — Quant research infrastructure

### aaosube/qlib
Role: quantitative research, ML pipeline, backtesting, factor research, market-dynamics modeling, portfolio optimization, and execution architecture.

Use for:
- data processing pipelines,
- factor/model research,
- supervised learning workflows,
- concept drift / market dynamics,
- reinforcement-learning research,
- backtesting architecture,
- high-frequency examples,
- portfolio and execution research.

### aaosube/rd-agent
Role: autonomous R&D / data-science / quant-research workflow reference.

Use for:
- iterative research loops,
- factor mining,
- factor–model co-optimization,
- data-centric quant research,
- automatic experiment generation and evaluation,
- research/development agent separation,
- benchmark-driven agent evaluation.

Treat performance claims as claims requiring independent verification before adoption.

## Tier B — Specialized financial/AI repositories

The following repositories are available and potentially useful. Inspect current documentation/code before routing a task to them:

### aaosube/FinGPT
Potential role: financial LLM/NLP patterns, financial language-model research.

### aaosube/FinRL
Potential role: reinforcement-learning trading research and environments.

### aaosube/finrobot
Potential role: financial agent architecture and research automation.

### aaosube/openbb
Potential role: financial data/platform architecture and provider integration patterns.

### aaosube/quantdataapi_sdk
Potential role: QuantData SDK/API integration reference where applicable.

### aaosube/vibe-trading
Potential role: trading application/platform patterns; inspect before use.

## Tier C — Supporting repositories

### aaosube/playwright-mcp
Potential role: browser automation / MCP patterns when a workflow requires controlled browser interaction.

### aaosube/books
Potential role: user-curated reading/reference repository. Use only after identifying the exact relevant file and respecting source/copyright constraints.

## Routing rules

### Financial analysis skill needed
1. Check `aaosube/finance-skills` for a specific Agent Skill.
2. If the task needs multi-agent decomposition, inspect `aaosube/tradingagents`.
3. If it requires model/factor/backtest research, inspect `aaosube/qlib` and/or `aaosube/rd-agent`.
4. Use Tier B only when its specialization materially improves the task.

### Quantitative experiment / forecasting research
1. Define observed inputs and target variable.
2. Use `qlib` for experiment/backtesting architecture.
3. Use `rd-agent` for iterative R&D loops where useful.
4. Use `finance-skills` for narrowly scoped financial skills.
5. Verify against leakage, look-ahead bias, timestamp errors, survivorship bias, overfitting, and unsupported causal claims.

## Trust policy

- Repository ownership does not establish empirical validity.
- README claims are hypotheses until supported by code, tests, data, or external evidence.
- Market data must come from the actual requested/current data source, not from repository examples.
- Never present simulation/backtest output as live market observation.