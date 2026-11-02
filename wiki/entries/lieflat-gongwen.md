# 公文写作 DNA（lieflat-gongwen）

**Tags:** writing, chinese, gongwen, style-distillation, skill
**Source:** [@bkdgiffug](https://x.com/bkdgiffug/status/2116809467853676972) · 2026-11-01
**Engagement:** larashero3-dotcom/lieflat-gongwen ~1.7k★；原帖 85 赞

## When to use
要让 Agent 起草**没有固定模板**的中文公文材料、又不想满篇「AI 味」套话：调研报告、领导讲话、工作意见、经验材料、工作方案、经验总结，以及千字级党建 / 基层经验材料。不适用于通知、请示、批复、函这类法定固定格式公文。

## What it does
用 102 万字真实公文做全量统计，把各文体的风格「蒸馏」成可测量参数（篇幅、一级标题数量与字数、句长、顿号密度、「一是二是」频次、三级标题用法等），Agent 按文体识别 → 按参数区间写作 → 用自检脚本验收。自检只把「文种识别错误」类硬冲突判为错误，其余参数偏离仅提示，保留真实优秀材料的个体差异。仓库附多篇范文和逐项参数对照。

## Recipe / links
- Repo: https://github.com/larashero3-dotcom/lieflat-gongwen （兼容 agents.md 的 Codex、Claude Code、Moxt 等）
- 范文目录：仓库内 `示例/`

## Why it made the cut
场景非常明确、边界写清楚（只做无固定模板文体），方法是语料统计而非经验套话清单，且带可量化的自检验收。对中文政务 / 国企写作场景是少见的高质量「风格蒸馏」skill。
