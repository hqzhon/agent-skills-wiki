# .NET Agent Skills（官方，带评测看板）

**Tags:** dotnet, csharp, official, skill-pack, evals
**Source:** [@1kevgriff](https://x.com/1kevgriff/status/2120197548006887443) · 2026-11-10
**Engagement:** dotnet/skills ~5.9k★ · .NET 团队维护

## When to use
用 Claude Code、Codex、Copilot、Cursor 等编码 agent 写 .NET / C# 项目时：构建失败诊断、MSBuild 调优、NuGet 依赖治理、框架升级迁移、性能排查、EF 数据访问、MAUI / Blazor / ASP.NET Core、.NET 里的 AI 与 RAG。

## What it does
.NET 团队维护的可移植 skills + 宿主专属 custom agents，按插件拆分（dotnet、dotnet-advanced、dotnet-data、dotnet-diag、dotnet-msbuild、dotnet-nuget、dotnet-upgrade、dotnet-maui、dotnet-ai、dotnet-test 等 17 个）。最大特点是公开 [Skill Value 看板](https://dotnet.github.io/skills/)：按插件、skill、执行模型和评审模型对比 token 用量、耗时、激活率和未通过率；原帖提到 C# expert skill 在 Sonnet 5 上省 41% token、快 73%，也有 skill 如实标「暂无明确结论」。

## Recipe / links
- Repo: https://github.com/dotnet/skills
- 看板: https://dotnet.github.io/skills/
- 遵循 Agent Skills / Agent Plugins 1.0 规范；Claude/Cursor 插件清单都在仓库里（`.claude-plugin`、`.cursor-plugin`）

## Why it made the cut
官方出品、覆盖面广，而且是少见的「带评测数据」的技能库，可以验证某个 skill 到底有没有用。
