# godot-agent（用 CLI/Skill/MCP 做可验证的 Godot 原型）

**Tags:** godot, gamedev, cli, mcp, skill
**Source:** [@vincentjuan0507](https://x.com/vincentjuan0507/status/2123272554773188883) · 2026-11-19
**Engagement:** 中文介绍帖（约 2 赞）；仓库 [aigengame/godot-agent](https://github.com/aigengame/godot-agent) 58★，MIT，PyPI 包名 `gda`。

## When to use
要用编码 agent 参与 Godot 4.6+ 项目：改场景/脚本之后需要无头验证能否启动、错误在哪，或在运行中的游戏里读状态、模拟输入、抓视口时使用。需要本机（或 CI）有 Godot 可执行文件。

## What it does
`gda` 是面向 agent 的 Godot 自动化层，三条入口共用同一套操作：CLI、仓库里的 `gda` Agent Skill（`npx skills add`）、以及 MCP server。两种模式：① **Headless** 创建/检查场景、节点、脚本、资源并校验、导出，不必开编辑器；② **Live** 通过项目内 daemon 检查运行时树和状态、注入输入、抓帧、读日志与性能。命令加 `--json` 只在 stdout 输出一个结构化对象，失败时按 `error.code` 分支，而不是解析人类可读报错。

## Recipe / links
- Repo: https://github.com/aigengame/godot-agent（MIT，58★）
- 站点: https://aigengame.xyz/ · PyPI: https://pypi.org/project/gda/
- 安装：
  ```bash
  uv tool install gda    # 或 pipx install gda
  npx skills add aigengame/godot-agent --skill gda -g
  ```
  然后让 agent 读 skill，为项目配好 Godot 路径（`GDA_GODOT` 或 `--godot`），再用 `gda info --json` 检查。
- 依赖：Python 3.13+、Godot 4.6+（macOS / Linux / Windows；Windows 用 `*_console.exe`）。

## Why it made the cut
把「生成代码之后场景能不能跑」写成可验证闭环：skill + CLI + MCP，输出是 agent 能分叉的 JSON，而不是只能打开编辑器肉眼看。有明确的 Godot 版本门槛和安装路径。
