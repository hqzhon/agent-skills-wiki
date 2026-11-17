# SciWrite（科学论文写作审校）

**Tags:** academic, scientific-writing, editing, review, skill
**Source:** [@LorenaABarba](https://x.com/LorenaABarba/status/2122599340262785153) · 2026-11-17
**Engagement:** 发现帖 12 赞 / 15 收藏；仓库 [labarba/sciwrite](https://github.com/labarba/sciwrite) 现 890★ / 107 forks；SKILL.md 声明 CC-BY-4.0，并有 Zenodo DOI

## When to use
要审校、压缩或理顺**自己的**科研/工程文稿（期刊论文、会议稿、学位论文章节、摘要/Nature 式 summary paragraph），或专门查赘词、被动语态、术语和数字是否一致。不要用来做方法或结果的技术审稿、统计核查、文献格式、翻译，或代写新段落。

## What it does
把斯坦福 Kristin Sainani《Writing in the Sciences》课上的编辑方法编成可加载技能，必要时再对照 Nature 对 summary paragraph 的结构要求。可对全文、单节、单段甚至一句话做审校，提供五种模式（全文 / 单节 / 针对性 / 互动逐段 / 摘要）。完整审校走六轮：赘词、语态与动词、句段结构、术语一致性、数字与引用、摘要结构。发现按 CRITICAL / MAJOR / MINOR 分组，给出位置和改写示例。技能不改动科学内容、数据或主张，只改表述。

## Recipe / links
- Repo: https://github.com/labarba/sciwrite（890★；SKILL.md 声明 CC-BY-4.0）
- DOI: https://doi.org/10.5281/zenodo.23728600
- SKILL.md: `skills/sciwrite/SKILL.md`（另有两份按需读取的 reference）
- 安装：
  ```bash
  npx skills add labarba/sciwrite
  # 或：gh skill install labarba/sciwrite sciwrite
  ```
  Claude Code 也可用：`/plugin install sciwrite --marketplace labarba/sciwrite`。Claude / ChatGPT / Gemini 应用可上传发行 ZIP（`sciwrite-<version>.zip`）。

## Why it made the cut
完整可加载 `SKILL.md`：使用边界、六轮审校和五种模式写得很清楚，并配有 DOI 与安装途径。作者 Lorena A. Barba 是把该课程方法做成 agent skill 的可核来源，890★ 也超过「仅有热度」的空喊帖。
