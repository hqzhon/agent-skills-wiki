# Swarm Cursors / reveal-cursors（多光标重建页面动效）

**Tags:** frontend, motion, landing-page, claude-skill, ui
**Source:** [@hrstwt](https://x.com/hrstwt/status/2118646279068881088) · 2026-11-06
**Engagement:** harshit403-pixel/reveal-cursors · ~44★ · 推文 ~18 likes / 31 bookmarks · 效果致敬 Joel Califa Swarm

## When to use
想给首页加一段 **「页面被一群多玩家光标擦掉再重建」** 的展示动效（框选、打字、钢笔、标尺、alt 拖复制），又希望 SEO / 表单 / 分析仍走真实 DOM。

## What it does
Claude skill（`swarm-cursors/SKILL.md` + 安装脚本）：可挂浮动按钮、自动播放、热键、`?swarm` 链接或 `data-swarm-trigger`。支持按页面白名单、排除 cookie/聊天组件、以及干净卸载。产物是一份无依赖 `swarm-cursors.js`（~157KB / ~44KB gzip），`defer` 加载，不向服务器回传。也可用 `python swarm-cursors/scripts/install.py` 不经 Claude 直接安装。

## Recipe / links
- Repo: https://github.com/harshit403-pixel/reveal-cursors (~44★)
- SKILL.md: https://github.com/harshit403-pixel/reveal-cursors/blob/main/swarm-cursors/SKILL.md
- Claude Code: `cp -r swarm-cursors ~/.claude/skills/`
- 原效果: https://califa.github.io/swarm-site/

## Why it made the cut
可验证 skill 包（SKILL.md + install 脚本 + demo）+ 清晰落地页动效场景 + 本轮推文有实质互动。
