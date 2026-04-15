# Deep Research与研究工作台

这一页聚焦“深度检索、证据汇总、长报告生成、研究计划可视化”这一类系统。它们通常不直接追求完整自动科研闭环，而是更强调信息获取、文献理解、来源追踪和研究工作台体验。

## 1. 代表性系统与项目

| 资源 | 定位 | 简述 | 链接 |
| --- | --- | --- | --- |
| Open Research | 研究工作台 | 强调 `research director in terminal`，覆盖 novelty check、source scout、paper explainer、reviewer response。 | [open-research.info](https://www.open-research.info/) |
| RTI | 文献工作流系统 | 把“方向输入 -> 检索 -> 筛选 -> 翻译 -> 深度分析”组织成完整链路。 | [yrc-better/RTI](https://github.com/yrc-better/RTI) |
| PaperQA2 | 科学文献问答 | 面向科学论文问答、证据引用与高精度引用式回答。 | [Future-House/paper-qa](https://github.com/Future-House/paper-qa) |
| STORM / Co-STORM | 知识策展与长报告 | 从检索、问题提出、提纲构建到带引用长文输出，适合 knowledge curation。 | [stanford-oval/storm](https://github.com/stanford-oval/storm) |
| Tongyi DeepResearch | 开源 deep research agent | 聚焦长时程信息搜寻、网页阅读、推理与搜索式深度研究。 | [Alibaba-NLP/DeepResearch](https://github.com/Alibaba-NLP/DeepResearch) |
| GPT Researcher | 自主 deep research | 支持 Web 与本地文档研究，输出长报告并带引用。 | [assafelovic/gpt-researcher](https://github.com/assafelovic/gpt-researcher) |
| ResearStudio | Human-intervenable deep research | 支持实时暂停、编辑、恢复计划，强调 plan-as-document 与人机协作。 | [ResearAI/ResearStudio](https://github.com/ResearAI/ResearStudio) |
| Jina DeepResearch | 迭代式深搜引擎 | 强调“搜索 -> 阅读 -> 推理 -> 再搜索”的迭代式答案发现。 | [jina-ai/node-DeepResearch](https://github.com/jina-ai/node-DeepResearch) |
| Deep Research | 轻量自部署 deep research app | 支持多模型、多搜索引擎、SSE API 与 MCP server。 | [u14app/deep-research](https://github.com/u14app/deep-research) |

## 2. 按能力拆开看

| 能力 | 更值得优先看的资源 | 说明 |
| --- | --- | --- |
| 文献与网页搜索 | `RTI`、`Tongyi DeepResearch`、`Jina DeepResearch`、`GPT Researcher` | 适合研究多轮检索、网页阅读和深搜策略。 |
| 证据式问答 | `PaperQA2`、`Open Research` | 适合构建引用可回查、回答可验证的 evidence QA 层。 |
| 提纲与长报告生成 | `STORM`、`GPT Researcher`、`ResearStudio` | 适合观察 outline-first、citation-first、report-first 的不同策略。 |
| 人机协作式工作台 | `ResearStudio`、`Co-STORM`、`Open Research` | 适合研究 plan editing、实时介入和 shared workspace。 |
| 自部署与接口化 | `Deep Research`、`Jina DeepResearch`、`GPT Researcher` | 更适合作为团队内部工作台或服务层基础。 |

## 3. 这些系统常见的核心设计

| 设计点 | 说明 |
| --- | --- |
| 多轮检索而不是单轮搜索 | 先 broad search，再 narrow search，再定向补证据，通常比一次性检索更稳。 |
| 引用优先 | 好的研究工作台通常把文献、网页、引用段落和证据卡片放在核心位置。 |
| 计划显式化 | `plan / outline / question tree / search trace` 可以被展示、编辑、恢复和复盘。 |
| 长文输出不是终点 | 报告常常只是中间产物，后面还需要 novelty 审计、实验计划和写作迁移。 |
| 本地文档与互联网并用 | 很多系统已经从“纯 Web 搜索”转向“Web + 本地文件 + 知识库”联合研究。 |

## 4. 适合放在科研工作流的哪一层

| 模块 | 更适合接入的系统 |
| --- | --- |
| 研究总控台 | `Open Research`、`ResearStudio` |
| 文献扫描与初筛 | `RTI`、`Tongyi DeepResearch`、`Jina DeepResearch` |
| 单篇论文问答 | `PaperQA2` |
| 知识策展与长报告 | `STORM`、`GPT Researcher` |
| 私有化 / 自部署工作台 | `GPT Researcher`、`Deep Research` |

## 5. 与 MCP / Skills 的连接方式

这类系统通常和以下资源形成自然互补：

- [MCP标准与发现平台](../92-MCP/MCP标准与发现平台.md)
- [文献检索与知识库MCP](../92-MCP/文献检索与知识库MCP.md)
- [科研写作与文献Skills](../91-Skills/科研写作与文献Skills.md)
- [文献检索与阅读](../95-文献检索与知识管理/文献检索与阅读.md)

## 6. 相关页面

- [科研Agent系统](./科研Agent系统.md)
- [自动科研与闭环系统](./自动科研与闭环系统.md)
- [科研工作流设计模式](./科研工作流设计模式.md)
