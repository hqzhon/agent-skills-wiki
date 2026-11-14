# repo-cinema（仓库自动拍成产品演示片）

**Tags:** video, demo, ffmpeg, chrome-cdp, skill
**Source:** [@A_Znk_](https://x.com/A_Znk_/status/2121494612749566127) · 2026-11-14（英文介绍见 [同一作者另一帖](https://x.com/A_Znk_/status/2121495777260314823)）
**Engagement:** 发现帖互动低；仓库 [Yuki-zik/repo-cinema](https://github.com/Yuki-zik/repo-cinema) 当日发布、0★，MIT；README 带自制演示 GIF

## When to use
要从一个代码仓库自动做出 Screen Studio 级的 60fps 产品演示、发布片或 README 走查 GIF：网页、CLI、IDE 插件、UI 库都可以。不想靠手动量指针、反复补拍。

## What it does
一条 Director SKILL.md，按五段确定性流水线执行：

1. **analyze**：读清单、路由、命令、组件和文档，归类原型，并提炼 `Persona → Pain Point → User Action → Durable Outcome` 场景（不拍内部调试页）
2. **plan**：写 `storyboard.json` / `storyboard.html`；镜头框的是 `bbox(trigger ∪ outcome)`，宽画面锁定水平焦点，避免坐标轴或右侧列被裁切
3. **stage**：搭可回放的演示台
4. **render**：虚拟时钟 + Chrome CDP → FFmpeg，60fps，带光标物理和微音效
5. **verify**：抽帧做成 contact sheet，自动检查裁切和点偏

## Recipe / links
- Repo: https://github.com/Yuki-zik/repo-cinema
- SKILL.md: https://github.com/Yuki-zik/repo-cinema/blob/main/skills/repo-cinema/SKILL.md
- 中文说明：仓库内 `README_ZH.md`
- 安装：`npx skills add Yuki-zik/repo-cinema`
- 需要 Node 20+

## Why it made the cut
不是「让 AI 录个屏」的空喊：有分镜原则、防裁切规则、确定性渲染和抽帧自检，SKILL.md 与安装命令齐全。仓库新、尚无星标，质量看流水线是否可执行。
