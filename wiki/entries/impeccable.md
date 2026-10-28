# Impeccable（前端设计词汇表）

**Tags:** design, frontend, anti-slop, ui-ux, skill-pack
**Source:** [@FReza1984](https://x.com/FReza1984/status/2115308533772439586) · 2026-10-28
**Engagement:** ~90.9k★ · Apache-2.0 · actively trending

## When to use
When your agent keeps shipping the **same purple SaaS look** (Inter everywhere, nested cards, gradient hero) and you need a shared design vocabulary—shape → build → critique → polish—plus deterministic anti-slop checks before ship.

## What it does
One installable skill with **24 commands** (`/impeccable init|shape|critique|audit|polish|bolder|quieter|distill|harden|animate|…`). `/init` writes durable product truth to `PRODUCT.md`; later commands use that context. Ships a **62-rule detector** CLI (`npx impeccable detect`) that needs no LLM, plus optional live browser iteration.

## Recipe / links
- Repo: https://github.com/pbakaus/impeccable (~90.9k★, Apache-2.0)
- Docs: https://impeccable.style
- Install: from project root `npx impeccable install`, then `/impeccable init`
- Skill path: `.agents/skills/impeccable/SKILL.md` (also Cursor/Hermes bundles)

## Why it made the cut
Concrete multi-command SKILL.md + installable CLI/detector, clear anti-slop use case, and a large verifiable open-source footprint—far beyond a taste rant.
