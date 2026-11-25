# Godot Agent Skills（EL4CTEO，面向 Godot 4.7）

**Tags:** godot, gamedev, gdscript, csharp, skill-pack
**Source:** [@ai_algoit](https://x.com/ai_algoit/status/2125435662598111587) · 2026-11-25
**Engagement:** 本窗介绍帖 0 赞；仓库 [EL4CTEO/godot-skills](https://github.com/EL4CTEO/godot-skills) 现 51★，MIT，2026-11-21 仍有推送。作者已有条目 [fast-anything](fast-anything.md)、[blender-skills](blender-skills.md)。

## When to use
要用编码 agent 在 **Godot 4.7+** 里做游戏（GDScript 或 C#），并且希望它查你本机引擎里的真实 API、通过编辑器改场景，再用编译 / 测试 / 导出验收时用。和已收录的 [godot-agent](godot-agent.md)（`gda` CLI / MCP，无头或运行时验证）互补：这边是 27 个按领域拆开的技能包，那边是可脚本化的验证层。Web 导出请选 GDScript——Godot 4.x 的 C# 项目不支持 Web。

## What it does
27 个技能，覆盖 core、GDScript / C#、2D / 3D、渲染、动画、物理、UI、输入、音频、shader、网络、关卡导航、XR、测试、导出 CI、从 3.x / 旧 4.x 迁移等。技能从已安装的引擎查 API，不靠模型记忆；示例代码由测试套件在 Godot 4.7.2 上编译。作者建议用 .NET 版 + C#，因为编译器能在运行前抓住类型错误。

## Recipe / links
- Repo: https://github.com/EL4CTEO/godot-skills（51★，MIT）
- Claude Code：`/plugin marketplace add EL4CTEO/godot-skills` → `/plugin install godot-agent-skills@godot-agent-skills`
- 其他宿主：

```bash
git clone https://github.com/EL4CTEO/godot-skills
./godot-skills/install/install.sh          # macOS / Linux
# Windows: .\godot-skills\install\install.ps1
```

- 依赖：Godot 4.7 或更新；Python 3.9+；若用 C# 还需 .NET 8 SDK 或更新

## Why it made the cut
可加载的 27 技能包，强调「查本机 API + 真编译验收」，和 godot-agent 不是同一仓库。51★、MIT，星数一般，但配方和版本门槛写得很清楚。
