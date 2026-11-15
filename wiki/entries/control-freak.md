# control-freak（一事一审再提交）

**Tags:** workflow, review, git, claude-code, skill
**Source:** [@IYoussef231](https://x.com/IYoussef231/status/2121659985587515646) · 2026-11-15
**Engagement:** 发现帖 1 赞；仓库 [IbrahimHYoussef/control-freak](https://github.com/IbrahimHYoussef/control-freak) 当天新建，0★，尚未看到 LICENSE 文件

## When to use
即将按一份多任务计划动手实现，希望每做完一件事就停下来给你审，修订到你点头后再提交，再进入下一件——而不是最后一次性看巨大 diff。项目里如果已有 `.control-freak/QUIRKS.md`，也应加载本技能。

## What it does
循环是：preflight → 实现**一件**任务 → 自检 → 停下汇报 → 按你的意见改到批准 → 再 commit → 下一件。进行中会覆盖其他技能里「连续做完不要停」的指示，但任务内部仍可用测试/调试类技能。preflight 检查 git 是否干净、复述或拆分任务清单，并读取 `.control-freak/QUIRKS.md`（按路径/glob 记录项目癖好；你的复审意见若会再次出现，agent 会提议写入，经你确认才落盘）。

## Recipe / links
- Repo: https://github.com/IbrahimHYoussef/control-freak（0★，新仓库）
- Skill：`skills/control-freak/SKILL.md`
- 安装：`npx skills add IbrahimHYoussef/control-freak`
- 或 Claude Code：`/plugin marketplace add IbrahimHYoussef/control-freak` 再 `/plugin install control-freak@control-freak`
- 也可把 `skills/control-freak` 软链到 Claude Code / OpenCode 的 skills 目录

## Why it made the cut
使用场景清楚，SKILL.md 把「一事一审」写成可执行循环，并带项目癖好记忆。仓库很新、暂无社区星数、也未见许可证，当作早期但可装的配方收录，后续需再观察维护情况。
