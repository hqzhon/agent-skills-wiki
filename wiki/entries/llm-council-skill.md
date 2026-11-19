# llm-council（五顾问合议决策）

**Tags:** decision-making, debate, evaluation, claude-code, skill
**Source:** [@Mostlybuilds](https://x.com/Mostlybuilds/status/2123083382267756769) · 2026-11-18
**Engagement:** 发现帖互动很低（0 赞）；仓库 [tenfoldmarc/llm-council-skill](https://github.com/tenfoldmarc/llm-council-skill) 现 1,065★（2026-04-18 一次发布，之后无推送）

## When to use
要把一个有利害、有权衡的问题或方案拿去压力测试，而不是问事实或随便问「要不要用 markdown」。触发语包括 `council this`、`run the council`、`pressure-test this`、`war room this`、`debate this`，或「该选 A 还是 B」这类真决策。

## What it does
按 Andrej Karpathy 的 [LLM Council](https://x.com/karpathy/status/1962263486196867115) 思路，在 Claude Code 里用子 agent 跑五位视角不同的顾问（唱反调、第一性原理、扩张主义者、局外人、执行派），匿名互评后由主席汇总：共识、分歧、盲点、建议和下一步，并生成 HTML 报告与 Markdown 实录。

## Recipe / links
- Repo: https://github.com/tenfoldmarc/llm-council-skill（1,065★；README 未标许可证）
- 安装：`git clone https://github.com/tenfoldmarc/llm-council-skill ~/.claude/skills/llm-council`
- 或把 `SKILL.md` 放进 `~/.claude/skills/llm-council/` 后重开 Claude Code
- 用法示例：`council this: 该把 297 美元的课程改成 97 美元的直播工作坊吗？`

## Why it made the cut
决策场景和五顾问流程写得很具体，有互评与产出物，不是一句「多问几个模型」。仓库较久未更新，且未声明许可证，装前自行确认。
