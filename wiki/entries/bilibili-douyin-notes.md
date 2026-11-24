# bilibili-douyin-notes（B站/抖音/YouTube/小红书视频课堂笔记）

**Tags:** video, notes, bilibili, douyin, youtube, xiaohongshu, chinese, skill
**Source:** [@Chenfacai0](https://x.com/Chenfacai0/status/2124994149250138117) · 2026-11-24
**Engagement:** 本窗介绍帖 6 赞 / 5 收藏 · 仓库 [lucky-Luor/bilibili-douyin-notes](https://github.com/lucky-Luor/bilibili-douyin-notes) 现 200★，MIT，带 CI、示例笔记和 `scripts/doctor.py` 自检

## When to use
收藏夹里堆着教程，看完记不住、复习还要拖进度条：把 B站、抖音、YouTube 或小红书的视频链接丢给 agent，让它整理成 Markdown 课堂笔记；也可以对已有课程说「考考我 / 复习这门课」。

## What it does
可加载的 Agent Skill：先抓字幕，没有字幕就在本地做语音识别，再按模板写出笔记，并可截重点画面。免登录可用，不调付费 API。可选扫码登录 B站以获取 AI 字幕。仓库带完整 `SKILL.md`、`examples/`（如李宏毅机器学习节选）和离线测试。

需要 Python 3.10+，不需要 GPU。无字幕时会在本地跑识别，依赖见 `requirements.txt`。

## Recipe / links
- Repo: https://github.com/lucky-Luor/bilibili-douyin-notes（200★，MIT）
- 一行安装（Claude Code）：
  ```bash
  git clone https://github.com/lucky-Luor/bilibili-douyin-notes.git ~/.claude/skills/bilibili-douyin-notes && pip install -r ~/.claude/skills/bilibili-douyin-notes/requirements.txt
  python ~/.claude/skills/bilibili-douyin-notes/scripts/doctor.py
  ```
- 其他 agent 把路径改成对应的 skills 目录（如 `~/.agents/skills/`、`~/.zcode/skills/`）
- 用法：对 AI 说「帮我把这个视频做成课堂笔记：https://www.bilibili.com/video/BVxxxx」

## Why it made the cut
中文场景非常具体，四平台链接、本地字幕/识别、笔记模板和自检脚本都在仓库里，200★ 且有示例可复核，不是「把视频总结一下」的空提示。
