# Anti-Slop（带确定性检查器的去 AI 味写作）

**Tags:** writing, editing, anti-slop, linter, skill
**Source:** [@double_burger_2](https://x.com/double_burger_2/status/2126621918472331517) · 2026-11-28
**Engagement:** 本窗介绍帖 4 赞 / 1 书签；仓库 [machina-exm/anti-slop](https://github.com/machina-exm/anti-slop) 现 0★，MIT，2026-11-26 建仓。介绍帖注明把禁词表和句长区间换成中文习惯即可照搬。

## When to use
要把草稿改得不像模型写的，并且希望用可重复的检查器盯住漏网句式，而不是只靠「再写得自然一点」时用。它按固定四步走：先扫描、再改结构、再换词并核对事实，最后用零依赖的 Python 检查器循环到没有硬伤。不要用它改 UI 视觉——那是 [unslop](unslop.md) / [unslop-ui](unslop-ui.md) / [unslop-anything](unslop-anything.md) 的范围。和已收录的 [Stop Slop](stop-slop.md)、[no-ai-slop](no-ai-slop.md)、[Humanizer-zh](humanizer-zh.md) 同属去写作 AI 味，但不是同一仓库：这边把 Wikipedia「Signs of AI writing」和 Pangram 的句式表写进规则库，并用 `slop_lint.py` 做硬性门禁。

## What it does
根目录可加载技能 `SKILL.md` 强制按四步执行，不要一次改结构、用词、语气和事实：

1. **基线扫描**：先把草稿存成文件，跑 `python3 scripts/slop_lint.py <draft.md> --json`，拿到确切命中
2. **改结构与节奏**：删掉“不是 A 而是 B”、空洞的 -ing 收尾、三段排比和“让我们深入”一类提纲腔，把句子长短拉开
3. **换词并做事实对照**：按 `references/patterns.json` 换成具体用词，并逐行对照原文，删掉草稿里没有的数字、人名和故事
4. **检查循环**：再跑检查器；硬伤（HARD）必须改到退出码为 0，最多三轮；软伤（SOFT）只改真正的套话，作者本人的标点习惯可以留

如果工作区里有 `voice-dna.json` 或 `writing-signature.md`，先读再给检查器加 `--voice`，以免把作者自己的破折号、省略号当成 AI 痕迹。最终只交改写正文和一行状态：`anti-slop: PASS · 0 hard · …`。

## Recipe / links
- Repo: https://github.com/machina-exm/anti-slop（0★，MIT）
- 安装（根目录就是技能）：
  ```bash
  npx skills add machina-exm/anti-slop
  ```
  或把仓库拷进 agent 的 skills 目录，确保 `SKILL.md`、`scripts/slop_lint.py` 和 `references/patterns.json` 在一起。
- 技能正文：[SKILL.md](https://github.com/machina-exm/anti-slop/blob/main/SKILL.md)
- 需要本机 Python 3；检查器声称零第三方依赖

## Why it made the cut
配方具体，规则有公开出处，还有可跑的检查器，不只是一份禁词清单。0★、仓很新，社区信号弱，按可验证材料收录，并在条目里写清和 Stop Slop / no-ai-slop / Humanizer-zh 的分工。
