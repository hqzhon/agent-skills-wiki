# Web Deck（单文件离线 WebGL2 演示文稿）

**Tags:** slides, webgl, threejs, presentation, html, skill
**Source:** [@Renzexi01](https://x.com/Renzexi01/status/2126595309841306072) · 2026-11-28
**Engagement:** 作者介绍帖 1 赞；仓库 [RZX00/web-deck](https://github.com/RZX00/web-deck) 现 0★，MIT，2026-11-28 建仓，带 CI。它把 @fluxxrider 的演示《The Last Boring Slide》（[thelastboringslide.com](https://thelastboringslide.com)）里的做法收成可复用技能，并不声称拥有该演示的画面。

## When to use
要把一个议题或研究简报做成**可离线打开的单文件交互 HTML 演示**（WebGL2 / GLSL、可拖分割对比、中英文排版），而不是静态幻灯片或一段 MP4 时用。不要用它做常规 PPT/HTML 翻页稿——那是 [PPT Agent Skill](ppt-agent-skill.md)、[Frontend Slides](frontend-slides.md) 或 [Dashi PPT Skill](dashi-ppt-skill.md) 的范围；也不要用它做口播剪辑。仓库自陈尚未在 Claude Code / Codex / Cursor 的真实会话里做过端到端托管验证，目前验证过的是 Windows / CI 里的构建和 7 帧视觉质检。

## What it does
可加载技能 `skills/web-deck/SKILL.md` 把演示拆成：先做一手资料和三种视觉方向提案，锁定论点、介质转变和互动预算；再复制自带的 `starter-engine`，用安全的引擎原语（`gfx.target3D()`、`gfx.drawSplit`、介质/半调/蓝图等附加层）搭场景；最后 `npm run build && npm run capture` 做单文件打包和 2× HiDPI 质检。成品是 `dist/<slug>.html`，构建时不请求 CDN，可从 `file://` 打开。可选再导出 MP4（需 ffmpeg）。技能对中文排版写了 `Intl.Segmenter("zh-CN")` 和禁则断行；音频用 Just Intonation 合成加上打包的 CC0 拟音。

## Recipe / links
- Repo: https://github.com/RZX00/web-deck（0★，MIT）
- 推荐：让编码 agent 阅读并执行 https://github.com/RZX00/web-deck/blob/main/docs/install.md
- 技能正文：https://github.com/RZX00/web-deck/blob/main/skills/web-deck/SKILL.md
- 依赖：Node.js 20+；视觉质检需要本机 Chrome / Edge / Chromium。构建和演示过程声称不上网、无遥测。
- 仓库也提供 `install.sh` / `install.ps1`；更稳妥的是先读 `docs/install.md`，再决定是否跑安装脚本。

## Why it made the cut
有明确的交付物（单文件离线 WebGL2 演示）、完整 SKILL.md、起步引擎和视觉质检，和已有的 HTML/PPTX 幻灯技能不是同一条。0★、当天新建，且作者写明部分宿主尚未实测，按可验证材料收录，并在条目里保留这些限制。
