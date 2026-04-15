# Skills 标准与生态

这一页不只回答“Skill 是什么”，还回答更现实的四个问题：

1. 现在 Skills 到底是不是开放标准？
2. 哪些平台真的支持跨工具复用？
3. 哪些官方 / 半官方生态最值得长期跟？
4. 做科研团队资源库时，应该把哪些 Skills 生态优先收进来？

## 1. 核心标准与官方文档

| 资源 | 定位 | 简述 | 链接 |
| --- | --- | --- | --- |
| Agent Skills | 开放标准入口 | 当前最关键的开放标准入口，定义了 `SKILL.md`、描述字段、安装方式和跨平台兼容思路。 | [agentskills.io](https://agentskills.io/) |
| Agent Skills 规范与参考 SDK | 规范实现 | `agentskills/agentskills` 提供规范、文档和参考实现，适合团队后续自己做兼容技能。 | [agentskills/agentskills](https://github.com/agentskills/agentskills) |
| Agent Skills 中文文档 | 官方中文入口 | 对需要中文理解 Skills 概念、预构建技能和自定义 Skills 的读者，这是很适合的入门入口。 | [Claude Docs 中文](https://docs.claude.com/zh-CN/docs/agents-and-tools/agent-skills/overview) |
| Claude Skills 总览 | 官方总览 | 从 Anthropic 视角解释为什么要用 Skills、在哪些产品里可用。 | [Claude Docs](https://docs.claude.com/en/docs/agents-and-tools/agent-skills) |
| Claude Code Skills | 官方实现文档 | 讲清楚 `.claude/skills/`、`allowed-tools`、插件技能、团队共享等实际做法。 | [Claude Code Docs](https://docs.claude.com/en/docs/claude-code/skills) |
| Agent Skills in the SDK | SDK 文档 | 对后续计划自行做 agent runtime 或 SDK 集成的场景，这页很重要。 | [Claude Agent SDK Docs](https://docs.claude.com/en/docs/agent-sdk/skills) |
| Anthropic Engineering Blog | 架构与最佳实践 | 官方工程博客，解释 Skills 为什么从“提示词”升级成“文件夹 + 脚本 + 资源”的能力层。 | [Anthropic Blog](https://www.anthropic.com/engineering/equipping-agents-for-the-real-world-with-agent-skills) |
| OpenAI Skills Catalog | Codex 官方目录 | `openai/skills` 是 Codex 的公开技能目录，适合从 Codex 视角理解 curated / experimental / system skills。 | [openai/skills](https://github.com/openai/skills) |
| GitHub Copilot Skills | 跨平台采纳 | GitHub 已明确把 Agent Skills 视为开放标准，并支持 `.github/skills` 与 `.claude/skills`。 | [GitHub Docs](https://docs.github.com/en/copilot/concepts/agents/about-agent-skills) |
| GitHub Copilot CLI 创建 Skills | 操作文档 | 对计划把同一套技能同时供 Copilot / Claude / Codex 使用的场景，这页很有参考价值。 | [GitHub Docs](https://docs.github.com/copilot/how-tos/copilot-cli/customize-copilot/create-skills) |
| Hugging Face Skills 文档 | 跨平台技能文档 | Hugging Face 把 Skills 明确做成面向 Claude Code、Codex、Gemini、Cursor 的跨平台包。 | [HF Hub Docs](https://huggingface.co/docs/hub/agents-skills) |
| OpenHands Skills 文档 | OpenHands 生态说明 | OpenHands 采用扩展版 AgentSkills 思路，支持公共 skills 仓库与触发式加载。 | [OpenHands Docs](https://docs.openhands.dev/sdk/guides/skill) |

## 2. 安装、分发与跨平台生态

| 资源 | 类型 | 简述 | 链接 |
| --- | --- | --- | --- |
| `npx skills` | 开放安装器 | 目前最像“通用包管理器”的技能安装工具，支持 Claude Code、Codex、Copilot、Cursor 等多个宿主。 | [vercel-labs/skills](https://github.com/vercel-labs/skills) |
| Skills Directory | 发现目录 | `skills.sh` 提供公开技能目录、安装量、热度和文档，是扫生态最有效的入口之一。 | [skills.sh](https://skills.sh/) |
| Skills Docs | 安装文档 | 对 `skills.sh` / `npx skills` 的使用、排名、安全说明讲得比较清楚。 | [skills.sh/docs](https://skills.sh/docs) |
| Hugging Face Skills | 跨平台技能组织 | 不只是一个仓库，而是完整的 Skills 组织、Space 和 Hub 文档体系。 | [hf-skills](https://huggingface.co/hf-skills) |
| HF Skill Finder | 技能检索工具 | Hugging Face 官方的 skill finder，适合查技能和看示例结构。 | [hf-skills/skill-finder](https://huggingface.co/spaces/hf-skills/skill-finder) |
| OpenHands 公共 Skills | 公共注册表 | OpenHands 的官方公共 skills 注册表，适合看另一种“平台级共享技能”做法。 | [OpenHands/skills](https://github.com/OpenHands/skills) |
| OpenHands 全局 Skills 文档 | 平台文档 | 说明 OpenHands 如何维护公共 global skills、如何触发、如何贡献。 | [OpenHands Global Skills](https://docs.openhands.dev/usage/prompting/microagents-public) |

## 3. 官方和高信号生态

| 资源 | 定位 | 适合场景 | 链接 |
| --- | --- | --- | --- |
| OpenAI Skills | Codex 官方技能目录 | 如果团队有人用 Codex，这是绝对不该漏掉的一条主线。 | [openai/skills](https://github.com/openai/skills) |
| Anthropic Skills | 官方基座技能库 | `pdf`、`docx`、`pptx`、`xlsx`、`mcp-builder`、`skill-creator` 这些都是科研团队极高频能力。 | [anthropics/skills](https://github.com/anthropics/skills) |
| Hugging Face Skills | AI/ML 官方技能库 | 偏模型训练、评测、数据构造、论文发布，对 AI/ML 科研团队很实用。 | [huggingface/skills](https://github.com/huggingface/skills) |
| OpenHands Skills | 公共 registry | 更适合把 skills 当平台能力层，而不只是个人插件。 | [OpenHands/skills](https://github.com/OpenHands/skills) |
| Azure Skills | 官方云与 AI 平台技能包 | 对需要云训练、推理、评测、Foundry/MCP/部署的一类科研团队很有价值。 | [microsoft/azure-skills](https://github.com/microsoft/azure-skills) |
| Vercel Agent Skills | 官方工程技能包 | 更偏前端、部署、界面审查，但对研究网站、demo、可视化展示同样有帮助。 | [vercel-labs/agent-skills](https://github.com/vercel-labs/agent-skills) |
| Expo Skills | 官方移动端技能包 | 如果团队做移动实验、可穿戴或 HCI 原型，值得关注。 | [expo/skills](https://github.com/expo/skills) |
| Remotion Skills | 官方视频与可视化技能 | 对做学术展示视频、动画讲解、演示素材很有帮助。 | [remotion-dev/skills](https://github.com/remotion-dev/skills) |

## 4. 对科研最有价值的三大 Skills 方向

### 方向 A：研究工程与实验执行

最值得优先看：

- [AI-Research-SKILLs](https://github.com/Orchestra-Research/AI-Research-SKILLs)
- [Hugging Face Skills](https://github.com/huggingface/skills)
- [Anthropic Skills](https://github.com/anthropics/skills)
- [Azure Skills](https://github.com/microsoft/azure-skills)

### 方向 B：学术写作、文献、审稿

最值得优先看：

- [K-Dense-AI/claude-scientific-writer](https://github.com/K-Dense-AI/claude-scientific-writer)
- [Imbad0202/academic-research-skills](https://github.com/Imbad0202/academic-research-skills)
- [CatVinci-Studio/paper-glance-skill](https://github.com/CatVinci-Studio/paper-glance-skill)
- [anthropics/skills](https://github.com/anthropics/skills)

### 方向 C：科学计算与学科领域

最值得优先看：

- [K-Dense-AI/scientific-agent-skills](https://github.com/K-Dense-AI/scientific-agent-skills)
- [HeshamFS/materials-simulation-skills](https://github.com/HeshamFS/materials-simulation-skills)
- [brunoasm/my_claude_skills](https://github.com/brunoasm/my_claude_skills)

## 5. 这页的结论

如果要把 Skills 当作科研能力库来长期建设，建议按下面顺序理解：

1. 先把 Skills 看成开放标准，而不是某一家产品的小功能
2. 再把 `Anthropic / HF / OpenHands / Copilot / Vercel skills` 这些生态串起来看
3. 最后才是选具体技能仓库和具体技能条目

也就是说，真正要做全面，不只是多收几个仓库，而是要把“标准、安装器、发现平台、官方生态、科研专用 bundle、单项高价值 skills”一起收录。

补充页：

- [跨平台宿主与官方技能库](./跨平台宿主与官方技能库.md)
- [Skill发现平台与精品合集](./Skill发现平台与精品合集.md)
- [科研工程与实验Skills](./科研工程与实验Skills.md)
- [科研写作与文献Skills](./科研写作与文献Skills.md)
- [科学计算与领域Skills](./科学计算与领域Skills.md)
