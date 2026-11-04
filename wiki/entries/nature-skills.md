# nature-skills（Nature 风格论文润色 / 科研绘图技能库）

**Tags:** research, academic-writing, figures, skill-pack, chinese, codex, claude-code
**Source:** [@musen9527](https://x.com/musen9527/status/2117766274919141681) · 2026-11-04
**Engagement:** 仓库 Yuan1z0825/nature-skills 约 5.2 万★（Apache-2.0，23 个技能）；推文本身新发

## When to use
写或改学术论文时，想让 agent 按 Nature 系期刊的表达习惯润色 / 中译英、起草摘要与引言、做投稿级科研图，或模拟审稿与写返修回复。

## What it does
- 一组围绕 `SKILL.md` 组织的科研技能（`nature-*`），外加供其他技能读取的共享包 `nature-shared`。
- 覆盖：PDF 图文对照中英 reader、论文转组会 PPT、Nature 风格润色 / 写作、三份互盲审稿报告模拟、逐点审稿回复 + cover letter、引用与他引画像、科研示意图。
- 不确定用哪个时直接描述任务；知道名字可在提示词里写「使用 `nature-reader`」。

## Recipe / links
- Repo: https://github.com/Yuan1z0825/nature-skills
- 列出技能：`npx skills add Yuan1z0825/nature-skills --list`
- 只装一个（带共享包）：`npx skills add Yuan1z0825/nature-skills --agent codex --skill nature-reader --skill nature-shared --yes --copy`
- Claude Code：README 建议保留稳定 clone，用 subagent / slash command 指向 `skills/*/SKILL.md`，以保留 `references/`、脚本等目录结构
- Python / R / 浏览器 / MCP 等运行依赖需另配

## Why it made the cut
有完整仓库、明确场景和逐技能的安装方式，社区信号很强，补足 wiki 的学术写作方向。注意 README 开头夹带作者的代充 / 商务推广，与技能本身无关，可忽略。
