# rea-video（任意视频逐镜逆向）

**Tags:** video, reverse-engineering, analysis, skill, cli
**Source:** [@Han722371523249](https://x.com/Han722371523249/status/2118579754760610090) · 2026-11-06
**Engagement:** discovery 称 ~2.2k★；repo JuneYaooo/rea-video · ~2278★ · Apache-2.0  
**Note:** 与已收录的 [leanrea](leanrea.md)（轻装软件逆向）不同——本条是**视频制作方式**逆向。

## When to use
拿到参考视频，要问「这镜是实拍 / AI / 3D / 代码模板 / 录屏？字幕花字怎么叠？声音哪来的？怎么复刻？」时。不要用于二进制/软件逆向（用 leanrea / REA 系）。

## What it does
CLI + `skills/rea-video/SKILL.md`：逐镜分类底层画面、后期包装、真实素材、人声/BGM/音效与剪辑节奏，输出 breakdown / HTML 报告 / storyboard，并给出可执行复刻方案。支持 Claude Code / Codex 一键安装脚本。

## Recipe / links
- 仓库：https://github.com/JuneYaooo/rea-video
- SKILL.md：https://github.com/JuneYaooo/rea-video/blob/main/skills/rea-video/SKILL.md
- 安装：`bash scripts/install_skill.sh`（需 ffmpeg、Python ≥ 3.10）

## Why it made the cut
强社区信号 + 完整可执行流水线；与 leanrea 场景不重叠；Apache-2.0。
