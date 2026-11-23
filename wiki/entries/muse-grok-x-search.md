# muse-grok-x-search（给 Muse 补上只读的 X 搜索）

**Tags:** muse, x-search, research, skill
**Source:** [@777iiikk](https://x.com/777iiikk/status/2124513964432502885) · 2026-11-22
**Engagement:** 实测安装帖 206 赞 / 18 转 / 319 收藏；仓库 [kgmkm/muse-grok-x-search](https://github.com/kgmkm/muse-grok-x-search) 227★，MIT。

## When to use
在 **Muse** 里要查 X（Twitter）上的实时讨论、引用和回复，而内置社交搜索只覆盖 Instagram / Facebook / Threads 时使用。它通过 xAI 的 Grok Build CLI 调用只读 `x_search`，不发帖、不点赞、不关注。

## What it does
Muse 专用 skill。把 `SKILL.md` 和 `skill.yaml` 放到 Muse 的 `~/workspace/custom-skills/grok_x_search/`，用 Grok Build 登录后即可用自然语言搜 X。技能写明：登录必须用 device-code，由用户在自己的设备上批准；禁止索要密码或验证码，也禁止读取 `~/.grok/auth.json`。每次搜索前用 `grok models` 检查会话，过期就重新走 device-code。作者在 Muse VM 上做过端到端实测（约 26 秒一次搜索）。受 Grok Build / X 账号档位和额度限制。

## Recipe / links
- Repo：https://github.com/kgmkm/muse-grok-x-search（MIT，227★）
- 依赖：带 shell 的 Muse、[Grok Build CLI](https://x.ai)，以及可用的 SuperGrok / X Premium 类方案或 `XAI_API_KEY`。
- 把仓库发给 Muse 并请它按 README / SKILL.md 安装；或手动拷贝 `SKILL.md` 与 `skill.yaml`。
- 这是 Muse + Grok Build 的专用技能，不是给 Claude Code / Cursor 通用的 X API 封装。

## Why it made the cut
有清晰的「何时用」、只读约束、登录安全步骤和作者实测，仓库材料完整。平台绑定强，但作为可装 skill 仍然值得单独成条。
