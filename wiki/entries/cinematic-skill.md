# Cinematic Skill（纯代码旁白电影）

**Tags:** video, documentary, skia, python, skill
**Source:** [@Alexvx_nft](https://x.com/Alexvx_nft/status/2122436232462700763) · 2026-11-17
**Engagement:** 出现在内容工具盘点帖（33 赞 / 10 书签）；仓库 [Moh4696/cinematic-skill](https://github.com/Moh4696/cinematic-skill) 现 635★ / 93 forks，MIT，带 CI。作者与已收录的 [Open 3D Skills](open-3d-skills.md) 为同一人。建于 2026-11-09。

## When to use
想让编码 agent 做一部有旁白的纪录片 / 品牌片 / 科普片：镜头在照片、地图、卡片和数字之间连续滑过，每个视觉落点对准旁白的词。适合「做一条关于……的电影 / 纪录片 / explainer」。它在本地用代码（Python + Skia）渲染，不是给 Runway / Seedance 写提示词——前期策划见 [Muse Video Skill](muse-video-skill.md)；three.js + Remotion 短片见 [Claude Animated Shorts](claude-animated-shorts.md)。

## What it does
`skills/cinematic-film/SKILL.md` 覆盖剧本、任意 TTS 旁白切成带时间轴的句子、图片来源（档案版权、自有照片或 AI 静帧）、节拍表、场景、自检静帧，以及省内存的并行渲染。成品是一个镜头在一块「证据板」世界上移动，配可选配乐、音效和烧录字幕。仓库有示例成片、`PROMPT.md` 和多 agent 插件包装（Claude Code / Codex / Cursor / Gemini）。

## Recipe / links
- Repo: https://github.com/Moh4696/cinematic-skill（MIT，635★）
- SKILL.md：https://github.com/Moh4696/cinematic-skill/blob/main/skills/cinematic-film/SKILL.md
- 安装：`npx skills add Moh4696/cinematic-skill`（需 Node 22.20+）
- Claude Code：`/plugin marketplace add Moh4696/cinematic-skill` 后 `/plugin install cinematic-skill@cinematic-skill`
- Codex：`codex plugin marketplace add Moh4696/cinematic-skill` 后 `codex plugin add cinematic-skill@cinematic-skill`
- Gemini：`gemini extensions install https://github.com/Moh4696/cinematic-skill`
- 依赖：`pip install -r requirements.txt`（skia-python、numpy、pillow）

## Why it made the cut
可加载 skill + 示例 + CI，安装路径清楚，MIT。与同作者的 Open 3D Skills（网页 3D / 滚动影片）以及仓库里其他成片技能互补：这条专攻「旁白对准画面的代码电影」。社区信号中等偏好（635★，约一周新仓），材料足够核验。
