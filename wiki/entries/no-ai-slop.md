# no-ai-slop（去写作 AI 味，保留个人声音）

**Tags:** writing, editing, anti-slop, voice, skill
**Source:** [@heyrimsha](https://x.com/heyrimsha/status/2125207339993276815) · 2026-11-24
**Engagement:** 本窗盘点帖提到；仓库 [petergyang/no-ai-slop](https://github.com/petergyang/no-ai-slop) 现 13,773★，MIT，2026-09-02 后推送较少

## When to use
要把草稿改得更清楚、更直接、更有个人判断，或只想**检测**文案里的 AI 套话时用。不要用它重做 UI 视觉方向——那是 [unslop](unslop.md) / [unslop-ui](unslop-ui.md) / [unslop-anything](unslop-anything.md) 的范围。和 [Humanizer](humanizer.md) 同属写作去 AI 味，但规则和仓库不同。

## What it does
可加载技能 `skills/no-ai-slop/SKILL.md`。两种模式：
- **Edit（默认）**：做最小有效修改，保留观点和声音，并列出改了什么；
- **Detect**：只点名命中的套话模式、引用原句、给出简短修法，不重写、不打「是不是 AI 写的」分数。
宣称覆盖 20+ 种写作套话。带 `eval.md` 自检和 Codex/ChatGPT 插件元数据。

## Recipe / links
- Repo: https://github.com/petergyang/no-ai-slop（13,773★，MIT）
- 安装：`npx skills add petergyang/no-ai-slop --skill no-ai-slop --global --yes`
  也可以把仓库地址发给编码 agent，请它全局安装 `/no-ai-slop`。
- Skill: [skills/no-ai-slop/SKILL.md](https://github.com/petergyang/no-ai-slop/blob/main/skills/no-ai-slop/SKILL.md)
- 仓最近推送停在 2026-09-02，规则是否跟上新套话需自行判断。

## Why it made the cut
高星漏收：针对**写作**而不是界面，可加载技能和 Detect/Edit 边界清楚，13,773★、MIT。与已收录的 Humanizer、ai-writing、unslop 系列不是同一仓库，条目里写清分工。本窗来自盘点帖，按仓库信号补上。
