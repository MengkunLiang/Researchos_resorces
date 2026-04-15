# AI / ML / Data Mining Benchmark 与公开评测集

这一页专门补足 `05-实验执行、复现与评测` 的 benchmark 层和公开评测层。重点不是只列榜单，而是把“真正适合做对照、复现、回归评测和系统设计”的公开资源按任务分层整理出来。

## 一、研究 agent 与 ML engineering benchmark

| 资源 | 类型 | 核心价值 | 链接 |
| --- | --- | --- | --- |
| MLE-bench | ML engineering benchmark | 专门测 agent 是否能完成真实 ML engineering 任务，是当前最重要的 ML 代理 benchmark 之一。 | [OpenAI - MLE-bench](https://openai.com/index/mle-bench/) |
| MLGym | AI research benchmark | 面向开放式机器学习研究任务，覆盖想法、数据、训练、分析与迭代。 | [facebookresearch/MLGym](https://github.com/facebookresearch/MLGym) |
| MLR-Bench | open-ended ML research benchmark | 覆盖 idea、proposal、experimentation 与 paper writing，更适合评测完整研究链路。 | [chchenhui/mlrbench](https://github.com/chchenhui/mlrbench) |
| FML-bench | automatic ML research benchmark | 强调探索广度与基础 ML 问题，适合自动 ML 研究代理比较。 | [qrzou/FML-bench](https://github.com/qrzou/FML-bench) |
| Aviary | language agent gym | 提供文献、notebook、生物序列等科学任务环境。 | [Future-House/aviary](https://github.com/Future-House/aviary) |
| LAB-Bench | biology research benchmark | 面向生物科学研究基础能力的科学 benchmark。 | [Future-House/LAB-Bench](https://github.com/Future-House/LAB-Bench) |
| LiveDRBench | deep research benchmark | 适合评测 deep research、claim discovery 和研究检索闭环。 | [microsoft/livedrbench](https://github.com/microsoft/livedrbench) |
| ToolSandbox | tool-use benchmark | 适合评测状态化工具调用、多轮对话和中间步骤执行。 | [apple/ToolSandbox](https://github.com/apple/ToolSandbox) |
| ML-Dev-Bench | ML development benchmark | 直接面向模型开发、debug、数据管理和实现新想法等任务。 | [ml-dev-bench/ml-dev-bench](https://github.com/ml-dev-bench/ml-dev-bench) |
| OpenHands Benchmarks | agent benchmark harness | 适合继续补软件代理、执行任务和工程工作流评测。 | [OpenHands/benchmarks](https://github.com/OpenHands/benchmarks) |
| SciEval | scientific LLM benchmark | 适合从 scientific knowledge、application、calculation 和 research ability 多层评估模型。 | [OpenDFM/SciEval](https://github.com/OpenDFM/SciEval) |
| SciCode | scientific coding benchmark | 适合测试科研编程、实验实现和科学问题编码能力。 | [scicode-bench/SciCode](https://github.com/scicode-bench/SciCode) |

## 二、通用模型、RAG 与 agent eval 框架

| 资源 | 类型 | 核心价值 | 链接 |
| --- | --- | --- | --- |
| OpenCompass | 大模型评测平台 | 中文社区常用，支持大量模型和数据集，适合统一基线评估。 | [open-compass/opencompass](https://github.com/open-compass/opencompass) |
| lm-evaluation-harness | 语言模型评测框架 | 通用、经典、可扩展，是很多论文和榜单的基础工具。 | [EleutherAI/lm-evaluation-harness](https://github.com/EleutherAI/lm-evaluation-harness) |
| LightEval | 多后端评测框架 | 适合快速调用 Hugging Face 生态中的大量任务，也适合做统一 benchmark 编排。 | [huggingface/lighteval](https://github.com/huggingface/lighteval) |
| HELM | holistic evaluation 框架 | 适合做多维度、可复现、可解释的综合评测。 | [stanford-crfm/helm](https://github.com/stanford-crfm/helm) |
| Ragas | RAG / agent eval | 适合评测知识检索、回答质量、faithfulness 和 workflow 质量。 | [Ragas](https://github.com/explodinggradients/ragas) |
| AgentBoard | agent benchmark 合集 | 适合快速扫 agent 评测基准和任务类型。 | [hkust-nlp/AgentBoard](https://github.com/hkust-nlp/AgentBoard) |
| Toolathlon | tool-use benchmark 合集 | 适合继续补工具调用和代理执行 benchmark。 | [hkust-nlp/Toolathlon](https://github.com/hkust-nlp/Toolathlon) |

## 三、tabular ML 与 AutoML benchmark

| 资源 | 类型 | 核心价值 | 链接 |
| --- | --- | --- | --- |
| OpenML | 开放 ML 平台 | 提供任务、runs、suite 和标准元数据，是最重要的 tabular benchmark 基座之一。 | [OpenML](https://openml.io/) |
| OpenML-CC18 | tabular benchmark suite | 是 OpenML 中最常被引用的标准 tabular 基准套件之一。 | [OpenML Benchmarking Suites](https://docs.openml.org/benchmark/) |
| PMLB | tabular benchmark 数据库 | 适合快速建立传统监督学习的对照实验与教学型 benchmark。 | [EpistasisLab/pmlb](https://github.com/EpistasisLab/pmlb) |
| AutoML Benchmark | AutoML benchmarking 框架 | 适合对比 AutoML 系统和自定义 benchmark。 | [openml/automlbenchmark](https://github.com/openml/automlbenchmark) |
| LCBench | 学习曲线 benchmark | 适合研究 HPO、早停、代理模型和算法选择。 | [automl/LCBench](https://github.com/automl/LCBench) |
| YAHPO Gym | HPO benchmark gym | 适合多保真、多目标超参数优化和 black-box optimization 评测。 | [slds-lmu/yahpo_gym](https://github.com/slds-lmu/yahpo_gym) |
| TabArena | living tabular benchmark | 适合做更强、更持续维护的 tabular ML 对照实验。 | [autogluon/tabarena](https://github.com/autogluon/tabarena) |
| TabRepo | tabular benchmark 结果库 | 适合复用 tabular 模型评测结果与组合策略。 | [autogluon/tabrepo](https://github.com/autogluon/tabrepo) |
| AutoGluon | AutoML 框架 | 适合快速搭稳定 baseline，并与 tabular benchmark 对接。 | [autogluon/autogluon](https://github.com/autogluon/autogluon) |

## 四、代码、数据科学与开发型 benchmark

| 资源 | 类型 | 核心价值 | 链接 |
| --- | --- | --- | --- |
| LiveCodeBench | code benchmark | 适合评测代码生成、代码执行、测试输出预测和长期污染控制。 | [LiveCodeBench/LiveCodeBench](https://github.com/LiveCodeBench/LiveCodeBench) |
| BigCodeBench | code benchmark | 适合评测复杂函数调用、真实任务自动化和更接近实际开发的代码能力。 | [bigcode-project/bigcodebench](https://github.com/bigcode-project/bigcodebench) |
| DS-1000 | data science code benchmark | 适合评测数据处理、分析、建模和 notebook 式数据科学代码能力。 | [xlang-ai/DS-1000](https://github.com/xlang-ai/DS-1000) |

## 五、检索、embedding、图学习与推荐 benchmark

| 方向 | 资源 | 核心价值 | 链接 |
| --- | --- | --- | --- |
| embedding / retrieval | MTEB | 适合 embedding、语义检索和多任务表示学习评测。 | [embeddings-benchmark/mteb](https://github.com/embeddings-benchmark/mteb) |
| IR / RAG retrieval | BEIR | 适合跨域检索、retriever、reranker 与 RAG retrieval 对照。 | [beir-cellar/beir](https://github.com/beir-cellar/beir) |
| graph ML | OGB | 图学习领域最重要的标准 benchmark 入口之一。 | [snap-stanford/ogb](https://github.com/snap-stanford/ogb) |
| graph robustness | GRB | 适合图模型鲁棒性和对抗评测。 | [THUDM/grb](https://github.com/THUDM/grb) |
| recommendation | RecBole | 覆盖推荐系统模型、训练和评测，是高频基线工具。 | [RUCAIBox/RecBole](https://github.com/RUCAIBox/RecBole) |
| recommendation | Cornac | 适合研究原型、多模态推荐和较轻量的基线比较。 | [PreferredAI/cornac](https://github.com/PreferredAI/cornac) |
| knowledge graph | PyKEEN | 适合知识图谱表示学习和 link prediction 评测。 | [pykeen/pykeen](https://github.com/pykeen/pykeen) |

## 六、异常检测、因果发现与数据中心 AI 评测

| 方向 | 资源 | 核心价值 | 链接 |
| --- | --- | --- | --- |
| tabular anomaly detection | ADBench | 对异常检测算法、监督设置、噪声与鲁棒性做系统 benchmark。 | [Minqi824/ADBench](https://github.com/Minqi824/ADBench) |
| anomaly detection | PyOD | 经典异常检测工具箱，适合快速建立基线。 | [yzhao062/pyod](https://github.com/yzhao062/pyod) |
| graph anomaly detection | PyGOD | 图异常检测主流工具箱。 | [pygod-team/pygod](https://github.com/pygod-team/pygod) |
| causal discovery | CausalBench | 适合比较因果发现算法和数据假设。 | [ravivanpong/CausalBench](https://github.com/ravivanpong/CausalBench) |
| causal discovery | causal-learn | 适合在 benchmark 之外快速试验主流因果发现算法。 | [py-why/causal-learn](https://github.com/py-why/causal-learn) |
| heterogeneous treatment effects | EconML | 适合把 CATE / DML / treatment effect 估计带进实验设计。 | [py-why/EconML](https://github.com/py-why/EconML) |
| data-centric AI | DataPerf | 适合补数据质量、数据选择和 dataset-centric AI 的评价视角。 | [DataPerf](https://www.dataperf.org/) |
| system performance | MLPerf Training / Inference | 适合补训练速度、推理吞吐、系统栈与硬件/软件性能基准。 | [MLPerf Training](https://mlcommons.org/benchmarks/training/)、[MLPerf Inference](https://mlcommons.org/working-groups/benchmarks/inference/) |

## 七、公开榜单与资料平台

| 资源 | 类型 | 核心价值 | 链接 |
| --- | --- | --- | --- |
| Papers with Code | 任务与榜单平台 | 适合追 SOTA、任务定义、论文代码与公开 leaderboard。 | [Papers with Code](https://paperswithcode.com/) |
| OpenML | runs / tasks / suites 平台 | 适合上传结果、复用 benchmark suites 和做标准对照。 | [OpenML](https://openml.io/) |
| TabArena Leaderboard | tabular 榜单 | 适合快速看当前 tabular 模型表现与设置差异。 | [TabArena](https://tabarena.ai/) |
| MTEB Leaderboard | embedding 榜单 | 适合快速对比 embedding 和 retrieval 模型。 | [MTEB](https://github.com/embeddings-benchmark/mteb) |
| OpenCompass Leaderboard | 大模型榜单 | 适合多任务、多数据集和多模型对照。 | [OpenCompass](https://github.com/open-compass/opencompass) |

## 八、几条常用路线

1. ML engineering / research agent 路线：
   `MLE-bench + MLGym + MLR-Bench + FML-bench + ToolSandbox + LiveDRBench`
2. tabular / AutoML 路线：
   `OpenML + OpenML-CC18 + PMLB + AutoMLBenchmark + YAHPO Gym + TabArena + AutoGluon`
3. code / data science 路线：
   `LiveCodeBench + BigCodeBench + DS-1000 + OpenHands Benchmarks`
4. retrieval / RAG 路线：
   `BEIR + MTEB + OpenCompass + Ragas`
5. graph / data mining 路线：
   `OGB + GRB + PyG / DGL + PyGOD`
6. recommendation 路线：
   `RecBole + Cornac + Papers with Code`
7. anomaly / causal / data-centric 路线：
   `ADBench + PyOD + CausalBench + causal-learn + EconML + DataPerf`
