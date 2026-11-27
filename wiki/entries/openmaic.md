# OpenMAIC（多 Agent 互动课堂：安装 / 生成 / 二开）

**Tags:** education, classroom, multi-agent, openclaw, chinese, skill-pack
**Source:** [@kewangx](https://x.com/kewangx/status/2126090842511389148) · 2026-11-27
**Engagement:** 教育开源盘点帖 2 赞 / 1 收藏（本窗同时提到 DeepTutor 等产品，那些不是本条）；仓库 [THU-MAIC/OpenMAIC](https://github.com/THU-MAIC/OpenMAIC) 现 44,605★，MIT。清华 MAIC 团队，有论文与在线 Demo，最近推送到 2026-11-27。

## When to use
想用 OpenMAIC 搭一节多 Agent 互动课堂（含理化虚拟实验）、在 Live Demo 或本地完成配置，或基于 @openmaic/* SDK 做二次开发时用。它不是通用家教 skill，而是围着这个课堂系统设计的安装与扩展配方。

## What it does
仓库本身是可一键体验的多 Agent 课堂产品，并带一组可加载技能：根目录 skills/openmaic/SKILL.md 负责安装、生成课堂和二开；另外还有 PBL、slide/stage DSL、事实核对、风格克隆等 skills/agent-runtime/* 技能。openmaic 技能强调分阶段确认、不要默认让用户把 API key 贴进对话、课堂所用模型以服务端 openmaic.yml / 网页设置为准，而不是复用宿主 agent 的密钥。

## Recipe / links
- Repo: https://github.com/THU-MAIC/OpenMAIC（44,605★，MIT）
- 主技能：https://github.com/THU-MAIC/OpenMAIC/blob/main/skills/openmaic/SKILL.md
- Live Demo: https://open.maic.chat/
- 把 skills/openmaic/（以及需要的 skills/agent-runtime/*）拷进 agent 的 skills 目录，然后按 SKILL.md 分阶段配置。不要把提供商密钥写入对话。

## Why it made the cut
官方团队仓库带完整可加载 SKILL.md 和清晰的使用边界，场景明确，社区信号非常高。同帖里的 DeepTutor / StoryCraft / OpenLingo 等是产品或平台，没有作为本条的附属技能收录。
