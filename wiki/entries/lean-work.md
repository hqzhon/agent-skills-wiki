# lean-work（少走步、少读上下文，守住质量底线）

**Tags:** workflow, tokens, glm, zcode, efficiency, skill
**Source:** [@xyun023](https://x.com/xyun023/status/2125936785998098465) · 2026-11-26
**Engagement:** 介绍帖 1 赞；仓库 [0505ttt/lean-work](https://github.com/0505ttt/lean-work) 现 0★，MIT。本窗新建。作者写明目前只在同一道调试任务上对照过 1 次，样本不能当结论。

## When to use
在 ZCode / GLM Coding 这类环境里，希望模型少规划、少串行试探、少把长输出读进上下文，同时仍做到「没验证不说做完」、有风险先问你时用。它和 superpowers 这类强制「先规划 / 先头脑风暴 / 完整调试流程」的插件方向相反；默认走精简做法，并说明跳过了什么。

## What it does
一份 MIT 的 SKILL.md：简单问题直接答；能并行的工具调用放一步；先定位再按行读文件，太长的输出只看摘要但保留退出码；答复只说改了什么、怎么验证、哪些没验证；改完集中验证一次，达到验收标准就停。三条底线不能被其他规则压过：没验证不说做完；该你决定或有风险的操作先问，不绕过权限；回复跟随你用的语言。作者在 ZCode 4.0.0 + GLM-5.4 上对同一道数组越界修复各跑了 1 次（不加载 vs /skill lean-work），自动验收都通过，步数/积分/耗时/输出 token 有下降，但没有人工盲评，也没有讲解/重构类任务的成对数据。

已知限制：在需要人工批准的权限模式（如 ZCode build 模式）下，「输出太长就存成文件」可能让会话停住等你点同意；它管不到思考档位和每次请求的固定工具开销。

## Recipe / links
- Repo: https://github.com/0505ttt/lean-work（0★，MIT）
- 安装（所有项目）：
  ```bash
  git clone https://github.com/0505ttt/lean-work.git
  mkdir -p ~/.agents/skills
  cp -R lean-work/.agents/skills/lean-work ~/.agents/skills/
  ```
  只想在某个项目用，就把 .agents/skills/lean-work/ 放进项目根目录。需要时可用 /skill lean-work 强制加载。想改成「先走完整流程」，改 SKILL.md 里的 Priority 一节。

## Why it made the cut
配方具体，边界和已知问题写得很老实，使用场景清楚。星标和对照样本都还很少，按可验证的 SKILL.md 收录，而不是按效果声称。
