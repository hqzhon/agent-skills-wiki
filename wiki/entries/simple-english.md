# SimpleEnglish（ASD-STE100 简化技术英语写作）

**Tags:** writing, docs, technical-writing, anti-slop, skill
**Source:** [@lunkertw](https://x.com/lunkertw/status/2117901847751213439) · 2026-11-04（GitHub 趋势榜提及）
**Engagement:** 仓库 AminBlg/SimpleEnglish，~4.2k★，MIT，v2.1.1，附 9 个 Claude 模型的评测结果

## When to use
要 agent 写文档、操作说明、Runbook、错误提示或回复，希望读者一次读懂、不被花哨措辞误导；或者团队文档需要符合航空业受控语言 ASD-STE100。

## What it does
按 ASD-STE100 Simplified Technical English 的规则约束输出：短句、一词一义、主动语态、指令句先说动作。默认是普通读者易读模式，按需切到严格 STE 模式。仓库自带评测，称可见回复缺陷减少约 95%。Claude Code 插件版还带会话 hook 和 output style，可全程生效。

## Recipe / links
- Repo: https://github.com/AminBlg/SimpleEnglish
- Skill 文件：`skills/simple-english/SKILL.md`
- 任意 agent：`npx skills add AminBlg/SimpleEnglish`（只装 skill）
- Claude Code 插件：按 README 用 `claude plugin marketplace add` 安装，可获得 hook 与 `simple-english:simple-english` 输出风格

## Why it made the cut
有成熟的外部标准做依据、带可复查评测、一个文件夹零依赖，补上 wiki 里「技术写作 / 文档清晰度」方向，与 humanizer、stop-slop 这类去 AI 味 skill 侧重点不同。
