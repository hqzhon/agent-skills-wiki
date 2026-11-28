# BeanStack（对齐 → 规格 → 红灯测试 → 分派 → 验收）

**Tags:** workflow, spec, testing, multi-agent, openspec, chinese, skill
**Source:** [@qiunai_ai](https://x.com/qiunai_ai/status/2126337946068668727) · 2026-11-27
**Engagement:** 作者第一方介绍帖 7 赞 / 2 书签，并附 X Article。仓库 [qiunai/beanstack](https://github.com/qiunai/beanstack) 现 1★，MIT；作者称这是他们做 Bean Boss 时用了约 8 个月的工作流。

## When to use
希望 agent 不要一上来就改代码，而是先对齐需求、写规格、先写失败测试，再分派子代理，并在真浏览器里由「不是实现者」的角色按你的原话验收时用。它是一条 agent-agnostic 的工程工作流技能，面向 Claude Code、Codex、Cursor 等能读 SKILL.md 并分派子代理的工具。

## What it does
`skills/beanstack/` 提供一条入口 SKILL.md，外加按需加载的参考文档和脚本。主循环六步：Align（重述目标与验收标准）→ Research / 写成 OpenSpec 提案 → 行为改动先交红灯测试 → 并行分派 → 只跑受影响测试并由独立验证者在真实浏览器核对 → 交付摘要，你确认后才开 PR。合并、发布和部署都要再次授权。作者把 OpenSpec 的提案/规格周期，以及从 [pstack](pstack-statechart.md) 等处吸收的验证思路写进了配方。

## Recipe / links
- Repo: https://github.com/qiunai/beanstack（1★，MIT）
- 中英 README：https://github.com/qiunai/beanstack/blob/main/README.zh-CN.md
- 安装：
  ```bash
  npx skills add qiunai/beanstack
  ```
- 介绍帖另有长文：https://x.com/i/article/2126331353675509760

## Why it made the cut
第一方发布，步骤和「什么算做完」写得很具体，有 SKILL.md、MIT 许可和中英文档。星标还很低，但使用场景、规格/测试门禁和授权边界都清楚，达到收录线。它借鉴了已收录的 pstack / OpenSpec 思路，但是一条可独立安装的工作流技能。
