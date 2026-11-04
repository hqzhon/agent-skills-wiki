# Gemini API Skills（Google 官方）

**Tags:** official, gemini, api, sdk, media-generation, skill-pack
**Source:** [@dngzsn37461](https://x.com/dngzsn37461/status/2117905219296346576) · 2026-11-04（引用 [@_philschmid 演示](https://x.com/_philschmid/status/2117674864907608543)）
**Engagement:** 仓库 google-gemini/gemini-skills，~4.4k★，Apache-2.0，Google 官方维护

## When to use
用 Gemini API 写应用，或想让 agent 直接在 shell 里生成图片、TTS 语音、音乐、视频、做 YouTube / 文件分析、Deep Research，而不想每次手写 SDK 胶水代码。

## What it does
官方技能包，目前包含：
- `gemini-api-dev`：用 Interactions API 构建应用（文本、多轮、流式、函数调用、结构化输出、图像 / TTS 生成、managed agents、Deep Research，Python 与 TypeScript SDK，含已弃用模型护栏）
- `gemini-api-cli`：用 `gemini-api` 命令行调用 API（`image` / `tts` / `music` / `video` 子命令、文件与 YouTube 分析、转写、`--jq` / `--body` 脚本化）
- `gemini-live-api-dev`：Live API 实时双向音视频流
- `gemini-omni-flash-api`
Google 自己的评测称加上 skill 后，agent 生成正确 API 代码的比例在 Gemini 3 Flash 上达到 87%，Gemini 3.1 Pro 上达到 96%。

## Recipe / links
- Repo: https://github.com/google-gemini/gemini-skills
- 安装单个：`npx skills add google-gemini/gemini-skills --skill gemini-api-cli`
- 原帖用法：对 agent 说「做封面 + 双人 intro.wav + 写进页面」，它读 SKILL.md 后直接跑 `gemini-api image` / `gemini-api tts`
- 需要 Gemini API key；Vertex AI 版本已迁到 google/skills

## Why it made the cut
官方出品、有评测数据、场景具体（把媒体生成收成 agent 会用的 shell 子命令），可直接安装验证。
