# skills CLI（Vercel 出品的 agent skills 包管理器）

**Tags:** meta, tooling, install, package-manager, multi-agent
**Source:** [@Eleazar39456213](https://x.com/Eleazar39456213/status/2116770933813969068) · 2026-11-01
**Engagement:** vercel-labs/skills ~37k★，MIT；wiki 里大量条目的安装命令 `npx skills add …` 都依赖它

## When to use
skill 越装越多、手动复制文件夹到 `.claude/skills` / `.cursor` 等目录变得麻烦时；或者想先试用某个 skill 而不安装、批量检查更新、在多个编程 agent 之间统一管理。

## What it does
统一的 skills 命令行：从 GitHub 仓库搜索、安装（默认装到当前项目，`-g` 全局）、列出、检查更新、更新、移除，并能生成新 skill 模板。支持 Claude Code、Codex、Cursor、OpenCode 等约 80 个 agent。`skills use` 可以不安装就生成该 skill 的提示词，或直接带着它启动指定 agent。

## Recipe / links
- Repo: https://github.com/vercel-labs/skills （需要 Node.js 22.20+）
- 安装某个包里的单个 skill：`npx skills add <owner>/<repo> --skill <name> -a claude-code`
- 常用：`npx skills find [query]`、`npx skills list`、`npx skills check`、`npx skills update`、`npx skills remove`、`npx skills init [name]`
- 不安装试用：`npx skills use <owner>/<repo>@<skill> --agent claude-code`
- 发现 skill：https://skills.sh

## Why it made the cut
不是单个 skill，而是本 wiki 里多数条目共用的安装 / 更新基础设施；有完整命令文档和很强的社区信号。装第三方 skill 前仍建议配合 [SkillSpector](skillspector.md) 或 [skill-guard](skill-guard.md) 先扫一遍。
