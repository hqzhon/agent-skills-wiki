# Compose Skill（Jetpack Compose 七件套）

**Tags:** android, compose, kotlin, multiplatform, skill-pack
**Source:** [@BIGBULLapp](https://x.com/BIGBULLapp/status/2119564545387577594) · 2026-11-09
**Engagement:** 1 like / 0 reposts / 1 reply / 0 bookmarks · Meet-Miyani/compose-skill · MIT · 303★

## When to use
你让 coding agent 写 Jetpack Compose 或 Compose Multiplatform，希望它按同一套房屋风格产出（MVI、Koin、Navigation 3、Ktor、Room），而不是每次重新发明架构。若项目已有自己的 Hilt / MVVM / Navigation 2 约定，技能应跟随现有模式，迁移另议。

## What it does
七个技能组成的 Compose Kit：入口树 `compose`（约 1.3k tokens，按任务类型路由到参考文件），加上 `compose-architecture`、`compose-feature`、`compose-ui`、`compose-data`、`compose-project`、`compose-platform`。覆盖模块图、MVI/`BaseViewModel`、特性切片（合同 → ViewModel → UI → 导航 → DI → 测试）、稳定性与无障碍、数据层（Ktor/Room/DataStore/Paging 3）、新项目脚手架，以及 `commonMain` / `expect`/`actual`。作者用多模型做了盲评（宣称 Gemini 3.8 Flash +30.8、GPT-6-Luna +23.1 等），仓库带 90 个 fixture / guard 测试。不同于 Google 官方 [android/skills](android-official-skills.md)（Compose 迁移、AGP、R8），这是第三方房屋风格包。

## Recipe / links
- Repo: https://github.com/Meet-Miyani/compose-skill （MIT）
- 网站与分 agent 安装：https://compose.avinya.dev/  ·  https://compose.avinya.dev/install/
- 适用：Claude Code、Codex、Cursor、OpenCode、Copilot、Gemini CLI、Antigravity、Android Studio
- 入口技能在 `skills/compose`，其余六个按路由按需加载

## Why it made the cut
有可安装的七件套、分 agent 指南和评测/CI，不是「请写好一点的 Compose」一句提示；303★，和官方 Android skill 包职责不重叠。
