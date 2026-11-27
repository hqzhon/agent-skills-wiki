# PPT Agent Skill（一句话生成设计向 HTML 预览和可编辑 PPTX）

**Tags:** slides, pptx, html, design, skill
**Source:** [@tzmc9700](https://x.com/tzmc9700/status/2126124094320185738) · 2026-11-27
**Engagement:** 介绍帖 3 赞；仓库 [Akxan/ppt-agent-skill](https://github.com/Akxan/ppt-agent-skill) 现 217★，MIT。在线风格画廊：https://akxan.github.io/ppt-agent-skill/ 。此前多次出现在盘点帖里未单列，本窗有专门介绍帖。

## When to use
要把一句话、一篇文档或汇报需求交给 agent，走完「先调研再设计」的流程，得到 **HTML 预览 + 可编辑 PPTX**（文本框、原生形状、可选页间/卡片动画）时用。和已收录的 [萝卜 PPT](luobo-ppt.md)（从零生成或照参考图美化原生 PPTX）、[GordenPPTSkill](gorden-ppt-skill.md)（中文模板只改文字，非商业许可）、[Dashi PPT Skill](dashi-ppt-skill.md)（浏览器里逐页改稿再导出，AGPL-3.0）、[Frontend Slides](frontend-slides.md)（单文件 HTML 幻灯片）都不是同一条工作流。

## What it does
根目录 `SKILL.md` 规定 6 步：需求调研（先问约 7 个问题）→ 资料搜集 → 大纲 → 策划稿 → 逐页 HTML 设计稿 → 后处理成 SVG / PPTX，产物写到 `ppt-output/`。内置 26 种风格（暗色专业 / 浅色高级 / 活力鲜明 / 东方文化 / 自然复古）和 18 种图表，强调内容驱动版式、跨页叙事和失败模式修复。可选 `validate.py` 逐步校验，以及 `smoke_test.py`。只出 HTML 预览时不需要额外依赖；导出 SVG/PPTX 需要 Python 3.9+（`python-pptx`、lxml、Pillow）和 Node.js 18+。首次跑 `html2svg.py` 会经 puppeteer 下载 Chrome，大约 600 MB。

## Recipe / links
- Repo: https://github.com/Akxan/ppt-agent-skill（217★，MIT）
- 画廊：https://akxan.github.io/ppt-agent-skill/
- 安装（新开一个会话后直接说「做一个关于 X 的 PPT」）：
  ```bash
  # 个人级
  git clone --depth 1 https://github.com/Akxan/ppt-agent-skill ~/.claude/skills/ppt-agent-skill
  # 或项目级
  git clone --depth 1 https://github.com/Akxan/ppt-agent-skill .claude/skills/ppt-agent-skill
  ```
- 导出依赖：`pip install python-pptx lxml Pillow`，以及 Node.js 18+。

## Why it made the cut
可加载的完整出片配方，场景清楚，和已有 PPT/幻灯片条目互补；有 SKILL.md、风格画廊、校验脚本和 MIT 仓库。此前只出现在盘点清单里，本窗补上专门介绍帖后单列。导出链路会下载 Chromium，体积不小。
