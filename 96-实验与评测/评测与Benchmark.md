# 评测与 Benchmark

这一页聚焦 benchmark 选择、公开评测集、回归测试和持续评估。对任务化使用更友好的主入口见：
[05-实验执行、复现与评测](../05-实验执行、复现与评测/README.md)

## 1. 研究工程与 research agent benchmark

| 资源 | 类型 | 简述 | 链接 |
| --- | --- | --- | --- |
| MLE-bench | ML engineering benchmark | 专门测 agent 是否真的能完成真实 ML engineering 任务。 | [OpenAI - MLE-bench](https://openai.com/index/mle-bench/) |
| MLGym | ML research benchmark | 更直接面向机器学习研究任务与 research agent。 | [facebookresearch/MLGym](https://github.com/facebookresearch/MLGym) |
| MLR-Bench | open-ended ML research benchmark | 覆盖 idea、proposal、experimentation 与 paper writing，更适合评测完整研究链路。 | [chchenhui/mlrbench](https://github.com/chchenhui/mlrbench) |
| FML-bench | automatic ML research benchmark | 强调探索广度与基础 ML 问题，适合自动 ML 研究代理比较。 | [qrzou/FML-bench](https://github.com/qrzou/FML-bench) |
| Aviary | language agent gym | 提供文献、notebook、生物序列等科学任务环境。 | [Future-House/aviary](https://github.com/Future-House/aviary) |
| LAB-Bench | scientific benchmark | 面向生物科学研究能力评测，也适合作为科学 agent 参考基准。 | [Future-House/LAB-Bench](https://github.com/Future-House/LAB-Bench) |
| LiveDRBench | deep research benchmark | 适合评测 deep research 与 claim discovery。 | [microsoft/livedrbench](https://github.com/microsoft/livedrbench) |
| ToolSandbox | tool-use benchmark | 适合评测多轮工具调用和状态化执行。 | [apple/ToolSandbox](https://github.com/apple/ToolSandbox) |
| ML-Dev-Bench | ML development benchmark | 直接面向模型开发、debug、数据处理和实现新想法等任务。 | [ml-dev-bench/ml-dev-bench](https://github.com/ml-dev-bench/ml-dev-bench) |
| OpenHands Benchmarks | agent benchmark harness | 适合继续补软件代理、执行任务和工程工作流评测。 | [OpenHands/benchmarks](https://github.com/OpenHands/benchmarks) |
| SciEval | scientific LLM benchmark | 适合从 scientific knowledge、application 和 research ability 多层评估模型。 | [OpenDFM/SciEval](https://github.com/OpenDFM/SciEval) |
| SciCode | scientific coding benchmark | 适合测试科研编程和实验实现能力。 | [scicode-bench/SciCode](https://github.com/scicode-bench/SciCode) |

## 2. 通用模型、RAG 与 agent eval 资源

| 资源 | 类型 | 简述 | 链接 |
| --- | --- | --- | --- |
| OpenCompass | 大模型评测平台 | 中文社区常用，适合做基线评估和模型对比。 | [open-compass/opencompass](https://github.com/open-compass/opencompass) |
| lm-evaluation-harness | 语言模型评测 | 经典的 LLM benchmark 执行框架。 | [EleutherAI/lm-evaluation-harness](https://github.com/EleutherAI/lm-evaluation-harness) |
| Ragas | RAG / workflow 评测 | 对文献问答、知识库检索和 RAG 系统评测很有参考价值。 | [Ragas](https://github.com/explodinggradients/ragas) |
| HELM | 综合评测框架 | 适合做多维度、可解释和可复现的综合评测。 | [stanford-crfm/helm](https://github.com/stanford-crfm/helm) |
| AgentBoard | agent benchmark 合集 | 适合快速扫 agent 评测任务和榜单。 | [hkust-nlp/AgentBoard](https://github.com/hkust-nlp/AgentBoard) |
| Toolathlon | tool-use benchmark 合集 | 适合继续补工具调用和代理评测。 | [hkust-nlp/Toolathlon](https://github.com/hkust-nlp/Toolathlon) |
| Papers with Code | 公开榜单与代码 | 适合做外部 baseline 对照和任务标准追踪。 | [Papers with Code](https://paperswithcode.com/) |

## 3. AI / ML / Data Mining 常用 benchmark 入口

| 方向 | 资源 | 为什么值得收录 | 链接 |
| --- | --- | --- | --- |
| tabular ML | OpenML | 开放任务、runs 和 suite 平台，是 tabular benchmark 的主入口之一。 | [OpenML](https://openml.io/) |
| AutoML | AutoMLBenchmark | 适合对比 AutoML 系统和自定义实验设置。 | [openml/automlbenchmark](https://github.com/openml/automlbenchmark) |
| tabular ML | LCBench | 适合研究 HPO、早停和算法选择。 | [automl/LCBench](https://github.com/automl/LCBench) |
| tabular ML | TabArena | 适合做持续维护的 tabular ML 对照实验。 | [autogluon/tabarena](https://github.com/autogluon/tabarena) |
| embedding / retrieval | MTEB | 适合 embedding、检索和多任务表示学习评测。 | [embeddings-benchmark/mteb](https://github.com/embeddings-benchmark/mteb) |
| 检索 / RAG | BEIR | 对 retriever、reranker、RAG retrieval 都很重要。 | [beir-cellar/beir](https://github.com/beir-cellar/beir) |
| 图学习 | OGB | graph ML 最通用的 benchmark 入口之一。 | [snap-stanford/ogb](https://github.com/snap-stanford/ogb) |
| 图鲁棒性 | GRB | 适合做 graph robustness / adversarial 评测。 | [THUDM/grb](https://github.com/THUDM/grb) |
| 推荐系统 | RecBole | 除了训练框架，本身也适合做 recommender benchmark 基线复现。 | [RUCAIBox/RecBole](https://github.com/RUCAIBox/RecBole) |
| 异常检测 | ADBench | 适合系统比较 anomaly detection 算法与设置。 | [Minqi824/ADBench](https://github.com/Minqi824/ADBench) |
| 图异常检测 | PyGOD | 适合图异常检测与 relational anomaly 评测。 | [pygod-team/pygod](https://github.com/pygod-team/pygod) |
| 因果发现 | CausalBench | 适合做 causal discovery 方法比较。 | [ravivanpong/CausalBench](https://github.com/ravivanpong/CausalBench) |
| 治疗科学 / AI for Science | TDC | 如果有 health / drug / bio 方向，这个值得优先跟进。 | [mims-harvard/TDC](https://github.com/mims-harvard/TDC) |

## 4. novelty / 审稿 / idea generation 的评测入口

| 资源 | 类型 | 简述 | 链接 |
| --- | --- | --- | --- |
| llm4novelty / NovBench | novelty benchmark | 专门针对学术新颖性判断，适合做 idea / novelty 系统基线与评测。 | [njust-winchy/llm4novelty](https://github.com/njust-winchy/llm4novelty) |
| ReviewAdvisor | scientific reviewing | 可作为 novelty、significance、weakness 等 review 维度的参考基线。 | [neulab/ReviewAdvisor](https://github.com/neulab/ReviewAdvisor) |
| NLPeer | peer review dataset | 公开 peer review 数据资源，适合做 review mining 和审稿结构分析。 | [UKPLab/nlpeer](https://github.com/UKPLab/nlpeer) |
| OpenReview | 公开审稿平台 | 顶会审稿过程和版本演化的真实数据入口。 | [OpenReview](https://openreview.net/) |

## 5. 一套更实用的评测分层

1. 文献理解与证据核验质量
2. 实验执行与研究工程质量
3. 工具调用和 workflow 稳定性
4. 领域 benchmark 表现
5. novelty 判断与 reviewer-style critique 质量

## 6. 更实用的落地方式

1. 先做 10 到 20 个内部黄金任务。
2. 再引入 `MLE-bench / MLGym / MLR-Bench / FML-bench / ToolSandbox / Ragas`。
3. 对 AI/ML/data mining 方向，再逐步补 `OpenML / TabArena / OGB / BEIR / RecBole / ADBench / CausalBench`。
4. 如果目标包含 idea / novelty，再补 `llm4novelty / NLPeer / OpenReview`。
5. 最后再把 benchmark、CI 和回归测试绑起来，形成持续评测闭环。

补充专题页：
[AI-ML-DataMining资源](../08-方向专题/AI-ML-DataMining资源.md)
