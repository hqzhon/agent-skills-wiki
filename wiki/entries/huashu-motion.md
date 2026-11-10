# huashu-motion（可指着改的产品发布片）

**Tags:** video, launch-video, motion, composition, skill
**Source:** [@zg0820](https://x.com/zg0820/status/2119626510005162204) · 2026-11-09
**Engagement:** 2 likes / 0 reposts / 3 replies / 0 bookmarks · alchaincyf/huashu-motion · MIT · 2535★

## When to use
你要给产品做 30 秒级发布/功能更新短片，卡点通常不是不会写脚本，而是**改不动**——整条重生成太贵。适合独立开发者/小团队、没有专职设计剪辑时，用 Claude Code / Codex / WorkBuddy / Grok Bot 等说一句「做个发布片」。与同门 [huashu-art-motion](huashu-art-motion.md)（艺术/参数化动画代码渲染）不同：这条是**可指着画面局部改的成片工作流**。

## What it does
Agent 先读产品、给三个方向、写出整支片子并本机作曲（ABC 记谱 → 采样演奏），再打开浏览器编辑器等你；按 C 点画面写下意见，评论带时间点/场景/元素与源码位置，agent 只改那一处，预览停在原处刷新。标题、数字、颜色、停留时长可在侧栏手改。遵循 Agent Skills 规范。

## Recipe / links
- Repo: https://github.com/alchaincyf/huashu-motion （MIT，约 2535★）
- Install: `npx skills add alchaincyf/huashu-motion`
- 运行时：README 列 Claude Code、Codex、WorkBuddy、Grok Bot、Muse、Dots 等
- 示例成片见仓库 Releases / README 媒体

## Why it made the cut
可安装 skill、明确「指着改」核心场景、高星 MIT 仓与多运行时说明；与已收录的 huashu-art-motion / openfilm 类路线互补而非重复。
