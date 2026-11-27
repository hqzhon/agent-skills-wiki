# Blender Skills（arjun988，94 个 MCP 技能）

**Tags:** 3d, blender, mcp, game-assets, skill-pack
**Source:** [@hsianghui](https://x.com/hsianghui/status/2125945423508762903) · 2026-11-26
**Engagement:** 介绍帖 12 赞 / 10 收藏 / 1 转；仓库 [arjun988/blender-skills](https://github.com/arjun988/blender-skills) 现 5,049★，MIT。v1.3.0，2026-07-05 创建，最近推送到 2026-11-06。与已收录的 [Blender Agent Skills（EL4CTEO，28 个技能）](blender-skills.md) 不是同一仓库。

## When to use
要在 Cursor、Claude Code、Kiro 或 Codex 里做 Blender 生产流程（硬表面、重拓扑、UV、材质、绑定，以及导出到 Unreal / Unity / Godot）时用。技能通过 Blender MCP 在本机 Blender 里执行，而不是只生成教程文字。不要把它和 EL4CTEO 的 28 技能包当成同一个安装源。

## What it does
提供 94 个专项技能（.claude/skills 与 .cursor/skills 各一份），把编码 agent 当成技术美术搭档：从 blockout 做到引擎导出。仓库另有 Blender MCP 安装说明和网站 [blender-skills.vercel.app](https://blender-skills.vercel.app/)。README 写明 Anthropic Marketplace 上架仍在审核，目前需从 GitHub 安装。

## Recipe / links
- Repo: https://github.com/arjun988/blender-skills（5,049★，MIT）
- 技能目录：https://github.com/arjun988/blender-skills/tree/main/.claude/skills
- MCP 说明：仓库内 docs/BLENDER_MCP_SETUP.md
- Claude Code：
  ```bash
  git clone https://github.com/arjun988/blender-skills.git
  cp -r blender-skills/.claude/skills /path/to/your/project/.claude/skills/
  ```
- Cursor（Windows 示例，仓库 README 提供）：把 .claude/skills 拷进项目的 .cursor/skills/。Kiro / Codex 同样拷贝技能文件夹后重启 agent。

## Why it made the cut
可安装的完整技能包 + 明确的 MCP 执行路径，使用场景清楚；5k★ 且与目录里已有的 EL4CTEO/blender-skills（Python、28 个技能）互补，不是换了个地址的同一仓库。
