# SEO Skills（Illyism，30 个可落地 SEO 工作流）

**Tags:** seo, geo, content, audit, skill-pack
**Source:** [@growaiskills](https://x.com/growaiskills/status/2124364557644697709) · 2026-11-22
**Engagement:** 本窗介绍帖 21 赞 / 6 转 / 24 收藏（介绍称作者原帖收藏量很高）；仓库 [Illyism/seo-skills](https://github.com/Illyism/seo-skills) 1,912★，README 标明 MIT（GitHub 许可证字段暂空）。

## When to use
想让 Claude Code / Cursor / Codex 等编码 agent **直接在仓库里改 SEO**（标题、robots.txt、301、内链、对比页等），交出可合并的 PR / 文件，而不是再出一份没人动手的审计 PDF 时使用。它和已收录的 [seo-canon](seo-canon.md)（Google 官方文档离线技能）、[SEO Prompt Master](seo-prompt-master.md)（技术 SEO / GEO 审计 CLI）互补：这一套是 30 个可执行工作流，并可接实时 SEO MCP。

## What it does
30 个符合 Agent Skills 规范的 `SKILL.md`：技术 SEO 体检、程序化 SEO、面向购买决策的竞品/替代页、目录站提交、外链与 GEO（生成式引擎优化）等。agent 启动时只读名称和描述，匹配到任务再打开全文。可用 `seo-autopilot` 等单技能安装。仓库还提供浏览目录（[il.ly/skills](https://il.ly/skills)）和 MCP 配置，用于拉取 Ahrefs、DataForSEO 等实时数据。

## Recipe / links
- Repo：https://github.com/Illyism/seo-skills（README 标 MIT，1,912★）
- 安装：
  ```
  npx skills add Illyism/seo-skills
  npx skills add Illyism/seo-skills --skill seo-autopilot
  npx skills add Illyism/seo-skills --list
  ```
- 部分工作流会调用第三方 SEO API / MCP，装前先看权限和收费项；评论区有人建议先做仓库安全扫描。

## Why it made the cut
场景清楚，产出是仓库里的具体改动而不是报告；30 个 SKILL.md 可逐个安装，星数高、持续在更新。本窗多条中文介绍帖把它从「错过的高信号包」补进目录。
