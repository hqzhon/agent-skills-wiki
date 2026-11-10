# ljg-skills（李继刚原子技能集）

**Tags:** skill-pack, thinking, writing, education, chinese, skill
**Source:** [@TammyBuilds](https://x.com/TammyBuilds/status/2119525126186111214) · 2026-11-09
**Engagement:** 0 likes / 0 reposts / 0 replies / 0 bookmarks · lijigang/ljg-skills · MIT · 7719★

## When to use
你要用 agent 做结构化思考、拆书/读论文、概念解剖、中文写作或把内容铸成卡片/画布，而且希望每件事是一个职责单一的原子 skill，而不是塞进一条超级提示词。

## What it does
李继刚把自己的思考方法做成 26 个 Codex 技能（仓库 `skills/` 目录）。覆盖八维概念解剖（`ljg-learn`）、假墙约束（`ljg-constraint`）、降秩引擎（`ljg-rank`）、九模块商业模式画布（`ljg-business-model`）、拆书/论文/问答、写作引擎、圆桌讨论、内容铸卡（长图 / 原文保真 / 漫画 / 白板）等。默认 master 分支输出 org-mode；`md` 分支输出 Markdown，方便 Obsidian / VSCode / Notion。`ljg-card` 额外依赖 Playwright 截图。

## Recipe / links
- Repo: https://github.com/lijigang/ljg-skills （MIT）
- 安装全部（Codex 全局，org-mode）：`bunx skills add lijigang/ljg-skills -g -a codex --skill '*' -y`
- Markdown 版：`bunx skills add lijigang/ljg-skills#md -g -a codex --skill '*' -y`
- 只装一个：`bunx skills add lijigang/ljg-skills#md -g -a codex --skill ljg-learn -y`
- 列出仓库技能：`bunx skills add lijigang/ljg-skills -l`
- 根目录不是技能目录；手动安装需把 `skills/` rsync 到 `~/.agents/skills/`
- `ljg-card` 安装后：`cd ~/.agents/skills/ljg-card && bun install && bunx playwright install chromium`

## Why it made the cut
26 个原子 skill、MIT、安装路径清楚，GitHub 约 7719★；不是空泛的「让 AI 更会思考」，每个技能都有可执行的产出合同（解剖、画布、铸卡、问答链）。
