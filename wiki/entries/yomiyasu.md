# yomiyasu（日语去 AI 味推敲）

**Tags:** writing, humanizer, japanese, editing, evals, skill
**Source:** [@laogeai](https://x.com/laogeai/status/2120037836842000573) · 2026-11-10
**Engagement:** nanaism/yomiyasu ~3.0k★ · MIT

## When to use
把 AI 生成的日语技术文章、设计文档、PR 描述、内部报告改得自然易读，同时不改变数字、否定、条件和主语宾语。只处理日语文本。

## What it does
修正不自然的比喻、主谓不清、把工具写成有意志、垫话，以及过量加粗/列表/emoji/句尾冒号；读起来自然的部分不动。识别 13 种文体（邮件、纪要、幻灯片、论文、小说等）并保留各自惯例。2.0 起在返回前跑内置检查，把数字、否定或主宾互换列为待复核项；含义无法判定时保留原文并反问作者。另有 `yomiyasu-mini`（SKILL.md ≤18k 字符）与 `yomiyasu-pocket`（400–500 字指令）。

## Recipe / links
- Repo: https://github.com/nanaism/yomiyasu
- 安装：`npx skills add nanaism/yomiyasu` / `gh skill install nanaism/yomiyasu yomiyasu` / Claude Code `/plugin marketplace add nanaism/yomiyasu`
- 仓库含 `evals/`、`tests/`、`references/`

## Why it made the cut
可装 skill + 多种安装路径，有 evals 与保义检查这种可验证设计，场景明确；日语方向填补了 Catalog 去 AI 味类的空白。
