# Skill Lens（看清本机哪一份 SKILL.md 真正生效）

**Tags:** diagnostics, skill-hygiene, cli, multi-agent, tool
**Source:** [@hazem_samak101](https://x.com/hazem_samak101/status/2125640392976519640) · 2026-11-26
**Engagement:** 本窗为 0.2.1 介绍帖（1 赞）；仓库 [Hazem-Samak/skill-lens](https://github.com/Hazem-Samak/skill-lens) 现 2★ / 1 fork，MIT，带 CI

## When to use
同一台机器上装着 Claude Code、Codex、OpenCode、Gemini 等多个编码 agent，技能目录、符号链接和插件副本开始分叉：你不确定「到底装了哪些技能、某个 agent 实际加载的是哪一份、两份 `SKILL.md` 差在哪里」时用。它是只读诊断，不是安全扫描（预安装投毒检测见已收录的 [SkillSpector](skillspector.md)），也不是又一个可加载业务技能。

## What it does
本地 CLI（包名 `skill-lens-cli`）。`skill-lens scan` 探测已安装的 agent，汇总规范库、项目技能、系统/捆绑技能和插件技能。`skill-lens diff <name>` 以一份副本为基线，显示其他副本的 `SKILL.md` 差异。逻辑离线、确定，用来回答：有哪些技能、谁能看见它们、哪一份优先级最高、快捷方式是否已漂成另一变体。可选 TUI（`skill-lens-cli[tui]`）。文档称 0.2.1 支持约 10 个 agent。不改你的技能文件。

## Recipe / links
- Repo: https://github.com/Hazem-Samak/skill-lens（2★，MIT）
- 安装：
  ```bash
  uv tool install skill-lens-cli     # 推荐
  # 或：pipx install skill-lens-cli
  ```
- 常用：`skill-lens scan`；`skill-lens diff deploy`
- 可选界面：`uv tool install 'skill-lens-cli[tui]'`
- 说明：https://github.com/Hazem-Samak/skill-lens/blob/main/README.md

## Why it made the cut
多 agent 并存后「哪一份技能真正在跑」是真实痛点，仓库提供可安装的只读 CLI、差异对比和 CI，场景清楚。2★、介绍帖互动很低，按可验证工具收录，与 SkillSpector（装前安全扫描）互补，而不是替代一条业务 SKILL.md。
