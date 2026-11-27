# Three.js Game Skills（可玩的 Three.js 浏览器游戏技能包）

**Tags:** 3d, threejs, gamedev, vfx, graphics, qa, skill-pack
**Source:** [@majidmanzarpour](https://x.com/majidmanzarpour/status/2126281851946103117) · 2026-11-27
**Engagement:** 作者更新帖发布时 0 赞（窗口内刚发出）；仓库 [majidmanzarpour/threejs-game-skills](https://github.com/majidmanzarpour/threejs-game-skills) 现 2,913★，MIT。本窗为等待已久的第一方更新：新增 AAA VFX 技能，并写明同时支持 Antigravity、Codex 与 Claude Code。仓在本窗有新推送（2026-11-27）。

## When to use
要让编码 agent 从零做出**可玩、能验收的 Three.js 浏览器游戏**，或给已有项目补玩法、AAA 风格特效、UI、资源和发布检查时用。先点名 `threejs-game-director`，由导演按任务路由到专家技能，不必自己挑齐 10 个技能。它偏「能玩、能测、能发」的游戏生产管线，和已收录的 [Three.js Awesome Graphics Agent Skills](threejs-awesome-graphics-agent-skills.md)（更偏画面/光照/程序化材质词汇）互补，不是同一仓库。

## What it does
同一套 10 个 `SKILL.md` 给 Codex、Claude Code 和 Antigravity 用：

- `threejs-game-director`：总导演，保留范围和美术方向，按需调用专家技能
- `threejs-gameplay-systems`、`threejs-aaa-graphics-builder`、本窗新增的 `threejs-aaa-vfx-builder`（法术、武器、冲击和起步套件）
- `threejs-game-ui-designer`、`threejs-3d-generator`、`threejs-image-generator`、`threejs-audio-generator`
- `threejs-debug-profiler`、`threejs-qa-release`

包内带参考文档、辅助脚本、可放入项目的 TypeScript VFX 起步套件，以及 Vite + TypeScript + Three.js 脚手架。生成的游戏带确定性测试钩子、种子 RNG，以及 Playwright 冒烟/视觉回归/机器人试玩模板，方便 agent 自己验收。不强制特定模型或付费 API key。作者在 README 里附了多款演示游戏（如 Neon Ridge Drift、Ripcore）。

## Recipe / links
- Repo: https://github.com/majidmanzarpour/threejs-game-skills（2,913★，MIT）
- 安装（skills CLI；`-g` 为全局）：
  ```bash
  npx skills add majidmanzarpour/threejs-game-skills --skill '*' -a claude-code -g -y
  npx skills add majidmanzarpour/threejs-game-skills --skill '*' -a codex -g -y
  npx skills add majidmanzarpour/threejs-game-skills --skill '*' -a antigravity -g -y
  ```
  若本地 `skills` CLI 不支持某个 target，可克隆后用 `./install.sh --claude` / `--codex` / `--antigravity` / `--all`。覆盖同名技能需 `--force`；默认不会删除用户其他技能。
- 技能目录：`skills/*/SKILL.md`

## Why it made the cut
完整可安装技能包，场景清楚（可玩游戏而不仅是好看的场景），有导演路由、VFX 套件和验收模板。此前多次因缺少第一方介绍帖放在观察名单；本窗作者亲自宣布 AAA VFX 更新并写明多 agent 支持，达到单列标准。与 [Three.js Awesome Graphics](threejs-awesome-graphics-agent-skills.md) 分工不同，两者都收。
