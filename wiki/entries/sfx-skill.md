# sfx-skill（合成 + CC0 采音做游戏音效）

**Tags:** audio, sfx, gamedev, synthesis, skill
**Source:** 上轮 Watch 复核（本窗未见新的介绍帖；仓库 2026-11-25 仍在推送）
**Engagement:** 上轮记录约 40★；仓库 [owoevan-dev/sfx-skill](https://github.com/owoevan-dev/sfx-skill) 现 42★，MIT。SKILL.md 路径已核对：`skills/sound-effects/SKILL.md`。

## When to use
要为游戏或应用做一套可编辑的音效，并且**不想走音频生成模型**时用：用合成层和 CC0 实地录音搭配，再导出多种变体、响度对齐，并按引擎格式输出。合成在安装后即可用；若要用真实录音，agent 会先征得同意再下载资料库（获取约 2.9 GB，解压后约 7.2 GB，可事后删除压缩包）。

## What it does
单一技能 `sound-effects`：按层设计音效、渲染变体、统一响度并导出。默认在本机用 Python 离线渲染；只有在你同意下载录音时才联网，并且按公开校验和核对文件，文档称不会把音频发到别处。可选 FFmpeg（Ogg / MP3 / FLAC）。作者另有独立的 `music-skill`（写可编辑的乐器片段），两套可一起用，也可分开。

## Recipe / links
- Repo: https://github.com/owoevan-dev/sfx-skill（42★，MIT）
- Skill: [skills/sound-effects/SKILL.md](https://github.com/owoevan-dev/sfx-skill/blob/main/skills/sound-effects/SKILL.md)
- Claude Code：`/plugin marketplace add owoevan-dev/sfx-skill` → `/plugin install sfx-skill@sfx-skill`
- 其他宿主：`npx skills add owoevan-dev/sfx-skill`
- 依赖：Python 3.10+ 与 NumPy；在技能目录执行 `python -m pip install -r skills/sound-effects/requirements.txt`（`doctor` 也会打印命令）

## Why it made the cut
上轮因未核对可加载路径而暂缓。现已确认 SKILL.md、本机离线渲染和可选录音库的同意门槛，场景清楚。42★、MIT，社区信号一般，按可验证配方收录。
