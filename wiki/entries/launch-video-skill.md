# Launch Video Skill

**Tags:** video, launch-video, product-demo, motion, skill
**Source:** [@ardent__dev](https://x.com/ardent__dev/status/2125476839691038804) · 2026-11-25
**Engagement:** 本窗介绍帖 1 赞 / 1 收藏；仓库 [HazimBhatt/launch-video-skill](https://github.com/HazimBhatt/launch-video-skill) 现 2★，MIT，含演示成片与本地渲染脚本。

## When to use
要从产品 URL 生成本地、零推理费用的 SaaS / 开发工具发布片（16:9 或 9:16，1080p 60 FPS）时用。适合 Product Hunt、X 首发或 Show HN 预告。不要和已收录的 [product-launch-motion](product-launch-motion.md)（Chan 风格 HTML 变形 UI 卷轴）、[huashu-motion](huashu-motion.md)（可指着画面局部改）、[spotlight-film](spotlight-film.md) / [onetake](onetake.md) 混淆：这条走「实拍级 2x Retina 界面抓取 + 六套风格预设 + 本机音频母带」管线。

## What it does
可加载 Agent Skill（根目录 `SKILL.md`）。探针先抓品牌 DNA 和 2x Retina 界面，再按所选风格搭场景，默认旗舰是 `cinema-launch`（Liquid Glass、三维前后对比窗、像素马赛克转场、宽立体声 -14 LUFS）。另外五套：`macro-studio`、`bento-proof`、`kinetic-noir`、`problem-story`、`terminal-launch`。渲染在本地用 Node / Chrome / FFmpeg / Python 完成，仓库带 `demo/` 样片和 `scripts/`、`styles/`、`references/`。

## Recipe / links
- Repo: https://github.com/HazimBhatt/launch-video-skill（2★，MIT）
- 安装：`npx skills add HazimBhatt/launch-video-skill`
- 手册管线见 README：`scripts/setup.mjs` → `probe.mjs` → `new_video.mjs` → 节拍/音频 → 捕获 → 渲染

## Why it made the cut
有完整 SKILL.md、六套风格、本地脚本和演示成片，使用场景清楚。本窗互动很低，但配方可验证，且与目录里其他发布片技能路线不同。
