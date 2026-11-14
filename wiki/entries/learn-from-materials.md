# learn-from-materials（可追溯的材料学习页）

**Tags:** learning, research, pdf, knowledge-base, quiz, chinese, skill
**Source:** [@ruyi3699](https://x.com/ruyi3699/status/2121321196922802586) · 2026-11-14
**Engagement:** 发现帖 9 赞 / 5 收藏；仓库 [dmoshehun-prog/learn-from-materials](https://github.com/dmoshehun-prog/learn-from-materials) 约 1.4k★，MIT

## When to use
要把 PDF、书、幻灯片、网页或长文交给 agent 做系统学习或摘要，但担心它分不清「原文依据」和「模型推断」，希望得到可回溯出处的知识库、交互学习页和测验，而不是一份无法核对的总结。

## What it does
一条完整 SKILL.md（v1.1.0）把材料编成可追溯知识库、离线交互 HTML 和同源 Markdown，中英文都支持。脚本负责提取、组装、校验和渲染；模型负责理解、判断关系和复核。流程按任务路由到不同 reference：系统学习、快速导读、增量更新、题库自检、方法库保存/检索/比较。强调来源指纹、第二遍原文回读、关系账本，以及把「材料依据 / 推断 / 外部核验」分开标注。需要文件系统和 Python 3.10+；扫描件建议有 OCR；浏览器校验可选 Playwright。

## Recipe / links
- Repo: https://github.com/dmoshehun-prog/learn-from-materials
- SKILL.md: https://github.com/dmoshehun-prog/learn-from-materials/blob/main/SKILL.md
- 中文说明：https://github.com/dmoshehun-prog/learn-from-materials/blob/main/README_CN.md
- 安装（若用 skills CLI）：`npx skills add dmoshehun-prog/learn-from-materials`
- 先跑 `pipeline.py preflight` 检查环境，再按 SKILL.md 的任务表读取对应 `references/`

## Why it made the cut
可执行配方明确针对「AI 总结无法溯源」这一痛点，有 SKILL.md、脚本和参考协议，仓库可验证。
