# kline-structure-chart（stock-skill）

**Tags:** finance, kline, research, python, skill
**Source:** [@Chengpengo45c](https://x.com/Chengpengo45c/status/2114549709482393888) · 2026-10-26
**Engagement:** 2 likes / 1 reply (discovery post; repo ~1★, strong docs/demos)

## When to use
When the user asks an agent to **analyze A-share / HK / US stock K-line structure** with real data—support/resistance, triple-barrier risk plan, 15-day normal volatility range, no-lookahead backtest—and wants JSON + PNG + offline HTML, **not** LLM chart-reading or buy tips. Research only, not investment advice.

## What it does
Agent Skills–compatible package `kline-structure-chart`: Python computes structure and risk from real OHLCV; the agent only relays numbers. Market-first veto when regime score &lt; 35. `lint_response.py` blocks invented prices/probability talk.

## Recipe / links
- Repo: https://github.com/xiongcp/stock-skill
- Site / demos: https://xiongcp.github.io/stock-skill/
- Skill path: `kline-structure-chart/SKILL.md`
- Install: `curl -fsSL https://raw.githubusercontent.com/xiongcp/stock-skill/main/install.sh | bash`
- Also: `npx skills add xiongcp/stock-skill` · Claude `/plugin marketplace add xiongcp/stock-skill`

## Why it made the cut
Concrete SKILL.md, installers, live demos, and a clear anti-hallucination design (compute in Python, agent narrates)—meets recipe + scenario + verifiable materials even with low star count.
