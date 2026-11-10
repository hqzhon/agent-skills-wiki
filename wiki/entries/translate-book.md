# translate-book（整书并行翻译）

**Tags:** translation, books, pdf, epub, subagents, skill
**Source:** [@laogeai](https://x.com/laogeai/status/2119975191636054287) · 2026-11-10
**Engagement:** 帖子互动低 · deusyu/translate-book ~2.4k★ · MIT

## When to use
要把一整本外文书（PDF / DOCX / EPUB / Markdown）翻成目标语言，并希望全书术语统一、输出 HTML / DOCX / EPUB / PDF。适用于 Codex、Claude Code、OpenClaw。

## What it does
收集参数（文件、目标语言、并发数、自定义要求）→ 用 `scripts/convert.py` 把书转成 Markdown 分块 → 按批派发并行子代理翻译各块 → 合并并导出多种格式。依赖 python3、pandoc、Calibre（ebook-convert）。

## Recipe / links
- Repo: https://github.com/deusyu/translate-book （根目录 `SKILL.md` + `scripts/`）
- 安装：把仓库放进 `~/.claude/skills/translate-book`（或对应 agent 的 skills 目录），先装好 pandoc 与 Calibre

## Why it made the cut
完整的多步流水线配方（分块 → 并行子代理 → 合并导出），场景明确，仓库与脚本可验证，星标可观。
