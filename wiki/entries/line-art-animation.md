# line-art-animation（SVG 线描动画技能 + 库）

**Tags:** animation, svg, illustration, typescript, skill
**Source:** [@ainotesus](https://x.com/ainotesus/status/2122434519680647477) · 2026-11-17
**Engagement:** 发现帖互动很低；仓库 [JDhruv14/line-art-animation](https://github.com/JDhruv14/line-art-animation) 现 920★ / 141 forks，MIT。建于 2026-11-10，同日推送。

## When to use
要做可交互的「纸上墨线」动画组件：人物行走/反应、街道场景、昼夜循环，全部用 SVG 现场绘制，任意缩放仍然清晰，并能跟指针互动或导出视频。不要用于依赖生成式视频模型的短片（见 [Claude Animated Shorts](claude-animated-shorts.md) 或 [Muse Video Skill](muse-video-skill.md)），也不要用正弦波上下颠、滑步或一次生成一整套长得一样的角色。

## What it does
一份可加载 Claude skill，外加 4 个无依赖 TypeScript 模块：`ink.ts`（描线）、`gait.ts`（走/跑求解）、`motion.ts`（弹簧、钟摆、风）、`daynight.ts`（昼夜色板）。技能工作流是：先定笔触和纸色 → 拷入 `lib/` → 先交出一个人物或角落等人确认 → 再按 `references/motion.md` 做动作，并按帧验收。仓库带两个示例（约 150 行的 walker；含茶屋、运河、日程村民和十余处互动的 village），以及用于确定性逐帧抓取和对照参考片的脚本。

## Recipe / links
- Repo: https://github.com/JDhruv14/line-art-animation（MIT，920★）
- SKILL.md：https://github.com/JDhruv14/line-art-animation/blob/main/SKILL.md
- 安装（Claude Code）：
  ```sh
  git clone https://github.com/JDhruv14/line-art-animation ~/.claude/skills/line-art-animation
  ```
  或拷到项目内 `.claude/skills/`。示例需要 Node 22.18+：`npm install && npm run dev`。
- 示例：「做一家黎明面包店的线描动画：面包师端托盘、炉口蒸汽、窗边一只猫。」

## Why it made the cut
技能 + 可运行库 + 示例 + 验收规则齐全，使用场景清楚，MIT。发现帖本身很弱，但仓库一周内到 920★ / 141 forks，材料可核对。偏新仓（11-10 创建），当作可用的线描组件配方，而不是已经长期维护的官方包。
