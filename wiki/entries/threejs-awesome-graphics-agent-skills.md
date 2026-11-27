# Three.js Awesome Graphics Agent Skills（高质量 Three.js 画面技能包）

**Tags:** 3d, threejs, graphics, shaders, webgpu, procedural, skill-pack
**Source:** [@scottstts](https://x.com/scottstts/status/2126115898566299705) · 2026-11-27
**Engagement:** 作者介绍 v0.14.0 更新帖 11 赞 / 9 收藏；仓库 [scottstts/Threejs-Awesome-Graphics-Agent-Skills](https://github.com/scottstts/Threejs-Awesome-Graphics-Agent-Skills) 现 1,033★。npm 包版本 0.14.0；package.json 许可为 MIT AND GPL-3.0-only（技能包 MIT，部分源材料 GPL-3.0）。本窗为等待已久的第一方更新帖。

## When to use
要用编码 agent 做 **Three.js 场景或游戏里「看起来像样」的画面**——光照、PBR、体积云、光谱海面、程序化植被/建筑、后处理等——而不是再让模型靠通用 3D 常识去猜时用。它强调「好画面的实现词汇」，不是 three.js API 速查。和已收录的 [papercraft](papercraft.md)（弹出式剪纸风）、[diorama](diorama.md)、[3dviz-pro-max](3dviz-pro-max.md) 互补；也不同于本窗单列的 [Three.js Game Skills](threejs-game-skills.md)（更偏可玩的游戏玩法、AAA VFX 与资源管线）。

## What it does
约 28 个技能，带 `threejs-skill-router` 把视觉目标拆到最小的专家系统，以及参考图解读、相机、程序化几何/材质/植被/建筑、地形、行星、光谱海面、体积云、Bloom、阴影、曝光与调色、时序稳定和视觉验收等。每个图形系统都要求可复现输入、可调参数、诊断输出和「无后处理基线仍然可读」。附带 example gallery，用来给 agent 看具体实现，而不只是文字描述。本窗 v0.14.0 是一次全包更新。需要 Node.js 18+。

## Recipe / links
- Repo: https://github.com/scottstts/Threejs-Awesome-Graphics-Agent-Skills（1,033★；MIT AND GPL-3.0-only）
- npm: `threejs-awesome-graphics-agent-skills@0.14.0`
- 安装（按 agent 选择 target，也支持 `--scope project`）：
  ```sh
  npx threejs-awesome-graphics-agent-skills@latest install --agent claude-code
  npx threejs-awesome-graphics-agent-skills@latest install --agent cursor
  npx threejs-awesome-graphics-agent-skills@latest install --agent antigravity
  ```
  还支持 `codex`、`github-copilot`、`grok`、`universal`（`~/.agents/skills`）等。卸载：`npx threejs-awesome-graphics-agent-skills uninstall --agent <target>`。

## Why it made the cut
完整可安装技能包，场景清楚，有 router、示例库和多 agent 安装器。此前因缺少第一方介绍帖放在观察名单；本窗作者发布 v0.14.0 大更新，达到单列标准。许可是混合的，装前看仓库的 THIRD_PARTY_NOTICES。
