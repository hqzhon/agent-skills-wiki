# Agentic Production Skills（12 个生产级门禁与韧性技能）

**Tags:** production, reliability, security, evaluation, skill-pack
**Source:** [@ParraEvan](https://x.com/ParraEvan/status/2124874359756234953) · 2026-11-23
**Engagement:** 本窗介绍帖 3 赞 · 仓库 [DevDizzle/agentic-production-skills](https://github.com/DevDizzle/agentic-production-skills) 现 0★，MIT，带 CI，Python 3.11+ / 严格 TypeScript 参考实现均为零依赖

## When to use
要把 agent 系统送进生产，问题往往不是模型不够聪明，而是缺门禁：工具路由、审计、幂等检查点、输入防火墙、影子评估等。需要可安装的 `SKILL.md`，并且能对照零依赖的参考库实现。

## What it does
12 个技能，按协调、治理、韧性、安全、发布分组，每个都配有 Python 与 TypeScript 参考实现，例如：

- 协调：`intent-and-tool-routing`、`supervisor-delegation-gate`、`pass-by-reference-blackboard`
- 治理：`constraint-anchoring`、`independent-auditor-gate`、`causal-audit-ledger`
- 韧性：`idempotent-checkpointing`、`watchdog-adaptive-retry`、`parallel-consensus-voting`、`tiered-human-escalation`
- 安全：`untrusted-input-firewall`（间接注入、隐写 Unicode 等）
- 发布：`shadow-canary-eval`

## Recipe / links
- Repo: https://github.com/DevDizzle/agentic-production-skills（0★，MIT）
- Claude Code（个人全局）：
  ```bash
  git clone https://github.com/DevDizzle/agentic-production-skills.git /tmp/agentic-production-skills
  mkdir -p ~/.claude/skills
  cp -r /tmp/agentic-production-skills/skills/* ~/.claude/skills/
  ```
- 也可拷到 `.agents/skills/`、`.cursor/skills/` 或 `~/.codex/skills/`；参考库可用 `pip install -e .`

## Why it made the cut
星数为 0，但 12 份 `SKILL.md` 加上可运行的零依赖参考实现和 CI，主题（生产门禁）具体可验证，不是空喊「生产级」。适合需要审计/重试/升级路径的人，不必等星数。
