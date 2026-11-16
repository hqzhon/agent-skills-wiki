# bookleme（读了么：把书编译成 Agent Skill）

**Tags:** skill-authoring, books, knowledge-base, meta, chinese
**Source:** [@jevlorde](https://x.com/jevlorde/status/2122255946860683316) · 2026-11-16
**Engagement:** 发现帖 3 赞 / 78 次展示；仓库 [bookleme/bookleme](https://github.com/bookleme/bookleme) 现 268★ / 4 forks，MIT（2026-11-09 建仓）

## When to use
要把一本书的「工作方法」编译成可调用、可校验的 Agent Skill，而不是写一份摘要或把全文塞进上下文。尤其在意引文必须能回源、第三方书默认不公开分发时。若只需要把 PDF/EPUB 抽成按章加载的知识包，已有更成熟的 [book-to-skill](book-to-skill.md)。

## What it does
Python 3.9+ 编译器工具链，核心只用标准库。一次阅读，双引擎产出：

- knowledge_pack：可查询的结构化知识包（主题路由、按需切片、决策备忘、出处清单）
- behavior_skill：带状态机的行为技能（角色、硬约束、输出契约、反模式、情绪护栏）

内置教练对话、框架检索两种体裁插件（专业分析、决策清单仍在规划）。强调逐字忠实度回验（7 项指标）和 6 道版权硬门（单段引文、总引用比、shingle 重叠等任一失败则不能安装/公开）。第三方书产物默认私有；公开需显式确认。带测试、校验器和真实中文书回归说明。

## Recipe / links
- Repo: https://github.com/bookleme/bookleme（MIT，268★）

```bash
git clone https://github.com/bookleme/bookleme.git
cd bookleme
python3 -m bookleme run --input <book> --title "书名"
python3 -m bookleme validate examples/coach
# 确认后再写入技能真源：
python3 -m bookleme run --input <book> --title "书名" --install --user-rights owned
```

- 对比说明见仓库 README「与同类项目对比」（相对 [book-to-skill](book-to-skill.md) / virgiliojr94/book-to-skill）

## Why it made the cut
与已收录的 book-to-skill 定位不同：这是带双引擎、忠实度指标和版权硬门的编译器，而不是「抽章节做成知识包」。有可运行的标准库实现、测试和示例产物，场景清楚。仓很新，星标主要来自近一周，后续需看体裁插件是否继续交付。
