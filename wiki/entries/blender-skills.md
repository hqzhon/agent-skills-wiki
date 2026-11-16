# Blender Agent Skills（28 个 Blender 全流程技能）

**Tags:** 3d, blender, skill-pack, python, game-assets
**Source:** [@27huff](https://x.com/27huff/status/2122165209376993338) · 2026-11-16
**Engagement:** 发现帖互动很少 · 仓库 [EL4CTEO/blender-skills](https://github.com/EL4CTEO/blender-skills) 现 1,246★ / 119 forks，MIT

## When to use
要让 Claude Code / Codex / Cursor / Gemini CLI / Copilot 等编码 agent 在 **Blender 5.2 LTS 或更新版本**（作者在 5.3 上逐项验证）里做建模、UV、PBR、烘焙、绑骨、动画、导出或质检。需要本机安装 Blender；可选 Blender MCP 以便在已打开的会话里操作，否则 agent 会无头跑 Blender。不要用它替代 [image-to-sculpt](image-to-sculpt.md) 那种「按一张图度量雕刻」的专用流程，也不要指望它在没装 Blender 的环境里凭空出 mesh。

## What it does
28 个可加载技能，覆盖 3D 资产全流程。`blender-core` 是入口：负责运行 bpy、任务分发，以及 5.x API 规则；其余按任务拆开，例如 `blender-hardsurface-modeling`、`blender-retopology-uv`、`blender-pbr-materials`、`blender-texture-baking`、`blender-character-rigging`、`blender-animation`、`blender-export-pipelines`（Roblox / Unity / Unreal / Godot / web / USD）、`blender-asset-qa`（检查 z-fighting、法线、权重和贴图）和 `blender-workflow-recipes`（完整资产剧本）。作者声称脚本在真实 Blender 里测过。

## Recipe / links
- Repo: https://github.com/EL4CTEO/blender-skills（MIT，1,246★）
- Claude Code 插件：
  ```
  /plugin marketplace add EL4CTEO/blender-skills
  /plugin install blender-agent-skills@blender-agent-skills
  ```
- 通用安装（默认写入 `~/.claude/skills` 与 `~/.agents/skills`）：
  ```bash
  git clone https://github.com/EL4CTEO/blender-skills
  ./blender-skills/install/install.sh          # macOS / Linux
  # Windows: .\blender-skills\install\install.ps1
  ```
  可用 `--agent claude|codex|opencode|gemini|copilot|cursor|all`，或 `--project DIR` 只装到某个项目。
- 建议升级到 Blender 5.3.0（KTX2 导出、合成器效果栈、Gaussian splats）；5.2 LTS 仍可用。

## Why it made the cut
有 28 份完整 `SKILL.md`、安装脚本和明确的 Blender 版本要求，仓库许可与星标都够清楚。它补上了 wiki 里「通用 Blender 制作管线」这一块：现有的 [image-to-sculpt](image-to-sculpt.md)、[grey2art](grey2art.md)、[dream-loop](dream-loop.md) 更偏按图雕刻、风格化场景或截图闭环，不是这套分技能的全流程包。
