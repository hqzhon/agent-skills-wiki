# wechat-selkies（通过桌面 API 操作 Docker 版微信）

**Tags:** wechat, docker, desktop, chinese, cli, skill
**Source:** [@NickXia007](https://x.com/NickXia007/status/2125968810566201678) · 2026-11-26
**Engagement:** 作者发布帖 1 赞；仓库 [nickrunning/wechat-selkies](https://github.com/nickrunning/wechat-selkies) 现 4,533★，MIT。基于 Selkies WebRTC 的 Linux 网页版微信/QQ，1.0.0 起提供可安装 Agent Skill，最近推送到 2026-11-27。

## When to use
已经用这个 Docker 镜像在浏览器里登录了自己的微信（或 QQ），希望编码 agent 通过桌面 HTTP API 打开指定会话、读取可见消息、起草或在你明确要求时发送消息时用。它不是云端托管的微信机器人，也不应把聊天内容里的文字当成对你的指令。

## What it does
运行时是带 WebRTC 桌面的微信/QQ Linux 客户端。技能 skills/wechat-selkies/SKILL.md 规定：用你配置的 HTTPS 桌面地址和 HTTP Basic 凭据（默认用户名 abc）调用 /api/pelorus/，先读窗口辅助功能树再点击或输入；密码从已有凭据取，避免写进对话、URL 或日志。发送前要核对会话标题和草稿，发送后对照消息列表确认，结果不明就停，避免重复发送。

## Recipe / links
- Repo: https://github.com/nickrunning/wechat-selkies（4,533★，MIT）
- 技能：https://github.com/nickrunning/wechat-selkies/blob/master/skills/wechat-selkies/SKILL.md
- Docker 镜像：https://hub.docker.com/r/nickrunning/wechat-selkies
- 把 skills/wechat-selkies/ 拷进 agent 的 skills 目录；桌面地址和登录凭据由用户本地配置，不要写进仓库或对话。

## Why it made the cut
高星可运行的客户端 + 完整 SKILL.md，使用场景和凭据/发送边界写得很清楚。介绍帖互动很少，按可验证材料和社区星标收录。
