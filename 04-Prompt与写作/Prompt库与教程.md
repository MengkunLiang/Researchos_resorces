# Prompt 库与教程

这一页收的是“能直接提升 AI 辅助科研效率”的 Prompt 资源与教程资源，不局限于单一模型。

## 1. 直接面向 AI 科研 / 学术写作的 Prompt 资源

| 资源 | 类型 | 简述 | 链接 |
| --- | --- | --- | --- |
| awesome-ai-research-writing | Prompt / 资源合集 | 面向 AI 科研写作的公开资源库，适合作为写作、审稿、提纲、改写的起点。 | [Leey21/awesome-ai-research-writing](https://github.com/Leey21/awesome-ai-research-writing) |
| HKUST-Got-Skills Resources | 课程化资源页 | 把 Skills、MCP、命令行工具、科研自动化材料放在一个入口里，特别适合新手建立整体视角。 | [HKUST-Got-Skills Resources](https://giggleliu.github.io/HKUST-Got-Skills/resources) |
| CARefully prompt your AI | 写作 Prompt 库 | 用 `Collect / Articulate / Refine / Evaluate` 四阶段组织学术写作 Prompt，并强调伦理边界。 | [CARefully prompt your AI](https://olivethree.github.io/carefullyprompt/) |

## 2. 学习如何设计更强 Prompt / Agent 的资源

| 资源 | 类型 | 简述 | 链接 |
| --- | --- | --- | --- |
| Hugging Face Agents Course | 课程 | 适合理解 Agent、工具调用、任务分解、RAG 与多步执行。 | [huggingface/agents-course](https://github.com/huggingface/agents-course) |
| Agent Skills | 标准站点 | 如果你已经不满足于一次性 prompt，建议直接学习如何把提示词做成可复用 Skill。 | [agentskills.io](https://agentskills.io/) |
| Anthropic Skills | 官方示例库 | 适合学习“从 prompt 走向可复用技能”的写法。 | [anthropics/skills](https://github.com/anthropics/skills) |
| OpenHands Global Skills Docs | 文档 | 适合理解共享技能、触发条件、边界和最佳实践。 | [OpenHands Docs](https://docs.openhands.dev/openhands/usage/microagents/microagents-public) |

## 3. 怎么用这些 Prompt 资源才更像做研究，而不是堆模板

### 更推荐的用法

- 用 Prompt 库启发工作流，而不是直接复制最终措辞。
- 尽快把高频 Prompt 固化成 Skills 或结构化模板。
- 对所有跟“结论、引用、novelty、实验结果”相关的输出，保留人工 gate。

### 不太推荐的用法

- 直接让模型“生成一篇完整论文然后就提交”。
- 用单个超长 Prompt 试图覆盖整个研究闭环。
- 不要求证据、不要求引用来源、不要求 artifact。

## 4. 我更推荐的升级路径

1. 先用 `awesome-ai-research-writing` 找启发
2. 再用 `CARefully prompt your AI` 补齐写作与伦理边界
3. 最后把最常用的 Prompt 固化为 `Skill` 或 `workflow template`

如果你的目标是做 ResearchOS，最终重心应该从“Prompt 收集”逐渐转向“Skill 化 + Artifact 化 + 可验证流程化”。
