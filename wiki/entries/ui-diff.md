# ui-diff（PR 界面前后对比）

**Tags:** frontend, visual-diff, pr-review, playwright, skill
**Source:** [@davidamunga_](https://x.com/davidamunga_/status/2122735807551152269) · 2026-11-18
**Engagement:** 发现帖 34 赞 / 5 转帖 / 11 收藏 / 802 次展示；仓库 [davidamunga/ui-diff](https://github.com/davidamunga/ui-diff) 现 1★，MIT（2026-11-17 建仓）

## When to use
前端 PR 的 CSS/组件 diff 审阅者「看不懂长什么样」时：需要在 base/head 上看到受影响页面的前后截图、像素差和量过的样式变化，或把视觉回归检查接到 CI。

## What it does
从改动文件推断受影响路由（Next.js、SvelteKit、Nuxt、Astro、Remix/React Router、纯 HTML 等），在 git worktree 里并排拉起 base/head，用 Playwright 截桌面和模拟 iPhone（可冻动画、可选暗色），测量间距/颜色/布局/对比度，标出本 PR 新引入的裁切、横滑、重叠、过小点击区域和 axe-core 无障碍问题，再把前后对比和设计摘要发到 PR 评论（重跑会更新同一条）。也可对 Storybook、对照 Figma 画板，并用 `ui-diff/design-review` 检查等设计签字。需要 macOS/Linux、Node 18+、`gh`（发评论）；首次运行会向 `~/.cache/ui-diff` 下载约 150 MB 的 Playwright/Chromium。

## Recipe / links
- Repo: https://github.com/davidamunga/ui-diff（MIT，1★）
- Claude Code：`/plugin marketplace add davidamunga/ui-diff` → `/plugin install ui-diff@ui-diff`
- 其他宿主：`npx skills add davidamunga/ui-diff -g`
- 或：`git clone https://github.com/davidamunga/ui-diff.git && ./ui-diff/install.sh`
- 纯 CI、不走 agent：用仓库提供的 GitHub Action（见 README「Run in CI」）

## Why it made the cut
场景具体，有 SKILL.md、安装脚本、GitHub Action、测试和评测目录，帖子互动也不错。仓当天新建、星标很少，属于早期条目，安装前需自审。
