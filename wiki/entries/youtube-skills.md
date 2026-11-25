# YouTube Skills（ZeroPointRepo：转写 / 搜索 / 频道）

**Tags:** youtube, transcript, research, captions, skill-pack
**Source:** [@heyrimsha](https://x.com/heyrimsha/status/2125207339993276815) · 2026-11-24
**Engagement:** 本窗盘点帖提到；仓库 [ZeroPointRepo/youtube-skills](https://github.com/ZeroPointRepo/youtube-skills) 现 1,230★，MIT，2026-11-03 仍有推送

## When to use
编码 agent 需要 YouTube **字幕/转写、搜视频、看频道或播放列表**时用——哪怕用户只是贴了一个链接，要摘要、引用、翻译或核对事实。不要用它上传或管理账号。和已收录的 [YouTube Agent Skill](youtube-agent-skill.md)（频道运营：脚本/标题/留存，不代发）不是同一包。

## What it does
一套面向 agent 的 YouTube 技能，走 [TranscriptAPI](https://transcriptapi.com) 而不是 yt-dlp 或无头浏览器。README 推荐先装 `youtube-full`（转写 + 搜索 + 频道 + 播放列表）；仓库里还有 `transcript`、`captions`、`subtitles`、`youtube-api`、`youtube-data` 等分项，并带 OpenClaw / Hermes 的副本目录。`transcript` 技能声明需要 `TRANSCRIPT_API_KEY`（站点称有免费额度，100 credits，不绑卡）。

## Recipe / links
- Repo: https://github.com/ZeroPointRepo/youtube-skills（1,230★，MIT）
- 推荐：`npx skills add ZeroPointRepo/youtube-skills --skill youtube-full`
- 一次装全部：`npx skills add ZeroPointRepo/youtube-skills`
- 其它 runtime：`npx clawhub@latest install youtube-full`，或 `hermes skills install skills-sh/ZeroPointRepo/youtube-skills/skills/youtube-full`
- 注意：核心能力依赖第三方 TranscriptAPI，配额和隐私以该服务条款为准；装前先准备或让 agent 协助申请 key。

## Why it made the cut
高星漏收：可加载技能多、使用场景清楚（读/搜 YouTube，而不是做频道运营），1,230★、MIT。必须标明对 TranscriptAPI 的依赖。本窗来自盘点帖，按仓库信号补上，并与 youtube-agent-skill、Hype Meter 写清分工。
