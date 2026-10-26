# Cognition Vulnerability Fixes（devin-vuln-fixes）

**Tags:** security, patching, php, nodejs, gitlab, skill-pack
**Source:** [@RL_landing](https://x.com/RL_landing/status/2114659803582620056) · 2026-10-26
**Engagement:** news/discovery posts this hour; official Cognition open-source plugin (MIT)

## When to use
When you need a coding agent to inventory and patch the Oct 2026 critical PHP2Shell, Node.js (Brotli RCE), or self-managed GitLab RCE advisories across Docker/CI/IaC—with an approval gate before any write.

## What it does
Three Agent Skills from CognitionAI: `fix-php-vuln`, `fix-node-vuln`, `fix-gitlab-vuln`. Flow: read-only inventory → approval → patch to verified fixed versions → test before/after → one PR per repo with risk label and rollback plan. Works in Devin, Claude Code, Codex, Cursor, and other SKILL.md agents.

## Recipe / links
- Repo: https://github.com/CognitionAI/devin-vuln-fixes
- Install: `npx skills add CognitionAI/devin-vuln-fixes`
- Product page: https://devin.ai/security/vulnerability-fixes
- Blog: https://devin.ai/blog/vulnerability-fixes-plugin

## Why it made the cut
Concrete installable SKILL.md trio; urgent clear security use case; verifiable Cognition-maintained open source (not empty CVE news).
