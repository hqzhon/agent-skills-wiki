# gpx-3d-video（GPX 轨迹同步 3D 路线叠加）

**Tags:** video, gpx, ffmpeg, outdoor, skill
**Source:** [@ymbkxc](https://x.com/ymbkxc/status/2118340878477783169) · 2026-11-05
**Engagement:** discovery post (low); repo ymbkxc/gpx-3d-video · MIT

## When to use
要把运动相机片段与 GPX 轨迹对齐，渲染经纬度/海拔随画面同步变化的 3D 路线叠加（徒步、骑行、越野记录片）时。

## What it does
标准 Agent Skill：先用脚本检查媒体元数据与时区，按内嵌录制时间排序合并片段，再按真实墙钟映射 GPX（禁止把整段轨迹均匀拉伸到剪辑后的视频），可出短预览或最终合成，并跑校验。缺 GPS 覆盖时显示缺失状态，不编造位置。

## Recipe / links
- Repo: https://github.com/ymbkxc/gpx-3d-video
- SKILL.md: https://github.com/ymbkxc/gpx-3d-video/blob/main/skill/gpx-3d-video/SKILL.md
- 依赖：ffmpeg / ffprobe、Python3、NumPy、Pillow
- 关键进 Claude Code / Codex 等 skills 目录后，让 agent「按 gpx-3d-video 合成这段徒步视频」

## Why it made the cut
有完整 SKILL.md + 脚本工作流；场景清晰；关键不变量（时间轴/不编造 GPS）可验证。
