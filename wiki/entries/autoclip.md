# AutoClip（本地优先的长视频切片出片技能）

**Tags:** video, clipping, short-form, mcp, local-first, chinese, skill-pack
**Source:** [@lengqie](https://x.com/lengqie/status/2126444455729246368) · 2026-11-28
**Engagement:** 本窗为中文介绍帖（6 赞），非仓库所有者第一方；仓库 [zhouxiaoka/autoclip](https://github.com/zhouxiaoka/autoclip) 现 17,578★ / 2,494 forks，MIT。项目同时提供桌面客户端、CLI、MCP 和可加载技能。

## When to use
要把 YouTube / B 站链接或本地长视频（讲座、访谈、播客、课程、直播回放）自动剪成各平台短视频，并一起交出封面、发布文案和 ZIP 发布包时用。它强调本地优先：裁剪和渲染在本机用 FFmpeg 跑，可以接自己的 API Key，也可以挂 Ollama / LM Studio 配本地 Whisper 或 SenseVoice 离线跑。只要原始高光列表、或把旧切片改发到 Upload-Post，不要走这条出片流程。

## What it does
仓库 `skills/` 下有多条技能，主技能 [autoclip](https://github.com/zhouxiaoka/autoclip/blob/main/skills/autoclip/SKILL.md) 的交付物是四样：按平台剪好的成片、封面、发布文案、ZIP。有 AutoClip MCP 时走工具（`start_quick_output` / 轮询状态），否则用 `autoclip produce <source> --json`。另外还有 `product-board`、`template-cloner`。桌面端、CLI 和 MCP 共用数据目录。v1.6 还支持 OBS 下播后截取回放、识别游戏高光。

## Recipe / links
- Repo: https://github.com/zhouxiaoka/autoclip（17,578★，MIT）
- 给 agent 装技能 / 启动 MCP：
  ```bash
  npx skills add zhouxiaoka/autoclip
  uvx autoclip-mcp
  ```
- 也可用桌面安装包（macOS / Windows）或 `docker compose up` 自托管网页版。模型密钥放桌面设置或环境变量 `AUTOCLIP_API_KEY`，不要写进对话。
- CLI 示例：`autoclip produce talk.mp4 --platform tiktok --portrait-style podcast --json`

## Why it made the cut
有具体出片配方和 SKILL.md，使用场景清楚，仓库星标很高且带 MIT 许可、MCP 与 CLI。本窗来自介绍帖而不是作者第一方，但上游材料足够独立核实。这是工具+技能一体的项目，条目记录的是可加载技能与 agent 用法。
