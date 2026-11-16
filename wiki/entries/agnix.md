# agnix（Agent 配置 linter / LSP）

**Tags:** devtools, linter, skill-safety, lsp, meta
**Source:** [@hsianghui](https://x.com/hsianghui/status/2121898878244904971) · 2026-11-15
**Engagement:** 4 likes / 6 replies · 仓库 [agent-sh/agnix](https://github.com/agent-sh/agnix) 现 484★，MIT / Apache-2.0

## When to use
在 Claude Code、Codex、Cursor、Copilot、OpenCode 等环境里维护 `CLAUDE.md`、`SKILL.md`、hooks、MCP 或 `AGENTS.md`，担心字段写错会导致技能被静默忽略，想在安装或提交前先 lint，并尽量自动修复。

## What it does
开源的 agent 配置 linter 与 LSP（Rust），宣称 760+ 条规则，覆盖多种编码助手的技能和配置文件，带 autofix。提供 CLI、GitHub Action，以及 VS Code / JetBrains / Neovim / Zed 插件。它本身不是一条可加载的 SKILL.md，而是装技能之前的卫生工具，和 SkillSpector（安全扫描）互补：一个查「写得对不对、会不会被忽略」，一个查「安不安全」。

## Recipe / links
- Repo: https://github.com/agent-sh/agnix（484★，MIT / Apache-2.0）
- npm：https://www.npmjs.com/package/agnix ；crates：`agnix-cli`
- GitHub Action：https://github.com/marketplace/actions/agnix-ci
- VS Code 扩展：https://marketplace.visualstudio.com/items?itemName=avifenesh.agnix
- 文档：https://agent-sh.github.io/agnix/

## Why it made the cut
可验证的开源工具、使用场景清楚（配置写错会静默失败），许可证双许可，和目录里已有的 SkillSpector / skill-guard 是同一类安装卫生能力，但切入点是 lint + autofix。
