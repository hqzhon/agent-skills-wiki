# wallstreet-explainer（华尔街式财经/科技解说短片）

**Tags:** video, finance, explainer, motion, short-video, chinese, skill
**Source:** [@ilexax](https://x.com/ilexax/status/2124826095442637150) · 2026-11-23
**Engagement:** 发现帖信号低；仓库 [HeyChengC/wallstreet-explainer](https://github.com/HeyChengC/wallstreet-explainer) 1,017★ / 186 forks。README 与 LICENSE 均标 MIT（代码和文档；样片里的第三方画面/Logo 不在 MIT 范围内）。

## When to use
要做 1–3 分钟的财经或科技解说短片，风格是深蓝织物底、金色大数字、用真新闻和真画面当证据：横屏（B 站/YouTube）或竖屏（小红书/抖音/视频号）。可以说「像小Lin说那种」「做一条讲清一笔账的片子」。给了口播视频（真人或数字人）就走真人口播包装，没给就走无人动效包装。

## What it does
给一个选题，技能按流程写文案、找素材、截新闻网页并给关键句刷黄、配音、对齐、渲染和混音。四种组合：16:9 / 9:16 × 有口播 / 无人出镜。竖屏版提供 20 个现成组件和 29 个 `v-` 场景，可用 `render.mjs --check` 检查镜头表。仓库带样片（黄金为何下跌、AI 有多烧钱、竖屏英伟达等）和 `kit/`、`scripts/`、`examples/`。

## Recipe / links
- Repo: https://github.com/HeyChengC/wallstreet-explainer（1,017★，MIT）
- 安装（Claude Code 手动）：
  ```bash
  git clone https://github.com/HeyChengC/wallstreet-explainer.git ~/.claude/skills/wallstreet-explainer
  cd ~/.claude/skills/wallstreet-explainer
  pip install -r requirements.txt
  npm install && npx playwright install chromium
  ```
  另需 ffmpeg，以及按 `kit/kit.css` 把指定字体放进 `fonts/`。
- 用法示例：`用 wallstreet-explainer 做一条 1 分钟的片子，讲 AI 到底有多烧钱`

## Why it made the cut
高星漏收：完整可运行流水线，有 SKILL.md、场景模板、渲染自检和可看的样片，不是只给提示词。和 [BB-Video](bb-video.md)（纯代码讲解/宣传片）路线不同，这边强调真实新闻画面作证据的财经解说腔。本窗由介绍帖带出仓库。
