# Talking Head Video Skill（口播前期策划包）

**Tags:** video, talking-head, pre-production, short-form, skill
**Source:** [@bancheng0521](https://x.com/bancheng0521/status/2125490881918890384) · 2026-11-25
**Engagement:** 本窗为作者发布帖（0 赞）；仓库 [lzx0711/talking-head-video-skill](https://github.com/lzx0711/talking-head-video-skill) 现 1★，MIT。

## When to use
你要做 15–90 秒口播或不出镜短视频（抖音 / 小红书 / TikTok / Reels / Shorts），卡点是「不知道说什么、怎么拆镜头」，需要一份能直接拿去录音、出图、成片的前期包时用。它**不渲染 MP4、不做 TTS、不调用视频生成模型**。不要和 [video-use](video-use.md)（对着已有口播成片对话式剪辑）或 [digital-human-koubo](digital-human-koubo.md)（一张照片 + 文稿生成对口型数字人）混淆。

## What it does
可加载 Agent Skill（`skills/talking-head-video/SKILL.md`）。输入一个主题，输出成片包：带停顿标记的口播稿、分镜表、提词、SRT、每镜中英图片提示词、10 个封面标题，以及给下游工具读的 `manifest.json`。出镜或不出镜都覆盖；references 里有脚本公式、钩子/标题、不出镜规则、平台规范，以及 MoneyPrinterTurbo / 剪映等下游交接说明。

## Recipe / links
- Repo: https://github.com/lzx0711/talking-head-video-skill（1★，MIT）
- 安装：`npx skills add lzx0711/talking-head-video-skill`
- 技能路径：https://github.com/lzx0711/talking-head-video-skill/tree/main/skills/talking-head-video

## Why it made the cut
SKILL.md 完整（约 10k 字）并带 references，使用边界写得很清楚（只做前期、交给下游渲染）。和目录里已有的口播剪辑、数字人生成不是同一层工作。本窗互动很低，按可验证配方收录。
