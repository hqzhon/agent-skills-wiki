# Google Cloud Skills（官方 / IAM Helper）

**Tags:** google-cloud, iam, security, official, skill-pack
**Source:** [@AiCybr_](https://x.com/AiCybr_/status/2114869950632403036) · 2026-10-27
**Engagement:** discovery post (low) · repo ~21.6K★ · Google official

## When to use
When a coding agent hits Google Cloud 403s, needs to simulate IAM policy changes, manage allow/deny policies, or request Privileged Access Management (PAM) grants — without inventing ad-hoc `gcloud` sequences.

## What it does
Official Agent Skills in [`google/skills`](https://github.com/google/skills). The IAM Helper slice packages four workflows: troubleshooting (requester vs resolver flows), policy simulator (must simulate before mutate), policy management (IAM v1 allow / v2 deny), and privileged-access-management. Skills orchestrate Policy Troubleshooter, PAM JIT, and least-privilege role discovery with approval gates for mutating commands. Broader catalog also covers GKE, BigQuery, Cloud Run, Agent Platform, etc.

## Recipe / links
- Repo: https://github.com/google/skills
- Blog: https://cloud.google.com/blog/products/identity-security/scale-agents-securely-with-iam-helper-agent-skills-and-mcp-tools/
- Install examples:
  - `npx skills add google/skills --skill iam-helper-for-troubleshooting`
  - `npx skills add google/skills --skill iam-helper-for-policy-simulator`
  - `npx skills add google/skills --skill iam-helper-for-policy-management`
  - `npx skills add google/skills --skill iam-helper-for-privileged-access-management`
- Catalog listings: https://www.skills.sh/google/skills/iam-helper-for-troubleshooting

## Why it made the cut
Vendor-official SKILL.md pack with clear when-to-use modes, verifiable GitHub + Cloud blog, and reusable IAM lifecycle recipes across Gemini CLI / Claude Code / Cursor.
