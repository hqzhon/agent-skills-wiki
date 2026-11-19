# tokenheimer（跨 harness 重建项目的 agent 用量考古）

**Tags:** analytics, tokens, productivity, coding-agents, skill
**Source:** [@alvaisy](https://x.com/alvaisy/status/2123381648012214476) · 2026-11-19
**Engagement:** 作者安装说明帖（0 赞）；仓库 [osspakistan/agent-skills](https://github.com/osspakistan/agent-skills) 0★，MIT。早期条目。

## When to use
想弄清自己在某个代码仓库上，**用过哪些 coding agent、花了多少有效时间、token / 模型 / 工具调用 / skill 使用情况如何**，并得到一份带出处的 HTML/Markdown 报告时使用。它读的是本机 harness 历史，不编造数字，也不估算「花了多少钱」。

## What it does
本地优先的考古技能：先给项目做指纹（路径、git remote 等），只读搜索 Codex、Claude Code、Cursor、Gemini CLI 等 harness 的本地记录，拷贝实际用到的证据（并去掉凭证），再归一化成会话账本和项目级指标。默认 Quick 模式给出汇总；Full 模式再加有证据支撑的逐会话摘要。强调「30 个有效小时，跨越 3 个有效天」这类成对表述，缺数据就标 unavailable，不用 0 填空。产出包括 `report.html`、`report.json`、`REPORT.md`、`sessions.csv`、证据清单，以及一份讲「项目做成了什么」的 `X-POST.md` 草稿。

## Recipe / links
- Repo：https://github.com/osspakistan/agent-skills/tree/main/skills/tokenheimer（MIT，所在仓库 0★）
- 安装：
  ```
  npx skills add osspakistan/agent-skills --skill tokenheimer
  # 或全局：加 -g
  ```
- 用法：`/tokenheimer quick — analyze this repository across my local coding agents` 或 `/tokenheimer full — investigate ~/projects/my-app from October 1 to November 1`。
- Agent 需要对相关本机历史目录有读权限；技能声明不修改 harness 数据库或缓存。

## Why it made the cut
场景清楚，有完整 SKILL.md、参考文档、归一化 schema 和固定报告模板，不是「帮我总结一下 token 用量」的临时提示。仓为 0★，属早期收录；因为它会读本机 agent 历史，装前建议先读脚本与路径白名单。
