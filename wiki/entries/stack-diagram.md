# stack-diagram（一句话出带官方 logo 的架构图）

**Tags:** diagram, architecture, visualization, docs, skill
**Source:** [@jojogh_007](https://x.com/jojogh_007/status/2117120779204833504) · 2026-11-02（另见 [@qyi_lab](https://x.com/qyi_lab/status/2117097120297820193)）
**Engagement:** 仓库 caru-ini/stack-diagram，~656★，MIT，2026-11-01 创建

## When to use
要给 README、设计文档、Pitch 或 wiki 配一张技术栈 / 部署架构图（Next.js + Vercel + Neon、AWS VPC、monorepo 工具链、AI 应用等），但不想自己找图标、对连线。

## What it does
用一句话描述技术栈，agent 自动从 svgl → devicon → gilbarbara/logos（AWS 用官方图标包）拉取官方 logo，不重绘不改色；连线绕开文字，渲染后自检再交付。默认产出单文件自包含 HTML（字体和 logo 内联），也可导出亮/暗两版 PNG、零依赖 React 组件或 Claude Artifact。画完会询问一次是否发到公开画廊，需两次确认、不上传 prompt。

## Recipe / links
- Repo: https://github.com/caru-ini/stack-diagram
- 安装：`npx skills add caru-ini/stack-diagram`（Claude 应用可上传 Releases 里的 `stack-diagram.zip`）
- 依赖：Python 3.9+、联网取 logo；PNG 导出用 Playwright + Chromium
- 用前建议：拿自己熟悉的项目试，核对依赖关系画得对不对

## Why it made the cut
场景清晰、可直接安装、有完整仓库和示例图，自带渲染自检与隐私确认；补上 wiki 里「架构图 / 技术栈图」这一类，与 svg-diagram 互补（一个偏 logo 拼栈，一个偏手写 SVG 规范）。
