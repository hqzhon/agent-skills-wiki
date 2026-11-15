# character-voice-lock（角色声线锁定）

**Tags:** video, voice, seedance, dreamina, character-consistency, skill
**Source:** [@PJaccetturo](https://x.com/PJaccetturo/status/2121611611286716750) · 2026-11-15
**Engagement:** 宣布帖约 207 赞 / 5 转 / 37 回复 / 226 收藏；技能正文在评论里的 Google 文档（[链接帖](https://x.com/PJaccetturo/status/2121611612989612162) 约 39 赞 / 71 收藏）。Nexus 团队公开的流程，不是 git 仓库。

## When to use
在 Dreamina 的 Seedance 2.5 里做 AI 角色视频时，角色声音机器、每镜不一样，或脸和声音对不上（面具反派、生物、外表温和但声音粗砺）。用来给一个角色锁定一条可复用的人声参考，而不是每镜重新描述声音。

## What it does
一份可复制的 `SKILL.md`：先要角色设定、3–5 句台词、目标声线，以及是否需要面具/对讲机等效果。流程是：① 写两段声线简述（年龄、音高、口音、节奏、压力下的变化），每条提示词都带上；② 用短时长、成片分辨率做 2–3 次纯文本便宜测试，稳定就直接锁定；③ 不稳定则录 10–15 秒真人参考；④ 仍不对就先生成「声音供体」角色取音频，再贴到真正的角色脸上；⑤ 需要特效时只在音频软件里处理一次，导出干净参考；⑥ 把最终约 10 秒片段存进项目，之后每镜都附上这段音频参考 + 声线简述；⑦ 提示词里控制句量、逐字台词、停顿和意图，避免语速过快或配乐盖声。文档明确要求：不要去复制可识别的真人声线。此流程针对 Seedance / Dreamina；其他生成器能否照搬，发帖回复里也有人存疑，需要自行试。

## Recipe / links
- 宣布帖：https://x.com/PJaccetturo/status/2121611611286716750
- 技能文档（复制 `SKILL.md` 一节，存为 `character-voice-lock/SKILL.md` 或贴进 Claude Project 说明）：https://docs.google.com/document/d/1vY5tu8qaQG4elTXmgoS5qy5-bJ1o8uu6K2Esh7U1lQE/edit?usp=sharing
- 用法：带上角色设定和几句台词，对 agent 说 “Lock this character's voice.”
- 没有独立 git 仓库；以该 Google 文档为权威正文

## Why it made the cut
有清楚的使用场景和可逐步执行的配方（测试 → 人声/供体参考 → 锁定存储），材料是可核验的长文档而非空喊，宣布帖互动也很强。适用范围主要是 Seedance 2.5 / Dreamina，收录时如实写明。
