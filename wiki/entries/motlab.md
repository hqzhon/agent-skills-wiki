# motlab（把视频写成代码并在审片器里改）

**Tags:** video, motion, canvas, webcodecs, agent-skills, skill-pack
**Source:** [@vintcessun](https://x.com/vintcessun/status/2126538582865444882) · 2026-11-28
**Engagement:** 本窗介绍帖 3 赞；仓库 [staryone/motlab](https://github.com/staryone/motlab) 527★，MIT OR Apache-2.0。仓库自称广告样片用这套技能写了 7 个镜头、审片后导出 4K。

## When to use
要用编程代理做产品广告、Logo 动画、讲解片、教程、屏幕录制或素材剪辑，并且希望**每一帧都是代码**、能在审片器里逐帧批注再改时用。不要用它去调视频生成模型——技能写明不走 AI 出图或出片，画面来自你给的参考素材。它和已收录的 [AutoClip](autoclip.md)（长视频切片）、[Remotion Agent Skills](remotion-skills.md)、[Moodreel](moodreel.md)（从参考片量风格再复刻）都不是同一条。

## What it does
三个可加载技能（`motlab` / `motlab-assets` / `motlab-styles`）配一个本地引擎：
1. 每个镜头是带 `renderAt(t)` 的 Canvas 页面，预览和导出走同一套场景
2. 无头 Chrome 逐帧绘制，页面内用 WebCodecs 编码成 720p 到 4K 的 MP4，不必把逐帧截图丢给 ffmpeg 拼片
3. 审片器可逐帧播放、框选批注；代理读 `selection.json` 按编号改，版本可并排对照
4. 你提供 Logo、截图、素材、字体、音乐和口播，代理写镜头并打开审片器；风格来自参考或 `motlab-styles`，技能本身没有默认「网红风」

需要 Node 24+、Chrome/Chromium 和带 ffprobe 的 ffmpeg；Blender 只在资产技能的三维路径里可选。

## Recipe / links
- Repo: https://github.com/staryone/motlab（527★，MIT OR Apache-2.0）
- 安装引擎并拷贝技能：
  ```bash
  npm install -g @motlab/cli
  npx @motlab/cli setup          # 默认 Claude Code；Codex/Cursor 等加 --skill agents
  ```
- 只装技能（skills.sh）：
  ```bash
  npx skills add staryone/motlab -g
  ```
  技能第一次运行若发现还没有引擎，会提示再执行 `npm install -g @motlab/cli` 和 `npx @motlab/cli setup --skill none`。
- 技能路径：`skills/motlab/SKILL.md`（另有 `skills/motlab-assets/`、`skills/motlab-styles/`）

## Why it made the cut
有完整 SKILL.md、审片闭环和双许可，仓库材料可核；本窗介绍把「代码即镜头、批注落到具体帧」讲清楚了，值得从「又一个视频工具」里单列出来。
