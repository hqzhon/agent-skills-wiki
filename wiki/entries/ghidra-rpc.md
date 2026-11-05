# ghidra-rpc（Cellebrite Labs 的 Ghidra 逆向 skill）

**Tags:** security, reverse-engineering, ghidra, binary-analysis
**Source:** [@tensorstaff](https://x.com/tensorstaff/status/2118151716223017172) · 2026-11-05
**Engagement:** 仓库 cellebrite-labs/ghidra-rpc，约 400★（未声明 license）

## When to use
需要 agent 自主做二进制逆向：反编译函数、追调用图、找不安全字符串操作、恢复结构体类型，或对比两个版本的二进制改了什么。

## What it does
把 Ghidra 作为常驻后台守护进程运行，通过返回结构化 JSON 的 CLI 暴露能力；任何能跑 shell 命令的编码 agent（Claude Code、Cursor 等）都能驱动完整逆向会话。覆盖反编译 / 反汇编 / CFG / P-code、交叉引用和模式搜索、重命名与注释、类型恢复、SLEIGH 打补丁、版本追踪与 BSim 函数匹配。

## Recipe / links
- Repo: https://github.com/cellebrite-labs/ghidra-rpc
- 前置：Ghidra 11+、Python 3.11+、Java 17+、uv；`uv tool install` 后对 agent 说「把 /usr/bin/ls 载入 Ghidra 找不安全的字符串操作」
- 手动：`ghidra-rpc start --project /tmp/work.gpr --headless`、`ghidra-rpc decompile ls main`、`ghidra-rpc xrefs-to ls strcmp`

## Why it made the cut
出自专业取证公司的实验室，接口设计清晰、文档完整；与已收录的 binsleuth（静态分诊）互补，提供完整逆向工作台。注意仓库未声明许可证，商用前先确认。
