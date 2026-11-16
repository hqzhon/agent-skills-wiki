# suzhe-ui（苏哲 UI 网页设计方法）

**Tags:** design, frontend, ui, claude-code, skill
**Source:** [@ai_algoit](https://x.com/ai_algoit/status/2121917469606699404) · 2026-11-15
**Engagement:** 发现帖互动低；仓库 [suzhe-ai/suzhe-ui](https://github.com/suzhe-ai/suzhe-ui) 现 11★，Apache-2.0；2026-11-15 当日建仓

## When to use
让 Claude 做或改任何网页 UI——落地页、商店、登录/注册、结账、公告、文档、后台或分享卡——或要求「高级 / 有质感 / 少一点乱 / Apple-like」时，希望它先选页面类型和语域，再按一套克制的方法出稿，而不是套默认的紫蓝渐变模板。

## What it does
把 suzhe.ai 背后的网页设计方法做成一条 Claude Skill。先把页面分成商务语域（白/#f5f5f7/黑、系统字体、一颗蓝色强调）或编辑语域（暖纸色、衬线标题、墨色按钮），每页只保留一个签名视觉，删掉站不住的元素，并把「在低端设备上也要流畅」写进规则。作者声明规则来自真实改版轮次，16 次被否方案和原因放在 `references/rejected.md`。技能正文是英文，页面文案按用户语言写；中文页另有 CJK 排版规则。装好后不必再调用命令，直接请它出落地页或做清理即可。

## Recipe / links
- Repo: https://github.com/suzhe-ai/suzhe-ui（11★，Apache-2.0；Suzhe 名称与 Logo 不在许可范围内）
- Claude Code：`/plugin marketplace add suzhe-ai/suzhe-ui`，再 `/plugin install suzhe-ui@suzhe-ui`
- 或把 skill 目录拷进 `~/.claude/skills`；网页版 Claude 可上传最新 Release 的 zip（Customize → Skills）
- Skill 正文：仓库 `skills/suzhe-ui/SKILL.md`

## Why it made the cut
可安装的具体设计配方，使用场景清楚，带被否案例和许可证说明。仓库很新、星数还少，先观察后续维护。
