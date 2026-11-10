# tethertrace（真机 Android 测试 skill）

**Tags:** testing, android, mobile, mcp, qa, skill
**Source:** [@Keshurai25](https://x.com/Keshurai25/status/2119770821866717198) · 2026-11-09
**Engagement:** 4♥ 2RT · Saurabhzz9/tethertrace · 新项目，星标尚低

## When to use
想让 Claude Code / Codex 在**自己的真机安卓手机**上测试 APK，但不想装 adb 或 Android SDK；只走 Wi-Fi。说一句「test my APK on my phone」即可。

## What it does
MCP server 提供约 23 个驱动手机的工具；`skills/` 下的 SKILL.md 告诉 agent 何时、如何用：检查连接 → 选测试类型 → 按屏幕真实文案写流程 → 跑到通过 → 诚实汇报覆盖与未覆盖的部分。

## Recipe / links
- Repo: https://github.com/Saurabhzz9/tethertrace （含 `skills/`、`examples/`、`docs/`）
- 用法：先按 README 连接 MCP server，再把 `skills/` 里的 skill 放进 `~/.claude/skills`（或对应 agent 目录）

## Why it made the cut
MCP + SKILL.md 组合的好范例：配方具体、场景清晰、带「诚实汇报覆盖范围」的收尾步骤，仓库可验证。社区信号还弱，按早期项目对待。
