# 科研向 Skills 合集

这一页只看“跟科研任务直接相关”的 Skills，不再泛泛讨论所有 Skill 生态。

## 1. 研究工程与实验技能

| 资源 | 类型 | 简述 | 链接 |
| --- | --- | --- | --- |
| AI-research-SKILLs | 科研工程技能库 | 面向 AI 研究实验的技能总库，覆盖模型架构、训练、推理、评测、服务化、论文写作、idea 生成等。 | [zechenzhangAGI/claude-ai-research-skills](https://github.com/zechenzhangAGI/claude-ai-research-skills) |
| HF Skills | AI/ML 技能市场 | 包含数据集创建、模型训练、模型评测、论文发布等能力入口。 | [hf-skills](https://huggingface.co/hf-skills) |
| obra/superpowers | 研发方法技能 | 对科研代码尤其有帮助，适合写实验计划、系统化调试、做验证闭环。 | [obra/superpowers](https://github.com/obra/superpowers) |

## 2. 科学研究与学术工作流技能

| 资源 | 类型 | 简述 | 链接 |
| --- | --- | --- | --- |
| Claude Scientific Skills | 科学技能库 | 覆盖 scientific writing、literature review、peer review、OpenAlex / PubMed 等数据库接入。 | [K-Dense-AI/claude-scientific-skills](https://github.com/K-Dense-AI/claude-scientific-skills) |
| Anthropic Skills | 官方技能仓库 | 仓库里和科研最相关的是 `pdf`、`docx`、`pptx`、`xlsx`、`doc-coauthoring`、`mcp-builder`、`skill-creator`。 | [anthropics/skills](https://github.com/anthropics/skills) |
| OpenHands Extensions | 技能与扩展生态 | 如果你希望在 OpenHands 生态中共享或复用科研工作流技能，这个仓库值得长期跟踪。 | [OpenHands/extensions](https://github.com/OpenHands/extensions) |

## 3. 用于“学习如何设计 Skill”的资源

| 资源 | 类型 | 简述 | 链接 |
| --- | --- | --- | --- |
| Agent Skills | 标准站点 | 理解 `SKILL.md` 的结构、目标和复用方式。 | [agentskills.io](https://agentskills.io/) |
| HKUST-Got-Skills | 教学资源页 | 把 Skills 与科研自动化、MCP、命令行工具一起串起来，适合拉通思路。 | [HKUST-Got-Skills Resources](https://giggleliu.github.io/HKUST-Got-Skills/resources) |
| Hugging Face Agents Course | 课程 | 虽然不是纯 Skills 课程，但对“如何组织 agent 能力”很有帮助。 | [huggingface/agents-course](https://github.com/huggingface/agents-course) |

## 4. 适合 ResearchOS 的优先接入顺序

### 阶段 A：先把研究主链路跑起来

- `AI-research-SKILLs`
- `Anthropic Skills`
- `Claude Scientific Skills`

### 阶段 B：再补方法论与工程纪律

- `obra/superpowers`
- `OpenHands Extensions`

### 阶段 C：最后做发现与规模化管理

- `awesome-claude-skills`
- `antigravity-awesome-skills`
- `everything-claude-code`

## 5. 设计自己的科研 Skill 时，建议固定四个槽位

推荐你后面自建 Skills 时，统一用下面这个模板思路：

1. 任务边界：这个 Skill 解决哪一步，不解决哪一步。
2. 输入输出：要求哪些 artifact，产出哪些 artifact。
3. 失败模式：最常见的误判、漏项、风险点是什么。
4. 验证动作：调用完后必须检查哪些证据。

这四个槽位比单纯写一段提示词更适合长期维护。
