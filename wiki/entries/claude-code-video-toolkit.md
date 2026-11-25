# claude-code-video-toolkit（brief 到已质检的 MP4）

**Tags:** video, claude-code, remotion, tts, ffmpeg, skill-pack
**Source:** [@0xClaudAI](https://x.com/0xClaudAI/status/2125267294783680939) · 2026-11-24
**Engagement:** 本窗为「10 个 GitHub 视频工具」盘点帖（39 赞）提到；仓库 [digitalsamba/claude-code-video-toolkit](https://github.com/digitalsamba/claude-code-video-toolkit) 现 2,751★，MIT，2026-11-24 仍在推送

## When to use
要把一份 brief 做成解说/演示短片，或单独调用配音、配乐、图片、镜头和渲染工具时用。技能按提交场景说明、轮询任务、取回质检过的 MP4 来写，不绑死某一种 agent 后台实现。需要本机或云端 GPU/存储来跑开源模型（也可先看免费示例）。

## What it does
主技能 `skills/video-toolkit/SKILL.md`（name: `video_toolkit`），另有 Remotion、ffmpeg、Blender、Qwen TTS、ACE-Step、LTX 等配套技能。模板覆盖 sprint review、产品演示、release notes、教程、竖屏解说和黑板讲解。默认偏向开源模型（Qwen3-TTS、FLUX.2、ACE-Step 等），部署到你自己的云 GPU 账户按用量计费；Cloudflare R2 / Modal 有免费额度说明。仓库为 Claude Code 设计，另有实验性 Codex / Kiro CLI 迁移脚本。

## Recipe / links
- Repo: https://github.com/digitalsamba/claude-code-video-toolkit（2,751★，MIT）
- 安装：`git clone https://github.com/digitalsamba/claude-code-video-toolkit.git`，用 [uv](https://docs.astral.sh/uv/) 执行 `uv sync`（也可先安装 uv）。
- 要求：Node.js 22+（推荐 24 LTS）、Claude Code；uv 推荐；FFmpeg 可选。
- 在 Claude Code 里：`/setup` 配置 GPU/存储/语音，`/video` 按模板做第一支片子。
- 想先看成品、跳过云配置：`cd examples/hello-world && npm install && npm run render`（无需 API key，直接出 MP4）。
- Codex / Kiro 迁移见仓库 `docs/codex.md`、`docs/kiro.md`。

## Why it made the cut
高星漏收：可加载技能数量多、主技能把 brief→质检 MP4 的合同写清楚，和 HyperFrames（HTML 成片）、Video Podcast Maker（主题解说播客）互补。2,751★、MIT，当日仍在维护。本窗来自盘点帖，按仓库信号补上；云 GPU 费用需自己评估。
