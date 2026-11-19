# cogsec（带着批判思维把想法过一遍）

**Tags:** critical-thinking, research, cognitive-security, skill
**Source:** [@sprice](https://x.com/sprice/status/2123234152053174301) · 2026-11-19
**Engagement:** 作者宣布开始公开自己的 agent skills，本条为第一枚（0 赞 / 1 书签）；仓库 [sprice/slow](https://github.com/sprice/slow) 今日新建、1★，CC0。早期条目。

## When to use
要用 LLM 探索一个想法、传闻或问题，又希望它先检查前提、钢化对立解释、再说证据实际支持什么时使用。适合「帮我理解 X」「验证这个判断」，而不是只要附和的检索摘要。

## What it does
`Slow` 插件里的 `cogsec` 技能：保持用户目标和第一手观察，拆开带倾向的标签，检查前提是否成立，给对立观点最强表述，再给出当前证据站得住的结论，并标明不确定之处。禁止用「我认为」带过；涉及数字时对照独立基准或从原始数据核算。仓库同时带 Claude / Cursor / ChatGPT 插件布局。

## Recipe / links
- Repo: https://github.com/sprice/slow（CC0，1★）
- 安装：
  ```bash
  npx skills add sprice/slow --skill cogsec
  ```
  ChatGPT 桌面版：Settings → Plugins → Skills → Add marketplace，源填 `https://github.com/sprice/slow`，再安装 `slow` 插件。Claude 也可在对话里请它安装该插件。
- 开口示例：「Use cogsec to help me understand [topic].」

## Why it made the cut
把「别被模型带着走」写成具体步骤（前提、钢化、证据边界），有可安装的 SKILL.md 和多种宿主入口。仓很新、星数低，属早期收录；作者称还会继续发布同系列技能。
