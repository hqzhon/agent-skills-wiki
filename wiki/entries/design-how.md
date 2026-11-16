# design.how（从现有 UI 搭建并迁移设计系统）

**Tags:** design, design-system, tokens, frontend, skill-pack
**Source:** [@hsianghui](https://x.com/hsianghui/status/2122154311266320525) · 2026-11-16
**Engagement:** 发现帖 1 赞 · 仓库 [arla6ka/design.how](https://github.com/arla6ka/design.how) 现 453★ / 37 forks，MIT；站点 [design.how](https://design.how)

## When to use
要对**已经在跑的应用 UI** 说「界面很乱，帮我收拾」：从仓库里抽出设计系统、把界面迁到 token 上、按截图做走查（含无障碍），或生成一款字体 / 一段动态图形。没有 UI 的空仓库不在范围内；只审一个指定页面走 `ui-review`，只文档化一个组件走 `component-docs`。

## What it does
一套互相调度的 Agent Skills。`design-system-boss` 是路由：读现有应用，选 playbook，把步骤抄进 `.design-system/state.md` 再执行；默认在一条 run branch 上提交，不写默认分支。核心技能包括 `build-design-system`、`migrate-design-system`、`token-mapping`、`component-docs`、`ui-review`、`make-font`、`make-motion`。共享词汇表和默认品味在 `build-design-system/references/` 的 `glossary.md` / `taste.md`。另外提供四套可 `shadcn` 安装的设计系统（Glaze / Lime / Quartz / Sodium），以及大量可单独安装的 Vault 视觉技能（例如 `npx skills add https://design.how/vault/warp-type`）。截图类技能需要 Playwright 和 Chromium；`make-font` 还需要 Python 与 fonttools 等。

## Recipe / links
- Repo: https://github.com/arla6ka/design.how（MIT，453★）
- 站点：https://design.how/skills
- 一次装上全部技能：`npx skills@latest add https://design.how`（或 `npx skills@latest add arla6ka/design.how`）
- 只装部分时，记得同时带上 `build-design-system`（共享 glossary / taste），例如：
  `npx skills@latest add arla6ka/design.how --skill build-design-system --skill ui-review`
- Claude Code 插件：`/plugin marketplace add arla6ka/design.how`，再 `/plugin install design-system-skills@design-how`
- 仓库提供 `node evals/run.mjs --lint` 检查技能本身

## Why it made the cut
有完整 `SKILL.md` 群、安装命令、共享品味文件和「不写默认分支」的落地护栏，使用场景是从**你自己的仓库**长出设计系统，而不是套一套现成气质模板。与 [Awesome Design Skills](awesome-design-skills.md)（67 套风格模板检索）和 [UX/UI Agent Skills](ux-ui-agent-skills.md)（可门禁化的 a11y 规范包）互补。
