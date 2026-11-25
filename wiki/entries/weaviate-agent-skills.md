# Weaviate Agent Skills（官方）

**Tags:** official, weaviate, vector-db, search, rag, skill-pack
**Source:** [@_jphwang](https://x.com/_jphwang/status/2125201260093607936) · 2026-11-24
**Engagement:** 本窗介绍帖 10 赞；仓库 [weaviate/agent-skills](https://github.com/weaviate/agent-skills) 现 104★，BSD-3-Clause，2026-11-09 仍有推送

## When to use
要让编码 agent 查询、管理或导入 **Weaviate** 向量库时用：语义/混合/关键词搜索、自然语言问答、集合与 schema、从 PDF/CSV/JSON 导入数据。没有 Weaviate 实例时，技能会引导去云控制台开免费 sandbox。不要把它当成通用网页搜索。

## What it does
官方技能包，目前公开：
- `weaviate`：搜索、过滤、集合管理、示例数据与导入；
- `weaviate-cookbooks`：配套 cookbook。
仓库说明兼容任何支持 Agent Skills 格式的 agent。脚本会用到一些第三方包，README 提醒上游安全需自行跟踪。

## Recipe / links
- Repo: https://github.com/weaviate/agent-skills（104★，BSD-3-Clause）
- 通用安装：`npx skills add weaviate/agent-skills`
- Claude Code 插件：
```
/plugin marketplace add weaviate/agent-skills
/plugin install weaviate@weaviate-plugins
```
- 也可 `git clone` 后 `claude --plugin-dir .`
- Skill: [skills/weaviate/SKILL.md](https://github.com/weaviate/agent-skills/blob/main/skills/weaviate/SKILL.md)
- 新用户可先在 [Weaviate Cloud](https://console.weaviate.cloud) 开免费 cluster，并阅读 `skills/weaviate/references/environment_requirements.md`。

## Why it made the cut
向量数据库厂商官方包，有明确「何时用」、可加载 SKILL.md 和标准安装命令。104★、BSD-3-Clause。本窗介绍帖互动一般，按官方仓库补收。
