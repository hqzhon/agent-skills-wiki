# Motion Prompt（216 个可点选的动效 / 镜头名词库）

**Tags:** motion, camera, ui, landing-page, prompt-library, skill
**Source:** [@zjcpzz](https://x.com/zjcpzz/status/2121415301879459970) · 2026-11-14
**Engagement:** 发现帖互动低；仓库 [showheyohtaki/motion-prompt](https://github.com/showheyohtaki/motion-prompt) 约 2.1k★，MIT

## When to use
做动效、镜头运动、UI 组件、落地页特效、照片光影或生图风格时，你或 agent 叫不出准确名称、只能说「那种感觉」。希望先从带动态样例的库里勾选（例如「用 #012 和 #045」），再按规格在项目里复现，或写成视频/图像模型提示词。

## What it does
可安装的 Agent Skill（`skills/motion-prompt/SKILL.md`，带 references 与 scripts）加上 216 个编号条目（9 组 × 24：`motion` / `camera` / `ui` / `lp` / `photo` / `motion2` / `lp2` / `camera2` / `artstyle`）。每条有三位编号、多语言名称、一行释义、时序与缓动说明，以及无依赖的 Canvas 2D 纯函数（同一段代码可实时播放也可逐帧渲染）。Skill 的主路径是：打开图库让用户勾选 → 收回选择 → 在 Canvas、Remotion、CSS/SVG/Lottie 或 After Effects 里精确重建，或转成提示词。图库：https://showheyohtaki.github.io/motion-prompt/ ；名称列表在 `packs/`（英 / 日 / 西 / 简中 / 繁中）。也可用仓库里的提示去为自己的领域做同类名词库。

## Recipe / links
- Repo: https://github.com/showheyohtaki/motion-prompt
- SKILL.md: https://github.com/showheyohtaki/motion-prompt/blob/main/skills/motion-prompt/SKILL.md
- 图库：https://showheyohtaki.github.io/motion-prompt/
- 安装：`npx skills add showheyohtaki/motion-prompt`（仓库含 `.claude-plugin` 市场配置）
- 作者：[Shohei Ohtaki](https://x.com/showheyohtaki)

## Why it made the cut
不只是灵感图册：有可加载 SKILL.md、编号可引用、样例可点、实现是可移植的纯函数；使用场景明确，仓库可验证。
