# Microsoft Skills（Azure / Foundry 官方）

**Tags:** official, microsoft, azure, foundry, sdk, skill-pack
**Source:** [@Astrodevil_](https://x.com/Astrodevil_/status/2125446900103209152) · 2026-11-25
**Engagement:** 本窗官方盘点帖（0 赞）；仓库 [microsoft/skills](https://github.com/microsoft/skills) 现 3,245★，MIT，2026-11-20 仍有推送。README 标明仓库仍在活跃开发。

## When to use
编码 agent 要写 Azure SDK 或 Microsoft Foundry 相关代码、查 AKS / 成本 / 可观测性，或需要配套 AGENTS.md 与 MCP 配置时用。不要和 [APM](microsoft-apm.md)（包管理器）或 [SkillOpt](microsoft-skillopt.md)（训练 SKILL.md）混淆。

## What it does
官方技能、自定义 agent、AGENTS.md 模板和 MCP 配置，用来把编码 agent 锚定在当前 Azure / Foundry SDK 写法上。文档站写明可浏览约 175 个技能并一键安装；仓库树里能看到 200+ 个 SKILL.md，按 AKS、Advisor、成本、可观测性，以及各语言 Azure SDK（如 .NET）等插件分组。带评测与 Copilot SDK 测试工作流。

## Recipe / links
- Repo: https://github.com/microsoft/skills（3,245★，MIT）
- 文档 / 浏览：https://microsoft.github.io/skills/
- 博客：https://devblogs.microsoft.com/all-things-azure/context-driven-development-agent-skills-for-microsoft-foundry-and-azure/
- 安装：`npx skills add microsoft/skills`（向导里勾选需要的技能）

## Why it made the cut
Microsoft 官方、可加载的 Azure / Foundry 技能目录，场景清楚，有文档站和安装命令。3,245★、MIT。本窗按官方盘点补收；仓库自称仍在扩充，装前以文档站清单为准。
