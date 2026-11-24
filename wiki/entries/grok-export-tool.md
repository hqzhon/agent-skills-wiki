# grok-export-tool（本地导出自己的 Grok Bot 与对话）

**Tags:** grok, export, backup, mcp, skill
**Source:** [@su_lofi](https://x.com/su_lofi/status/2124910293851729922) · 2026-11-23
**Engagement:** 本窗作者介绍帖 9 赞 · 仓库 [LofiSu/grok-export-tool](https://github.com/LofiSu/grok-export-tool) 现 6★；文档站点中英双语

## When to use
想把**已经登录在本机**的 Grok Bot 名册、完整对话和附件，或普通 Grok 聊天，导出成本地 JSONL / Markdown 存档，并让 OpenCode / Claude Code / Codex 等通过 MCP 或 skill 查询这份档案。不把数据送到第三方 API。

## What it does
本地 CLI + 零依赖 stdio MCP + Agent Skill（`.claude/skills/grok-export/`）。从本机已登录的 grok.com 会话读取你自己的历史（按平台用本地 cookie / DPAPI 等，Windows 的 App-Bound Encryption 可能需要 `--cookie`）。每个 Bot 带名册、全文和附件；普通聊天另存一目录。无 API key。

## Recipe / links
- Repo: https://github.com/LofiSu/grok-export-tool（6★）
- 文档: https://lofisu.github.io/grok-export-tool/ （[中文](https://lofisu.github.io/grok-export-tool/index.zh-CN.html)）
- 快速开始：建 venv 后 `pip install -r requirements.txt`，再运行 `python3 grok-bot-export.py`（`--mode chat` / `--mode all`）
- Skill 名称是 `grok-export`：Claude Code / OpenCode 可读项目内 `.claude/skills/grok-export/`；其他 agent 把该目录拷到各自的 skills 路径

## Why it made the cut
有明确「备份自己的 Bot 和聊天」场景，CLI、MCP 和可加载 skill 都在仓库里，并且强调本地、无 API key。星数不高，但步骤可验证，也和本目录读者常用的 Grok Bot 工作流相关。
