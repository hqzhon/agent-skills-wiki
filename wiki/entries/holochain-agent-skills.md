# Holochain Agent Skills

**Tags:** holochain, rust, p2p, happ, skill, official-adjacent
**Source:** [@soushi888](https://x.com/soushi888/status/2121366095647093016) · 2026-11-14（另见同作者 [v1.0 说明](https://x.com/soushi888/status/2121378871836569880)）
**Engagement:** 发布帖 9 赞 / 2 转；仓库 [Soushi888/holochain-agent-skills](https://github.com/Soushi888/holochain-agent-skills) 约 24★，LICENSE 为 Apache-2.0

## When to use
在 Claude Code、Cursor、Copilot、Gemini CLI 等兼容 Agent Skills 的工具里开发 Holochain 0.7 的 hApp，希望 agent 按当前 HDK / Sweettest 惯例来写，而不是用过时训练数据里的旧 API。

## What it does
面向 Holochain 0.7 的技能包，按 [Agent Skills Open Standard](https://agentskills.io) 组织。核心是 `skills/holochain/SKILL.md`（约 26KB）加 `references/` 与 `assets/`。作者称对照一个能实际编译的参考 hApp 做过校验。本轮发现的是 v1.0.0-rc.2：安装脚本把技能链接进项目里已有的 `.claude` / `.cursor` / `.opencode` / `.gemini` / `.agents` / Copilot 目录；也提供 release 归档（含 SHA256SUMS）和 Nix flake。

## Recipe / links
- Repo: https://github.com/Soushi888/holochain-agent-skills
- SKILL.md: https://github.com/Soushi888/holochain-agent-skills/blob/main/skills/holochain/SKILL.md
- 安装（先读脚本再执行）：`curl -fsSL https://raw.githubusercontent.com/Soushi888/holochain-agent-skills/main/install.sh | sh`
- 全局安装：同上，在 `sh -s --` 后加 `--global`；可用 `--dry-run`、`--target claude,cursor`、`--copy`
- 或从 [v1.0.0-rc.2](https://github.com/Soushi888/holochain-agent-skills/releases/tag/v1.0.0-rc.2) 解压归档到 `.claude/skills`
- 需要 git，以及 Node 22.18+ 或 Bun（安装器会检查）

## Why it made the cut
维护者自己发布的可安装 SKILL.md，场景清楚（Holochain hApp），有校验 workflow、release 校验和和多 harness 安装方式。社区星数不高，但是垂直领域里一份能核对的配方。
