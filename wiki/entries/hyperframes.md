# HyperFrames（HeyGen 官方：HTML 渲染成片）

**Tags:** official, video, html, heygen, motion-graphics, skill-pack
**Source:** [@0xClaudAI](https://x.com/0xClaudAI/status/2125267294783680939) · 2026-11-24
**Engagement:** 本窗盘点帖（39 赞）将其列为视频生成项，另有多条演示帖；仓库 [heygen-com/hyperframes](https://github.com/heygen-com/hyperframes) 现 89,560★，Apache-2.0，2026-11-24 仍在推送

## When to use
要用 **HTML 渲染成视频** 时用：发布片、解说、音乐视频、图表、地图、竖屏、标题卡、字幕和叠加层。也适合剪自己的素材，或让 Claude Code / Codex 按官方技能来改和渲染。Wiki 里不少视频条目已经把 HyperFrames 当作依赖，这条是官方技能/工具本身。

## What it does
HeyGen 开源的 AI 视频编辑器：把 HTML（可含 GSAP 等）渲染成 MP4。仓库带官方技能包，其中包括 `skills/hyperframes/SKILL.md`（渲染合同与工作循环），以及 `hyperframes-cli`、`reverse-any-video`、`slideshow`、`media-use`、`figma`、`style-sampling` 等。另有免费档 Studio 桌面应用。技能要求第一次使用前告知一次会发送用量记录（已登录则关联账号），用户说 no 可跳过。

## Recipe / links
- Repo: https://github.com/heygen-com/hyperframes（89,560★，Apache-2.0）
- 给编码 agent 安装技能：`npx skills add heygen-com/hyperframes`
- CLI / 项目内命令以技能文档为准（`npx hyperframes <command>` 或技能目录里的 plugin CLI）。
- Studio：https://hyperframes.studio/studio/download（有免费计划）
- 主技能：[skills/hyperframes/SKILL.md](https://github.com/heygen-com/hyperframes/blob/main/skills/hyperframes/SKILL.md)

## Why it made the cut
高星漏收：官方组织仓、可加载技能齐全，89,560★、Apache-2.0，是很多已收录视频技能的上游。此前只在其它条目里被当作依赖提到，没有独立条目。本窗盘点帖再次出现，按仓库信号补上官方页，便于从 Catalog 直接找到安装方式。
