# Contributing / 贡献指南

Thanks for helping keep this wiki useful! 感谢帮忙完善这个 wiki。

## Submit a skill / 推荐 skill

The easiest way: **[open a "Submit a skill" issue](https://github.com/hqzhon/agent-skills-wiki/issues/new?template=submit-skill.yml)**. Self-promotion is fine if the skill is genuinely useful.
最简单：直接提一个 Issue。推荐自己做的 skill 也完全 OK。

### Quality bar / 收录标准

An entry should meet at least two of:

1. **Concrete recipe** — steps, a checklist, or a `SKILL.md`
2. **Clear use case** — you can say *when* an agent should use it
3. **Verifiable material** — a public repo, gist, or detailed post
4. **Community signal** — stars, real usage (a bonus, never the only reason)

We skip ads, pure hype, prompt dumps without steps, and anything that needs credentials-scraping or ToS-violating automation.

## Send a PR / 提交 PR

1. Add `wiki/entries/<slug>.md` using this template:

   ```markdown
   # <Name>（<一句中文或英文说明>）

   **Tags:** tag1, tag2, skill
   **Source:** [@author](https://x.com/author/status/...) · YYYY-MM-DD
   **Engagement:** owner/repo ~N★ · LICENSE

   ## When to use
   ## What it does
   ## Recipe / links
   - Repo: https://github.com/owner/repo
   - Install: `npx skills add owner/repo` (or the upstream's documented command)
   ## Why it made the cut
   ```

2. Add one row at the top of `wiki/Catalog.md` (newest first).
3. Optional: add it to a topic list in `README.md` if it is a standout.

Corrections (dead links, wrong install commands, license changes) are very welcome — small PRs are fine.
纠错、补安装命令、更新许可信息都欢迎，小 PR 也行。

## License

By contributing you agree your contribution is released under [CC BY 4.0](LICENSE).
