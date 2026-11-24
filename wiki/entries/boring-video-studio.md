# boring-video-studio（先把内容与分镜批完再交给制作）

**Tags:** video, planning, narration, skill-pack, chinese
**Source:** [@verysmallwoods](https://x.com/verysmallwoods/status/2125036183730213131) · 2026-11-24
**Engagement:** 本窗是口播录音 skill 的更新说明，互动很低 · 仓库 [sugarforever/boring-video-studio](https://github.com/sugarforever/boring-video-studio) 现 195★，MIT，2026-11-24 仍在推送

## When to use
做内容向视频、却不想一上来就渲染时用：先把选题、文章、节拍、口播稿、分场和分镜写成可批准的合同，再交给后续制作。也适用于要在本地用提词器录自己的口播，并保留原音、做重录和字幕校对。

## What it does
一套视频企划 Agent Skills。主技能 `boring-video` 按 `content/TOPIC.md → ARTICLE.md → BEATS.md → NARRATION.md → SCENES.md → STORYBOARD.md` 推进；产品演示、锁定脚本等可跳过文章链，从 HyperFrames 入口进入制作。可选 `listenhub-tts` / `minimax-tts` 做配音字幕；`verysmallwoods-video` 仍覆盖发布、封面和平台文案。本窗更新的 `record-narration` 在本地浏览器提词器里录音，默认可选降噪，保留原录音和前后对照，再交给 agent 做裁剪、规范化和字幕校正。

## Recipe / links
- Repo: https://github.com/sugarforever/boring-video-studio（195★，MIT）
- 安装企划链：
  ```bash
  npx skills add sugarforever/boring-video-studio \
    --skill setup-boring-video-skills boring-video develop-topic to-article to-spec-beats to-narration to-scenes to-storyboard to-video record-terminal
  ```
- 口播录音 skill：`skills/boring-video/record-narration/SKILL.md`
- 后续成片依赖 [HyperFrames](https://www.hyperframes.dev)；TTS 技能会用到 ListenHub / MiniMax，用前先看其账号与费用。

## Why it made the cut
可加载的多步企划配方，场景清楚，MIT 仓库和安装命令齐全。本窗补充了可本地运行的口播录音步骤。和已收录的 Remotion / BB-Video / Muse Video 等成片技能互补：这条先把内容和分镜批完，而不是直接出片。
