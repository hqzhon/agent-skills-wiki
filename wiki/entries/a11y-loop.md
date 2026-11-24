# a11y-loop（先写出无障碍 UI，再用真浏览器审计）

**Tags:** a11y, accessibility, frontend, audit, skill
**Source:** [@chanmeng666](https://x.com/chanmeng666/status/2124964644603465858) · 2026-11-24
**Engagement:** 本窗为作者对 0.4.1 实跑输出的说明，互动很低 · 仓库 [ChanMeng666/a11y-loop](https://github.com/ChanMeng666/a11y-loop) 现 2★，MIT，npm 包与评测、文档齐全，2026-07 起持续维护

## When to use
让编码 agent 默认按无障碍方式写 UI，并且不只做静态检查：在真实浏览器里审计已渲染页面，修得了的修，查不了的明确告诉你。

## What it does
一套 Agent Skill + CLI：先约束 agent 的写入，再对页面做可验证的浏览器审计，并区分「已证明」和「无法证明」。仓库含 `skills/a11y-loop/SKILL.md`、CLI、GitHub Action、evals 与文档站点。

## Recipe / links
- Repo: https://github.com/ChanMeng666/a11y-loop（2★，MIT）
- npm: https://www.npmjs.com/package/a11y-loop
- 文档: https://ChanMeng666.github.io/a11y-loop/
- 跨 agent 安装：
  ```bash
  npx skills add ChanMeng666/a11y-loop -g -y
  ```
- Claude Code 插件：
  ```bash
  claude plugin marketplace add ChanMeng666/a11y-loop
  claude plugin install a11y-loop@chanmeng-a11y-loop --scope user
  ```

## Why it made the cut
星数低，但材料完整：可加载 skill、CLI、评测和作者本窗贴出的真实运行输出，使用场景清晰。和已收录的 jakubkrehel Interface Skills（含 a11y 原则）以及 Chrome DevTools 的 `a11y-debugging` 技能互补——本包把「写入 + 浏览器复验」收成一条回路。
