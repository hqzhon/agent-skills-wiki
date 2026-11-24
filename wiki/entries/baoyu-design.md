# baoyu-design（本地 Claude Design / Slides / Dashboard）

**Tags:** design, slides, dashboard, html, skill-pack, chinese
**Source:** [@dotey](https://x.com/dotey/status/2115667965328977920) · 2026-10-29
**Engagement:** 原仓 [JimLiu/baoyu-design](https://github.com/JimLiu/baoyu-design) 收录时约 4.7k★、MIT；2026-11 起项目重建为 [JimLiu/open-artifact](https://github.com/JimLiu/open-artifact)（现 453★，Apache-2.0，2026-11-24 仍在推送）。本窗有第三方提到 v0.12.3（Motion 长片粗剪预览与中文多音字校对）。

## When to use
When you want **Claude Design / Slides / Dashboard**-class UI mockups, decks, and data dashboards **inside Cursor / Claude Code / Codex** as self-contained HTML—without claude.ai Artifacts or uploading files to the web UI.

## What it does
最初是把 Claude Design 方法收成可在 Cursor / Claude Code / Codex 本地运行的技能包，产出 UI、原型、幻灯片和 Dashboard。2026-11 起作者将项目重建为 **Open Artifact**：一份 agent 无关的本地格式、一个本机 daemon、一个页面框架、一条 `/open-artifact` skill，以及幻灯片 / UI 设计 / 设计系统 / 白板 / 表格 / 仪表盘 / 文档 / Motion 等类型技能。Agent 把普通文件写到本地目录，本机编辑器打开后可改稿、批注，再把意见送回 agent 会话。不强制绑定某一家模型，也不把文件上传到网页版 Artifact。

## Recipe / links
- 当前仓库: https://github.com/JimLiu/open-artifact（453★，Apache-2.0；旧址 https://github.com/JimLiu/baoyu-design 会跳转过来）
- 主 skill: `skills/open-artifact/SKILL.md`；类型技能在 `artifact-types/{slides,design,design-system,whiteboard,sheets,data,docs,motion}/`
- 安装与用法以新仓 README 为准。本机需要运行 Open Artifact daemon 才能预览和回传批注。

## Why it made the cut
当初就因可加载技能包和明确的本地 Artifact 场景收录。本窗确认项目已更名并重建为 Open Artifact，故更新条目指向新仓，避免继续引导到旧结构。不另开重复条目。
