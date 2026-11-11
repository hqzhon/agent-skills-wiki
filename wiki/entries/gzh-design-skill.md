# gzh-design-skill（公众号 Markdown 排版）

**Tags:** writing, wechat, layout, html, chinese, skill
**Source:** [@laogeai](https://x.com/laogeai/status/2120095751707775212) · 2026-11-10
**Engagement:** 1♥ · isjiamu/gzh-design-skill ~4.3k★ · LICENSE 见仓库（GitHub 识别为 NOASSERTION）

## When to use
要把 Markdown / Word / PDF / 纯文本文章排成可直接粘进微信公众号编辑器、粘贴后样式不丢的 HTML；或想按描述/参考图生成一套自定义公众号主题并复用。不用于普通网页、落地页或 PPT。

## What it does
`SKILL.md` 只管流程与决策：非 Markdown 先归一化（`scripts/extract_docx.py` 等）→ 按题材从 `references/theme-index.md` 推荐主题（6 套，如摸鱼绿、石墨极简、留白禅意）并让用户确认 → 读该主题组件库 + 通用组件库（代码块/图片/GIF）→ 解析结构、自动章节编号、引言卡、目录、签名 → 双关卡校验后交付。支持「一键自动排版」全自动模式，以及主题生成器。HTML 一律从组件库取，不凭记忆手写。

## Recipe / links
- Repo: https://github.com/isjiamu/gzh-design-skill
- 结构：`SKILL.md` + `references/`（主题组件库）+ `scripts/` + `docs/`

## Why it made the cut
完整 SKILL.md（触发词、反例场景、分步工作流），渐进加载 references 的结构清晰，场景具体，仓库星标可验证。
