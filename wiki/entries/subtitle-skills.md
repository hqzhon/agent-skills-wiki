# subtitle-skills（本地 SRT ↔ VTT 转换、检查、平移、合并与拆分）

**Tags:** subtitles, srt, vtt, video, skill
**Source:** [@woshiyanali](https://x.com/woshiyanali/status/2124880506827510117) · 2026-11-23
**Engagement:** 本窗作者介绍帖 2 赞 · 仓库 [yanaaibuilders/subtitle-skills](https://github.com/yanaaibuilders/subtitle-skills) 现 0★，MIT，单一标准库 Python 脚本，中英 README

## When to use
处理本地字幕文件：SRT 与 WebVTT 互转、导出纯文本、检查重叠/时码损坏、整体平移、合并或拆分。不希望脚本访问网络，也不需要 ASS/TTML 等其他格式。

## What it does
一个可加载的 Agent Skill（`skills/subtitle-tools`）加一个只用 Python 标准库的 `subtool.py`：

- `convert`：SRT ↔ VTT，或导出 TXT；SRT→SRT 会重编号、去 BOM、统一 LF，保留 `<i>` `<b>` `<u>`
- `check`：重叠、零/负时长、乱序、编号、非法 UTF-8、BOM、UTF-16、换行等
- `shift` / 合并 / 拆分

不读写 ASS/SSA、SBV、TTML；VTT 的定位设置转到 SRT 时会丢掉（SRT 没有对应字段）。

## Recipe / links
- Repo: https://github.com/yanaaibuilders/subtitle-skills（0★，MIT）
- 安装：`npx skills add yanaaibuilders/subtitle-skills`
- 或拷贝 `skills/subtitle-tools` 到 `~/.claude/skills/subtitle-tools` 或 `~/.agents/skills/subtitle-tools`
- 也可直接跑：`python3 scripts/subtool.py check samples/broken.srt`

## Why it made the cut
范围写得很清楚（做什么、不做什么），MIT、零网络、标准库即可复核。星数为 0，但是完整可装的小工具技能，适合做字幕的人直接用。
