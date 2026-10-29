# leanrea（轻装逆向）

**Tags:** reverse-engineering, cli, token-budget, skill, chinese
**Source:** [@Easycompany333](https://x.com/Easycompany333/status/2115778368822182247) · 2026-10-29
**Engagement:** tipster post; repo ~3.5k★ · MIT · ~8 KB single skill (no MCP)

## When to use
When an agent should **逆向分析**桌面 / Electron / 原生二进制，但你不想把几百个 MCP 工具定义灌进上下文——只要一份指路小抄，让 agent 用本机已有 CLI（`asar`、`otool` 等）干活。

## What it does
One compact `SKILL.md` that replaces heavy “Reverse Engineer Anything” MCP stacks: routes target types to the cheapest CLI path, marks pitfalls, and requires each conclusion tagged `seen` / `inferred` / `unknown` so the model cannot silently invent. Author benchmarks claim ~38% faster / ~35% cheaper vs REA MCP with similar accuracy.

## Recipe / links
- Repo: https://github.com/aicodeking/leanrea (~3.5k★, MIT)
- Install: `npx skills add aicodeking/leanrea`
- Skill lives under `leanrea/` (plain CLI guidance, no MCP server)

## Why it made the cut
Concrete installable skill with clear when-to-use, verifiable OSS, strong star signal, and an explicit anti-hallucination labeling rule—not a “just reverse it” rant.
