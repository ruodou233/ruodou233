# 错误乱码的 AI 工作流｜Practical AI Agent Workflows

Open-source skills and workflows to help AI agents review their work, manage costs, coordinate long-running tasks, and retain reusable lessons.

我把日常与 AI Agent 协作中用到的任务编排、独立审查、成本优化和经验沉淀方法，做成可复用的开源 Skill，帮助 Agent 减少返工、接续长任务，并扩展研究与创作能力。

这些 Skill 面向 Claude Code / Codex 等支持 SKILL.md 的平台，可由 Agent 按你的电脑、订阅和已装工具调整接入方式。

这些 skill 遵循同一条分发原则：当多个 Agent 需要接入同一权威源时，采用单源维护——核心逻辑只改一处，减少同一规则在多处各自演化、重复漂移的风险；设计原则和两种实现结构（整包共享 / 共享规范+平台适配层）见 [agent-orchestration](https://github.com/ruodou233/agent-orchestration) 的"Skill 结构原则"一节。

## 可以拿来干什么

- **提高交付质量，减少人工返工**：用 cross-review 让另一家 AI 独立审查代码与方案，检查正确性、复杂度和替代思路；用 upgrade-audit 把对话中的偏好、踩坑经验沉淀进记忆与 Skill，减少重复纠正。
- **算清成本，合理安排任务**：用缓存保温先实测命中率和成本，确认划算再启用；配合额度监测，判断重任务何时运行、如何安排消耗。
- **让 Agent 接续完成长任务**：用 agent-orchestration 拆分任务、协调分工、衔接结果；用 connect-computers 接入远端电脑与 Agent，让多机资源参与工作。
- **扩展 Agent 获取信息和操作网页的能力**：用 web-access 处理检索、动态网页与需要登录态的页面；结合领域探索和社区口碑，为分析与决策补充可追溯的资料和真实使用反馈。
- **把研究推进到可实施的方案**：让聪明买手比较候选、成本和取舍，再用产品方案 Skill 明确首版范围、实现阶段与验收标准，形成可交给开发 Agent 的说明。
- **把资料和想法做成作品**：转写会议、访谈与播客，审阅中文里的套路表达；制作网页、演讲和作品集，让视觉、动效与声音共同服务内容。

## 最新研究

一个月 Codex 会话、392 个日志文件拆开算：长会话里一半以上 token 花在改，不是花在做；最贵的一条线程返工是首次交付的 52 倍。委派没救回来——多花的 10% 是父会话在轮询等工人。[一手数据与改掉的规则](https://github.com/ruodou233/agent-orchestration/blob/main/research/2026-09-delegation-study.md)

## 开源 Skill 目录

以下各表按 GitHub Star 数降序排列，同星保留原顺序。排序核验：2026-09-13；徽章显示最新星标数。

<!-- 同步目录时保留 Star 降序规则 -->
| Skill | Stars | 一句话介绍 |
|---|---|---|
| [de-ai-taste](https://github.com/ruodou233/de-ai-taste) | ![GitHub Stars](https://img.shields.io/github/stars/ruodou233/de-ai-taste?style=flat) | AI 写的中文一眼就能看出来？逐条找出 AI 味、给出具体修改建议，让文章、讲稿和文案读起来像你写的。<br>Review AI-written Chinese and suggest edits to remove formulaic phrasing while preserving the author's voice. |
| [cross-review](https://github.com/ruodou233/cross-review) | ![GitHub Stars](https://img.shields.io/github/stars/ruodou233/cross-review?style=flat) | AI 的活总差一点，总要你擦屁股，总打丑补丁？让另一家 AI 挑刺复查，自己把活干完整，不用你一直兜底。<br>An agent skill for independent code and design reviews across AI providers, checking correctness, complexity, and better approaches. |
| [claude-cache-keepalive](https://github.com/ruodou233/claude-cache-keepalive) | ![GitHub Stars](https://img.shields.io/github/stars/ruodou233/claude-cache-keepalive?style=flat) | 缓存保温：实测命中、算清收益，让长会话少花冤枉 token<br>Measure prompt cache hits and costs, then configure automatic keepalive when the savings justify it. |
| [free-token-eggs](https://github.com/ruodou233/free-token-eggs) | ![GitHub Stars](https://img.shields.io/github/stars/ruodou233/free-token-eggs?style=flat) | 免费额度找半天、领一圈，模型还不好用？帮你挑值得领的免费 AI token——太蠢的大模型不收录，吃点好的。<br>Find worthwhile free LLM API credits and AI trials, with eligibility, expiry dates, and claim links checked. |
| [domain-explorer](https://github.com/ruodou233/domain-explorer) | ![GitHub Stars](https://img.shields.io/github/stars/ruodou233/domain-explorer?style=flat) | 速通新领域：入门、转行、选课题，先把来龙去脉和各路说法弄明白<br>Get up to speed on a new topic through its history, competing approaches, expert debates, and practical experience. |
| [upgrade-audit](https://github.com/ruodou233/upgrade-audit) | ![GitHub Stars](https://img.shields.io/github/stars/ruodou233/upgrade-audit?style=flat) | 把你教过 AI 的东西留下来：沉淀偏好、复盘踩坑、更新 skill 和工作流程<br>Review conversation history, agent memory, and skills to identify reusable lessons and propose updates to outdated instructions. |
| [smart-buyer](https://github.com/ruodou233/smart-buyer) | ![GitHub Stars](https://img.shields.io/github/stars/ruodou233/smart-buyer?style=flat) | AI 推荐了一堆，到底该选哪个还是没弄明白？聪明买手帮你把商品、软件、服务和技术方案研究明白再选。<br>Research and compare products, software, services, and technical options using buying criteria, verified costs, and real user feedback. |
| [agent-orchestration](https://github.com/ruodou233/agent-orchestration) | ![GitHub Stars](https://img.shields.io/github/stars/ruodou233/agent-orchestration?style=flat) | 复杂任务跑到半夜，你不可能一直盯着。让 Agent 分工跑长任务和批量工作，你只管第二天早上收结果。<br>Coordinate AI agents for long-running tasks, parallel work, and overnight workflows. |
| [audio-transcribe](https://github.com/ruodou233/audio-transcribe) | ![GitHub Stars](https://img.shields.io/github/stars/ruodou233/audio-transcribe?style=flat) | 把会议、访谈、课程和播客变成文字稿，需要说话人、时间戳和字幕也能安排<br>Transcribe Mandarin recordings, podcasts, meetings, and videos with speaker labels, timestamps, subtitles, and transcript review. |
| [community-buzz](https://github.com/ruodou233/community-buzz) | ![GitHub Stars](https://img.shields.io/github/stars/ruodou233/community-buzz?style=flat) | 想听真实口碑？从社区里挖使用体验、竞品痛点和技术争议<br>Find real user experiences, product comparisons, and disagreements in online communities, with links to the original discussions. |
| [craft-frontend-ppt](https://github.com/ruodou233/craft-frontend-ppt) | ![GitHub Stars](https://img.shields.io/github/stars/ruodou233/craft-frontend-ppt?style=flat) | 让网页成为舞台：演讲、作品集、品牌页面和交互文章，让视觉、动效与声音一起表达<br>Create HTML slide decks, portfolios, landing pages, and interactive stories with visual design, animation, and sound. |
| [wisdom-roundtable](https://github.com/ruodou233/wisdom-roundtable) | ![GitHub Stars](https://img.shields.io/github/stars/ruodou233/wisdom-roundtable?style=flat) | 大事拿不定，小事没思路？拉一桌不同视角，看看盲区和分歧<br>Explore ideas and decisions through multiple mental models, then compare their assumptions, blind spots, agreements, and disagreements. |
| [improve-product-plan](https://github.com/ruodou233/improve-product-plan) | ![GitHub Stars](https://img.shields.io/github/stars/ruodou233/improve-product-plan?style=flat) | 想做成一个作品？把应用、工具、自动化和游戏想法打磨成能开工的方案<br>Plan product requirements and MVP scope, then produce a development spec with milestones and acceptance criteria. |
| [connect-computers](https://github.com/ruodou233/connect-computers) | ![GitHub Stars](https://img.shields.io/github/stars/ruodou233/connect-computers?style=flat) | 把电脑连起来：轻薄本调家中工作机，闲置电脑跑任务，出门也能接着干<br>Set up SSH, VPN, remote desktop access, and remote AI agents across your computers for work at home and on the go. |
| [codex-reset-watch](https://github.com/ruodou233/codex-reset-watch) | ![GitHub Stars](https://img.shields.io/github/stars/ruodou233/codex-reset-watch?style=flat) | Codex 额度哨兵：看看还能蹬多久，重任务该现在上还是缓一缓<br>Track Codex usage limits, spending pace, and reset signals to plan your next tasks. |
| [web-access](https://github.com/ruodou233/web-access) | ![GitHub Stars](https://img.shields.io/github/stars/ruodou233/web-access?style=flat) | 给 AI 装上联网能力：查资料、读动态网页、用登录态，把网页上的事办完<br>An agent skill for web research and browser automation, including logged-in pages, dynamic content, and browser history search. |

### 机制参考仓

这些仓库把我的具体实现放出来，按各仓说明接到你自己的环境。

| Skill | Stars | 一句话介绍 |
|---|---|---|
| [claude-code-feishu](https://github.com/ruodou233/claude-code-feishu) | ![GitHub Stars](https://img.shields.io/github/stars/ruodou233/claude-code-feishu?style=flat) | 出门前电脑上开的活，到手机上就接不上了？用飞书接着指挥同一个 Claude Code 会话，回来接着干。<br>Continue the same desktop Claude Code session from your phone through Feishu / Lark. |
| [growth-radar](https://github.com/ruodou233/growth-radar) | ![GitHub Stars](https://img.shields.io/github/stars/ruodou233/growth-radar?style=flat) | 想学爆款先看清涨粉从哪来：筛案例、找作品、拆内容<br>Research social media follower growth through creator rankings, published content, and public comments. |
| [polymarket-anomaly-watch](https://github.com/ruodou233/polymarket-anomaly-watch) | ![GitHub Stars](https://img.shields.io/github/stars/ruodou233/polymarket-anomaly-watch?style=flat) | 每天醒来就有一份科技情报——市场异动、GitHub 热榜、App Store 榜单，AI 替你盯着。<br>Monitor Polymarket anomalies, GitHub trends, and App Store rankings for a daily tech briefing. |
| [multi-upstream-agent-routing](https://github.com/ruodou233/multi-upstream-agent-routing) | ![GitHub Stars](https://img.shields.io/github/stars/ruodou233/multi-upstream-agent-routing?style=flat) | 给 Agent 挑线路：核能力、算实付、配主备，把上游选择理清楚<br>A design guide for multi-provider LLM routing, fallback policies, capability checks, and cost accounting. |
| [turn-guard](https://github.com/ruodou233/turn-guard) | ![GitHub Stars](https://img.shields.io/github/stars/ruodou233/turn-guard?style=flat) | Claude Code 老忘流程？把该做的检查变成每回合提醒<br>Claude Code hooks for background task follow-ups and reminders to review plans and completed changes. |

## 找到我

- 小红书：错误乱码
- 微信公众号：能工智人错误乱码
- B站：若逗道人

有修改方案或问题，欢迎在对应仓库提 issue / PR。
