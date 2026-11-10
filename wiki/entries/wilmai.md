# WilmAI（芬兰 Wilma 家校技能）

**Tags:** education, school, finland, mcp, grok-bot, skill
**Source:** [@DanKornas](https://x.com/DanKornas/status/2119579725857227013) · 2026-11-09
**Engagement:** 3 likes / 0 reposts / 1 reply / 0 bookmarks · aikarjal/wilmai · MIT · 83★

## When to use
家里有孩子在用芬兰学校系统 Wilma，你想用已经在用的 AI 助手查询课表、作业、考试、成绩和需要家长处理的事项，而不是再开一个学校 App 标签页。

## What it does
独立开源项目（与 Visma / 官方 Wilma 无隶属）：在本机跑 MCP 服务器、CLI 和两个 agent skill。`wilma` 教 agent 使用工具和命令；`wilma-triage` 做成家庭晨报，标出待办并把考试写入日历。约 20 个只读 MCP 工具覆盖摘要、课表、作业、考试、成绩、缺勤、消息、通知和附件。登录在本地浏览器完成，密码不进聊天；不能代发消息或改 Wilma 数据。另有 WilmAI Home 桌面端（Mac / Windows，beta）。支持 Claude Desktop/ChatGPT Desktop、Grok Bot、Meta Muse、OpenClaw、Claude Code、Codex。

## Recipe / links
- Repo: https://github.com/aikarjal/wilmai （MIT）
- 网站（英/芬）：https://wilm.ai
- Claude Code：`claude mcp add --scope user wilma -- npx -y @wilm-ai/wilma-cli@2 mcp`
- Codex：`codex plugin marketplace add aikarjal/wilmai && codex plugin add wilma@wilmai`
- 终端：`npm i -g @wilm-ai/wilma-cli && wilma login && wilma summary`
- Agent skills：`npx skills add aikarjal/wilmai`
- Grok Bot / OpenClaw 等逐步指南见 wilm.ai

## Why it made the cut
垂直场景清楚，MCP + CLI + 两个 skill 都可安装，强调本机登录和只读；不是空喊「用 AI 管孩子作业」。83★ 对小众学校系统来说信号足够，且配方完整。
