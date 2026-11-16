# scroll-world（滚动穿越 3D 世界落地页）

**Tags:** frontend, landing-page, scroll, video, generative, skill
**Source:** [@bkdgiffug](https://x.com/bkdgiffug/status/2122308200565522721) · 2026-11-16
**Engagement:** 中文介绍帖 8 赞 / 6 书签；仓库 [oso95/scroll-world](https://github.com/oso95/scroll-world) 现 11,029★ / 1,203 forks，MIT。仓最近推送停在 2026-07-29。

## When to use
要做「边滚边飞」的品牌 / 行业落地页：镜头从每个微缩场景外部钻进去，再无剪辑地飞向下一个场景（类似 Emons 式等距立体世界，或你指定的美术方向）。不要用于普通文档站、后台，或只要 CSS/HTML 滚动叙事、不需要生成视频链的页面——后者更适合 [scroll-craft](scroll-craft.md)。

## What it does
可加载 Agent Skill：先访谈主题、故事节拍和品牌套件，再生成连贯场景静帧、每场「钻入」镜头，以及用相邻真实帧锁定的衔接镜头，最后接上与框架无关的滚动 scrub 引擎（`references/scrub-engine.js`，可放进纯 HTML / Next.js / Vue 等）。默认视频链走 Monid（Seedance 2.0，按条计费，README 称 6 场 1080p 链大约 27 美元，技能每次构建会复查接口）；Higgsfield 积分是备选计费与静帧来源，也可选用 Codex 内置出图。关键规则是衔接必须帧级相同，否则场景之间会「跳一下」。

依赖：Monid 和/或 Higgsfield CLI 及额度、ffmpeg/ffprobe、Python 3 + Pillow。这是付费生成管线，不是纯本地渲染。

## Recipe / links
- Repo: https://github.com/oso95/scroll-world（MIT，11,029★）
- SKILL.md：https://github.com/oso95/scroll-world/blob/main/skills/scroll-world/SKILL.md
- Claude Code 插件：
  ```text
  /plugin marketplace add oso95/scroll-world
  /plugin install scroll-world@scroll-world
  ```
- 其他 agent：`npx skills add oso95/scroll-world`
- 手动：把 `skills/scroll-world` 拷到 `~/.claude/skills/` 或 `~/.codex/skills/`

## Why it made the cut
完整 SKILL.md + 可验证的管线说明和 portable 引擎，使用场景与已收录的 scroll-craft（手写滚动语法 / 截图验收）明确互补。MIT，社区信号很强（1.1 万★）。需注意：依赖付费视频 API，且仓库自 2026-07-29 后再无推送，接口若变更需要以技能内的探活步骤为准。
