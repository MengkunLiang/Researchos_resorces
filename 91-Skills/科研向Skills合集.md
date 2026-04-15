# 科研向 Skills 合集

这一页是 `91-Skills` 的科研总入口。目标不是简单列仓库，而是帮助快速判断：

1. 哪些 Skills 最适合科研团队先接
2. 哪些更偏研究工程，哪些更偏写作文献，哪些更偏科学计算
3. 哪些是“标准/发现平台”，哪些是“真正能直接上手的技能包”

## 1. 先记住这几类最值得优先看的资源

| 资源 | 角色 | 为什么重要 | 链接 |
| --- | --- | --- | --- |
| OpenAI Skills | Codex 官方目录 | 这是从 Codex 视角理解 skills 生态的核心入口，不能只看 Claude 而漏掉它。 | [openai/skills](https://github.com/openai/skills) |
| Anthropic Skills | 官方基座 | `pdf/docx/pptx/xlsx/mcp-builder/skill-creator` 这些对科研团队是最高频通用能力。 | [anthropics/skills](https://github.com/anthropics/skills) |
| AI Research SKILLs | AI 研究工程总库 | 目前最强的一类 AI/ML 研究工程技能库之一，覆盖从 idea 到实验再到 paper 的全链路。 | [Orchestra-Research/AI-Research-SKILLs](https://github.com/Orchestra-Research/AI-Research-SKILLs) |
| Claude Scientific Skills | 科学计算超集 | 这轮补搜里最重要的新发现之一，覆盖 120+ 到 128+ 科学 skills，适合做实验室科学底座。 | [K-Dense-AI/claude-scientific-skills](https://github.com/K-Dense-AI/claude-scientific-skills) |
| Scientific Agent Skills | 跨学科科学技能库 | 覆盖 100+ 数据库、70+ Python 包、多个科学与工程学科，适合科研团队做“大底座”。 | [K-Dense-AI/scientific-agent-skills](https://github.com/K-Dense-AI/scientific-agent-skills) |
| Claude Scientific Writer | 写作与深研工具包 | 对论文、综述、基金、海报、同行评审、citation 管理特别强。 | [K-Dense-AI/claude-scientific-writer](https://github.com/K-Dense-AI/claude-scientific-writer) |
| Academic Research Skills | 学术研究流水线 | 更强调 `research -> write -> review -> revise -> finalize` 的完整多 agent 流程。 | [Imbad0202/academic-research-skills](https://github.com/Imbad0202/academic-research-skills) |
| Hugging Face Skills | AI/ML 官方技能包 | 数据集、训练、评测、发布和 Hub 操作都很实用。 | [huggingface/skills](https://github.com/huggingface/skills) |

## 2. 按科研任务拆开看

### 研究工程与实验执行

优先看：

- [科研工程与实验Skills](./科研工程与实验Skills.md)
- [Orchestra-Research/AI-Research-SKILLs](https://github.com/Orchestra-Research/AI-Research-SKILLs)
- [huggingface/skills](https://github.com/huggingface/skills)
- [microsoft/azure-skills](https://github.com/microsoft/azure-skills)

### 写作、文献、审稿与投稿

优先看：

- [科研写作与文献Skills](./科研写作与文献Skills.md)
- [K-Dense-AI/claude-scientific-writer](https://github.com/K-Dense-AI/claude-scientific-writer)
- [Imbad0202/academic-research-skills](https://github.com/Imbad0202/academic-research-skills)
- [CatVinci-Studio/paper-glance-skill](https://github.com/CatVinci-Studio/paper-glance-skill)

### 科学计算、学科数据库与领域分析

优先看：

- [科学计算与领域Skills](./科学计算与领域Skills.md)
- [K-Dense-AI/claude-scientific-skills](https://github.com/K-Dense-AI/claude-scientific-skills)
- [K-Dense-AI/scientific-agent-skills](https://github.com/K-Dense-AI/scientific-agent-skills)
- [HeshamFS/materials-simulation-skills](https://github.com/HeshamFS/materials-simulation-skills)
- [brunoasm/my_claude_skills](https://github.com/brunoasm/my_claude_skills)

### 发现平台与生态扫描

优先看：

- [跨平台宿主与官方技能库](./跨平台宿主与官方技能库.md)
- [Skill发现平台与精品合集](./Skill发现平台与精品合集.md)
- [skills.sh](https://skills.sh/)
- [VoltAgent/awesome-agent-skills](https://github.com/VoltAgent/awesome-agent-skills)
- [github/awesome-copilot](https://github.com/github/awesome-copilot)

## 3. 面向科研团队的最小 Skills 组合

对于希望尽快把 Skills 用起来的科研团队，可以先从这套组合开始：

1. 通用文档层：`anthropics/skills`
2. Codex 官方层：`openai/skills`
3. AI/ML 研究工程层：`AI-Research-SKILLs`
4. 科学数据库 / 学科分析层：`claude-scientific-skills` + `scientific-agent-skills`
5. 写作与评审层：`claude-scientific-writer`
6. 学术完整流程层：`academic-research-skills`

这几套叠起来，已经能覆盖大多数 AI 科研团队的第一版需求。

## 4. 设计自己的科研 Skill 时，建议固定五个槽位

1. 任务边界：这项 Skill 负责哪一步，不负责哪一步。
2. 触发条件：什么词、什么文件、什么上下文下应该触发。
3. 输入输出：要读哪些 artifact，要产出哪些 artifact。
4. 失败模式：最容易出错的地方是什么。
5. 验证动作：调用后必须检查哪些证据、引用、日志或中间结果。

相比把一整段提示词塞进去，这种结构更适合团队维护、版本化和评测。

## 5. 一个重要提醒

面向公开资源库的“尽可能全面”，并不意味着把所有技能都装上，而是：

1. 先把高信号技能仓库摸清楚
2. 再按研究方向做子集
3. 最后再把最常用的 skills 固化成自己的内部能力层

不然很容易变成“仓库看起来很大，但团队没人真的用”。
