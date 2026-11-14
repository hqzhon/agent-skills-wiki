# ghost-qa（真浏览器闭环 QA）

**Tags:** testing, qa, playwright, frontend, a11y, skill
**Source:** [@FoundryVibe](https://x.com/FoundryVibe/status/2121530062575174091) · 2026-11-14
**Engagement:** 发现帖互动低；仓库 [avivgerz-hue/ghost-qa](https://github.com/avivgerz-hue/ghost-qa) 23★，2 forks，MIT；有 npm 包和 CI

## When to use
刚改过页面、路由、表单、样式或客户端数据请求，准备向用户说「UI 做完了」之前，要让 agent 在真实无头浏览器里验收，而不是只靠单测、类型检查和 lint。也适用于修过只在浏览器里复现的 bug。

## What it does
一条很长的 SKILL.md，把「Staff QA」写成必须按顺序走完的五段闭环，目标是 QA Health Score 95–100（A+）、无严重/主要问题、无新增回归：

- 先做 doctor 就绪检查
- 8-Trap 深度巡检：Desktop / Tablet / Mobile × 浅色/深色
- 把 DOM 问题映射回源码并做小范围修复
- 用对比（`ghost_qa_compare`）做闭环验证

它明确不是单测/E2E 套件或完整 WCAG 人工审计的替代。引擎会看 hydration、布局、网络、对比度和焦点等问题——这些是类型检查看不到的。同作者套件还有 [vibe-shield](vibe-shield.md) 和 [unslop](unslop.md)。

## Recipe / links
- Repo: https://github.com/avivgerz-hue/ghost-qa
- SKILL.md: https://github.com/avivgerz-hue/ghost-qa/blob/main/SKILL.md
- 运行：`npx -y ghost-qa@latest test http://localhost:3000`
- 也可作为 Agent Skill / MCP 接入编码 agent

## Why it made the cut
使用场景非常具体（前端交稿前的真机验收），有分阶段协议、Health Score 和可安装的 Playwright 工具，仓库带 CI 与 npm 包。和 [tethertrace](tethertrace.md)（真机 Android）不重复，这条专攻 Web UI。
