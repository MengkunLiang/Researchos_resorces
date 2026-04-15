# 新颖性、同行评审数据集与 Benchmark

这一页专门补足 `04-新颖性判断与综述` 的数据层、评测层和公开资料层。重点不只是列论文，而是把“真正能拿来做 benchmark、复现、对照和方法设计”的公开资源集中起来。

## 一、直接面向 novelty 判断与 idea evaluation 的资源

| 资源 | 类型 | 核心价值 | 链接 |
| --- | --- | --- | --- |
| NovBench / llm4novelty | novelty benchmark | 直接围绕 academic paper novelty assessment 构建数据与评测代码，是当前最应该优先看的 novelty 资源之一。 | [njust-winchy/llm4novelty](https://github.com/njust-winchy/llm4novelty) |
| HypoSpace | 假设生成评测 | 面向多假设、开放式 hypothesis generation 的评测资源。 | [CTT-Pavilion/_HypoSpace](https://github.com/CTT-Pavilion/_HypoSpace) |
| VirSci | 科研能力评测与模拟 | 从 multi-agent scientific collaboration 和 idea generation 视角做评测。 | [open-sciencelab/Virtual-Scientists](https://github.com/open-sciencelab/Virtual-Scientists) |
| SciEval | 科学研究能力评测 | 适合从 scientific knowledge、application、calculation 和 research ability 多层面评估模型。 | [OpenDFM/SciEval](https://github.com/OpenDFM/SciEval) |
| SciCode | scientific coding benchmark | 适合测试模型在科学问题编码、实验实现和研究编程上的能力。 | [scicode-bench/SciCode](https://github.com/scicode-bench/SciCode) |
| AI Scientist review bench | 自动审稿评测 | `AI-Scientist` 与 `AI-Scientist-v2` 仓库内均包含 review 相关流程与 `review_iclr_bench` 分析入口。 | [SakanaAI/AI-Scientist](https://github.com/SakanaAI/AI-Scientist) |

## 二、同行评审与 meta-review 的核心公开数据集

| 资源 | 类型 | 核心价值 | 链接 |
| --- | --- | --- | --- |
| PeerRead | peer review 数据集 | 最经典的公开 peer review 数据集之一，包含论文草稿、决定与审稿文本。 | [allenai/PeerRead](https://github.com/allenai/PeerRead) |
| NLPeer | 统一 peer review 资源 | 汇聚多会议、多期刊、多年份 peer review 数据，是 review mining 的主底座之一。 | [UKPLab/nlpeer](https://github.com/UKPLab/nlpeer) |
| PeerQA | peer review QA 数据集 | 问题来自 reviewer、答案来自作者，适合 evidence retrieval、answerability 和 answer generation。 | [UKPLab/PeerQA](https://github.com/UKPLab/PeerQA) |
| PeerSum | meta-review 数据集 | 适合做多评审到元审的汇总生成评测。 | [oaimli/PeerSum](https://huggingface.co/datasets/oaimli/PeerSum) |
| HedgePeer | 审稿不确定性数据集 | 适合分析 hedge、uncertainty 与 reviewer confidence。 | [Tirthankar-Ghosal/HedgePeer-Dataset](https://github.com/Tirthankar-Ghosal/HedgePeer-Dataset) |
| SciDQA | scientific paper deep QA | 问题来自 peer review，强调图表、附录、方程和长文档推理。 | [yale-nlp/SciDQA](https://github.com/yale-nlp/SciDQA) |
| ReviewAdvisor | 审稿分析资源 | 是很多自动 reviewing / novelty 研究引用的重要早期资源。 | [neulab/ReviewAdvisor](https://github.com/neulab/ReviewAdvisor) |
| ICLR 2023 OpenReview Data | OpenReview 爬取与可视化 | 适合直接抓取和分析 ICLR OpenReview 数据。 | [fedebotu/ICLR2023-OpenReviewData](https://github.com/fedebotu/ICLR2023-OpenReviewData) |
| Openreview 中文 | 中文分析资源 | 基于 ICLR OpenReview 数据的中文分析仓库，适合做本地探索和可视化。 | [Seafoodair/Openreview](https://github.com/Seafoodair/Openreview) |

## 三、审稿生成、审稿模拟与 reviewer-style critique 系统

| 资源 | 类型 | 核心价值 | 链接 |
| --- | --- | --- | --- |
| AgentReview | 多 agent peer review 模拟 | 适合研究 peer review 动态、偏差与潜在因素。 | [ahren09/agentreview](https://github.com/ahren09/agentreview) |
| MARG | multi-agent review generation | 适合做科学论文多 agent 审稿生成、对齐评估和 demo 系统。 | [allenai/marg-reviewer](https://github.com/allenai/marg-reviewer) |
| ReviewRobot | explainable review generation | 适合关注知识合成驱动的 explainable review generation。 | [EagleW/ReviewRobot](https://github.com/EagleW/ReviewRobot) |
| AI Peer Review | 多模型元审工具 | 支持独立评审、meta-review、concerns table 和结果导出。 | [poldrack/ai-peer-review](https://github.com/poldrack/ai-peer-review) |
| Paper Reviewer | 论文自动 review 与 blog 化 | 适合把 arXiv / OpenReview 论文转成 review 和博客化总结。 | [deep-diver/paper-reviewer](https://github.com/deep-diver/paper-reviewer) |
| PiCO / Peer Review in LLMs | consistency optimization | 适合关注 LLM 互评、judge consistency 和自动评审优化。 | [PKU-YuanGroup/PiCO](https://github.com/PKU-YuanGroup/PiCO) |

## 四、claim verification、evidence synthesis 与 systematic review 相关数据层

| 资源 | 类型 | 核心价值 | 链接 |
| --- | --- | --- | --- |
| SciFact | scientific claim verification | 最经典的 scientific claim verification 公开资源之一。 | [allenai/scifact](https://github.com/allenai/scifact) |
| SciFact-Open | open-domain scientific claim verification | 适合从封闭语料走向 open-domain claim verification。 | [dwadden/scifact-open](https://github.com/dwadden/scifact-open) |
| Scientific Claim Generation | claim generation | 适合把 citation context 生成可验证 scientific claims。 | [allenai/scientific-claim-generation](https://github.com/allenai/scientific-claim-generation) |
| Valsci | 大批量 scientific claim verification | 面向大批量 claim verification、自托管和 literature-backed report。 | [bricee98/Valsci](https://github.com/bricee98/Valsci) |
| MSVEC | 多领域 scientific claim verification eval | 适合测试跨领域 claim verification 的泛化。 | [lamps-lab/msvec](https://github.com/lamps-lab/msvec) |
| ASReview | active learning for systematic reviews | 适合做高量文献筛选、systematic review 和 meta-analysis 入口。 | [asreview/asreview](https://github.com/asreview/asreview) |
| SYNERGY Dataset | systematic review study selection | 对 sparse labels 和 study selection 很有价值。 | [asreview/synergy-dataset](https://github.com/asreview/synergy-dataset) |

## 五、OpenReview 基础设施与 reviewer matching 工具

| 资源 | 类型 | 核心价值 | 链接 |
| --- | --- | --- | --- |
| OpenReview | 开放评审平台 | 顶会和部分期刊的公开评审、rebuttal 与 discussion 主入口。 | [OpenReview](https://openreview.net/) |
| OpenReview Python Client | API 客户端 | 适合做数据抓取、筛选和分析脚本。 | [openreview/openreview-py](https://github.com/openreview/openreview-py) |
| OpenReview Expertise | reviewer affinity modeling | 适合做 paper-reviewer affinity 建模与 reviewer matching。 | [openreview/openreview-expertise](https://github.com/openreview/openreview-expertise) |
| OpenReview Matcher | reviewer assignment | 适合研究约束优化下的 paper-reviewer 匹配。 | [openreview/openreview-matcher](https://github.com/openreview/openreview-matcher) |
| OpenReview MCP | MCP 接入层 | 适合把 review、rebuttal 和会议信息接入 agent 工作流。 | [openreview/openreview-mcp](https://github.com/openreview/openreview-mcp) |

## 六、值得长期跟踪的公开综述与资料库

| 资源 | 类型 | 核心价值 | 链接 |
| --- | --- | --- | --- |
| NLP for Peer Review | 数据集与任务汇总 | 专门汇总 peer review 数据集和任务，是补 benchmark 的高价值入口。 | [OAfzal/nlp-for-peer-review](https://github.com/OAfzal/nlp-for-peer-review) |
| LLM4SR | survey 资源库 | 对 peer review、meta-review、科学写作和 ideation 的 benchmark 整理很系统。 | [du-nlp-lab/LLM4SR](https://github.com/du-nlp-lab/LLM4SR) |
| Transforming Science with LLMs | survey 资源库 | 对 idea generation、peer review、scientific rigor 和 claim verification 条目很全。 | [NL2G/TransformingScienceLLMs](https://github.com/NL2G/TransformingScienceLLMs) |
| AI-4-Research | 大型综述站点 | 对 AI for peer review、自动科研、AAAR 类资源的汇总很密。 | [AI-4-Research/AI-4-Research.github.io](https://github.com/AI-4-Research/AI-4-Research.github.io) |
| Awesome Scholarly Data Analysis | scholarly data 合集 | 对 peer review、bibliometrics、citation、scholarly commons 很有帮助。 | [napsternxg/awesome-scholarly-data-analysis](https://github.com/napsternxg/awesome-scholarly-data-analysis) |
| research-automation-papers | 自动科研论文清单 | 对 peer review、novelty、claim verification 和 review generation 线索密度很高。 | [t46/research-automation-papers](https://github.com/t46/research-automation-papers) |

## 七、几条实用路线

1. novelty 评估路线：
   `llm4novelty / NovBench + ReviewAdvisor + NLPeer + PeerRead`
2. reviewer question 与证据核验路线：
   `PeerQA + SciDQA + PaperQA2 + scite`
3. claim verification 路线：
   `SciFact + SciFact-Open + Valsci + MSVEC`
4. systematic review 路线：
   `ASReview + SYNERGY Dataset + Elicit / Consensus`
5. automated reviewing 路线：
   `AgentReview + MARG + ReviewRobot + AI Peer Review`
