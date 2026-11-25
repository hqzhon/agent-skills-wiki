# Vercel Agent Skills（官方技能包）

**Tags:** official, vercel, react, nextjs, performance, skill-pack
**Source:** [@Astrodevil_](https://x.com/Astrodevil_/status/2125446900103209152) · 2026-11-25
**Engagement:** 本窗为 9 家官方技能包盘点帖（0 赞）；仓库 [vercel-labs/agent-skills](https://github.com/vercel-labs/agent-skills) 现 34,881★，2026-11-20 仍有推送。仓库根目录未声明 SPDX 许可证。

## When to use
要让编码 agent 按 Vercel 工程实践写 React / Next.js、审查界面、部署到 Vercel，或给已上线项目做成本/性能审计时用。不要和 [skills CLI](vercel-skills-cli.md)（`vercel-labs/skills`，安装器）混淆：本包是官方技能内容。浏览器自动化请看 [agent-browser](agent-browser.md)。

## What it does
Vercel 官方 Agent Skills 集合，目前公开 9 个技能，其中包括：
- `react-best-practices`：40+ 条 React / Next.js 性能规则，按 8 类、影响优先级排列（消除 waterfall、捆包、服务端/客户端取数等）；
- `vercel-optimize`：先拉 Vercel 指标，再只深挖指标指向的路由，产出成本与性能排序报告；
- `deploy-to-vercel`、`vercel-cli-with-tokens`、`web-design-guidelines`（100+ 条无障碍/性能/UX 审查规则），以及 React Native、View Transitions、composition 与 writing guidelines。

## Recipe / links
- Repo: https://github.com/vercel-labs/agent-skills（34,881★；根目录未见 LICENSE）
- 安装：`npx skills add vercel-labs/agent-skills`
- 目录：https://skills.sh/vercel-labs/agent-skills
- 也可按需只装一个 skill，例如 `npx skills add vercel-labs/agent-skills --skill react-best-practices`

## Why it made the cut
此前多轮 Watch，等一条能对应到官方仓的介绍。本窗盘点帖给出完整官方仓库与主要技能说明；34,881★、可加载 SKILL.md、场景清楚。和 skills CLI、agent-browser 分工不同，这里是 Vercel 协议栈的技能内容本身。
