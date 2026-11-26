# wx-downloader（微信视频号下载 CLI + Agent Skill）

**Tags:** video, wechat, downloader, cli, skill
**Source:** [@khyssabc](https://x.com/khyssabc/status/2125893827215171796) · 2026-11-26
**Engagement:** 介绍帖 1 赞；仓库 [QinGeneral/wx-downloader](https://github.com/QinGeneral/wx-downloader) 现 93★。许可是 **MIT + Commons Clause**（可按 MIT 使用，但不得出售本软件本身）。技能在 `skills/wx-downloader/SKILL.md`，需先单独安装 Python CLI。

## When to use
要用命令行（或让支持 Skill 的助手调用该 CLI）把**微信视频号分享链接**存成 MP4，并且不想先装微信客户端时用。登录走腾讯元宝扫码/手机号验证。只接受 `https://weixin.qq.com/sph/...` 形式的普通分享链接；不是通用视频下载器，也不能绕过账号或平台限制去抓未分享的内容。

## What it does
`wx-downloader` CLI（PyPI 当前文档版本 0.1.2，Python 3.10+）支持单条或 JSON 批量下载、按文件大小去重、自定义成品目录（默认 `~/Downloads/wx-channels`）和缓存目录。没有本地凭据时，`download` 会打开浏览器等你登录；无人值守应加 `--no-login`。技能本身不安装 CLI，只指导助手调用已安装的命令；并明确要求不要读取或输出 `auth.json` 里的 Cookie 和请求头。

## Recipe / links
- Repo: https://github.com/QinGeneral/wx-downloader（93★，MIT + Commons Clause）
- 技能：https://github.com/QinGeneral/wx-downloader/blob/main/skills/wx-downloader/SKILL.md
- 安装 CLI：`uv tool install wx-downloader`（或 `pip install wx-downloader`）
- 技能需从源码仓库复制 `skills/wx-downloader/` 到 agent 的 skills 目录（PyPI 包只含命令）
- 单条下载示例：`wx-downloader download 'https://weixin.qq.com/sph/VIDEO_ID' --json`

## Why it made the cut
可验证的 CLI + 配套 `SKILL.md`，场景具体，技能里对登录凭据有明确约束。93★ 不算高，但材料完整；注意 Commons Clause，不能把这个工具当商品再卖。只用于你有权保存的分享链接。
