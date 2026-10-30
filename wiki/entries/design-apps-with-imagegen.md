# design-apps-with-imagegen（swyx：图像探索 → 真实现产品）

**Tags:** design, ui-ux, imagegen, product, skill
**Source:** [@swyx](https://x.com/swyx/status/2115903364320129053) · 2026-10-29
**Engagement:** ~95 likes / ~88 bookmarks / ~92 replies · repo ~177★ · MIT

## When to use
When agents keep producing **好看但不耐真实内容/状态的 demo UI**，你需要一条强制流程：先审计现有界面与合约 → 用真实参考探索多个方向 → 选定后再实现，并用截图对照验收。

## What it does
`design-apps-with-imagegen` in swyxio/skills: (1) establish scope from real screens/content/capabilities; (2) research free Mobbin refs via computer use, generate **four** distinct ImageGen directions (incl. a wildcard) that differ in composition/interaction not just palette; (3) present A–D with thesis/tradeoffs; (4) implement the chosen direction and compare matched screenshots. Author calls it the most valuable addition for “real working software instead of flashy designer demos.”

## Recipe / links
- Repo: https://github.com/swyxio/skills (~177★, MIT)
- Skill page: https://www.skills.sh/swyxio/skills/design-apps-with-imagegen
- Install: clone/link into agent skills dir, or `npx skills add swyxio/skills --skill design-apps-with-imagegen` when supported
- Companion skills in the same repo: `visual-playtest`, `skill-cutter`, etc.

## Why it made the cut
Concrete multi-step design recipe with clear anti-demo-slop intent, verifiable SKILL.md, and strong author + X engagement—not another “make it pretty” one-liner.
