# Open 3D Skills（3D 与动效网页 8 件套）

**Tags:** 3d, threejs, motion, web, video, skill-pack
**Source:** [@QingQ77](https://x.com/QingQ77/status/2117831200316526621) · 2026-11-04
**Engagement:** 推文约 290 次浏览；仓库 Moh4696/open-3d-skills 约 230★（MIT，带 CI 检查）

## When to use
让编码 agent 做 3D / 动效网页时：纯代码搭 three.js 场景、滚动驱动的影片、Safari 也能播的透明视频、跟随光标的角色、机器爆炸图，以及在真实浏览器里自检并录成 60fps 视频。

## What it does
- 8 个独立技能（如 `threejs-scene`、`exploded-view`、`frame-capture` 等），每个技巧都先在真实网站上用过、脚本在真实素材上跑过才收进来。
- 示例场景（凉亭、电机拆解）全部由代码生成，不依赖模型文件或贴图下载。
- 教 agent 用真实浏览器检查结果，并逐帧录制成流畅视频。

## Recipe / links
- Repo: https://github.com/Moh4696/open-3d-skills
- 交互安装：`npx skills add Moh4696/open-3d-skills`（需 Node 22.20+）
- 全装免询问：`npx skills add Moh4696/open-3d-skills -g -y`；单个：`--skill threejs-scene`
- Claude Code 插件：`/plugin marketplace add Moh4696/open-3d-skills` 后 `/plugin install open-3d-skills@open-3d-skills`
- Codex 插件：`codex plugin marketplace add Moh4696/open-3d-skills`

## Why it made the cut
仓库完整、MIT、安装路径清晰，场景具体（3D / 动效网页），有可验证示例和 CI，社区信号也不错；补足 wiki 中 three.js 网页方向。
