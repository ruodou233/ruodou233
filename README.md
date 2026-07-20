# 你好，我是错误乱码 👋

我把自己日常和 AI Agent 协作沉淀出来的工作流做成开源 Skill 分享出来。每个 skill 都能直接装进 Claude Code / Codex 等支持 SKILL.md 的平台，下载后由你的 Agent 按你的电脑数量、订阅和已装 CLI 自适应成你自己的方案。

这些 skill 遵循同一条分发原则：当多个 Agent 需要接入同一权威源时，采用单源维护——核心逻辑只改一处，减少同一规则在多处各自演化、重复漂移的风险；设计原则和两种实现结构（整包共享 / 共享规范+平台适配层）见 [agent-orchestration](https://github.com/ruodou233/agent-orchestration) 的"Skill 结构原则"一节。

## 开源 Skill 目录

<!-- 本表由维护脚本生成 -->
| Skill | 一句话介绍 |
|---|---|
| [wisdom-roundtable](https://github.com/ruodou233/wisdom-roundtable) | 智慧圆桌：11 位思想家并行独立分析你的决策 |
| [domain-explorer](https://github.com/ruodou233/domain-explorer) | 速通新领域：四线并行调研，产出交互式知识地图 |
| [de-ai-taste](https://github.com/ruodou233/de-ai-taste) | 中文去 AI 味：逐条检测 AI 生成痕迹并给修改建议 |
| [improve-product-plan](https://github.com/ruodou233/improve-product-plan) | 把模糊的产品想法梳理成可开发、可验收的 SPEC.md |
| [free-token-eggs](https://github.com/ruodou233/free-token-eggs) | 免费 Token 领鸡蛋：筛选值得领的中国 AI 平台免费额度 |
| [smart-buyer](https://github.com/ruodou233/smart-buyer) | 聪明买手：正反双轨设标 + 社区口碑核验，排出可追溯的性价比排序 |
| [agent-orchestration](https://github.com/ruodou233/agent-orchestration) | 长任务治理：主代理指挥、子代理干活、状态落盘、断点续跑 |
| [cross-review](https://github.com/ruodou233/cross-review) | 跨厂商双审：让另一家公司的最强模型独立审你的方案 |
| [upgrade-audit](https://github.com/ruodou233/upgrade-audit) | 升级审计：让 Agent 定期把对话里的知识沉淀进文档体系 |
| [claude-cache-keepalive](https://github.com/ruodou233/claude-cache-keepalive) | Claude 缓存保温：实测 TTL、按环境设计保温节拍，控制冷读成本 |
| [connect-computers](https://github.com/ruodou233/connect-computers) | 多电脑互联：VPN+SSH+远控+远端 Agent 的分层配置方案 |

## 找到我

- 小红书：错误乱码
- 微信公众号：能工智人错误乱码
- B站：若逗道人

有修改方案或问题，欢迎在对应仓库提 issue / PR。
