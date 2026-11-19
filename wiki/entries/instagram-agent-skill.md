# Instagram Agent Skill（13 个 Instagram 运营技能）

**Tags:** instagram, content, hooks, social, skill-pack
**Source:** [@AKhomssi](https://x.com/AKhomssi/status/2123170873628655974) · 2026-11-19
**Engagement:** 发现帖约 1 赞；仓库 [Jakeschincariol/instagram-agent-skill](https://github.com/Jakeschincariol/instagram-agent-skill) 现 7,116★，MIT（与已收录的 [YouTube Agent Skill pack](youtube-agent-skill.md) 为同一作者的姊妹包）

## When to use
要用 Claude 等 agent 做 Instagram 内容，但不自动发帖：写 Reels 脚本与钩子、打分、找对标、caption 检查、主页审计、周计划、故事/轮播/留言，以及去 AI 腔。技能只写草稿，发布仍由人确认。

## What it does
13 个技能（`ig-reel`、`ig-viral`、`ig-caption`、`ig-human`、`ig-plan`、`ig-profile`、`ig-audit`、`ig-carousel`、`ig-story`、`ig-comment`、`ig-dm`、`ig-reply`、`ig-repurpose`）。其中 `ig-reel` 按 26 种钩子公式出选项并用本地 `hookscore.py` / `beats.py` 打分、排拍点；humanizer 去掉常见 AI 套话后再做一轮检查。可写 `~/.claude/instagram/voice.md` 固定口吻。无需 API Key。

## Recipe / links
- Repo: https://github.com/Jakeschincariol/instagram-agent-skill（MIT，7,116★）
- Claude Code：`cp -r instagram-agent-skill/skills/ig-* ~/.claude/skills/`
- 或插件：`/plugin marketplace add Jakeschincariol/instagram-agent-skill` 后 `/plugin install instagram-agent`
- 也可把单个 `SKILL.md` 贴进对话当模式（会失去本地 Python 工具）

## Why it made the cut
结构与已收录的 YouTube 包同类，但是独立的 Instagram 运营配方：带可运行的钩子/拍点工具和 humanizer，安装路径清楚，默认不代发。
