# roblox-dev-skill（按当前 Studio / Luau 写 Roblox 的专家技能）

**Tags:** gamedev, roblox, luau, mcp, skill
**Source:** [@0xKense1](https://x.com/0xKense1/status/2124248203629306061) · 2026-11-22
**Engagement:** 本窗为 14 个 Roblox+Claude 项目合集帖（1,292 赞 / 70 转 / 1,952 收藏）；本条取其中可装的技能仓 [MSayib/roblox-dev-skill](https://github.com/MSayib/roblox-dev-skill) 101★，MIT。合集里的 MCP、Rojo、LSP 等是配套工具，不是 skill，未单独建条。

## When to use
让编码 agent 写 **Roblox / Luau / Roblox Studio** 代码，并希望它按**已核对过的当前引擎版本**来写（而不是过时 API 记忆）时使用。适合架构、反作弊、DataStore、UI、性能、变现，以及通过 Studio 内置 MCP 安全驱动编辑器。

## What it does
符合 Agent Skills 规范的专家技能：一份路由 `SKILL.md`，外加 14 篇参考指南。技能 2.22.0 标明对照 Roblox Studio **0.746.0.7461269** 与 **Luau 0.745**（2026-11-07）验证：示例在 `--!strict` 下类型检查，并在真实 Studio place 里跑过。它本身不是 MCP、也不带工具；要操作 Studio，需另外启用官方内置 MCP。作者提醒 Roblox 每周发版，版本戳只说明「上次核对时」，不是今天的版本。和合集中的 [TabooHarmony/roblox-brain](https://github.com/TabooHarmony/roblox-brain)（技能库，204★）方向相近，本条因版本核对和参考文档更完整而收录。

## Recipe / links
- Repo：https://github.com/MSayib/roblox-dev-skill（MIT，101★）
- 安装脚本（会改本机 agent 技能目录，先读脚本再执行）：
  ```
  # macOS / Linux / WSL
  curl -fsSL https://raw.githubusercontent.com/MSayib/roblox-dev-skill/master/install.sh | bash
  ```
  Windows 可用仓库中的 `install.ps1` / `install.cmd`。也可按 Agent Skills 格式手动链到 Claude Code、Codex、Cursor、Gemini CLI、Antigravity、GitHub Copilot。
- Studio MCP：见 [Roblox Studio MCP 文档](https://create.roblox.com/docs/studio/mcp)。

## Why it made the cut
有明确使用场景、版本核对说明和 14 篇可验证参考，不是「会写 Roblox」的空喊。本窗经高互动合集带出；合集里的其它仓库多为工具链，不重复建条。
