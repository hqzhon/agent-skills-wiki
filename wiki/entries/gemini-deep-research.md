# Gemini Deep Research Skill（官方实验：把编程代理变成调研员）

**Tags:** official, google, gemini, research, deep-research, skill
**Source:** [@_philschmid](https://x.com/_philschmid/status/2126312943520243885) · 2026-11-27
**Engagement:** 作者第一方介绍帖约 2,000 赞 / 2,009 书签；同串[回复给出安装命令](https://x.com/_philschmid/status/2126312946389377447)。技能位于 [google-gemini/demolab](https://github.com/google-gemini/demolab) 的 `skills/deep-research/`，仓库现 974★，Apache-2.0。官方称在数百次盲测中，带技能优于无技能的比例约 90%。

## When to use
要用 coding agent（Gemini 4 Neon / Antigravity 等）做**宽话题、多角度或需要对照一手来源**的调研，并产出带引用的短报告时用。不要用它做简单事实查询——技能说明里写了：窄问题直接回答，或最多派一两个子代理。它和 Gemini 应用里面向普通用户的 Deep Research 产品不是同一套东西：这里是约 16 行、可加载的 agent skill。

## What it does
[SKILL.md](https://github.com/google-gemini/demolab/blob/main/skills/deep-research/SKILL.md) 把代理设成调研主控，要点是：
1. 先定向，宽话题拆成 3–5 个不重叠的子问题（高思考模型可降到 2–3 路）
2. 并行派 `research` 子代理，需要读完整页面时用 `browser`；每路最多 8–12 步
3. 用一手来源和原始摘录核对数字，禁止只靠搜索摘要
4. 大部分完成后取消卡住的 worker，最多再做一轮补洞
5. 报告用简短两句结论、行内可点引用，并单列未决冲突；有 Artifact 目录就写文件，聊天里只给指针

同一仓库里已收录过 [gemini-frontend-design](gemini-frontend-design.md)，这是另一条可独立安装的技能。

## Recipe / links
- Repo: https://github.com/google-gemini/demolab（974★，Apache-2.0）
- 安装：
  ```bash
  npx skills add google-gemini/demolab --skill deep-research
  ```
- 技能路径：`skills/deep-research/SKILL.md`

## Why it made the cut
Google / Gemini 团队第一方发布，信号极强；技能虽短，但使用边界、子代理预算和引用要求都写得很具体，仓库可核，也有公开评测陈述。与已收的 Gemini API 技能包、gemini-frontend-design 不是同一条。
