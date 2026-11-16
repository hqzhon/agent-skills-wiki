# ECC（Agent 工程系统 / 技能棚）

**Tags:** skill-pack, agent-harness, memory, hooks, engineering, meta
**Source:** [@VaibhavSisinty](https://x.com/VaibhavSisinty/status/2122366618705797317) · 2026-11-17
**Engagement:** 发现帖为当周 Top 10 技能盘点（59 赞 / 104 书签）；仓库 [affaan-m/ECC](https://github.com/affaan-m/ECC) 现约 305k★ / 4.5 万 forks（GitHub API 304,622★），MIT。Alyn 本周榜亦将其列为 Agent Harness Construction，周增约 2.8k★。站点 [ecc.tools](https://ecc.tools)。

## When to use
要用 Claude Code、Codex、Cursor、Kimi Code 等编码助手，但希望它们按同一套工程系统工作：先规划、用测试验证、换新鲜上下文做评审、记住跨会话要点，并把重复成功的做法沉淀成可复用 skill。不要把整个仓库一次性塞进每次对话；ECC 用按需加载的 skills、子 agent、可选 rules 和 hooks 把职责拆开。只想要某一个垂直技能（例如单一设计包）时，不必上整套 harness。

## What it does
MIT 开源的「agent harness 操作系统」（README 称 2.2.3）：约 327 个按需加载的工作流 skill、72 个专职子 agent、98 个兼容斜杠命令，以及 hooks、instincts（从会话里学到的模式）和 AgentShield（扫描提示词、hooks、MCP 配置、权限和密钥）。核心流程是 plan → test → implement → review → verify → remember → improve。另有 Unified Memory（`ecc-universal` CLI / 可选 MCP）在项目范围内保存可移植记忆。OSS 仓库保持免费；ECC Pro 是面向私有仓的托管 GitHub App（单独付费），与开源技能包分开。

## Recipe / links
- Repo: https://github.com/affaan-m/ECC（MIT，约 305k★）
- 文档 / 站点：https://ecc.tools
- 推荐安装（Node.js 18+；Claude 插件还需 Git 与 Claude Code 2.1+）：
  ```bash
  npx ecc-universal@2.2.3 setup
  ```
  多 harness（Claude Code / Codex / Kimi Code）可用 `npx ecc-universal@2.2.3 install --guided`。
- Claude Code 原生插件（不要再叠一套手动全量安装）：
  ```text
  /plugin marketplace add https://github.com/affaan-m/ECC
  /plugin install ecc@ecc
  ```
- Codex：
  ```bash
  codex plugin marketplace add affaan-m/ECC
  codex plugin add ecc@ecc
  ```
- 只从官方渠道安装：GitHub 仓库、npm 包 `ecc-universal` / `ecc-agentshield`、插件标识 `ecc@ecc`、网站 ecc.tools。第三方镜像不被维护。

## Why it made the cut
完整可加载的工程技能棚：有明确使用场景、官方安装路径、大量可核验的 SKILL.md / agents / hooks，许可证为 MIT。社区信号极高（约 30 万★），且本窗口有独立盘点帖和 Alyn 周榜背书。此前目录未收录，属于高信号补录。付费 Pro 只覆盖托管 GitHub App，不改变开源技能包本身。
