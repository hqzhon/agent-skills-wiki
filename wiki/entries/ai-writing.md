# ai-writing（先砍篇幅和清晰度，再去 AI 腔）

**Tags:** writing, editing, clarity, anti-slop, skill-pack
**Source:** [@akalsey](https://x.com/akalsey/status/2121490236937289950) · 2026-11-14
**Engagement:** 发现帖互动低；仓库 [akalsey/ai-writing](https://github.com/akalsey/ai-writing) 当日发布、0★，MIT；作者有长文说明设计理由

## When to use
agent 写出来的状态汇报、文档或回复太长、对局外人不知所云，或带常见 AI 腔。和只洗「delve / 破折号 / It's not X, it's Y」的 humanizer 不同：这里先解决篇幅和清晰度，最后才去痕迹。适用于 Claude，以及支持 Agent Skills 的 ChatGPT / Grok 等。

## What it does
`writing-quality` 插件里有五条技能、一个 hook 和一个 output style。入口是 `writing-pipeline`，按固定顺序跑完再通读，并定义何谓写完：

1. `concise`：先给答案，再删读者不需要的整句/整段（复述需求、已知背景、写作过程、被否决的方案、收束回顾）；不删动作、日期、负责人、决策和请求；不给原本没有格式的草稿加格式。思路来自 *Writing for Busy Readers*。
2. `cold-reader-docs`：让没参与对话的人也能读懂；抓住未定义术语、「我们讨论过的方案」和临时造的简称。
3. `clear-prose`：句子层面的清晰——主语是行动者、谓语是动作，用读者会用的名字，段落先说重点。
4. `avoid-ai-writing`：再清理 AI 写作模式（分层词汇、格式习惯、结构腔），有 detect / rewrite / edit，以及博客、文档、内部备忘、LinkedIn 等情境。

顺序是关键：先砍掉的句子后面不必再打磨；精简后的篇幅成为后续步骤的预算。作者举例：一份 495 词的状态汇报可压到 85 词且更好读。

## Recipe / links
- Repo: https://github.com/akalsey/ai-writing
- 作者说明：https://kalsey.com/2026/11/ai_writing_is_intolerable_im_trying_to_fix_it/
- 按 Agent Skills 标准编写，MIT

## Why it made the cut
有明确问题定义（AI 文字难读主因是长和含糊，不是表面用词）、可执行的顺序管道和开源技能包，和 [humanizer](humanizer.md)、[stop-slop](stop-slop.md)、[sepia](sepia.md) 互补。仓库虽新、无星标，长文和技能表足以验证。
