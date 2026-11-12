<!--
  Routine note: when new entries are added, update (1) the entry count in the badge and in "完整目录 Catalog（N 条）",
  (2) the "## 精选（按主题）· Picks by topic" bullets. Keep everything else as-is.
-->
<p align="center">
  <img src="assets/social-preview.png" alt="Agent Skills Wiki — hand-picked, installable agent skills mined from X" width="100%">
</p>

<h1 align="center">Agent Skills Wiki</h1>

<p align="center">
  <b>Hand-picked, installable agent skills (<code>SKILL.md</code>) for Claude Code, Codex, Cursor, Gemini CLI & more —<br>found on X within hours of launch, including the Chinese creator scene most English lists miss.</b><br>
  从 X 实时挖掘、人工筛过的 Agent Skills 百科：每条都有「何时用 / 怎么装 / 原帖出处 / 为何收录」。
</p>

<p align="center">
  <a href="wiki/Catalog.md"><img src="https://img.shields.io/badge/skills-251-2ea44f?style=flat-square" alt="Skills count"></a>
  <img src="https://img.shields.io/github/last-commit/hqzhon/agent-skills-wiki?label=updated&style=flat-square" alt="Last update">
  <img src="https://img.shields.io/badge/scans-3×%20daily-blue?style=flat-square" alt="Scanned 3x daily">
  <a href="CONTRIBUTING.md"><img src="https://img.shields.io/badge/PRs-welcome-brightgreen?style=flat-square" alt="PRs welcome"></a>
  <a href="LICENSE"><img src="https://img.shields.io/badge/license-CC%20BY%204.0-lightgrey?style=flat-square" alt="CC BY 4.0"></a>
  <a href="https://github.com/hqzhon/agent-skills-wiki/stargazers"><img src="https://img.shields.io/github/stars/hqzhon/agent-skills-wiki?style=flat-square" alt="Stars"></a>
</p>

<p align="center">
  <a href="wiki/Catalog.md"><b>📚 Full Catalog</b></a> ·
  <a href="wiki/digests/"><b>🆕 Latest finds</b></a> ·
  <a href="#-top-picks"><b>⭐ Top picks</b></a> ·
  <a href="#-quick-start"><b>🚀 Quick start</b></a> ·
  <a href="#-submit-a-skill--推荐一个-skill"><b>➕ Submit a skill</b></a>
</p>

**[→ 打开完整目录 Catalog（251 条）](wiki/Catalog.md)** · **[最新扫描摘要](wiki/digests/)** · 每天 8:00 · 14:00 · 20:00（Asia/Shanghai）增量更新

---

## Why this list / 为什么值得 Star

| | |
| --- | --- |
| 🕒 **Fresh** | Scanned from X three times a day. New skills land here hours after their author tweets them — not weeks later. <br>每天 3 次扫 X，作者发帖几小时内收录。 |
| ✅ **Curated, not dumped** | Each entry passes a quality bar: a real use case, concrete steps or a `SKILL.md`, and something verifiable (repo / gist). Ads and hype are skipped. <br>只收可复用配方，广告和空喊一律跳过。 |
| 🔗 **Traceable** | Every entry links to the original post **and** the upstream repo, with install commands. <br>每条链回原帖 + 上游仓库 + 安装命令。 |
| 🌏 **EN + 中文** | Covers both the English and the Chinese AI-builder scene (李继刚, 宝玉, 花叔, 公众号/小红书 tooling…). <br>中英文创作者一起覆盖，很多中文好 skill 英文列表里没有。 |

**If this saves you time, a ⭐ helps others find it.** 觉得有用就点个 Star，让更多人看到。

---

## 🚀 Quick start

1. Pick a skill from the **[Catalog](wiki/Catalog.md)** or the tables below. Each entry page has *When to use · What it does · Install · Why it made the cut*.
2. Install it. Most skill repos work with the open [`skills` CLI](https://github.com/vercel-labs/skills):
   ```bash
   npx skills add <owner>/<repo>          # e.g. npx skills add blader/humanizer
   ```
   Or copy the skill folder (the one containing `SKILL.md`) into your agent's skills directory, e.g. `~/.claude/skills/` (Claude Code) or `~/.codex/skills/` (Codex). Repos that ship a Claude Code plugin can also be added with `/plugin marketplace add <owner>/<repo>`. The entry page lists the exact command when the upstream repo documents one.
3. Ask your agent to do the task — the skill loads when its description matches.

> 中文：在 Catalog 里挑一条 → 照条目页的安装命令装上（多数可 `npx skills add 作者/仓库`）→ 直接让 agent 干活即可。

---

## ⭐ Top picks

Most-starred skills in the wiki (GitHub stars as of 2026-11-11). 按 GitHub Star 排序的高信号精选。

| Skill | Repo | ★ | What it does |
| --- | --- | --- | --- |
| [Matt Pocock Skills](wiki/entries/mattpocock-skills.md) | [mattpocock/skills](https://github.com/mattpocock/skills) | 321k | Small, composable "skills for real engineers" |
| [Superpowers](wiki/entries/superpowers.md) | [obra/superpowers](https://github.com/obra/superpowers) | 316k | Brainstorm → plan → TDD delivery workflow |
| [UI UX Pro Max](wiki/entries/ui-ux-pro-max.md) | [nextlevelbuilder/ui-ux-pro-max-skill](https://github.com/nextlevelbuilder/ui-ux-pro-max-skill) | 148k | Design-system intelligence for UI work |
| [gstack](wiki/entries/gstack.md) | [garrytan/gstack](https://github.com/garrytan/gstack) | 141k | Garry Tan's review / QA / shipping stack |
| [Addy Osmani Agent Skills](wiki/entries/addyosmani-agent-skills.md) | [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills) | 116k | Engineering-lifecycle skill pack |
| [Taste Skill](wiki/entries/taste-skill.md) | [Leonxlnx/taste-skill](https://github.com/Leonxlnx/taste-skill) | 113k | Art direction for non-generic frontends |
| [Impeccable](wiki/entries/impeccable.md) | [pbakaus/impeccable](https://github.com/pbakaus/impeccable) | 108k | Frontend design vocabulary for agents |
| [Humanizer](wiki/entries/humanizer.md) | [blader/humanizer](https://github.com/blader/humanizer) | 68k | Remove 26 patterns of AI-sounding writing |
| [last30days](wiki/entries/last30days-skill.md) | [mvanhorn/last30days-skill](https://github.com/mvanhorn/last30days-skill) | 67k | Research what Reddit / X / HN said in the last 30 days |
| [Marketing Skills](wiki/entries/marketingskills.md) | [coreyhaines31/marketingskills](https://github.com/coreyhaines31/marketingskills) | 60k | CRO, copywriting, SEO, customer research |
| [Obsidian Skills](wiki/entries/obsidian-skills.md) | [kepano/obsidian-skills](https://github.com/kepano/obsidian-skills) | 52k | Work inside Obsidian vaults (Markdown, Bases, Canvas) |
| [Knowledge Work Plugins](wiki/entries/knowledge-work-plugins.md) | [anthropics/knowledge-work-plugins](https://github.com/anthropics/knowledge-work-plugins) | 35k | Anthropic's role-based skill plugins |
| [video-use](wiki/entries/video-use.md) | [browser-use/video-use](https://github.com/browser-use/video-use) | 31k | Edit talking-head footage by chatting |
| [improve](wiki/entries/shadcn-improve.md) | [shadcn/improve](https://github.com/shadcn/improve) | 10k | Strong model audits & plans, cheap model executes |
| [ljg-skills（李继刚）](wiki/entries/ljg-skills.md) | [lijigang/ljg-skills](https://github.com/lijigang/ljg-skills) | 7.7k | 26 atomic thinking / writing skills (中文) |
| [.NET Agent Skills](wiki/entries/dotnet-skills.md) | [dotnet/skills](https://github.com/dotnet/skills) | 5.9k | Official C# / MSBuild / NuGet skills with public evals |
| [gzh-design-skill](wiki/entries/gzh-design-skill.md) | [isjiamu/gzh-design-skill](https://github.com/isjiamu/gzh-design-skill) | 4.3k | Markdown → WeChat 公众号-ready HTML (中文) |
| [Modern Web Guidance](wiki/entries/modern-web-guidance.md) | [GoogleChrome/modern-web-guidance](https://github.com/GoogleChrome/modern-web-guidance) | 4.0k | Chrome + Edge + Firefox + MDN: use modern web APIs |

---

## 精选（按主题）· Picks by topic

> 以下为 Catalog 中近期高信号 / 官方包摘录。完整列表 → **[Catalog](wiki/Catalog.md)**

### 官方 / 厂商包
- [Modern Web Guidance（浏览器厂商官方）](wiki/entries/modern-web-guidance.md) — 让编码 agent 用原生 Web API，附 legacy-scan
- [improve（shadcn）](wiki/entries/shadcn-improve.md) — 强模型审计写计划、便宜模型执行
- [.NET Agent Skills（官方）](wiki/entries/dotnet-skills.md) — C# / MSBuild / 升级迁移，附公开评测看板
- [Meteor Agent Skills（官方）](wiki/entries/meteor-agent-skills.md) — Meteor 3 开发与迁移 17 技能
- [last30days](wiki/entries/last30days-skill.md) — 近 30 天 Reddit / X / Polymarket 真实讨论调研
- [Gemini API Skills（Google 官方）](wiki/entries/gemini-skills.md) — Gemini API / 媒体生成 CLI
- [Expo Skills（官方）](wiki/entries/expo-skills.md) — React Native / EAS
- [NVIDIA Agent Skills（官方）](wiki/entries/nvidia-skills.md) — CUDA / Physical AI
- [Google Cloud Skills（官方）](wiki/entries/google-cloud-skills.md) — IAM Helper 等
- [Google Workspace CLI Skills（gws）](wiki/entries/google-workspace-cli-skills.md) — Gmail/Calendar/Drive 等 ~95 skills
- [Remotion Agent Skills（官方）](wiki/entries/remotion-skills.md) — React 视频创作与渲染
- [ElevenLabs Skills（官方）](wiki/entries/elevenlabs-skills.md) — 语音 / 实时音频
- [Anthropic Knowledge Work Plugins](wiki/entries/knowledge-work-plugins.md) — Cowork 角色技能包
- [Microsoft SkillOpt](wiki/entries/microsoft-skillopt.md) — 训 Skill.md、不动权重
- [PixiJS Skills（官方）](wiki/entries/pixijs-skills.md) · [Android Official Skills](wiki/entries/android-official-skills.md) · [Compose Skill（Jetpack Compose 七件套）](wiki/entries/compose-skill.md)
- [Tailscale Skill（官方）](wiki/entries/tailscale-skill.md) — networking / tsnet / k8s
- [Jane Street Socratic Tutor（官方）](wiki/entries/janestreet-agent-skills.md) — 苏格拉底式家教：诊断、0–5 技能图、间隔复习
- [FlyAI（飞猪官方旅行搜索）](wiki/entries/flyai-skill.md) — 自然语言查机票/酒店/火车，结构化可预订结果
- [campus-recruiting-skill](wiki/entries/campus-recruiting-skill.md) — 中国非技术岗校招：核岗/简历/面试/Offer（不代投）

### 设计 / UI / 品味
- [sepia（去 AI 味写作）](wiki/entries/sepia.md) — 叙事架构层去 AI 味
- [Humanizer（blader）](wiki/entries/humanizer.md) — 26 种 AI 写作痕迹改写，~67k★ · 日语版思路见 [yomiyasu](wiki/entries/yomiyasu.md)
- [gzh-design-skill](wiki/entries/gzh-design-skill.md) — Markdown 一键排成公众号可粘贴 HTML，6 套主题
- [Taste Skill](wiki/entries/taste-skill.md) — 艺术指导 + 去 AI 味前端
- [baoyu-design（本地 Claude Design）](wiki/entries/baoyu-design.md) — 幻灯片 / Dashboard / HTML
- [Impeccable](wiki/entries/impeccable.md) — 前端设计词汇表
- [ip-as-logo](wiki/entries/ip-as-logo.md) — 极简 IP 吉祥物 Logo：三方向、六候选、严格复杂度预算
- [unslop](wiki/entries/unslop.md) — 把 vibecoded 的 AI 味 UI 逐轮改成有性格的设计
- [UI UX Pro Max](wiki/entries/ui-ux-pro-max.md) — 设计系统智能技能 + CLI
- [oil-ui](wiki/entries/oil-ui.md) — UI 方向探索与并排对比
- [Emil Kowalski Skills](wiki/entries/emilkowalski-skills.md) — UI / 动效 taste
- [jakubkrehel/skills（Interface Skills）](wiki/entries/jakubkrehel-skills.md) — a11y / 字体 / 布局
- [Apple Human Interface Skills](wiki/entries/apple-human-interface-skills.md) — Apple HIG
- [design-apps-with-imagegen（swyx）](wiki/entries/design-apps-with-imagegen.md) — 图像探索 → 真实现产品
- [garden-skills（ConardLi）](wiki/entries/garden-skills.md) — 网页设计 / RAG / 生图 / 动效小花园
- [萝卜 PPT](wiki/entries/luobo-ppt.md) — 生成 / 照参考图美化原生可编辑 PPTX
- [GordenPPTSkill](wiki/entries/gorden-ppt-skill.md) — 中文商务模板 + 只改文字（非商业许可）
- [Kubai Icons](wiki/entries/kubai-icons.md) — 统一画风动态/静态功能图标 skill + 2600+ 开源图标
- [Awesome Design Skills](wiki/entries/awesome-design-skills.md) — 67 套设计系统 SKILL.md + DESIGN.md（npx 拉取）
- [Stageshow](wiki/entries/stageshow.md) — 像真产品的假 UI 插画 / 光标演示
- [stack-diagram](wiki/entries/stack-diagram.md) · [svg-diagram](wiki/entries/svg-diagram.md) — 架构图 / SVG 图解（带 lint 自检）
- [Floorplan](wiki/entries/floorplan.md) — 从真实代码画出大白话交互地图

### 工程 / 交付 / Meta
- [gstack（Garry Tan）](wiki/entries/gstack.md) — review / QA / shipping
- [pstack `/statechart`](wiki/entries/pstack-statechart.md) — TLA+ 状态图找 bug
- [next-bundle-optimizer](wiki/entries/next-bundle-optimizer.md) — Next.js 官方捆包优化
- [Webcrawl Anything](wiki/entries/webcrawl-anything.md) — 本地免 Key 抓取 / 8 个 agent skills + CLI/MCP
- [Graphify](wiki/entries/graphify.md) — 本地 AST 知识图谱 CLI
- [skill-diet](wiki/entries/skill-diet.md) — 给臃肿 Skill 减重（token ↓）
- [better-skill](wiki/entries/better-skill.md) — 技能体检 / 打分 / 选型标准
- [Superpowers (obra)](wiki/entries/superpowers.md) — brainstorming + TDD 交付流
- [founder-skill](wiki/entries/founder-skill.md) — 创业压力测试包
- [Addy Osmani Agent Skills](wiki/entries/addyosmani-agent-skills.md) · [Matt Pocock Skills](wiki/entries/mattpocock-skills.md)
- [CCPM](wiki/entries/ccpm.md) — PRD → Issues → 并行 agents
- [CodexQA](wiki/entries/codexqa.md) — 合入前本地验证包
- [skill-guard](wiki/entries/skill-guard.md) · [SkillSpector](wiki/entries/skillspector.md) · [aig-skill-scan](wiki/entries/aig-skill-scan.md) — 安装卫生 / 信任门
- [Elephant-Goldfish Model（Google）](wiki/entries/elephant-goldfish-model.md) — 带上下文起草规格，无记忆子 agent 评审
- [Anthropic-Cybersecurity-Skills](wiki/entries/anthropic-cybersecurity-skills.md) — 817 安全技能包（授权场景）
- [AI Research Skills Library](wiki/entries/ai-research-skills.md) — 98 个 AI 研究工程技能（训练 → 论文）
- [commerce-agent-skills](wiki/entries/commerce-agent-skills.md) — 29 个电商技能，带评测 fixtures
- [tinker-ai-skill](wiki/entries/tinker-ai-skill.md) — 用自己的 Claude Code/Codex 会话在 Tinker 上微调并导出本机 GGUF
- [/optimize](wiki/entries/optimize-skill.md) — 31 项性能体检：先测量、安全修复、再对比
- [SwiftUI Pro（Paul Hudson）](wiki/entries/swiftui-pro.md) — 专治 LLM 写 SwiftUI 的废弃 API / 无障碍 / 性能错误 (~6.5k★)

### 营销 / 增长
- [Marketing Skills（coreyhaines31）](wiki/entries/marketingskills.md) — CRO / 文案 / SEO / 客户研究 (~58.8k★)
- [marketing-skill-hub](wiki/entries/marketing-skill-hub.md) — 出海投放 / UGC / 开发信
- [Apify Agent Skills](wiki/entries/apify-agent-skills.md) — 官方抓取 / Actor 技能

### 视频 / 成片
- [huashu-motion](wiki/entries/huashu-motion.md) — 可指着画面局部改的产品发布片（本机作曲）
- [GIF 工厂（gif-factory）](wiki/entries/gif-factory.md) — 像素/插画/真人表情包与动态海报技能
- [video-use（browser-use）](wiki/entries/video-use.md) — 对话式剪辑口播/教程毛片
- [rea-video](wiki/entries/rea-video.md) — 任意视频逐镜逆向拆解
- [Scenario Labs Skills](wiki/entries/scenario-labs-skills.md) — 图片/视频/音频/3D + 本机 DCC 技能包
- [gpx-3d-video](wiki/entries/gpx-3d-video.md) — GPX 轨迹同步 3D 路线叠加
- [Claude Animated Shorts](wiki/entries/claude-animated-shorts.md) — three.js + Remotion 本地渲染竖屏动画故事短片
- [Remotion Agent Skills（官方）](wiki/entries/remotion-skills.md)
- [video-talkcraft（口播 Remotion）](wiki/entries/video-talkcraft.md)
- [Lemo-Opuscar](wiki/entries/lemo-opuscar.md) — 代码成片风格工具箱
- [vvv](wiki/entries/vvv.md) — Remotion 视频模板工厂
- [product-launch-motion](wiki/entries/product-launch-motion.md) — URL → 发布片
- [onetake](wiki/entries/onetake.md) — 一镜到底发布片 / 功能演示，带连贯性评分（非商业许可）
- [Spotlight Film](wiki/entries/spotlight-film.md) — Apple 发布会风格产品片，代码逐帧渲染
- [Open 3D Skills](wiki/entries/open-3d-skills.md) — three.js 场景 / 滚动影片 / 爆炸图 / 60fps 录制 8 件套
- [image-to-sculpt](wiki/entries/image-to-sculpt.md) — 一张图 → 可对图度量的 Blender 雕刻技能
- [story-to-handdrawn-video](wiki/entries/story-to-handdrawn-video.md) — 中文故事 → 3:4 手绘动画
- [Bang Motion](wiki/entries/bang-motion.md) — 浏览器动效成片（非 PPT）
- [match-cut](wiki/entries/match-cut.md) — 接力匹配剪辑宣传片
- [teardown](wiki/entries/teardown.md) — 任意机器 → 可拆解的离线 3D 模拟器 + 60fps 讲解片
- [Reelsmith Media](wiki/entries/reelsmith-media.md) — 素材文件夹 → 本地字幕对齐的竖版 Reel
- [Stickman Video Director](wiki/entries/stickman-video-director.md) — 不露脸火柴人动画出片

### 知识库 / 科学 / 其他高信号
- [fundraising](wiki/entries/fundraising-skill.md) — 融资 / LP / M&A 操盘护栏
- [BLA / Blind LLM Agents](wiki/entries/bla-blind-llm-agents.md) — Counter-REA 加固 skill + MCP/CLI（防御自有产物）
- [ghidra-rpc](wiki/entries/ghidra-rpc.md) — Cellebrite Labs 出品，agent 驱动 Ghidra 做二进制逆向
- [khazix-skills（数字生命卡兹克）](wiki/entries/khazix-skills.md) — leader 定目标 / neat-freak 收工对齐 / 横纵分析 (~22k★)
- [ljg-skills（李继刚）](wiki/entries/ljg-skills.md) — 26 个原子思考/写作/铸卡技能（MIT，约 7719★）
- [书脉（weread-atlas）](wiki/entries/weread-atlas.md) — 微信读书划线 → Obsidian 主题卡片 + 知识环地图
- [WilmAI](wiki/entries/wilmai.md) — 芬兰学校系统 Wilma：MCP + CLI + 家校晨报 skill
- [Obsidian Skills (kepano)](wiki/entries/obsidian-skills.md)
- [md2html](wiki/entries/md2html.md) — AI 长文档 → 带目录和图表的单文件 HTML
- [NVIDIA BioNeMo Agent Toolkit](wiki/entries/bionemo-agent-toolkit.md)
- [Chaperone（RosettaCommons）](wiki/entries/chaperone.md) — 蛋白质设计
- [leanrea（轻装逆向）](wiki/entries/leanrea.md) · [BAMA](wiki/entries/bama.md) — Build Any Mac App
- [史鉴人生抉择](wiki/entries/shiji-tongjian-decisions.md) — 史记/通鉴核源决策

---

## What counts as a good skill / 什么叫「好 skill」

A skill here = a multi-step recipe an agent can load: clear *when to use*, concrete steps, ideally a shareable `SKILL.md` / repo. An entry usually meets at least two of:

1. **Concrete recipe** — steps / checklist / `SKILL.md`（具体配方）
2. **Clear use case**（清晰使用场景）
3. **Verifiable material** — repo, gist, long post（可验证材料）
4. **Community signal** — a bonus, never the only reason（社区信号，加分项）

Details: [wiki/Home.md](wiki/Home.md).

---

## ➕ Submit a skill / 推荐一个 skill

Found (or built) a great skill? **[Open a "Submit a skill" issue](https://github.com/hqzhon/agent-skills-wiki/issues/new?template=submit-skill.yml)** or send a PR — see [CONTRIBUTING.md](CONTRIBUTING.md). Corrections and better install notes are just as welcome.

发现或自己做了好 skill？欢迎 [提 Issue](https://github.com/hqzhon/agent-skills-wiki/issues/new?template=submit-skill.yml) 或 PR，纠错、补安装说明也欢迎。

---

## Repo layout / 仓库结构

```
wiki/
  Catalog.md    # full index, newest first ← start here
  entries/      # one page per skill
  digests/      # what each scan found
  Home.md       # inclusion criteria
meta/
  last-scan.json
```

## Star history

[![Star History Chart](https://api.star-history.com/svg?repos=hqzhon/agent-skills-wiki&type=Date)](https://star-history.com/#hqzhon/agent-skills-wiki&Date)

## Related / 相关

- [OPC Opportunity Wiki](https://github.com/hqzhon/opc-opportunity-wiki) — one-person-company opportunities（一人公司机会清单）

## License

Content is licensed under [CC BY 4.0](LICENSE) — credit "Agent Skills Wiki" with a link to this repo. Quoted posts and upstream repositories remain the property of their authors.
本仓库内容采用 CC BY 4.0；被引用的推文与上游仓库版权归原作者。
