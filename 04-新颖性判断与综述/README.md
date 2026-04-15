# 新颖性判断与综述

这一模块聚焦 novelty 判断、peer-review 结构化分析、系统综述、证据综合与研究空白识别。适合在“是否继续做这个题”以及“怎样把相关工作讲清楚”这两个阶段使用。

## 这一步通常要回答的问题

1. 一个候选问题究竟是“有意思”，还是“在现有文献里已经相当拥挤”。
2. 一组论文之间真正的差异点、争议点和空白点是什么。
3. 哪些 reviewer-style critique 会最先挑战这个想法。
4. 系统综述、evidence synthesis 和 novelty check 应该怎样形成清晰结论。

## 推荐先看

- [新颖性判断、综述与评审工具详表](./新颖性判断、综述与评审工具详表.md)
- [新颖性、同行评审数据集与Benchmark](./新颖性、同行评审数据集与Benchmark.md)
- [08-方向专题/科研新颖性与Idea生成](../08-方向专题/科研新颖性与Idea生成.md)
- [94-Prompt与写作/系统综述与证据综合](../94-Prompt与写作/系统综述与证据综合.md)
- [01-课题扫描与选题](../01-课题扫描与选题/README.md)

## 最小工具栈

1. `Paper Search MCP + OpenAlex MCP + OpenReview MCP`
   适合先搭建 broad search、landscape 和 reviewer 语境。
2. `paper-glance-skill + literature-review + scientific-critical-thinking`
   适合把核心论文拆成统一结构，并快速拉出差异点和逻辑链。
3. `llm4novelty / NovBench + ReviewAdvisor + NLPeer`
   适合做 novelty 判断、review mining 和 reviewer-style critique。
4. `SciFact / PeerQA / SciDQA + scite`
   适合继续做 claim 证据核验、review question answering 和引用语境判断。

## 高频公开资源

| 资源 | 类型 | 更适合的用途 | 链接 |
| --- | --- | --- | --- |
| llm4novelty / NovBench | novelty benchmark | 学术论文新颖性评估、novelty ranking 与基线比较。 | [njust-winchy/llm4novelty](https://github.com/njust-winchy/llm4novelty) |
| OpenReview | 开放评审平台 | 追 review、rebuttal、discussion 和 reviewer 语境。 | [OpenReview](https://openreview.net/) |
| PeerRead / PeerQA / PeerSum | peer review 数据集 | 适合做 review mining、question answering 和 meta-review 任务。 | [allenai/PeerRead](https://github.com/allenai/PeerRead)、[UKPLab/PeerQA](https://github.com/UKPLab/PeerQA)、[oaimli/PeerSum](https://huggingface.co/datasets/oaimli/PeerSum) |
| ReviewAdvisor / NLPeer | 审稿分析工具与语料 | 适合 reviewer concern 抽取、review style 分析和 critique 建模。 | [neulab/ReviewAdvisor](https://github.com/neulab/ReviewAdvisor)、[UKPLab/nlpeer](https://github.com/UKPLab/nlpeer) |
| SciFact / SciDQA | 科学证据核验与 reviewer QA | 适合做 claim verification、review-style question answering 和证据核查。 | [allenai/scifact](https://github.com/allenai/scifact)、[yale-nlp/SciDQA](https://github.com/yale-nlp/SciDQA) |
| ASReview / SYNERGY Dataset | systematic review 工具与数据集 | 适合做高量文献筛选、study selection 和 active review。 | [asreview/asreview](https://github.com/asreview/asreview)、[asreview/synergy-dataset](https://github.com/asreview/synergy-dataset) |
| scite / Elicit / Consensus | 引用语境与 evidence synthesis | 适合看 citation context、形成 evidence map 和快速综述。 | [scite](https://scite.ai/)、[Elicit](https://elicit.com/)、[Consensus](https://consensus.app/) |

## 一、相关 Skills

| 资源 | 类型 | 适合环节 | 简述 | 链接 |
| --- | --- | --- | --- | --- |
| 科研写作与文献Skills | 仓库内附录 | 总览 | 当前仓库里综述、审稿、批判阅读与写作相关 Skills 的主归属页。 | [91-Skills/科研写作与文献Skills](../91-Skills/科研写作与文献Skills.md) |
| `literature-review` | 子技能 | 相关工作归并 | 适合把多篇论文归并成方法脉络、差异点和综述提纲。 | [K-Dense-AI/claude-scientific-writer](https://github.com/K-Dense-AI/claude-scientific-writer) |
| `peer-review` | 子技能 | reviewer-style critique | 适合生成结构化评审意见和主要质疑点。 | [K-Dense-AI/claude-scientific-writer](https://github.com/K-Dense-AI/claude-scientific-writer) |
| `scientific-critical-thinking` | 子技能 | 论证拆解 | 适合聚焦逻辑链、证据充分性和结论外推边界。 | [K-Dense-AI/claude-scientific-writer](https://github.com/K-Dense-AI/claude-scientific-writer) |
| `hypothesis-generation` | 子技能 | 候选假设扩展 | 适合在 novelty 判断后继续扩展替代假设和变体路线。 | [K-Dense-AI/claude-scientific-writer](https://github.com/K-Dense-AI/claude-scientific-writer) |
| `research-lookup` | 子技能 | 事实回查 | 适合对 reviewer concern 继续补文献、补出处、补近作。 | [K-Dense-AI/claude-scientific-writer](https://github.com/K-Dense-AI/claude-scientific-writer) |
| `academic-paper-reviewer` | 子技能 | 审稿模拟 | 适合用 rubric、多角色 reviewer 与主编视角做系统性检查。 | [Imbad0202/academic-research-skills](https://github.com/Imbad0202/academic-research-skills) |
| `deep-research` | 子技能 | 系统综述 | 适合做长链检索、证据归并和 question refinement。 | [Imbad0202/academic-research-skills](https://github.com/Imbad0202/academic-research-skills) |
| `academic-pipeline` | 子技能 | 结果沉淀 | 适合把检索、评审、修订和写作输出串成统一流程。 | [Imbad0202/academic-research-skills](https://github.com/Imbad0202/academic-research-skills) |
| paper-glance-skill | 单篇精读技能 | 对比阅读 | 适合在 novelty 判断前把核心论文拆成统一结构。 | [CatVinci-Studio/paper-glance-skill](https://github.com/CatVinci-Studio/paper-glance-skill) |
| NotebookLM Skill | 知识库技能 | 主题资料复查 | 适合把已有论文池、proposal 和项目笔记放进同一问答入口。 | [PleasePrompto/notebooklm-skill](https://github.com/PleasePrompto/notebooklm-skill) |

## 二、相关 MCP

| 资源 | 类型 | 适合环节 | 简述 | 链接 |
| --- | --- | --- | --- | --- |
| 文献检索与知识库MCP | 仓库内附录 | MCP 总览 | 当前仓库里文献检索、图谱分析和评审平台相关 MCP 的主归属页。 | [92-MCP/文献检索与知识库MCP](../92-MCP/文献检索与知识库MCP.md) |
| OpenReview MCP | 投稿与评审 MCP | reviewer 语境 | 适合追踪 review、rebuttal、顶会热点和审稿脉络。 | [openreview/openreview-mcp](https://github.com/openreview/openreview-mcp) |
| OpenAlex MCP | 学术图谱 MCP | research landscape | 适合做作者、主题、机构和引文网络分析。 | [hbiaou/openalex-mcp](https://github.com/hbiaou/openalex-mcp) |
| OpenAlex Research MCP | landscape MCP | gap analysis | 更适合做 trend analysis、citation analysis 和 research landscaping。 | [oksure/openalex-research-mcp](https://github.com/oksure/openalex-research-mcp) |
| Paper Search MCP | 学术检索 MCP | broad search | 适合补跨平台检索和相关工作池。 | [openags/paper-search-mcp](https://github.com/openags/paper-search-mcp) |
| Semantic Scholar MCP | 引文网络 MCP | 作者与影响路径 | 适合对 candidate papers 继续扩展作者和引用关系。 | [zongmin-yu/semantic-scholar-fastmcp-mcp-server](https://github.com/zongmin-yu/semantic-scholar-fastmcp-mcp-server) |
| Crossref MCP | 元数据 MCP | DOI 与出版核验 | 适合校正正式出版状态、DOI 和元数据。 | [botanicastudios/crossref-mcp](https://github.com/botanicastudios/crossref-mcp) |
| arXiv LaTeX MCP | LaTeX 源码 MCP | 公式与附录核对 | 适合深查表格、伪代码、附录和方法细节。 | [takashiishida/arxiv-latex-mcp](https://github.com/takashiishida/arxiv-latex-mcp) |
| GitHub MCP Server | 代码与项目 MCP | 代码配套核验 | 适合核对论文配套仓库、Issue、PR、release 和复现说明。 | [github/github-mcp-server](https://github.com/github/github-mcp-server) |
| GitMCP | 文档型远程 MCP | 仓库文档回查 | 适合快速查公共 GitHub 仓库文档、README 和代码入口。 | [idosal/git-mcp](https://github.com/idosal/git-mcp) |
| Exa MCP Server | 搜索增强 MCP | 外部资料补充 | 适合补项目页、新闻稿、技术博客和非论文型证据。 | [exa-labs/exa-mcp-server](https://github.com/exa-labs/exa-mcp-server) |
| Tavily MCP | 搜索增强 MCP | 开放网页检索 | 适合对最新材料做二次补检。 | [tavily-ai/tavily-mcp](https://github.com/tavily-ai/tavily-mcp) |
| Zotero MCP | 文献库 MCP | 证据池沉淀 | 适合把 reviewer concern 和证据条目回存到文献库。 | [54yyyu/zotero-mcp](https://github.com/54yyyu/zotero-mcp) |

## 三、相关 Agent、评审系统与公开工具

| 资源 | 类型 | 适合环节 | 简述 | 链接 |
| --- | --- | --- | --- | --- |
| 科研新颖性与Idea生成 | 仓库内专题 | 专题总览 | 当前仓库里 novelty、idea generation 和 review mining 的主归属页。 | [08-方向专题/科研新颖性与Idea生成](../08-方向专题/科研新颖性与Idea生成.md) |
| 系统综述与证据综合 | 仓库内附录 | 综述工具总览 | 当前仓库里系统综述与 evidence synthesis 的主归属页。 | [94-Prompt与写作/系统综述与证据综合](../94-Prompt与写作/系统综述与证据综合.md) |
| llm4novelty / NovBench | novelty benchmark | novelty 评估 | 这是当前最应该优先看的 novelty 专题资源之一，聚焦“学术论文新颖性评估”本身。 | [njust-winchy/llm4novelty](https://github.com/njust-winchy/llm4novelty) |
| ReviewAdvisor | 审稿分析工具 | review mining | 适合抽取和分析审稿意见、关注点与反馈模式。 | [neulab/ReviewAdvisor](https://github.com/neulab/ReviewAdvisor) |
| NLPeer | 审稿数据与代码 | peer review 研究 | 统一了多会议、多期刊 peer review 数据，是 review mining 的核心底座之一。 | [UKPLab/nlpeer](https://github.com/UKPLab/nlpeer) |
| AgentReview | LLM agent 审稿模拟 | peer review dynamics | 适合从多 agent 角度模拟 peer review 动态。 | [ahren09/agentreview](https://github.com/ahren09/agentreview) |
| MARG | 多 agent review generation | review generation | 适合研究多 agent reviewer 架构、对齐评估与演示系统。 | [allenai/marg-reviewer](https://github.com/allenai/marg-reviewer) |
| ReviewRobot | explainable review generation | review generation | 适合关注基于知识合成的 explainable 评审生成。 | [EagleW/ReviewRobot](https://github.com/EagleW/ReviewRobot) |
| AI Peer Review | AI 辅助元审 | meta-review | 适合生成多模型评审、concerns table 和 meta-review。 | [poldrack/ai-peer-review](https://github.com/poldrack/ai-peer-review) |
| OpenReview Expertise | reviewer matching | 专家匹配 | 适合理解 reviewer-paper affinity 和专家匹配建模。 | [openreview/openreview-expertise](https://github.com/openreview/openreview-expertise) |
| OpenReview Matcher | reviewer assignment | 指派优化 | 适合理解 paper-reviewer matching 的约束优化。 | [openreview/openreview-matcher](https://github.com/openreview/openreview-matcher) |
| HypoGeniC / HypoRefine | 假设生成框架 | hypothesis generation | 适合围绕数据与文献生成候选假设。 | [ChicagoHAI/hypothesis-generation](https://github.com/ChicagoHAI/hypothesis-generation) |
| AI Scientist / AI Scientist-v2 | 自动科研系统 | ideation 与自审 | 两代系统都包含 idea generation、paper review 或 `review_iclr_bench` 相关流程。 | [SakanaAI/AI-Scientist](https://github.com/SakanaAI/AI-Scientist) |

## 四、相关数据集、Benchmark 与平台

| 资源 | 类型 | 适合环节 | 简述 | 链接 |
| --- | --- | --- | --- | --- |
| 新颖性、同行评审数据集与Benchmark | 仓库内详表 | Benchmark 总览 | 当前仓库里 novelty、peer review、claim verification 和 systematic review benchmark 的主归属页。 | [新颖性、同行评审数据集与Benchmark](./新颖性、同行评审数据集与Benchmark.md) |
| PeerRead | 审稿数据集 | review 数据建模 | 最经典的 peer review 数据集之一，含论文草稿、决定与评论。 | [allenai/PeerRead](https://github.com/allenai/PeerRead) |
| PeerQA | peer review QA 数据集 | 证据问答 | 问题来自 reviewer，答案来自作者，适合 evidence retrieval 和 answerability 评测。 | [UKPLab/PeerQA](https://github.com/UKPLab/PeerQA) |
| PeerSum | meta-review 数据集 | 元审摘要 | 适合做多评审到 meta-review 的汇总生成评测。 | [oaimli/PeerSum](https://huggingface.co/datasets/oaimli/PeerSum) |
| HedgePeer | 审稿不确定性数据集 | review quality 分析 | 适合研究 hedge、uncertainty 与 reviewer confidence。 | [Tirthankar-Ghosal/HedgePeer-Dataset](https://github.com/Tirthankar-Ghosal/HedgePeer-Dataset) |
| SciDQA | 科学论文深度问答 | reviewer questions | 问题来自 peer review，强调表格、图、附录和多文档推理。 | [yale-nlp/SciDQA](https://github.com/yale-nlp/SciDQA) |
| SciFact / SciFact-Open | 科学 claim verification | 证据核验 | 适合把 novelty 论断或论文 claim 放到证据支持/反驳任务中检验。 | [allenai/scifact](https://github.com/allenai/scifact) |
| Valsci | scientific claim verification tool | 批量证据核验 | 面向大批量 scientific claim verification 和 report 生成。 | [bricee98/Valsci](https://github.com/bricee98/Valsci) |
| MSVEC | scientific claim verification eval | 跨领域鲁棒性 | 适合测试 scientific claim verification 的跨领域泛化。 | [lamps-lab/msvec](https://github.com/lamps-lab/msvec) |
| ASReview | systematic review 工具 | active screening | 适合高量文献筛选、systematic review 和交互式 study selection。 | [asreview/asreview](https://github.com/asreview/asreview) |
| SYNERGY Dataset | systematic review 数据集 | 稀疏标签检索 | 适合做 systematic review study selection 和 IR/active learning。 | [asreview/synergy-dataset](https://github.com/asreview/synergy-dataset) |
| OpenReview | 开放评审平台 | review 语料 | 适合研究 review、rebuttal 和顶会讨论。 | [OpenReview](https://openreview.net/) |
| OpenAlex | 开放学术图谱 | landscape | 适合做 topic、venue、author、citation 级分析。 | [OpenAlex](https://openalex.org/) |
| scite | 引用语境平台 | 证据与争议 | 适合判断论文是被支持、被提及还是被质疑。 | [scite](https://scite.ai/) |
| Elicit / Consensus | evidence synthesis 平台 | 证据综合 | 适合从问题出发快速形成 evidence map。 | [Elicit](https://elicit.com/) |

## 五、外部整合入口

| 资源 | 类型 | 适合用途 | 简述 | 链接 |
| --- | --- | --- | --- | --- |
| AI-4-Research | 大型综述站点 | peer review / benchmark 扫库 | 对 AI for peer review、自动科研、AAAR 类资源的汇总很密。 | [AI-4-Research/AI-4-Research.github.io](https://github.com/AI-4-Research/AI-4-Research.github.io) |
| LLM4SR | survey 资源库 | benchmark 扫库 | 对 peer review、meta-review、scientific writing、ideation 的 benchmark 整理很系统。 | [du-nlp-lab/LLM4SR](https://github.com/du-nlp-lab/LLM4SR) |
| Transforming Science with LLMs | survey 资源库 | peer review / claim verification | 对 idea generation、peer review、scientific rigor 和 claim verification 的条目很全。 | [NL2G/TransformingScienceLLMs](https://github.com/NL2G/TransformingScienceLLMs) |
| NLP for Peer Review | 数据集汇总 | peer review datasets | 专门汇总 peer review 相关公开数据和任务，是补 benchmark 的高价值入口。 | [OAfzal/nlp-for-peer-review](https://github.com/OAfzal/nlp-for-peer-review) |
| Awesome Scholarly Data Analysis | scholarly data 合集 | bibliometrics / peer review | 对学术图谱、引文、peer review 数据和分析工具整理很全。 | [napsternxg/awesome-scholarly-data-analysis](https://github.com/napsternxg/awesome-scholarly-data-analysis) |
| research-automation-papers | 自动科研论文清单 | 审稿与 novelty 线索 | 对 peer review、novelty、claim verification、review generation 的论文线索密度很高。 | [t46/research-automation-papers](https://github.com/t46/research-automation-papers) |
| Awesome LLM Scientific Discovery | 科学发现合集 | broad scan | 适合继续补 scientific discovery、co-scientist 和自动科研资源。 | [HKUST-KnowComp/Awesome-LLM-Scientific-Discovery](https://github.com/HKUST-KnowComp/Awesome-LLM-Scientific-Discovery) |
| 外部导航与合集 | 仓库内索引 | 继续扫库 | 当前仓库里的外部公开合集总入口。 | [98-全局索引/外部导航与合集](../98-全局索引/外部导航与合集.md) |

## 六、推荐组合

1. `openreview-mcp + openalex-mcp + paper-search-mcp`
   适合做 broad search、review 追踪和 landscape 分析。
2. `llm4novelty / NovBench + ReviewAdvisor + NLPeer + PeerRead`
   适合做 novelty 判断、review mining 和历史基线对照。
3. `PeerQA / SciDQA + PaperQA2 + scite`
   适合做 reviewer question、claim 证据和细粒度问答核验。
4. `SciFact / SciFact-Open + Valsci + MSVEC`
   适合做科学 claim verification 与跨领域鲁棒性评测。
5. `ASReview + SYNERGY Dataset + Elicit / Consensus`
   适合做 systematic review、study selection 和 evidence synthesis。
6. `MARG / AgentReview / AI Peer Review / AI Scientist`
   适合做 automated reviewing、meta-review 和 reviewer-style critique 实验。
7. `HypoGeniC / HypoSpace + AI Scientist-v2`
   适合做假设生成与 hypothesis evaluation 视角的探索。
8. `Elicit / Consensus / scite / PaperQA2`
   适合做 evidence synthesis、citation context 和证据核验。

## 七、仓库内延伸阅读

- [01-课题扫描与选题](../01-课题扫描与选题/README.md)
- [02-文献检索与单篇精读](../02-文献检索与单篇精读/README.md)
- [06-写作、审稿与投稿](../06-写作、审稿与投稿/README.md)
