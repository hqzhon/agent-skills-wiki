# Perler-Bead MV Skill（像素拼豆风动画 MV）

**Tags:** animation, video, pixel-art, perler-beads, chinese, skill
**Source:** [@ay1285640043181](https://x.com/ay1285640043181/status/2126224510198362598) · 2026-11-27
**Engagement:** 作者介绍帖 46 赞；仓库 [xyong934-gif/perler-bead-mv-skill](https://github.com/xyong934-gif/perler-bead-mv-skill) 现 3★（本窗当天新建），MIT。

## When to use
要把角色设定或拼豆参考图，做成**带塑料豆孔和高光的 1080p 像素拼豆（Perler beads）游戏风动画 MV**，或 4K 模切贴纸表时用。它走程序化豆格渲染，而不是把图丢进视频生成模型（那种结果容易把豆子糊成马赛克）。支持 Antigravity / Claude Code / Codex 等，README 称无需 npm 依赖即可拷目录使用。

## What it does
交互式导演技能 `perler-bead-mv`：装好后说「帮我做个像素拼豆视频」，agent 会分步询问角色、音乐、主题世界、道具/Boss 和字幕偏好。没有现成图或歌时，会给出可抄的出图提示词和 Suno 配乐提示词。随后：

- `scripts/extract_beads.js` 1:1 提取豆格、去底并聚类有限色板
- `scripts/analyze_audio.js` 分析 BPM、鼓点和逐帧能量，用来卡点
- 先出角色道具贴纸表和 16 格分镜预览，让用户改完再渲染
- `scripts/perler_renderer.js` 按豆孔、塑料高光和白色模切描边画每一颗豆子
- `scripts/render_mv.js` 用 Headless Chromium + FFmpeg 出 1080p MP4（自动选 NVIDIA NVENC / Apple VideoToolbox / CPU libx264）

## Recipe / links
- Repo: https://github.com/xyong934-gif/perler-bead-mv-skill（3★，MIT）
- 安装：把仓库里的 `skills/perler-bead-mv` 拷到对应 skills 目录，例如：
  - Antigravity 项目级：`<项目>/.agents/skills/perler-bead-mv/`
  - Antigravity 全局：`~/.gemini/config/skills/perler-bead-mv/`
  - Claude Code：`~/.claude/skills/perler-bead-mv/`
  - Codex：`~/.codex/skills/perler-bead-mv/`
- 技能文件：`skills/perler-bead-mv/SKILL.md`

## Why it made the cut
作者第一方发布，使用场景清楚，有完整 SKILL.md 和可检查的本地脚本（提豆、分析音频、渲染），不是只丢提示词。GitHub 星标还很少（当天新建），但介绍帖互动明显（46 赞），材料够核。成片质量仍取决于输入图和本机 FFmpeg/Chromium 环境。
