# pstack `/statechart`（TLA+ → Mermaid 状态图）

**Tags:** formal-verification, tla, state-machine, debugging, skill-pack
**Source:** [@poteto](https://x.com/poteto/status/2115880102601101414) · 2026-10-29
**Engagement:** ~3.7k likes / ~186 reposts / ~221 replies / ~3.7k bookmarks · tipster post; repo ~3.2k★ · MIT

## When to use
When you need an agent to **把产品流 / 协议 / 分布式服务建模成可检查的状态机**，用最短违规路径讲清真实 bug——尤其适合配合 `/create-formal-verification-skill` 先建模再画图。

## What it does
`statechart` skill（pstack v0.15.36 起标为稳定）内含迷你 TLC 编译管线：解析 TLA+ → 小 IR → Mermaid / [Pele](https://pele.run/) 可主题化图表。报告给出每个破坏规则状态的最短路径。作者帖中展示了 skill 自身状态图及两处真实 bug。可与 `create-formal-verification-skill` 联用，对抽象状态机与分布式系统做形式化摸底。

## Recipe / links
- Pack repo: https://github.com/backnotprop/pstack (~3.2k★, MIT)
- Also mirrored in Cursor plugins: https://github.com/cursor/plugins (pstack)
- Install one skill: `npx skills add backnotprop/pstack --skill statechart`  
  （或 `npx skills add cursor/plugins --skill statechart`）
- Cursor: `/add-plugin pstack` · Claude Code marketplace: `cursor/plugins` → `pstack`
- Skill path: `skills/statechart/SKILL.md` · first run may install TLC/Java via mise (~305 MB)

## Why it made the cut
Concrete installable skill + clear when-to-use, verifiable OSS with scripts, and outsized community signal on the announcement post—not a “just draw a diagram” tip.
