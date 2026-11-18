# OpenMotion（参考片 → 可编辑品牌动效）

**Tags:** video, motion, brand-kit, skill-pack
**Source:** [@hx0000001](https://x.com/hx0000001/status/2122844696783598036) · 2026-11-18
**Engagement:** 发现帖互动很低；仓库 [nexu-io/openmotion](https://github.com/nexu-io/openmotion) 现 11,251★ / 1,119 forks，Apache-2.0（2026-05-11 建仓，本轮仍在推送）

## When to use
要把一条参考成片或社交平台视频，按自己的品牌套件和文案重做成可编辑的动效，并导出 YouTube / Shorts / Reels / TikTok 用的 MP4；或者从模板库改一版，而不是在 CapCut / Claude Motion 里从头手搓。

## What it does
开源的全栈 Agent 视频工作室：用 HTML 写镜头，Agent 拆解参考片、重建镜头与转场、补齐缺失素材，再在 Studio 里改时间轴并渲染。仓库带 300+ 份 `Motion.md`（镜序、时码、转场）和品牌套件；核心工作流是 5 个 `SKILL.md`：

- `openmotion-recreate`：按参考片重建并对结果
- `openmotion-template-to-video`：改已有可编辑模板
- `openmotion-director`：原创影片的叙事、运动、声音和创意审看
- `openmotion-video-to-template`：做成可复用的便携模板
- `openmotion-production`：局部修改、预览、检查、排错和导出

README 写明支持 Claude Code、Codex、WorkBuddy 等约 22 个 agent。生图 / 视频 / 配乐 / 旁白可接 GPT Image、Seedance、Suno、Eleven 等，需自备密钥。只把 skill 装进 agent **不会**带上运行时或 MCP，还要按 `install.md` 接通 Studio。

## Recipe / links
- Repo: https://github.com/nexu-io/openmotion（Apache-2.0，11,251★）
- 在当前 agent 里从源码安装（仓库推荐路径）：让 agent 阅读并执行 https://github.com/nexu-io/openmotion/blob/main/install.md
- 可选：安装已发布的 npm 应用，见 https://github.com/nexu-io/openmotion/blob/main/docs/install.md（发布渠道可能落后于主仓）
- 只拷贝技能说明（需先有仓库检出，不安装运行时 / MCP）：
  ```sh
  npx skills add ./skills --list
  npx skills add ./skills --skill openmotion-director openmotion-production openmotion-template-to-video openmotion-recreate openmotion-video-to-template
  ```
- 本地跑 Studio：`git clone` 后 `npm ci && npm run build:studio && npm start`，以启动时打印的 `studioUrl` / `previewUrl` 为准
- 官网：https://open-design.ai/motion/

## Why it made the cut
有明确使用场景、可验证的官方仓库和一组分工清楚的 SKILL.md，社区信号很高。与已收录的 OpenMontage（更偏整条制作流水线）以及 Remotion / Zazzy 等成片技能互补：OpenMotion 主打「参考片 + 品牌套件 → 可编辑重制」。
