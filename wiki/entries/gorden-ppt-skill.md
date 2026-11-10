# GordenPPTSkill（中文模板填字 PPT）

**Tags:** slides, pptx, templates, chinese, skill
**Source:** [@zg0820](https://x.com/zg0820/status/2119581853988598047) · 2026-11-09
**Engagement:** 1 like / 0 reposts / 1 reply / 0 bookmarks · GordenSun/GordenPPTSkill · 非商业（仅个人学习与研究） · 3984★

## When to use
你要做一份信息密度高、看起来偏商务的中文 PPT（汇报、复盘、述职、开题、提案），并且希望保留人工打磨过的版式，而不是让模型从零排版或把每页压成图片。注意：内置模板禁止商用。

## What it does
原生 PPTX 技能：从约 17–21 套中文模板里选一套（或用你自己的 `.pptx`），AI 只写 `edits.json` 替换文字，`scripts/build_pptx.py`（python-pptx）生成版式不变的可编辑 PPTX。三种模式：内置模板、用户自带模板、完全原创简洁版式。规则是不改位置/颜色/字号，禁止用省略号硬截断。首次调用必须先跑 `python3 scripts/apply_update.py` 做增量更新。可选 LibreOffice + Poppler 渲染预览图。

## Recipe / links
- Repo: https://github.com/GordenSun/GordenPPTSkill （非商业许可，禁止任何商业用途）
- 对 agent 说：安装这个 Skill：https://github.com/GordenSun/GordenPPTSkill ，然后读取本地文件做 PPT
- 依赖：Python 3.9+、`python-pptx` 1.0+；预览需要 LibreOffice 与 `pdftoppm`
- 命令行构建：`python3 scripts/build_pptx.py <template.pptx> edits.json out/final.pptx --detail <detail.json>`
- 入口：根目录 `SKILL.md`、`templates/INDEX.md`
- 和 [萝卜 PPT](luobo-ppt.md) 的区别：萝卜是从零生成 / 照参考图美化原生 PPT；这里是「选模板 + 只改文字」，版式锁定在模板里

## Why it made the cut
有完整 SKILL.md、构建脚本、模板清单和自动更新机制，GitHub 约 3984★，中文商务 PPT 场景具体。必须把非商业许可写进条目，避免当成可商用模板库。
