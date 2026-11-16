# kr-career-skill（韩国就业 / 跳槽助理）

**Tags:** career, job-search, korea, resume, skill
**Source:** [@doodi_dev](https://x.com/doodi_dev/status/2122151418123456741) · 2026-11-16
**Engagement:** 发现帖为韩语项目介绍 · 仓库 [Whosekey-Labs/kr-career-skill](https://github.com/Whosekey-Labs/kr-career-skill) 现 14★ / 3 forks，MIT；2026-11-11 建仓，带测试工作流

## When to use
要在**韩国就业市场**找匹配职位、分析公司与任职要求、起草自我介绍/简历到自己的 Google 文档，或预约每日新职位提醒。面向会读链接的 agent（Claude、Codex、ChatGPT 等）。不要用它自动投递或登录代填；也不适合中国校招（见 [campus-recruiting-skill](campus-recruiting-skill.md)）或通用英文面试操练。

## What it does
一条完整 `SKILL.md` 加 `career.py` 与分步 `guides/`：先做连接检查和最小档案（职务、地区、经验、条件），再按职群在约 100 个脚本可搜站点（사람인、잡코리아、원티드、리멤버 等）找匹配职位；用户选定 1–2 个后再做公司分析与要件整理，然后把自我介绍草稿写进自己的 Google 文档；可选每日提醒。能跑 Python 时用脚本省 token，脚本失败或不支持的站点改用浏览器。家规包括：不编造招聘信息或履历数字、不进行高频率抓取、遇到验证码把画面交还给用户、不替用户投递。

## Recipe / links
- Repo: https://github.com/Whosekey-Labs/kr-career-skill（MIT，14★）
- 直接让 agent 读取技能并开始：
  `https://raw.githubusercontent.com/Whosekey-Labs/kr-career-skill/main/SKILL.md 이 스킬 설치하고 지침대로 진행해줘. 나 취업(이직) 준비 도와줘.`
- Claude Code 项目内安装：
  ```bash
  git clone https://github.com/Whosekey-Labs/kr-career-skill .claude/skills/kr-career-skill
  ```
- 可选：本机 Python 3.9+ 跑 `career.py`；Google 文档输出需要 agent 能用的 Drive 连接（MCP / 连接器 / CLI），否则改落到本地文件或对话里。
- 仓库声明带 CI 测试；本轮未实测搜索与文档导出。

## Why it made the cut
有可执行的 `SKILL.md`、脚本、分步指南和测试，使用场景清楚，也写明了反编造、不代投和反封禁节奏。社区信号还很弱（新建仓、星标低），先按完整配方收录，后续需再观察维护情况。与中国非技术岗校招技能 [campus-recruiting-skill](campus-recruiting-skill.md) 市场不同，并不重复。
