# md2html（长 Markdown → 可读 HTML 页面）

**Tags:** docs, markdown, html, mermaid, writing, skill
**Source:** [@wiksongkim](https://x.com/wiksongkim/status/2116444461878198748) · 2026-10-31
**Engagement:** tipster; material = haidang1810/md2html ~420★ MIT

## When to use
AI 产出了很长的计划、规格、系统设计、RFC、运行手册、复盘或笔记，纯 Markdown 读不下去、也不好分享；想要一份带目录、图表、可单文件发出去的阅读页面。

## What it does
不是机械转换器，而是让 agent 先理解原文，再按仓库里的 `template.html` + `components.md` 组织内容：流程变 Mermaid 图、步骤变卡片、取舍变对比卡、要点变提示块，带侧边目录、明暗主题、打印样式；输出与源文件同名的自包含 HTML。界面语言跟随源文档（含中文）。无构建、无服务器，但需要你已有能读写文件的 agent。

## Recipe / links
- Repo: https://github.com/haidang1810/md2html
- Claude Code: `git clone https://github.com/haidang1810/md2html ~/.claude/skills/md2html`，重载后 `/md2html plan.md` → 同目录 `plan.html`
- Codex CLI: clone 到 `~/.config/md2html`，把 `SKILL.md` 软链到 `~/.codex/prompts/md2html.md`
- README 另有 Antigravity / Cursor 等接入说明

## Why it made the cut
场景清晰（读 AI 长文档）、仓库完整、零依赖、多 agent 通用；与 answer-me-with-html 互补——那个是回答用 HTML，这个是把已有长文档重排成阅读页。
