# ruby-memsafety-exposure（升级前审查 Ruby 内存安全暴露面）

**Tags:** security, ruby, rails, audit, skill
**Source:** [@hsbt](https://x.com/hsbt/status/2123375901232845046) · 2026-11-19
**Engagement:** 公告帖约 12 赞 / 5 转 / 3 收藏；仓库 [hsbt/ruby-memsafety-exposure](https://github.com/hsbt/ruby-memsafety-exposure) 当天新建，0★，未标许可证。早期条目。

## When to use
Ruby 于 2026-11-18 发布 String 大小写转换与正则引擎的内存安全修复（4.0.10 / 3.4.13 / 3.3.14）之后，想知道自己的 **Rails 或 Sinatra 应用在升级完成前有哪些暴露面、过渡期该做什么** 时使用。不要把它当成攻击教程，也不要在未升级时用它去复现漏洞。

## What it does
只读审查：对照官方公告，检查应用（及可获取的公开 gem 源码）里与这些修复相关的表面，并给出升级前的过渡建议（升级 Ruby 才是修复；在此之前可能涉及 gem 更新、initializer、代理或 WAF 规则等）。技能写明**不改应用文件、不向应用发请求、不尝试触发问题**。提供完整 `SKILL.md` + `references/` + 检查/WAF 相关脚本，以及一份可直接粘进会话的单文件版 `dist/ruby-memsafety-exposure.md`。

## Recipe / links
- Repo: https://github.com/hsbt/ruby-memsafety-exposure（未标许可证，0★）
- 官方公告：https://www.ruby-lang.org/en/news/2026/11/18/multiple-vulnerabilities-in-regexp-and-string/
- 安装：把 `ruby-memsafety-exposure/` 拷到 agent 的 skills 目录（如 `~/.claude/skills/`），然后询问该应用是否受影响。
- 单文件：打开应用仓库的 agent 会话，让它阅读并遵循 [`dist/ruby-memsafety-exposure.md`](https://github.com/hsbt/ruby-memsafety-exposure/blob/master/dist/ruby-memsafety-exposure.md)。
- 3.2 及更早分支已停止维护，公告写明这些版本没有对应修复。

## Why it made the cut
与官方安全公告同日发布，场景清楚，流程只读、材料完整（SKILL.md、参考和脚本）。仓为 0★ 且未标许可证，属早期收录；装前建议先读脚本，升级 Ruby 仍是正道。
