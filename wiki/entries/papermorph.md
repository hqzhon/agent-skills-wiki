# Papermorph（把书做成有旁白的互动网页课 / 剪纸片 / 纪录片）

**Tags:** education, animation, documentary, books, claude, skill
**Source:** [@hsianghui](https://x.com/hsianghui/status/2126540166554939698) · 2026-11-28
**Engagement:** 本窗介绍帖 2 赞 / 2 书签；仓库 [DozenTwelve/Papermorph](https://github.com/DozenTwelve/Papermorph) 2,267★，MIT。产出是可托管的静态页面，现场书架见 [papermorph.diamonddoge.org](https://papermorph.diamonddoge.org/)。

## When to use
要把教材 PDF 做成带旁白和随堂练习的互动网页课，把故事/笑话/童话做成剪纸木偶短片，或把一本书、一个论点做成纪录片和竖屏短片时用。不要用它做书架设计、注册或托管——技能说明里把这些列成另一次任务。它和已收录的 [papercraft](papercraft.md) 不是同一条：papercraft 是 Three.js 弹出式剪纸场景风格，Papermorph 是「一本书 → 可运行的静态书页」。

## What it does
可加载技能 [`.claude/skills/papermorph/SKILL.md`](https://github.com/DozenTwelve/Papermorph/blob/main/.claude/skills/papermorph/SKILL.md) 在同一套引擎上做三档书：
1. **课**：从教材 PDF 拆出章节动画课，画面承担讲解，旁白跟着走，检查和练习做在画面里
2. **绘本**：纸偶在代码绘制或模型绘制的布景前演出，配声音、音效和音乐；也可从扫描绘本里裁出原画当偶
3. **影片**：用公有领域图片、文字和地图做成旁白纪录片，并可再切成三分钟以内、只讲一个点的竖屏短片；还有随滚动变画的长页，以及可点选人物地点的历史地图

成品是 SVG 舞台加播放器（横屏 1600×900，竖屏短片 900×1600），不依赖服务器、数据库或账号。旁白可用免费的 Edge TTS 或本地 Kokoro；ElevenLabs 演技配音、静帧出片段、绘本布景绘制是可选付费步骤。

## Recipe / links
- Repo: https://github.com/DozenTwelve/Papermorph（2,267★，MIT）
- 安装：
  ```bash
  npx skills add DozenTwelve/Papermorph --skill papermorph --agent claude-code   # 或 --agent opencode
  ```
- 技能路径：`.claude/skills/papermorph/SKILL.md`
- 依赖：uv、ffmpeg，以及 Playwright 浏览器（`uv run --with playwright playwright install chromium firefox`）

## Why it made the cut
仓库星数高、许可清楚，技能对使用边界和交付物写得很具体，还有可打开的公开样书。本窗由经常供稿的 @hsianghui 给出可核链接，值得单列。
