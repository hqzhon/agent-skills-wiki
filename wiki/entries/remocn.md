# Remocn（用组件库给 Remotion 做演示/发布视频）

**Tags:** video, remotion, components, mcp, skill-pack
**Source:** [@forevercompo](https://x.com/forevercompo/status/2125388129506869565) · 2026-11-25
**Engagement:** 本窗设计/动效盘点帖（0 赞）列为第 1 项、当时约 1,856★；仓库 [Remocn/remocn](https://github.com/Remocn/remocn) 现 1,869★，MIT，2026-11-24 仍有推送

## When to use
已经（或准备）用 Remotion 做产品演示、发布视频、changelog 或社交短片，希望 agent 先分镜、再从组件库安装镜头并成片时用。它不是 [Remotion 官方技能](remotion-skills.md) 的替代：官方包教 Remotion API 与工程实践，这边提供约 935 个 MIT 组件和一条 brief → 分镜 → 安装 → 合成的工作流。注意：Remotion 本身对超过 3 人的公司需要付费许可。

## What it does
Claude Code 插件 / Agent Skill / MCP。`/remocn:video` 走 brief → 分镜（会在写代码前停下来让你改方向）→ 用 shadcn CLI 把组件装进 Remotion 项目 → 合成 → `scene-reviewer` 抽帧检查裁字、空镜和低对比。技能包括 `remocn`、`video`、`setup`、`add`、`changelog`。也可单独把 MCP 接到 `https://remocn.dev/mcp`。

## Recipe / links
- Repo: https://github.com/Remocn/remocn（1,869★，MIT）
- 站点 / 文档：https://remocn.dev
- 通用：`npx skills add Remocn/remocn`
- Claude Code：`/plugin install remocn --marketplace Remocn/remocn`
- Codex：`codex plugin marketplace add Remocn/remocn` 然后 `codex plugin add remocn@remocn`
- 前置：Remotion；在空目录里插件可代为创建项目，手动则 `npx create-video@latest`

## Why it made the cut
可加载技能 + 组件注册表 + 分镜门禁，和官方 Remotion skills 互补。1,869★、技能仓为 MIT；公司规模超过 3 人时仍要遵守 Remotion 许可证。
