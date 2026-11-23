# antialgorithm（先点名再躲开模型的第一平均解）

**Tags:** creativity, design, naming, writing, skill
**Source:** [@TheArthiAI](https://x.com/TheArthiAI/status/2124167079087759602) · 2026-11-21
**Engagement:** 本窗为热榜转述帖（0 赞）；仓库 [mankidev/antialgorithm](https://github.com/mankidev/antialgorithm) 707★，MIT。2026-11-14 建仓，本窗仍在更新。

## When to use
做**仍然开放的创意选择**时使用：起名、故事、玩法、海报、UI、配色、标题口号等。尤其是你觉得结果「太泛、太安全、很 AI、看过无数次」的时候。不用于代码标识符、修 bug、用户已经做决定的选择，以及 README / 商店页 / commit message 这类已有固定体例的文本。

## What it does
强制模型先说出自己会脱口而出的「平均解」，再根据项目里的真实上下文主动离开它。起点必须来自外部（项目、地点、人物、约束），不能只靠模型自己的品味。请求很瘦且工作很短时，先给一个带种子的成品，再在结尾问一个能让它更贴案的短问题；工作又长又贵时，先问那一个问题。用户在 `CLAUDE.md` / `AGENTS.md` 里的既有规则始终优先。仓库用同一句海报提示做了有/无该技能的对照图。

## Recipe / links
- Repo：https://github.com/mankidev/antialgorithm（MIT，707★）
- 安装：
  ```
  npx skills add mankidev/antialgorithm
  ```
- 也提供多语言 README。

## Why it made the cut
有完整 SKILL.md、明确的「何时用 / 何时不用」，以及可核对的前后视觉对照，不是一句「做的特别一点」的提示词。星数已经不低。
