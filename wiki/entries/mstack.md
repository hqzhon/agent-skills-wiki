# mstack（Claude Code + Codex 双宿主工程技能包）

**Tags:** engineering, spec, tdd, debugging, handoff, claude-code, codex, plugin
**Source:** [@mauroubeda](https://x.com/mauroubeda/status/2120852746236780810) · 2026-11-12
**Engagement:** 新开源，社区信号弱（仓库刚发布）· Apache-2.0

## When to use
同时用 Claude Code 和 Codex CLI，想要一套「先规格、再测试优先计划、修 bug 先证明根因」的工程流程，并让两家模型互相做只读评审。

## What it does
一个插件 marketplace，两边原生可读，每个技能一份 SKILL.md：
- **brainstorm → write-specs → plan**：想法 → 设计简报 → EARS 需求规格 → 红绿 TDD 分阶段计划（跨厂商评审）
- **diagnose**：崩溃/回归/flaky/泄漏，先分级举证并写回归测试，再修
- **handoff**：写一份可续跑的交接文件（分支、HEAD、未提交路径、门禁命令、下一步）
- **backlog-triage**：读全部 open issue，分 now/next/defer，只发经批准的评论
- 三种协作工作流：Claude 主导 + Codex 只读评审、反过来、Claude 当 PM 让 Codex 写码

## Recipe / links
- 仓库：https://github.com/mubeda/mstack
- 按 README 把 marketplace 加到 Claude Code / Codex CLI，再按需装单个插件

## Why it made the cut
配方非常具体（每个阶段的输入输出和护栏都写清），场景明确、仓库可核；热度低，作为工程流程参考收录，可和 [Superpowers](superpowers.md)、[Elephant-Goldfish Model](elephant-goldfish-model.md) 对照。
