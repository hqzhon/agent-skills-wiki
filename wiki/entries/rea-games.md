# rea-games（逐帧复刻游戏并验证玩法一致）

**Tags:** gamedev, reverse-engineering, testing, replay, skill
**Source:** [@GitTrend0x](https://x.com/GitTrend0x/status/2126277437969387839) · 2026-11-27
**Engagement:** 出现在技能盘点帖（本窗 0 赞）中；仓库 [erkamyaman/rea-games](https://github.com/erkamyaman/rea-games) 现 349★（2026-11-25 新建，本窗仍在推送），MIT。项目站点：https://erkamyaman.github.io/rea-games

## When to use
要**逆向一款游戏的行为、用另一个引擎重做，并证明玩法一致**时用——例如把原作迁到 Web、Godot、Bevy 或 Unity，或理解它到底怎么运行。口号是 “rea this game”。它记录输入与状态，写成公开的 `GAME.md` 行为规格，再逐帧对照，而不是靠眼看「好像差不多」。不要用它去复制受版权保护的美术、音乐、名称或源码；技能要求先确认原作许可，并从开源/宽松许可的原作开始。

## What it does
可加载技能 `rea-games`，核心循环是：记录原作 → 写规格 → 做移植 → 验证 → 修复 → 重复。在 `rea-games verify` 报告所有用例一致之前，不得宣称移植完成。开始前会检查 Node.js 22+，浏览器游戏还需要 Playwright / Chromium。流程包括：

1. `rea-games new <game>` 脚手架：`games/<game>/` 下生成 `game.json`、`record.mjs`、`GAME.md` 和移植桩
2. 让原作可复现：替换时钟和 `requestAnimationFrame`，卡住随机数和输入时序
3. 记录行为并写成 `GAME.md`，再在目标引擎重建
4. 逐帧/按用例验证，失败就修，直到验证通过

仓库还带若干示范游戏。这和已收录的 [rea-video](rea-video.md)（视频逐镜逆向）名字相近，但对象是游戏行为而不是影像剪辑。

## Recipe / links
- Repo: https://github.com/erkamyaman/rea-games（349★，MIT）
- 站点：https://erkamyaman.github.io/rea-games
- 技能路径：`skills/rea-games/SKILL.md`
- 安装（把技能目录拷到 agent skills 目录，或使用 skills CLI）：
  ```bash
  npx skills add erkamyaman/rea-games
  ```

## Why it made the cut
配方很具体（记录、规格、重建、强制验证），使用场景清楚，有 SKILL.md、MIT 许可和短时间内可观的星标。本窗来自盘点帖而不是作者第一方介绍，但仓库材料足够独立核实。务必遵守原作许可，只做干净室式的行为复刻。
