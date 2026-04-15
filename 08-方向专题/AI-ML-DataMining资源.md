# AI / ML / Data Mining 资源

这一页作为 `AI / ML / data mining` 的方向总入口，重点负责“按子方向分流”和“把公共底座串起来”。详细条目继续下沉到子方向页，避免一页塞满 tabular、graph、retrieval、recsys、anomaly、causal 等所有内容而难以使用。

## 这一步通常要回答的问题

1. AI/ML 主线里哪些 benchmark 最适合用来做稳定 baseline 与 agent 评测。
2. tabular、graph、推荐、检索、异常检测、因果推断等子方向分别应当从哪一页进入。
3. 哪些 `Skills`、`MCP` 和实验平台最适合优先接到 AI/ML 研究链路里。
4. 哪些公开合集最适合继续补库，而不是停留在单条仓库链接。

## 推荐先看

- [Tabular-AutoML与HPO](./Tabular-AutoML与HPO.md)
- [Graph-Retrieval-Recsys与DataMining](./Graph-Retrieval-Recsys与DataMining.md)
- [Causal-Anomaly与Data-Centric-AI](./Causal-Anomaly与Data-Centric-AI.md)
- [05-实验执行、复现与评测](../05-实验执行、复现与评测/README.md)
- [91-Skills/科研工程与实验Skills](../91-Skills/科研工程与实验Skills.md)
- [92-MCP/实验执行与数据工程MCP](../92-MCP/实验执行与数据工程MCP.md)

## 最小工具栈

1. `OpenML / OpenML-CC18 / PMLB / TabArena`
   适合快速搭 tabular 与 AutoML 基线。
2. `Jupyter MCP + GitHub MCP + Optuna MCP + dbhub`
   适合把 notebook、代码、搜索实验和数据连接起来。
3. `AutoGluon / PyG / Pyserini / RecBole / PyOD / DoWhy`
   适合按不同子方向快速建立第一个可比 baseline。
4. `MLflow / DVC + MLE-bench / MLGym / OpenHands Benchmarks`
   适合把实验追踪与研究代理评测接起来。

## 一、子方向专题页

| 子方向 | 更适合的问题 | 首选入口 |
| --- | --- | --- |
| Tabular / AutoML / HPO | 表格任务、基线比较、超参搜索、多保真优化 | [Tabular-AutoML与HPO](./Tabular-AutoML与HPO.md) |
| Graph / Retrieval / Recsys | 图学习、知识图谱、检索、embedding、推荐 | [Graph-Retrieval-Recsys与DataMining](./Graph-Retrieval-Recsys与DataMining.md) |
| Causal / Anomaly / Data-Centric AI | 因果发现、异常检测、数据质量与鲁棒性 | [Causal-Anomaly与Data-Centric-AI](./Causal-Anomaly与Data-Centric-AI.md) |

## 二、共享 Skills 与 MCP 入口

| 资源 | 类型 | 更适合的用途 | 链接 |
| --- | --- | --- | --- |
| 科研工程与实验Skills | 仓库内附录 | 当前仓库中训练、评测、自动化执行和实验工程 Skills 的主归属页。 | [91-Skills/科研工程与实验Skills](../91-Skills/科研工程与实验Skills.md) |
| 科学计算与领域Skills | 仓库内附录 | 当 AI/ML 与科学计算、领域数据交叉时的 Skill 入口。 | [91-Skills/科学计算与领域Skills](../91-Skills/科学计算与领域Skills.md) |
| AI Research SKILLs / Hugging Face Skills / obra/superpowers | 技能主线 | 分别对应研究工程、模型训练评测和方法论工作流。 | [Orchestra-Research/AI-Research-SKILLs](https://github.com/Orchestra-Research/AI-Research-SKILLs)、[huggingface/skills](https://github.com/huggingface/skills)、[obra/superpowers](https://github.com/obra/superpowers) |
| 实验执行与数据工程MCP | 仓库内附录 | Jupyter、GitHub、Kaggle、Optuna、Prefect、ZenML 等执行层入口。 | [92-MCP/实验执行与数据工程MCP](../92-MCP/实验执行与数据工程MCP.md) |
| 文献检索与知识库MCP | 仓库内附录 | OpenAlex、paper-search、OpenReview、Zotero 等文献与知识层入口。 | [92-MCP/文献检索与知识库MCP](../92-MCP/文献检索与知识库MCP.md) |
| Jupyter MCP / GitHub MCP / Optuna MCP / dbhub | 常用 MCP 组合 | 对应 notebook、代码、超参搜索和数据连接。 | [datalayer/jupyter-mcp-server](https://github.com/datalayer/jupyter-mcp-server)、[github/github-mcp-server](https://github.com/github/github-mcp-server)、[optuna/optuna-mcp](https://github.com/optuna/optuna-mcp)、[bytebase/dbhub](https://github.com/bytebase/dbhub) |

## 三、高频 benchmark、框架与平台总览

| 资源 | 类型 | 更适合的用途 | 链接 |
| --- | --- | --- | --- |
| OpenML / OpenML-CC18 / PMLB / TabArena | tabular benchmark | 适合表格任务、AutoML 和标准基线对照。 | [OpenML](https://openml.org/)、[OpenML Benchmarking Suites](https://docs.openml.org/benchmark/)、[EpistasisLab/pmlb](https://github.com/EpistasisLab/pmlb)、[autogluon/tabarena](https://github.com/autogluon/tabarena) |
| OGB / BEIR / MTEB / RecBole | graph / retrieval / recommender benchmark | 适合图学习、检索、embedding 与推荐系统评测。 | [snap-stanford/ogb](https://github.com/snap-stanford/ogb)、[beir-cellar/beir](https://github.com/beir-cellar/beir)、[embeddings-benchmark/mteb](https://github.com/embeddings-benchmark/mteb)、[RUCAIBox/RecBole](https://github.com/RUCAIBox/RecBole) |
| PyOD / ADBench / DoWhy / CausalBench / DataPerf | anomaly / causal / data-centric AI | 适合异常检测、因果推断和数据质量评测。 | [yzhao062/pyod](https://github.com/yzhao062/pyod)、[Minqi824/ADBench](https://github.com/Minqi824/ADBench)、[py-why/dowhy](https://github.com/py-why/dowhy)、[ravivanpong/CausalBench](https://github.com/ravivanpong/CausalBench)、[DataPerf](https://www.dataperf.org/) |
| MLE-bench / MLGym / OpenHands Benchmarks / ToolSandbox | 研究代理与自动化实验 benchmark | 适合评测 AI 代理能否真正完成实验、工具调用和工程任务。 | [OpenAI - MLE-bench](https://openai.com/index/mle-bench/)、[facebookresearch/MLGym](https://github.com/facebookresearch/MLGym)、[OpenHands/benchmarks](https://github.com/OpenHands/benchmarks)、[apple/ToolSandbox](https://github.com/apple/ToolSandbox) |
| LiveCodeBench / BigCodeBench / DS-1000 | 代码与数据科学 benchmark | 适合补 coding、数据科学脚本和程序执行维度。 | [LiveCodeBench/LiveCodeBench](https://github.com/LiveCodeBench/LiveCodeBench)、[bigcode-project/bigcodebench](https://github.com/bigcode-project/bigcodebench)、[xlang-ai/DS-1000](https://github.com/xlang-ai/DS-1000) |

## 四、外部整合入口

| 资源 | 类型 | 更适合的用途 | 链接 |
| --- | --- | --- | --- |
| HKUST-Got-Skills Resources | 综合资源页 | 同时补 `Skills`、`MCP`、CLI、notebook 与 benchmark 入口。 | [HKUST-Got-Skills Resources](https://giggleliu.github.io/HKUST-Got-Skills/resources) |
| awesome-data-agents | 外部合集 | 数据代理、分析代理与 data-centric agent 资源入口。 | [HKUSTDial/awesome-data-agents](https://github.com/HKUSTDial/awesome-data-agents) |
| Toolathlon | 外部合集 | tool-use benchmark、agent benchmark 和任务型评测入口。 | [hkust-nlp/Toolathlon](https://github.com/hkust-nlp/Toolathlon) |
| AgentBoard | 外部合集 | 继续扩展 agent benchmark 与任务维度。 | [hkust-nlp/AgentBoard](https://github.com/hkust-nlp/AgentBoard) |
| awesome-production-machine-learning | 外部合集 | MLOps、训练、部署、监控与生产级机器学习入口。 | [EthicalML/awesome-production-machine-learning](https://github.com/EthicalML/awesome-production-machine-learning) |
| awesome-causal-inference | 外部合集 | 因果推断论文、工具和资源入口。 | [matteocourthoud/awesome-causal-inference](https://github.com/matteocourthoud/awesome-causal-inference) |
| awesome-RecSys | 外部合集 | 推荐系统方向的资源和项目入口。 | [wusw14/awesome-recsys](https://github.com/wusw14/awesome-recsys) |

## 五、推荐组合

1. `OpenML + AutoGluon / FLAML + MLflow + DVC`
   适合建立稳定 tabular baseline 与可复现实验闭环。
2. `PyG / DGL + OGB + PyGOD / PyKEEN`
   适合 graph mining、知识图谱和图异常方向。
3. `RecBole / Cornac + Pyserini + BEIR + MTEB`
   适合推荐、检索、embedding 和 RAG 基线比较。
4. `DoWhy + causal-learn + EconML / DoubleML`
   适合 AI/ML 与政策、机制识别、平台治理交叉研究。
5. `MLE-bench + MLGym + ToolSandbox + ML-Dev-Bench`
   适合系统评估 AI/ML research agent 与自动化实验系统。

## 六、仓库内延伸阅读

- [05-实验执行、复现与评测](../05-实验执行、复现与评测/README.md)
- [07-安全与治理](../07-安全与治理/README.md)
- [Computational-Design-Science与管理技术交叉](./Computational-Design-Science与管理技术交叉.md)
