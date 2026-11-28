# reel-animated-explainer（口播视频做成动画解说 Reel）

**Tags:** video, reels, remotion, captions, explainer, skill
**Source:** [@J_srv001](https://x.com/J_srv001/status/2126592976231317518) · 2026-11-28
**Engagement:** 作者介绍帖 10 赞 / 1 书签 / 4 回复，称已自用约两个月；仓库 [srvjha/reel-animated-explainer](https://github.com/srvjha/reel-animated-explainer) 现 5★，MIT，2026-09-27 建仓，本窗仍有推送。README 带 Instagram 样片。

## When to use
你已经录好一段竖屏口播（最好再给逐字稿），想做成带逐词字幕、讲解动画、配乐和音效的解说 Reel，又不想在时间线上手拖关键帧时用。每一帧由代码渲染（Remotion / 经典 Python 管线），不走视频生成模型。它和已收录的 [Reelsmith Media](reelsmith-media.md)（已有分镜素材和配音，只要拼成片）、[wallstreet-explainer](wallstreet-explainer.md)（财经解说腔 + 新闻画面）、[Moodreel](moodreel.md) / [motlab](motlab.md)（从参考片或镜头脚本写新片）不是同一条。

## What it does
把 1080×1920 口播视频交给 Claude 后，技能会：归一化帧率、用 whisper.cpp 转写并对齐你的逐字稿、按你开口的时间点安排示意图、写动画、先出预览帧修溢出，再混缩到约 30 MB 以内的成片，并抽检最终文件。推荐用法是 Claude Code 插件 `reel-studio`（`/edit-reel`），带 27 个可按需安装的主题，也可让它按你的色彩和参考做新主题。另有旧版 `reel-classic` 技能：用 Pillow/FFmpeg 做「上方面板 + 下方真人」或抠像全屏。任何能跑代码的 agent 也可以只加载 `skill/reel-animated-explainer/SKILL.md` 这份剧本。

硬性规则包括：逐字稿只断行不改写、标题和字幕避免孤词、预览后再出成片、真实产品截图不得捏造。

## Recipe / links
- Repo: https://github.com/srvjha/reel-animated-explainer（5★，MIT）
- Claude Code 插件（推荐）：
  ```text
  /plugin marketplace add srvjha/reel-animated-explainer
  /plugin install reel-studio@reel-animated-explainer
  ```
  然后 `/reel-studio:edit-reel ./my-video.mp4`，或直接附上视频说「edit this reel」。
- 只用技能文件：https://github.com/srvjha/reel-animated-explainer/blob/main/skill/reel-animated-explainer/SKILL.md
- 依赖：Node.js 与 ffmpeg；插件主题按需安装。样片见作者 Instagram [@srvjha.official](https://www.instagram.com/srvjha.official/)

## Why it made the cut
有可加载技能、插件、主题和可看的成片，步骤和检查项写得很具体。星数还少，但作者第一方说明和仓库材料对得上，值得单列。
