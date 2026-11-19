# simulator（把任意行业做成可看的玩具比例模拟器）

**Tags:** 3d, visualization, simulation, video, skill
**Source:** [@grok](https://x.com/grok/status/2123323747889184807) · 2026-11-19（指向 [@Nyxera0x](https://x.com/Nyxera0x) 的仓库）
**Engagement:** 本窗为回复贴出的安装信息；仓库 [Nyxera0x/simulator](https://github.com/Nyxera0x/simulator) 19★ / 9 fork，MIT。此前扫描因缺少有效仓库而放在 watch。

## When to use
希望把机场、工厂、工地、仓储一类**运营系统**做成「玩具比例、一个镜头、可点击的产品 UI」的离线 HTML 模拟器，并录成 60fps 影片时使用。适合「按参考片的格式，重建我这个行业」而不是再造一套游戏引擎。

## What it does
Claude Code 技能：先拆参考片的构图、配色和面板，再用两个子 agent 按同一尺度合同分别建建筑和车辆，把一天写成时间的函数，做碰撞扫描，然后逐帧录成片子（可配动作音效）。仓库自带四套示例（机场 Rampline、汽车厂 Plantline、工地 Buildline、仓储网 Stockline），规则包括：全程一个镜头只平移/缩放、玩具尺度、蓝白主色、界面数字来自场景、选中车辆画出路线。模型全是代码，不下载 3D 资产。

## Recipe / links
- Repo: https://github.com/Nyxera0x/simulator（MIT，19★）
- 安装：`npx skills add Nyxera0x/simulator -g -a claude-code`
- 首次在安装目录执行：`npm install && npx playwright install chromium`。出片需要 ffmpeg，音效需要 Python 3；ElevenLabs key 可选。
- 用法：在 Claude Code 输入 `/simulator`，或「按这个片子的格式，做一个包裹分拨中心模拟器，跟着一个包裹从卡车到货车」。
- 也可先跑示例：`node sims/build.mjs warehouse-film`，再用 `sims/capture.mjs` 录 mp4。

## Why it made the cut
此前同类演示帖缺仓库；现在有完整 SKILL.md、示例场景、构建/录制脚本和 MIT 许可，和已收录的 teardown（拆解一台机器）互补：这边做的是行业运营的活地图。
