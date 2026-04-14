# Skills 标准与生态

这一部分主要回答三个问题：

1. Skill 到底是什么？
2. 现在有哪些主流 Skill 生态？
3. 哪些生态最适合往科研智能体里接？

## 1. 核心标准与官方入口

| 资源 | 定位 | 简述 | 链接 |
| --- | --- | --- | --- |
| Agent Skills | 标准 | Agent Skills 的公开标准与说明网站，适合先理解 `SKILL.md` 这类能力封装的基本范式。 | [agentskills.io](https://agentskills.io/) |
| Anthropic Skills | 官方技能仓库 | 官方公开的 Claude Skills 仓库，包含 `pdf`、`pptx`、`docx`、`xlsx`、`mcp-builder` 等高价值技能。 | [anthropics/skills](https://github.com/anthropics/skills) |
| OpenHands Global Skills Docs | 文档 | OpenHands 对全局 Skills 的使用与贡献说明，适合理解“公共技能注册表”的实践方式。 | [OpenHands Docs](https://docs.openhands.dev/openhands/usage/microagents/microagents-public) |
| OpenHands Extensions | 注册表 | OpenHands 的公开扩展注册表，适合当作 Skills 与扩展能力的发现入口。 | [OpenHands/extensions](https://github.com/OpenHands/extensions) |
| HF Skills | 技能广场 | Hugging Face 的 `hf-skills` 页面，偏向训练、评测、发布、数据构建等 AI/ML 场景。 | [hf-skills](https://huggingface.co/hf-skills) |

## 2. 对科研最有价值的 Skills 生态

| 资源 | 定位 | 适合场景 | 链接 |
| --- | --- | --- | --- |
| AI-research-SKILLs | AI 研究工程技能库 | 覆盖分布式训练、评测、推理服务、论文写作、research ideation 等，最像“AI 科研工程操作手册”。 | [zechenzhangAGI/claude-ai-research-skills](https://github.com/zechenzhangAGI/claude-ai-research-skills) |
| Claude Scientific Skills | 科学研究技能库 | 面向生物、化学、医学、数据库、科学写作等领域，适合跨学科科研支持。 | [K-Dense-AI/claude-scientific-skills](https://github.com/K-Dense-AI/claude-scientific-skills) |
| Anthropic Skills | 通用高价值技能 | 如果你更看重 PDF、表格、文档协作和通用生产力能力，这个仓库非常值得长期跟。 | [anthropics/skills](https://github.com/anthropics/skills) |
| obra/superpowers | 方法论技能 | 不是科研专用，但对“测试、调试、计划、验证、并行分工”非常强，适合研究代码与实验工程。 | [obra/superpowers](https://github.com/obra/superpowers) |

## 3. 面向“收集与发现”的辅助仓库

| 资源 | 定位 | 简述 | 链接 |
| --- | --- | --- | --- |
| awesome-claude-skills | Awesome 列表 | 一个适合持续扫新的 Skills 汇总列表。 | [ComposioHQ/awesome-claude-skills](https://github.com/ComposioHQ/awesome-claude-skills) |
| antigravity-awesome-skills | 大型聚合库 | 可安装技能数量非常多，适合找灵感，但要注意筛选质量。 | [sickn33/antigravity-awesome-skills](https://github.com/sickn33/antigravity-awesome-skills) |
| everything-claude-code | Claude Code 配置与增强 | 更偏“让 AI coding agent 变强”的实践集，对科研开发也有帮助。 | [affaan-m/everything-claude-code](https://github.com/affaan-m/everything-claude-code) |
| HKUST-Got-Skills | 教学与资源入口 | 把 Skills、MCP、命令行工具和训练资料串成课程化入口，很适合做入门总览。 | [HKUST-Got-Skills Resources](https://giggleliu.github.io/HKUST-Got-Skills/resources) |

## 4. 选型建议

### 如果你要做“ResearchOS 的主链路”

- Skills 标准：先看 `Agent Skills`
- 官方技能范式：优先参考 `anthropics/skills`
- 研究工程能力库：优先接 `AI-research-SKILLs`
- 跨学科科研技能：补 `claude-scientific-skills`
- 方法论与工程纪律：补 `obra/superpowers`

### 如果你只想快速增强一个 coding agent

- 先装 `anthropics/skills`
- 再挑 `AI-research-SKILLs` 里与你当前实验相关的几个目录
- 最后用 `awesome-claude-skills` 和 `antigravity-awesome-skills` 补边角能力

## 5. 一个很实用的判断标准

选择 Skill 时，优先保留下面这三类：

- 能稳定复用的方法论，而不是一次性 prompt。
- 能显著降低上下文长度的知识封装。
- 能让 Agent 在科研场景里“少犯低级错”的流程化经验。

如果一个 Skill 只是把一段 prompt 换个目录名，长期价值通常不高。
