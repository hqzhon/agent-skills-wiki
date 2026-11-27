# Visual Learning Skill（把知识点做成可交互讲解页）

**Tags:** education, explainer, animation, html, skill
**Source:** [@kewangx](https://x.com/kewangx/status/2126090842511389148) · 2026-11-27
**Engagement:** 出现在教育开源盘点帖（2 赞 / 1 收藏）；仓库 [andrewalumkal/VisualLearning.Skill](https://github.com/andrewalumkal/VisualLearning.Skill) 现 24★，MIT。2026-10-16 创建，最近推送到 2026-10-23。

## When to use
要把一个有部件关系或分步过程的抽象概念，做成能在浏览器里播的讲解页时用：一种是带旁白、章节和逐步出现的引导动画，一种是可切换视角、带控件和白话提示的交互探索。不要用它做没有事实来源的装饰动画。

## What it does
一份不绑定单一模型的 SKILL.md，外加两份示例 HTML。开工前 agent 要先基于核查过的来源提出 2–3 种方案并等你选；页面上的每条事实都应对着真实来源，并在页上列出。每做完一部分，再用子 agent（没有子 agent 就自己另起一轮，并标明不是独立审）检查论断、教学效果和浏览器行为，修好后再交付。成品跟随系统浅色/深色模式，带时间轴、倍速和章节按钮。

## Recipe / links
- Repo: https://github.com/andrewalumkal/VisualLearning.Skill（24★，MIT）
- 技能：https://github.com/andrewalumkal/VisualLearning.Skill/blob/main/SKILL.md
- 文件夹名必须是 visual-learning，以匹配技能的 name：
  ```bash
  git clone https://github.com/andrewalumkal/VisualLearning.Skill.git ~/.claude/skills/visual-learning
  ```
  agent 需要能读文件、搜网页和写 HTML；能驱动浏览器和开子 agent 时，核查会更完整。把 assets/ 和 SKILL.md 放在一起，以便打开示例。

## Why it made the cut
可加载的完整配方 + 示例页 + 先核源再出图的验收步骤，使用场景清楚。星标和介绍帖都一般，按可验证材料收录，而不是按热度。
