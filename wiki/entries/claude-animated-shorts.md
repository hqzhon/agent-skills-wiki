# Claude Animated Shorts（本地渲染竖屏动画故事短片）

**Tags:** video, shorts, threejs, remotion, animation
**Source:** [@Manojkumar2257](https://x.com/Manojkumar2257/status/2117974328298094897) · 2026-11-05
**Engagement:** 仓库 mromidev/claude-animated-shorts，约 1.6k★，MIT，2026-11-01 创建

## When to use
想做 55–70 秒的竖屏动画故事短片（2D 角色 + 彩色 3D 世界），又不想花 AI 视频生成额度，愿意在自己电脑上用 Remotion 渲染。

## What it does
`SKILL.md` 写了完整流水线：选题与事实 → 脚本 → 配音 → 在 `story.ts` 里做分镜 → 出静帧 → 渲染。用 three.js 在 Remotion 里渲染墨线描边、手绘小镇、镜头虚化和运镜，并合成音效与配乐（含闪避和响度处理）；agent 会拿你的帧对照参考报告和参考帧做逐帧 QA，最后输出 2K 成片。

## Recipe / links
- Repo: https://github.com/mromidev/claude-animated-shorts
- 安装：复制到 `~/.claude/skills/cartoon-3d-short/`；需要 Remotion + `@remotion/three`、Node、Python 3、ffmpeg
- 附带完整示例短片源码、`references/STYLE_BIBLE.md`、7 份测量报告和 38 张参考帧
- 提示：把 `REMOTION_TMP` 指到大磁盘，每次打包会复制约 1.3 GB 的 `public/`

## Why it made the cut
配方极其具体（每条规则、修复和最终画面参数都写进了 SKILL.md），附可复现模板和验证素材，社区信号也强。
