# 科研新颖性与 Idea 生成

这一页专门补“新颖性判断、idea 生成、peer-review 结构化分析”这一条线。它关系到科研系统能否从“会检索”进一步走向“会发现空白、会判断 novelty、会辅助构思研究问题”。

## 1. 直接相关的 novelty / idea 资源

| 资源 | 类型 | 简述 | 链接 |
| --- | --- | --- | --- |
| NovBench / llm4novelty | novelty benchmark | 围绕学术论文 novelty assessment 构建数据与代码，适合直接做“新颖性判断”基线。 | [njust-winchy/llm4novelty](https://github.com/njust-winchy/llm4novelty) |
| AI Co-Scientist | 科研 idea 生成系统 | Google Research 的公开项目页面，核心价值是把 idea generation、reflection、ranking、evidence retrieval 串成一个科学假设生成闭环。 | [Google Research Blog](https://research.google/blog/accelerating-scientific-breakthroughs-with-an-ai-co-scientist/) |
| Can LLMs Generate Novel Research Ideas? | 人类对照研究 | 这篇工作很适合做“LLM 生成研究 idea 到底行不行”的参考起点，强调和人类研究者 head-to-head 比较。 | [OpenReview](https://openreview.net/forum?id=M23dTGWCZy) |
| HypoGeniC | hypothesis generation | Chicago HAI 的 hypothesis generation 项目，强调“从数据中提出可迁移假设，再做 OOD 验证”，很适合借鉴 idea discovery 的程序化流程。 | [项目页](https://chicagohai.github.io/hypogenic-demo/) |
| Hypothesis-Generation Repo | 开源实现 | HypoGeniC 对应的代码入口，更适合直接看实现细节。 | [ChicagoHAI/hypothesis-generation](https://github.com/ChicagoHAI/hypothesis-generation) |
| ResearchAgent | idea + review agents | 把 idea 生成和 reviewing agents 结合起来，适合作为“先出想法、再做自我审稿”的多 agent 参考。 | [ACL Anthology](https://aclanthology.org/2025.naacl-long.342/) |
| VirSci | 多 Agent idea 系统 | 强调多个 agent 生成、批判、修正 research ideas，适合参考“idea 多样性”和“内部辩论”机制。 | [ACL Anthology](https://aclanthology.org/2025.acl-long.1368/) |
| Dolphin | 闭环科研框架 | 把 `Thinking -> Practice -> Feedback` 明确写成闭环，更适合借鉴从 idea 到实验反馈的状态机。 | [ACL Anthology](https://aclanthology.org/2025.acl-long.1056/) |
| AI Scientist | 自动科研系统 | 公开提供从 idea 到 review 的端到端自动科研代码与实验。 | [SakanaAI/AI-Scientist](https://github.com/SakanaAI/AI-Scientist) |
| AI Scientist-v2 | 自动科研系统 | 第二代版本更强调 open-ended ideation、agentic tree search 与 workshop-level paper generation。 | [SakanaAI/AI-Scientist-v2](https://github.com/SakanaAI/AI-Scientist-v2) |
| SciAgents | multi-agent scientific discovery | 利用知识图谱和多 agent 推进科学发现，适合和 novelty / idea generation 结合阅读。 | [lamm-mit/SciAgentsDiscovery](https://github.com/lamm-mit/SciAgentsDiscovery) |

## 2. novelty 评测和审稿数据相关资源

| 资源 | 类型 | 简述 | 链接 |
| --- | --- | --- | --- |
| ReviewAdvisor | scientific review 数据与方法 | 早期很重要的“自动 scientific reviewing”资源，`llm4novelty` 也明确引用了它。 | [neulab/ReviewAdvisor](https://github.com/neulab/ReviewAdvisor) |
| NLPeer | peer review 数据资源 | 统一了多会议、多来源 peer review 研究数据，是做 review mining、novelty sentence identification 的基础资源。 | [UKPLab/nlpeer](https://github.com/UKPLab/nlpeer) |
| Identifying Aspects in Peer Reviews | review aspect 数据 | 对 peer review 中的具体 aspect 做结构化识别，适合扩展 novelty / weakness / significance 等维度。 | [UKPLab/emnlp2025-aspects-in-reviews](https://github.com/UKPLab/emnlp2025-aspects-in-reviews) |
| PeerRead | peer review 数据集 | 最经典的公开 peer review 数据之一，适合做基础建模和历史对照。 | [allenai/PeerRead](https://github.com/allenai/PeerRead) |
| PeerQA | reviewer QA 数据集 | 问题来自 reviewer、答案来自作者，适合做 reviewer question 的证据核验。 | [UKPLab/PeerQA](https://github.com/UKPLab/PeerQA) |
| PeerSum | meta-review 数据集 | 适合从多个 review 生成元审摘要。 | [oaimli/PeerSum](https://huggingface.co/datasets/oaimli/PeerSum) |
| HedgePeer | review uncertainty 数据集 | 适合分析 hedge、uncertainty 和 reviewer confidence。 | [Tirthankar-Ghosal/HedgePeer-Dataset](https://github.com/Tirthankar-Ghosal/HedgePeer-Dataset) |
| AgentReview | LLM 审稿模拟 | 从多 agent 视角分析 peer review dynamics。 | [ahren09/agentreview](https://github.com/ahren09/agentreview) |
| MARG | 多 agent review generation | 适合做 automated reviewing、alignment 评估和 demo。 | [allenai/marg-reviewer](https://github.com/allenai/marg-reviewer) |
| ReviewRobot | explainable review generation | 适合关注 explainable scientific reviewing。 | [EagleW/ReviewRobot](https://github.com/EagleW/ReviewRobot) |
| AI Peer Review | 多模型元审工具 | 可生成独立评审、meta-review 和 concerns table。 | [poldrack/ai-peer-review](https://github.com/poldrack/ai-peer-review) |
| OpenReview | 审稿平台与数据入口 | 很多 AI 顶会的审稿、讨论、版本演化都能从这里拿到公开数据。 | [OpenReview](https://openreview.net/) |
| OpenReview MCP | MCP 接入层 | 若需要把 novelty 判断接入 agent 工作流，MCP 接 OpenReview 是最直接的一层。 | [openreview/openreview-mcp](https://github.com/openreview/openreview-mcp) |
| NLP for Peer Review | 数据集汇总 | 专门汇总 peer review 数据和任务，是补 benchmark 的高价值入口。 | [OAfzal/nlp-for-peer-review](https://github.com/OAfzal/nlp-for-peer-review) |

## 3. 做 novelty 这一类任务时，最值得优先接的公共数据层

| 数据层 | 为什么重要 | 资源 |
| --- | --- | --- |
| 顶会审稿文本 | 可以直接观察审稿人如何表达 novelty / significance / weakness | [OpenReview](https://openreview.net/)、[NLPeer](https://github.com/UKPLab/nlpeer) |
| 论文引文与图谱 | novelty 不只是“新”，还要知道相对既有工作差在哪 | [OpenAlex](https://openalex.org/)、[Semantic Scholar API](https://www.semanticscholar.org/product/api) |
| 论文全文与结构化文本 | novelty 常常在 introduction / related work / contributions 中显式出现 | [GROBID](https://github.com/kermitt2/grobid)、[Marker](https://github.com/VikParuchuri/marker)、[Docling](https://github.com/docling-project/docling) |
| 最新论文流 | novelty 需要跟最新工作比较，不能只看静态语料 | [paper-search-mcp](https://github.com/openags/paper-search-mcp)、[OpenReview MCP](https://github.com/openreview/openreview-mcp)、[OpenAlex MCP](https://github.com/hbiaou/openalex-mcp) |
| claim verification 数据集 | novelty 论断常常需要回到“证据是否支持 claim”这一层 | [SciFact](https://github.com/allenai/scifact)、[SciFact-Open](https://github.com/dwadden/scifact-open)、[MSVEC](https://github.com/lamps-lab/msvec) |
| systematic review 数据集 | 当目标是系统综述和证据综合时，需要更高量的筛选与 study selection 语料 | [ASReview](https://github.com/asreview/asreview)、[SYNERGY Dataset](https://github.com/asreview/synergy-dataset) |

## 4. 最有价值的落地方向

### 方向 A：做“novelty 审计员”

适合的组合：

1. `openreview-mcp + openalex-mcp + paper-search-mcp`
2. `llm4novelty / ReviewAdvisor / NLPeer`
3. `PaperQA2`

这样可以把系统做成：

- 先找最新和相近工作
- 再抽取论文自述贡献
- 再参考 reviewer 风格写出“novelty claim 是否站得住”的结构化意见

### 方向 B：做“idea 生成 + 自审闭环”

适合的组合：

1. `AI Co-Scientist`
2. `HypoGeniC`
3. `ResearchAgent / VirSci`

这样比较适合做：

- 问题空间扫描
- idea draft 生成
- novelty / feasibility / evidence 三维排序
- reviewer-style critique

### 方向 C：做“review mining + benchmark 基线”

适合的组合：

1. `NovBench / llm4novelty`
2. `PeerRead / NLPeer / PeerQA / PeerSum`
3. `ReviewAdvisor / AgentReview / MARG / AI Peer Review`

这样比较适合做：

- novelty text 评估
- reviewer question 与 evidence retrieval
- meta-review 生成
- reviewer-style benchmark 对照

## 5. 优先补齐的三个能力

1. `Novelty Retrieval`
   把“相似论文检索、时间线追踪、贡献句抽取、citation neighborhood”打通。
2. `Novelty Judging`
   用 `NovBench + NLPeer + OpenReview` 做一个内部评测集，别只靠主观感觉。
3. `Idea Diversification`
   借鉴 `HypoGeniC / VirSci / ResearchAgent`，不要只让模型给一个想法，而是同时给多个路线并排序。

## 6. 一个很现实的提醒

“新颖性”不是只看语义差异。真正可靠的 novelty 系统至少要同时看四层：

1. 和已有工作的语义相似度
2. 方法机制是否真的不同
3. 适用场景或研究问题是否有扩展
4. 证据是否足以支持这种“新”

这也是为什么 `llm4novelty` 这类资源特别有价值，它把 novelty 从模糊印象往“可评测任务”上推了一步。
