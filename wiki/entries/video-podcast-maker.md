# Video Podcast Maker（题目到解说视频）

**Tags:** video, podcast, remotion, tts, youtube, bilibili, skill-pack
**Source:** [@heyrimsha](https://x.com/heyrimsha/status/2125207339993276815) · 2026-11-24
**Engagement:** 盘点帖将其列为第 1 项（79 赞）；仓库 [Agents365-ai/video-podcast-maker](https://github.com/Agents365-ai/video-podcast-maker) 现 1,733★，MIT，v5.3.0（2026-10-01 推送）

## When to use
给一个主题，要自动做成有旁白的知识向视频、播客或解说片（Bilibili / YouTube / 小红书 / 抖音 / 视频号）时用。也可以从参考视频/图片学习视觉节奏后再生成。不要用它做通用剪辑、转码或无关的短剧制作。若只是在已有 `videos/{name}/` 上改脚本或配乐，应复用该目录，不要新开项目。

## What it does
可加载技能包，三个变体：`video-podcast-maker`（完整）、`-lite`、`-nano`。流程是研究 → 脚本 → TTS → Remotion 合成 → Studio 预览 → 4K 成片 + BGM。v5.3.0 支持本地 TTS（Edge 免费或 Azure）、按清单管理素材、成本门控的 AI 生成。最终 4K 渲染需你明确确认。README 建议人工反复打磨 `podcast.txt`。

## Recipe / links
- Repo: https://github.com/Agents365-ai/video-podcast-maker（1,733★，MIT）
- 安装其中一个变体：`npx skills add Agents365-ai/video-podcast-maker/skills/video-podcast-maker -g`；去掉路径后缀可一次装三个。
- 环境：Python 3.8+、Node.js 18+、FFmpeg，以及一个 Remotion 项目（全新项目会下载约 2.2 GB npm 包 + 约 90 MB headless Chrome，推荐复用已有项目）。
- 配置 `TTS_BACKEND` 及对应 key，详见仓库 TTS 说明。
- Skill: [skills/video-podcast-maker/SKILL.md](https://github.com/Agents365-ai/video-podcast-maker/blob/main/skills/video-podcast-maker/SKILL.md)

## Why it made the cut
高星漏收：主题→解说成片的完整可加载技能，和已有 Remotion / HyperFrames / video-use（剪毛片）不是同一条路径。1,733★、MIT，配方和依赖写得很清楚。本窗来自盘点帖，按仓库信号补上，并标明 Remotion/TTS 的体积与费用。
