# Agent Skills Wiki

从 X（Twitter）持续挖掘、人工筛过的 **可复用 Agent Skills** 清单。面向 Cursor / Claude Code / Codex / Grok Bot 等 coding agent 用户。

**[→ 打开完整目录 Catalog（全部条目）](wiki/Catalog.md)**

当前约 **80+** 条 · 每小时增量扫描（Asia/Shanghai 白天）· [CC BY 4.0](LICENSE)

---

## 从这里开始

| 想找什么 | 去哪 |
| --- | --- |
| 全部技能索引 | **[wiki/Catalog.md](wiki/Catalog.md)** |
| 单条详情 | [wiki/entries/](wiki/entries/) |
| 每小时扫到了什么 | [wiki/digests/](wiki/digests/) |
| 收录标准 | [wiki/Home.md](wiki/Home.md) |

每条 entry 都包含：何时用、做什么、安装/仓库链接、原始推文来源、为何收录。

---

## 按主题挑（精选）

### 设计 / UI / 动效
- [UI UX Pro Max](wiki/entries/ui-ux-pro-max.md) — 设计系统智能技能 + CLI（高星）
- [Emil Kowalski Skills](wiki/entries/emilkowalski-skills.md) — UI / 动效 taste 包
- [AI Design Skills](wiki/entries/ai-design-skills.md) — 落地页 + 动效
- [Apple Human Interface Skills](wiki/entries/apple-human-interface-skills.md) — Apple HIG 路由 + 子技能
- [Pristine](wiki/entries/pristine.md) — UI 截图打分与 polish
- [Hallmark Design Skill](wiki/entries/hallmark-design-skill.md) — 前端主题 / 设计配方

### 视频 / 成片
- [Remotion Agent Skills（官方）](wiki/entries/remotion-skills.md) — React 视频创作与渲染
- [Lemo-Opuscar](wiki/entries/lemo-opuscar.md) — 多种代码成片风格工具箱
- [vvv](wiki/entries/vvv.md) — Remotion 视频模板工厂
- [ffmpeg-skill](wiki/entries/ffmpeg-skill.md) — 本地 FFmpeg 剪辑
- [YouTube Agent Skill pack](wiki/entries/youtube-agent-skill.md) — YouTube 运营技能包
- [Digital Human Koubo](wiki/entries/digital-human-koubo.md) — 照片 + 文案 → 口型口播

### 工程 / 交付流程
- [Addy Osmani Agent Skills](wiki/entries/addyosmani-agent-skills.md) — 工程生命周期技能包
- [Matt Pocock Skills](wiki/entries/mattpocock-skills.md) — 可组合工程技能
- [Superpowers (obra)](wiki/entries/superpowers.md) — brainstorming + TDD 交付流
- [Oldhand 2.0](wiki/entries/oldhand.md) — 用脚本判定「做完了」
- [ub-mode（Uncle Bob）](wiki/entries/ub-mode.md) — 纪律化写码 + 质量门
- [ayushjj/skills](wiki/entries/ayushjj-skills.md) — 日常工程技能（含 harden）
- [Autoresearch](wiki/entries/autoresearch.md) — 可量化目标的自动迭代

### 安全 / 安装卫生
- [SkillSpector](wiki/entries/skillspector.md) — 安装前检查
- [skill-guard](wiki/entries/skill-guard.md) — 技能内容哈希信任门
- [xss-audit](wiki/entries/xss-audit.md) — 多层静态 XSS 审计
- [Cloudflare Security Audit Skill](wiki/entries/cloudflare-security-audit-skill.md)
- [Brotli Checker](wiki/entries/brotli-checker.md) — Trail of Bits CVE 排查
- [Cognition Vulnerability Fixes](wiki/entries/cognition-devin-vuln-fixes.md)

### SEO / 增长 / 内容
- [qiaomu-seo](wiki/entries/qiaomu-seo.md) — 技术 SEO / AI Search 可见性
- [Claude SEO](wiki/entries/claude-seo.md) — Claude Code SEO 审计插件
- [social-auto-upload](wiki/entries/social-auto-upload.md) — 多平台发布
- [Stop Slop](wiki/entries/stop-slop.md) — 去 AI 腔写作

### 知识库 / 科学 / 其他高信号
- [Obsidian Skills (kepano)](wiki/entries/obsidian-skills.md)
- [book-to-skill](wiki/entries/book-to-skill.md) — 把技术书蒸馏成 skill
- [Archify](wiki/entries/archify.md) — 交互 HTML 架构图
- [NVIDIA BioNeMo Agent Toolkit](wiki/entries/bionemo-agent-toolkit.md)
- [Chaperone（RosettaCommons）](wiki/entries/chaperone.md) — 蛋白质设计
- [PixiJS Skills（官方）](wiki/entries/pixijs-skills.md)
- [Awesome Game Dev Agent Skills](wiki/entries/awesome-gamedev-agent-skills.md)

完整列表与来源推文 → **[Catalog](wiki/Catalog.md)**

---

## 什么叫「好 skill」

这里的 skill = agent 可加载的多步配方：有明确「何时用」、具体步骤，最好有可分享的 `SKILL.md` / 仓库。

**通常至少满足两条才收录：**

1. 具体配方（步骤 / checklist / SKILL.md）
2. 清晰使用场景
3. 可验证材料（仓库、gist、长帖）
4. 社区信号（加分项，不单独决定）

跳过广告、空喊、无可执行内容的帖子。

---

## 目录结构

```
wiki/
  Home.md       # 说明与收录标准
  Catalog.md    # 全量索引 ← 主入口
  entries/      # 每个 skill 一篇
  digests/      # 每小时扫描摘要
meta/
  last-scan.json
```

---

## 相关

- [一人公司机会 Wiki](https://github.com/hqzhon/opc-opportunity-wiki) — 跨境 / SaaS 一人公司机会清单

## License

本仓库内容采用 [CC BY 4.0](LICENSE)。被引用的推文与上游仓库版权归原作者。

## Maintenance

约每小时扫描 X（Asia/Shanghai 白天）。新发现先进入 digest，过线后写入 `wiki/entries/` 并更新 Catalog。欢迎 PR 补条目或纠错。
