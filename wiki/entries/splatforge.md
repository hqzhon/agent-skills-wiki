# SplatForge（把 3D 高斯溅射扫描做成可走路场景或可放置物体）

**Tags:** 3d, gaussian-splatting, threejs, physics, cli, skill
**Source:** [@zeshen_tian](https://x.com/zeshen_tian/status/2125637865938067658) · 2026-11-26
**Engagement:** 本窗为作者开源帖（0 赞）；仓库 [ZeshenTian/splatforge](https://github.com/ZeshenTian/splatforge) 现 0★，MIT，含 `skills/splatforge/SKILL.md`、本地 Studio 和 Three.js loader

## When to use
手里有 3DGS 扫描（`.spz` / `.ply` / `.splat` / `.ksplat` / 单文件 `.sog`），要在本机转成带碰撞的可走路场景（房间、院子、地形）或带阴影代理的可放置物体（产品、植物、雕塑），并在浏览器里第一人称或转盘预览后再导出时用。扫描全程在本地处理，不上传。普通点云 PLY 需要先做成 Gaussian 重建。它不是通用 three.js 场景技能（见 [Open 3D Skills](open-3d-skills.md)）。

## What it does
技能 `splatforge` 按用途选 **scene** 或 **object**（也可用 `--mode auto` 按几何分类），调用 CLI 转换、打开本地 Studio 复查，再给出 Three.js 加载示例。场景导出 `.world.zip`（扫描 + 地面/墙碰撞 + 出生点 + manifest）；物体导出 `.object.zip`（烘焙 SPZ + 可射线检测的碰撞/阴影代理 + manifest）。复查可在 Studio 里调水平、尺度、裁剪，再写回文件。CLI 从仓库运行是 `node src/cli.mjs`，装包后用 `npx splatforge`。无头转换依赖 Playwright 与本机 Chrome / Chromium；`inspect` 可在 Node 里直接读包。

## Recipe / links
- Repo: https://github.com/ZeshenTian/splatforge（0★，MIT）
- SKILL.md：https://github.com/ZeshenTian/splatforge/blob/main/skills/splatforge/SKILL.md
- 本地 Studio（需 Node 22.13+）：
  ```bash
  npm ci
  npm run dev
  ```
  把扫描拖到画布即可预览，导出完整包或碰撞资产。
- 物体转换示例：
  ```bash
  node src/cli.mjs convert ./plant.splat --mode object --height 0.40 -o ./plant.object.zip --json
  node src/cli.mjs review ./plant.object.zip
  ```
- Three.js：从 `splatforge` 导入 `loadSplatObject`（或对应的世界加载器）

## Why it made the cut
有可加载 SKILL.md、本地 CLI/Studio 和明确的 scene/object 导出格式，场景很窄但步骤完整。仓库与介绍帖都在本窗刚发布、尚无星，按完整配方收录，不是凭热度。GitHub Pages 演示仍在计划中，目前以本地 Studio 为准。
