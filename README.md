# 错误乱码的 AI 工作流｜Practical AI Agent Workflows

Open-source agent skills and workflows for research, decision making, writing, and creative work.

我把自己日常和 AI Agent 协作沉淀出来的工作流做成开源 Skill 分享出来。每个 skill 都能直接装进 Claude Code / Codex 等支持 SKILL.md 的平台，下载后由你的 Agent 按你的电脑数量、订阅和已装 CLI 自适应成你自己的方案。

这些 skill 遵循同一条分发原则：当多个 Agent 需要接入同一权威源时，采用单源维护——核心逻辑只改一处，减少同一规则在多处各自演化、重复漂移的风险；设计原则和两种实现结构（整包共享 / 共享规范+平台适配层）见 [agent-orchestration](https://github.com/ruodou233/agent-orchestration) 的"Skill 结构原则"一节。

## 可以拿来干什么

- **研究明白再决定**：想买个东西、换个软件、了解新行业，先用领域探索摸清来龙去脉，再让聪明买手比较候选，社区口碑补上真实使用感受。
- **把想法做成作品**：让 AI 产品经理把想法问清楚，写成能开工的方案；做网页、演讲、作品集时，再把视觉、动效和声音安排上。
- **把资料变成自己的表达**：会议、访谈、播客先转成文字，写成文章、讲稿或口播后，再过一遍去 AI 味，留下自己的语气。
- **让 AI 把活接着干**：长任务分工跑，多台电脑连起来，重要方案找独立审查；干完再把踩过的坑、教过的东西沉淀下来。

## 开源 Skill 目录

<!-- 本表由维护目录同步 -->
| Skill | 一句话介绍 |
|---|---|
| [domain-explorer](https://github.com/ruodou233/domain-explorer) | 速通新领域：入门、转行、选课题，先把来龙去脉和各路说法弄明白<br>Get up to speed on a new topic through its history, competing approaches, expert debates, and practical experience. |
| [de-ai-taste](https://github.com/ruodou233/de-ai-taste) | AI 写的中文一眼就能看出来？逐条找出 AI 味、给出具体修改建议，让文章、讲稿和文案读起来像你写的。<br>Review AI-written Chinese and suggest edits to remove formulaic phrasing while preserving the author's voice. |
| [improve-product-plan](https://github.com/ruodou233/improve-product-plan) | 想做成一个作品？把应用、工具、自动化和游戏想法打磨成能开工的方案<br>Plan product requirements and MVP scope, then produce a development spec with milestones and acceptance criteria. |
| [free-token-eggs](https://github.com/ruodou233/free-token-eggs) | 免费额度找半天、领一圈，模型还不好用？帮你挑值得领的免费 AI token——太蠢的大模型不收录，吃点好的。<br>Find worthwhile free LLM API credits and AI trials, with eligibility, expiry dates, and claim links checked. |
| [smart-buyer](https://github.com/ruodou233/smart-buyer) | AI 推荐了一堆，到底该选哪个还是没弄明白？聪明买手帮你把商品、软件、服务和技术方案研究明白再选。<br>Research and compare products, software, services, and technical options using buying criteria, verified costs, and real user feedback. |
| [agent-orchestration](https://github.com/ruodou233/agent-orchestration) | 复杂任务跑到半夜，你不可能一直盯着。让 Agent 分工跑长任务和批量工作，你只管第二天早上收结果。<br>Coordinate AI agents for long-running tasks, parallel work, and overnight workflows. |
| [cross-review](https://github.com/ruodou233/cross-review) | AI 的活总差一点，总要你擦屁股，总打丑补丁？让另一家 AI 挑刺复查，自己把活干完整，不用你一直兜底。<br>An agent skill for independent code and design reviews across AI providers, checking correctness, complexity, and better approaches. |
| [upgrade-audit](https://github.com/ruodou233/upgrade-audit) | 把你教过 AI 的东西留下来：沉淀偏好、复盘踩坑、更新 skill 和工作流程<br>Review conversation history, agent memory, and skills to identify reusable lessons and propose updates to outdated instructions. |
| [claude-cache-keepalive](https://github.com/ruodou233/claude-cache-keepalive) | 缓存保温：实测命中、算清收益，让长会话少花冤枉 token<br>Measure prompt cache hits and costs, then configure automatic keepalive when the savings justify it. |
| [connect-computers](https://github.com/ruodou233/connect-computers) | 把电脑连起来：轻薄本调家中工作机，闲置电脑跑任务，出门也能接着干<br>Set up SSH, VPN, remote desktop access, and remote AI agents across your computers for work at home and on the go. |
| [audio-transcribe](https://github.com/ruodou233/audio-transcribe) | 把会议、访谈、课程和播客变成文字稿，需要说话人、时间戳和字幕也能安排<br>Transcribe Mandarin recordings, podcasts, meetings, and videos with speaker labels, timestamps, subtitles, and transcript review. |
| [community-buzz](https://github.com/ruodou233/community-buzz) | 想听真实口碑？从社区里挖使用体验、竞品痛点和技术争议<br>Find real user experiences, product comparisons, and disagreements in online communities, with links to the original discussions. |
| [codex-reset-watch](https://github.com/ruodou233/codex-reset-watch) | Codex 额度哨兵：看看还能蹬多久，重任务该现在上还是缓一缓<br>Track Codex usage limits, spending pace, and reset signals to plan your next tasks. |
| [craft-frontend-ppt](https://github.com/ruodou233/craft-frontend-ppt) | 让网页成为舞台：演讲、作品集、品牌页面和交互文章，让视觉、动效与声音一起表达<br>Create HTML slide decks, portfolios, landing pages, and interactive stories with visual design, animation, and sound. |
| [web-access](https://github.com/ruodou233/web-access) | 给 AI 装上联网能力：查资料、读动态网页、用登录态，把网页上的事办完<br>An agent skill for web research and browser automation, including logged-in pages, dynamic content, and browser history search. |
| [wisdom-roundtable](https://github.com/ruodou233/wisdom-roundtable) | 大事拿不定，小事没思路？拉一桌不同视角，看看盲区和分歧<br>Explore ideas and decisions through multiple mental models, then compare their assumptions, blind spots, agreements, and disagreements. |

### 机制参考仓

这些仓库把我的具体实现放出来，按各仓说明接到你自己的环境。

| Skill | 一句话介绍 |
|---|---|
| [growth-radar](https://github.com/ruodou233/growth-radar) | 想学爆款先看清涨粉从哪来：筛案例、找作品、拆内容<br>Research social media follower growth through creator rankings, published content, and public comments. |
| [polymarket-anomaly-watch](https://github.com/ruodou233/polymarket-anomaly-watch) | 每天醒来就有一份科技情报——市场异动、GitHub 热榜、App Store 榜单，AI 替你盯着。<br>Monitor Polymarket anomalies, GitHub trends, and App Store rankings for a daily tech briefing. |
| [claude-code-feishu](https://github.com/ruodou233/claude-code-feishu) | 出门前电脑上开的活，到手机上就接不上了？用飞书接着指挥同一个 Claude Code 会话，回来接着干。<br>Continue the same desktop Claude Code session from your phone through Feishu / Lark. |
| [multi-upstream-agent-routing](https://github.com/ruodou233/multi-upstream-agent-routing) | 给 Agent 挑线路：核能力、算实付、配主备，把上游选择理清楚<br>A design guide for multi-provider LLM routing, fallback policies, capability checks, and cost accounting. |
| [turn-guard](https://github.com/ruodou233/turn-guard) | Claude Code 老忘流程？把该做的检查变成每回合提醒<br>Claude Code hooks for background task follow-ups and reminders to review plans and completed changes. |

## 找到我

- 小红书：错误乱码
- 微信公众号：能工智人错误乱码
- B站：若逗道人

有修改方案或问题，欢迎在对应仓库提 issue / PR。
