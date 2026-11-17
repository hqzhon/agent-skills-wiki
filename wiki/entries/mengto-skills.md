# MengTo Skills（设计师 / 前端技能包）

**Tags:** design, frontend, 3d, illustration, skill-pack, html
**Source:** [@qi_zhen85546](https://x.com/qi_zhen85546/status/2122621565422501917) · 2026-11-17
**Engagement:** 发现帖是安装说明、互动很低；仓库 [MengTo/Skills](https://github.com/MengTo/Skills) 现 7,671★ / 883 forks，MIT；作者为 Design+Code 的 Meng To

## When to use
要用 agent 做可复用的界面、落地页、HTML 演示、Three.js / 插画或设计参考工作流（把录屏/页面变成提示词、做可播放的产品演示窗、按画风画 SVG 等），而不是一次性聊天出一段代码。本窗被点名的是 `html-demo`：想用实时 HTML 替代产品 UI 的录屏 / GIF / MP4，并且要能循环、拖动进度、跳到某一步。

## What it does
面向设计师和 builder 的便携技能包，仓库内可检索到约 177 个 `SKILL.md`，覆盖 web-design、3d、illustration、media、codex 等目录。本窗安装说明针对 **html-demo**：在固定 1200×750 舞台上把每帧写成 `View(t)` 的纯函数，再用 CSS 缩放适配宽度，做出可循环、可拖动、可跳步的 Mac 风应用演示窗（React / DOM，另有 vanilla 脚本）；边界是：真要录浏览器成 MP4 或把页面做成定长影片，应走仓库里的其它技能，而不是这条。

## Recipe / links
- Repo: https://github.com/MengTo/Skills（MIT，7,671★）
- html-demo SKILL.md: https://github.com/MengTo/Skills/blob/main/agent-skills/web-design/html-demo/SKILL.md
- 只装 html-demo（Claude Code / Codex）：
  ```bash
  # 也可从 https://fil.design/skills/html-demo.zip 下载后，把 html-demo 文件夹放到 skills 目录
  npx degit MengTo/Skills/agent-skills/web-design/html-demo ~/.claude/skills/html-demo
  # Codex：把同一文件夹放到 ~/.codex/skills/html-demo，最终路径应为 …/html-demo/SKILL.md
  ```
  装好后可说：「用 $html-demo，把这个应用的主要流程做成网页演示，支持循环播放、拖动进度和跳到指定步骤。」
- 其它技能按目录把对应文件夹拷进 agent 的 skills 目录即可；浏览 [DEMOS.md](https://github.com/MengTo/Skills/blob/main/DEMOS.md) 看可运行演示。

## Why it made the cut
高星、可核对的大型设计技能包，`SKILL.md` 数量和分类都清楚；本窗又给出了 html-demo 的具体安装路径与调用句。和已收录的 [Effective HTML](effective-html.md)、[Stitch Skills](stitch-skills.md) 互补（这边偏 Meng To 的演示/3D/插画工作流，不是设计系统迁移或 Stitch 出码）。
