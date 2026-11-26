# SoundKit（给 Remotion 视频做逐帧音效）

**Tags:** audio, sfx, remotion, video, shadcn, skill
**Source:** [@SahilPanhotra](https://x.com/SahilPanhotra/status/2125876896688963853) · 2026-11-26
**Engagement:** 介绍帖 4 赞 / 1 收藏；仓库 [soundza/soundkit](https://github.com/soundza/soundkit) 现 16★。代码 MIT，随仓库分发的 250 条音效/床垫为 CC0、非 AI 生成；技能文件在 `skills/soundza-remotion/SKILL.md`。

## When to use
要给 **Remotion** 合成片加音效或床垫，希望 whoosh 落在剪辑点、打击落在标题/Logo 的**精确帧**上时用。也可以用 shadcn 命令把随仓库提供的 225 条音效 + 25 条音乐床垫装进项目。不要把它当成通用游戏音效包——那更接近已收录的 [sfx-skill](sfx-skill.md)；本技能面向 Remotion 成片。

## What it does
两部分：① 一份 shadcn registry，可一条命令加入带 `sync_ms`（命中点）的 CC0 音效；② 给 Claude Code / Codex / Cursor 用的 agent skill，会找出需要声音的位置，在 Soundza 曲库里搜索，只下载用到的条目，并按命中点对齐到帧。技能脚本是无依赖的 `scripts/soundza.mjs`（Node 18+）。搜索完整曲库需要 `SOUNDZA_API_KEY`（或跑 `soundza signin` 在浏览器里授权）。曲库条目采用 Soundza Standard License（个人/商用免版税，致谢可选），与仓库内那 250 条 CC0 不是同一许可。

## Recipe / links
- Repo: https://github.com/soundza/soundkit（16★；代码 MIT，随附音频 CC0）
- 浏览试听：https://soundza.com/soundkit
- 技能：https://github.com/soundza/soundkit/blob/main/skills/soundza-remotion/SKILL.md
- 安装技能：`npx skills add soundza/soundkit`
- 添加单条音效示例：`npx shadcn add https://soundza.com/r/air-whoosh.json`

## Why it made the cut
可加载技能 + 带命中点的音效库，场景（Remotion 逐帧对齐）清楚，和 sfx-skill 的合成/采音路线互补。介绍帖热度一般，按可验证仓库收录；用完整曲库搜索前要准备 API key / 登录。
