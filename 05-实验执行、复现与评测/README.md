# 实验执行、复现与评测

这一模块聚焦实验落地、notebook 与脚本执行、工作流编排、环境与依赖锁定、结果追踪、benchmark 选择以及持续评测。适合把“已有想法”推进成“可运行、可复验、可对照、可持续迭代”的研究资产。

## 这一步通常要回答的问题

1. 一套实验应当怎样组织，才能把数据、配置、代码、环境、日志和结果全部留痕。
2. notebook、脚本、pipeline、容器和调度系统之间，怎样形成稳定的执行闭环。
3. AI/ML、data mining、computational design science 相关研究应当优先接入哪些 benchmark。
4. 研究 agent 或自动化工作流究竟应当如何评估，而不是只看单次演示。
5. 哪些 `Skills`、`MCP` 和执行框架值得优先接入实验主链路。

## 推荐先看

- [实验框架、追踪与复现工具详表](./实验框架、追踪与复现工具详表.md)
- [AI-ML-DataMining-Benchmark与公开评测集](./AI-ML-DataMining-Benchmark与公开评测集.md)
- [96-实验与评测/实验执行与复现](../96-实验与评测/实验执行与复现.md)
- [96-实验与评测/评测与Benchmark](../96-实验与评测/评测与Benchmark.md)
- [98-全局索引/实验与Benchmark索引](../98-全局索引/实验与Benchmark索引.md)
- [91-Skills/科研工程与实验Skills](../91-Skills/科研工程与实验Skills.md)
- [92-MCP/实验执行与数据工程MCP](../92-MCP/实验执行与数据工程MCP.md)
- [08-方向专题/AI-ML-DataMining资源](../08-方向专题/AI-ML-DataMining资源.md)

## 最小工具栈

1. `Jupyter MCP + GitHub MCP + uv / conda-lock`
   适合搭一个可执行、可追溯、可回放的最小实验闭环。
2. `MLflow / Weights & Biases + DVC`
   适合记录参数、指标、artifact 和数据版本。
3. `Optuna + Ray Tune + Chart MCP`
   适合做调参、结果分析和可视化。
4. `OpenML / TabArena / OGB / BEIR / MTEB`
   适合快速补 AI/ML/data mining 的标准公开 benchmark。

## 高频公开资源

| 资源 | 类型 | 更适合的用途 | 链接 |
| --- | --- | --- | --- |
| MLflow / Weights & Biases / DVC | 实验追踪与数据版本 | 适合建立参数、指标、artifact、数据版本一体化记录。 | [MLflow](https://mlflow.org/)、[Weights & Biases](https://wandb.ai/site)、[DVC](https://dvc.org/) |
| MLE-bench / MLGym / MLR-Bench / FML-bench | ML engineering 与 research-agent benchmark | 适合评测 AI 代理是否真能做机器学习实验、调参、debug 和开放研究任务。 | [OpenAI - MLE-bench](https://openai.com/index/mle-bench/)、[facebookresearch/MLGym](https://github.com/facebookresearch/MLGym)、[chchenhui/mlrbench](https://github.com/chchenhui/mlrbench)、[qrzou/FML-bench](https://github.com/qrzou/FML-bench) |
| OpenHands Benchmarks / ToolSandbox / ML-Dev-Bench | tool-use 与开发型 benchmark | 适合测多轮工具调用、状态化执行和 ML 开发能力。 | [OpenHands/benchmarks](https://github.com/OpenHands/benchmarks)、[apple/ToolSandbox](https://github.com/apple/ToolSandbox)、[ml-dev-bench/ml-dev-bench](https://github.com/ml-dev-bench/ml-dev-bench) |
| OpenML / OpenML-CC18 / PMLB / TabArena / YAHPO Gym | tabular / AutoML / HPO benchmark | 适合建立标准 tabular 基线、多保真搜索与可复现实验。 | [OpenML](https://openml.io/)、[OpenML Benchmarking Suites](https://docs.openml.org/benchmark/)、[EpistasisLab/pmlb](https://github.com/EpistasisLab/pmlb)、[autogluon/tabarena](https://github.com/autogluon/tabarena)、[slds-lmu/yahpo_gym](https://github.com/slds-lmu/yahpo_gym) |
| OGB / BEIR / MTEB / RecBole | graph / retrieval / recommender benchmark | 适合图学习、检索、embedding 与推荐系统对照实验。 | [snap-stanford/ogb](https://github.com/snap-stanford/ogb)、[beir-cellar/beir](https://github.com/beir-cellar/beir)、[embeddings-benchmark/mteb](https://github.com/embeddings-benchmark/mteb)、[RUCAIBox/RecBole](https://github.com/RUCAIBox/RecBole) |
| LiveCodeBench / BigCodeBench / DS-1000 | 代码与数据科学 benchmark | 适合评测 coding、数据分析脚本、函数调用与修复能力。 | [LiveCodeBench/LiveCodeBench](https://github.com/LiveCodeBench/LiveCodeBench)、[bigcode-project/bigcodebench](https://github.com/bigcode-project/bigcodebench)、[xlang-ai/DS-1000](https://github.com/xlang-ai/DS-1000) |
| DataPerf / MLPerf | data-centric 与系统性能 benchmark | 适合补 dataset-centric AI、训练性能和推理性能维度。 | [DataPerf](https://www.dataperf.org/)、[MLPerf Training](https://mlcommons.org/benchmarks/training/)、[MLPerf Inference](https://mlcommons.org/working-groups/benchmarks/inference/) |

## 按子方向快速进入

| 子方向 | 更适合先看 |
| --- | --- |
| tabular / AutoML / HPO | [08-方向专题/Tabular-AutoML与HPO](../08-方向专题/Tabular-AutoML与HPO.md) |
| graph / retrieval / recommender | [08-方向专题/Graph-Retrieval-Recsys与DataMining](../08-方向专题/Graph-Retrieval-Recsys与DataMining.md) |
| causal / anomaly / data-centric AI | [08-方向专题/Causal-Anomaly与Data-Centric-AI](../08-方向专题/Causal-Anomaly与Data-Centric-AI.md) |
| benchmark 快查 | [98-全局索引/实验与Benchmark索引](../98-全局索引/实验与Benchmark索引.md) |
| CLI / notebook / 数据工程工具 | [98-全局索引/CLI与终端工具索引](../98-全局索引/CLI与终端工具索引.md) |
| 研究代理与自动化实验 | `MLE-bench`、`MLGym`、`MLR-Bench`、`FML-bench`、`OpenHands Benchmarks` |

## 一、相关 Skills

| 资源 | 类型 | 适合环节 | 简述 | 链接 |
| --- | --- | --- | --- | --- |
| 科研工程与实验Skills | 仓库内附录 | Skills 总览 | 当前仓库里实验工程、训练、评测和自动化执行相关 Skills 的主归属页。 | [91-Skills/科研工程与实验Skills](../91-Skills/科研工程与实验Skills.md) |
| AI Research SKILLs | 研究工程技能总库 | 训练与评测 | 覆盖训练、推理、分布式、评测、MLOps 和 agent 开发，是实验链路最值得优先补的公开 skill 库之一。 | [Orchestra-Research/AI-Research-SKILLs](https://github.com/Orchestra-Research/AI-Research-SKILLs) |
| Development Methodology | 方法论技能库 | 调试与验证 | `systematic-debugging`、`verification-before-completion`、`test-driven-development` 很适合实验回归与复现。 | [obra/superpowers](https://github.com/obra/superpowers) |
| Everything Claude Code | 跨宿主技能生态 | research-first workflow | 适合继续补研究工程、自动化开发与工具组合类 skills。 | [affaan-m/everything-claude-code](https://github.com/affaan-m/everything-claude-code) |
| `hf_model_evaluation` | HF Skill | 模型评测 | 适合统一跑模型评测、收集指标并沉淀评测报告。 | [huggingface/skills](https://github.com/huggingface/skills) |
| `hf-llm-trainer` | HF Skill | 训练与微调 | 适合快速搭建训练、微调、资源估算与脚手架。 | [huggingface/skills](https://github.com/huggingface/skills) |
| `hf_dataset_creator` | HF Skill | 数据集准备 | 适合做数据集草案、字段规划和 Hub 对接。 | [huggingface/skills](https://github.com/huggingface/skills) |
| `hf-cli` | HF Skill | Hub 与产物管理 | 适合把模型、数据、评测结果与 Hub 工作流接起来。 | [Hugging Face Agents Skills](https://huggingface.co/docs/hub/agents-skills) |
| `mcp-builder` | Anthropic Skill | 工具层建设 | 适合把实验平台、数据库和评测脚本封装成 MCP 工具层。 | [anthropics/skills](https://github.com/anthropics/skills) |
| OpenAI Skills | 官方技能目录 | 代码执行与诊断 | 更适合把调试、代码审查、CI 和工程诊断接进实验开发流程。 | [openai/skills](https://github.com/openai/skills) |
| OpenHands Skills | 技能文档与注册表 | 开发与自动化执行 | 适合把技能化执行扩展到软件代理和实验工程代理。 | [OpenHands Skills Docs](https://docs.openhands.dev/overview/skills/overview) |

## 二、相关 MCP

| 资源 | 类型 | 适合环节 | 简述 | 链接 |
| --- | --- | --- | --- | --- |
| 实验执行与数据工程MCP | 仓库内附录 | MCP 总览 | 当前仓库里 notebook、数据库、数据平台与实验执行相关 MCP 的主归属页。 | [92-MCP/实验执行与数据工程MCP](../92-MCP/实验执行与数据工程MCP.md) |
| Jupyter MCP Server | Notebook MCP | 交互式实验 | 支持查看、编辑和执行 notebook，是实验链路里最关键的执行入口之一。 | [datalayer/jupyter-mcp-server](https://github.com/datalayer/jupyter-mcp-server) |
| GitHub MCP Server | 代码协作 MCP | 仓库与 CI | 适合读取代码、Issue、PR、提交记录和 CI 状态。 | [github/github-mcp-server](https://github.com/github/github-mcp-server) |
| GitMCP | 仓库文档 MCP | 公共仓库阅读 | 适合快速查询开源 benchmark、README、配置与示例。 | [idosal/git-mcp](https://github.com/idosal/git-mcp) |
| Hugging Face MCP Server | 模型与数据生态 MCP | 资产回查 | 适合把模型、数据集、space 和评测资产接回实验链路。 | [huggingface/hf-mcp-server](https://github.com/huggingface/hf-mcp-server) |
| Optuna MCP Server | HPO MCP | 调参与结果分析 | 适合让 agent 发起 study、查看 trial、分析优化结果和可视化。 | [optuna/optuna-mcp](https://github.com/optuna/optuna-mcp) |
| Prefect MCP Server | orchestration MCP | pipeline 观察与调试 | 适合读取 flow run、deployment、日志和运行状态。 | [PrefectHQ/prefect-mcp-server](https://github.com/PrefectHQ/prefect-mcp-server) |
| MCP for ZenML | MLOps MCP | pipeline 与 artifact | 适合查看 pipeline run、step log、artifact 和触发新运行。 | [zenml-io/mcp-zenml](https://github.com/zenml-io/mcp-zenml) |
| MCPAdapt | MCP 适配层 | 工具兼容 | 适合把现有 Python 工具或 API 快速适配到 MCP 生态。 | [grll/mcpadapt](https://github.com/grll/mcpadapt) |
| Docker Hub MCP | 容器 MCP | 镜像与环境选择 | 适合为实验环境和 benchmark 容器选择基础镜像。 | [docker/hub-mcp](https://github.com/docker/hub-mcp) |
| Kaggle MCP | 数据平台 MCP | benchmark 数据获取 | 适合补 Kaggle 竞赛与数据集入口。 | [arrismo/kaggle-mcp](https://github.com/arrismo/kaggle-mcp) |
| Chart MCP Server | 可视化 MCP | 实验结果整理 | 适合把训练曲线、表格和对比结果快速转为图表。 | [antvis/mcp-server-chart](https://github.com/antvis/mcp-server-chart) |

## 三、相关 Agent、执行环境与工作流框架

| 资源 | 类型 | 适合环节 | 简述 | 链接 |
| --- | --- | --- | --- | --- |
| 实验框架、追踪与复现工具详表 | 仓库内详表 | 框架总览 | 当前模块里工作流编排、实验追踪、环境复现和 notebook 执行的主归属页。 | [实验框架、追踪与复现工具详表](./实验框架、追踪与复现工具详表.md) |
| RD-Agent | 研究开发代理 | 研究工程自动化 | 适合围绕研发与实验任务组织 agent 工作流。 | [microsoft/RD-Agent](https://github.com/microsoft/RD-Agent) |
| CMBAgent | 科学发现 Agent | 实验设计与研究协作 | 适合把科学研究任务拆成协作式 agent 工作流并接入评测。 | [CMBAgents/cmbagent](https://github.com/CMBAgents/cmbagent) |
| OpenHands Software Agent SDK | 代理开发框架 | 软件与实验代理 | 适合搭建能执行代码、工具和工作流的实验代理。 | [OpenHands/software-agent-sdk](https://github.com/OpenHands/software-agent-sdk) |
| AI-Scientist-v2 | 自动科研系统 | 提案到实验闭环 | 包含自动科研与实验链路的最新代表性系统之一。 | [SakanaAI/AI-Scientist-v2](https://github.com/SakanaAI/AI-Scientist-v2) |
| AgentLaboratory | 多代理科研框架 | 多步骤研究流程 | 适合把假设、实验、审查与写作拆成协作环节。 | [SamuelSchmidgall/AgentLaboratory](https://github.com/SamuelSchmidgall/AgentLaboratory) |
| Metaflow | 工作流框架 | 从 notebook 到部署 | 适合把 notebook 原型逐步升级为可管理的 AI/ML 系统。 | [Netflix/metaflow](https://github.com/Netflix/metaflow) |
| Prefect | orchestration 框架 | 调度与观察 | 适合有状态调度、重试、缓存和运行监控。 | [PrefectHQ/prefect](https://github.com/PrefectHQ/prefect) |
| Dagster | 编排与观测框架 | 数据资产与 pipeline | 适合把数据、模型、表和评测资产一起纳入可观测控制面。 | [dagster-io/dagster](https://github.com/dagster-io/dagster) |
| Kedro | 可维护数据科学框架 | 模块化项目 | 适合把脚本式实验改造成模块化、可维护项目。 | [kedro-org/kedro](https://github.com/kedro-org/kedro) |
| Snakemake / Nextflow | 科学工作流系统 | 可复现实验流水线 | 在多步骤、数据依赖明确的研究流程中非常强，尤其适合大规模批处理。 | [snakemake/snakemake](https://github.com/snakemake/snakemake)、[nextflow-io/nextflow](https://github.com/nextflow-io/nextflow) |

## 四、实验追踪、环境与复现工具

| 资源 | 类型 | 适合环节 | 简述 | 链接 |
| --- | --- | --- | --- | --- |
| DVC | 数据与流水线版本控制 | 数据、模型与 pipeline | 适合追踪数据版本、模型产物和可复现实验 DAG。 | [DVC](https://dvc.org/) |
| MLflow | 实验追踪平台 | 指标、参数与模型 | 适合统一记录参数、指标、artifact、model registry。 | [mlflow/mlflow](https://github.com/mlflow/mlflow) |
| Aim | 实验追踪工具 | 大规模 run 比较 | 适合高频实验比较、聚合和查询。 | [aimhubio/aim](https://github.com/aimhubio/aim) |
| ClearML | 追踪与远程执行平台 | tracking + orchestration | 适合把实验追踪、远程执行、数据管理与 pipeline 合并在同一套平台里。 | [clearml/clearml](https://github.com/clearml/clearml) |
| Hydra | 配置管理 | 配置组合与 sweep | 适合处理实验配置爆炸和参数组合。 | [facebookresearch/hydra](https://github.com/facebookresearch/hydra) |
| Optuna | HPO 框架 | 调参与搜索 | 适合做 study、trial、可视化和自动调参。 | [optuna/optuna](https://github.com/optuna/optuna) |
| Weights & Biases | 实验追踪平台 | tracking 与可视化 | 适合记录 runs、对比实验、保存配置并做团队协作。 | [wandb/wandb](https://github.com/wandb/wandb) |
| Ray Tune | 调参与分布式实验 | HPO 与并行搜索 | 适合大规模搜索、调度和资源感知实验。 | [ray-project/ray](https://github.com/ray-project/ray) |
| uv / micromamba / conda-lock | 依赖管理 | 环境锁定 | 适合把环境与依赖固定成可重建状态。 | [astral-sh/uv](https://github.com/astral-sh/uv)、[mamba-org/micromamba-releases](https://github.com/mamba-org/micromamba-releases)、[conda/conda-lock](https://github.com/conda/conda-lock) |
| Docker / Apptainer | 容器化工具 | 可移植运行环境 | 适合把训练、评测和依赖打包成一致执行环境。 | [Docker](https://www.docker.com/)、[apptainer/apptainer](https://github.com/apptainer/apptainer) |
| ReproZip / DataLad | 复现与数据管理 | 复验与 provenance | 适合打包命令行实验、管理大文件和追踪数据 provenance。 | [VIDA-NYU/reprozip](https://github.com/VIDA-NYU/reprozip)、[DataLad](https://www.datalad.org/) |
| Papermill / marimo / Quarto | notebook 与报告 | 可复验文档与输出 | 适合参数化 notebook、以纯 Python 存储实验、把结果转成可发布文档。 | [nteract/papermill](https://github.com/nteract/papermill)、[marimo-team/marimo](https://github.com/marimo-team/marimo)、[quarto-dev/quarto-cli](https://github.com/quarto-dev/quarto-cli) |

## 五、benchmark 与公开评测集

| 资源 | 类型 | 适合环节 | 简述 | 链接 |
| --- | --- | --- | --- | --- |
| AI-ML-DataMining-Benchmark与公开评测集 | 仓库内详表 | Benchmark 总览 | 当前模块里 AI/ML、data mining、agent eval 与 benchmark 资源的主归属页。 | [AI-ML-DataMining-Benchmark与公开评测集](./AI-ML-DataMining-Benchmark与公开评测集.md) |
| MLE-bench | ML engineering benchmark | 端到端 ML 工程评估 | 专门测 AI 代理是否真能做 ML 工程任务。 | [OpenAI - MLE-bench](https://openai.com/index/mle-bench/) |
| MLGym / MLR-Bench / FML-bench | AI/ML research benchmark | 研究任务评估 | 适合覆盖开放式机器学习研究、自动 ML 研究与完整研究链路评测。 | [facebookresearch/MLGym](https://github.com/facebookresearch/MLGym)、[chchenhui/mlrbench](https://github.com/chchenhui/mlrbench)、[qrzou/FML-bench](https://github.com/qrzou/FML-bench) |
| Aviary / LAB-Bench | 科学 agent benchmark | 科学任务与 notebook 环境 | 适合评测文献检索、科学问答、notebook 执行和生物科学任务。 | [Future-House/aviary](https://github.com/Future-House/aviary)、[Future-House/LAB-Bench](https://github.com/Future-House/LAB-Bench) |
| LiveDRBench / NewtonBench | deep research 与科学发现 benchmark | 适合补 long-horizon research、科学推理和自动发现类评测。 | [THUDM/LiveDRBench](https://github.com/THUDM/LiveDRBench)、[HKUST-KnowComp/NewtonBench](https://github.com/HKUST-KnowComp/NewtonBench) |
| ToolSandbox / ML-Dev-Bench / OpenHands Benchmarks | tool-use 与 ML dev benchmark | 工具调用与开发任务 | 适合评测状态化工具调用、多轮任务、ML 开发能力和软件代理执行。 | [apple/ToolSandbox](https://github.com/apple/ToolSandbox)、[ml-dev-bench/ml-dev-bench](https://github.com/ml-dev-bench/ml-dev-bench)、[OpenHands/benchmarks](https://github.com/OpenHands/benchmarks) |
| OpenCompass / lm-eval-harness / LightEval / HELM / Ragas | 通用评测框架 | LLM、RAG 与 agent eval | 适合建立通用大模型评测、RAG/agent 回归评测以及多后端 benchmark 执行体系。 | [open-compass/opencompass](https://github.com/open-compass/opencompass)、[EleutherAI/lm-evaluation-harness](https://github.com/EleutherAI/lm-evaluation-harness)、[huggingface/lighteval](https://github.com/huggingface/lighteval)、[stanford-crfm/helm](https://github.com/stanford-crfm/helm)、[Ragas](https://github.com/explodinggradients/ragas) |
| LiveCodeBench / BigCodeBench / DS-1000 | 代码与数据科学 benchmark | coding 与 data science eval | 适合评测代码生成、代码修复、真实函数调用和数据科学代码能力。 | [LiveCodeBench/LiveCodeBench](https://github.com/LiveCodeBench/LiveCodeBench)、[bigcode-project/bigcodebench](https://github.com/bigcode-project/bigcodebench)、[xlang-ai/DS-1000](https://github.com/xlang-ai/DS-1000) |
| OpenML / OpenML-CC18 / PMLB / TabArena / YAHPO Gym / AutoMLBenchmark | tabular 与 AutoML benchmark | 基线与对照实验 | 适合标准化 tabular 任务、AutoML 比较、多保真 HPO 与可复现实验。 | [OpenML](https://openml.io/)、[OpenML Benchmarking Suites](https://docs.openml.org/benchmark/)、[EpistasisLab/pmlb](https://github.com/EpistasisLab/pmlb)、[autogluon/tabarena](https://github.com/autogluon/tabarena)、[slds-lmu/yahpo_gym](https://github.com/slds-lmu/yahpo_gym)、[openml/automlbenchmark](https://github.com/openml/automlbenchmark) |
| OGB / BEIR / MTEB / RecBole / ADBench / CausalBench | 领域 benchmark | AI/ML/data mining 专题评测 | 覆盖图学习、检索、embedding、推荐、异常检测与因果发现。 | [snap-stanford/ogb](https://github.com/snap-stanford/ogb)、[beir-cellar/beir](https://github.com/beir-cellar/beir)、[embeddings-benchmark/mteb](https://github.com/embeddings-benchmark/mteb)、[RUCAIBox/RecBole](https://github.com/RUCAIBox/RecBole)、[Minqi824/ADBench](https://github.com/Minqi824/ADBench)、[ravivanpong/CausalBench](https://github.com/ravivanpong/CausalBench) |
| DataPerf / MLPerf | data-centric 与系统性能 benchmark | 数据与性能评测 | 适合补数据中心 AI、训练/推理性能和 dataset-centric AI 的评价维度。 | [DataPerf](https://www.dataperf.org/)、[MLPerf Training](https://mlcommons.org/benchmarks/training/)、[MLPerf Inference](https://mlcommons.org/working-groups/benchmarks/inference/) |

## 六、外部整合入口

| 资源 | 类型 | 更适合的用途 | 链接 |
| --- | --- | --- | --- |
| awesome-data-agents | 数据智能与 agent 合集 | 补数据工作流、数据代理与实验代理资源。 | [HKUSTDial/awesome-data-agents](https://github.com/HKUSTDial/awesome-data-agents) |
| Toolathlon | 工具使用 benchmark 合集 | 扫工具调用、agent benchmark 和 tool-use 任务。 | [hkust-nlp/Toolathlon](https://github.com/hkust-nlp/Toolathlon) |
| AgentBoard | agent 评测合集 | 快速扫 agent benchmark 和评测维度。 | [hkust-nlp/AgentBoard](https://github.com/hkust-nlp/AgentBoard) |
| DataPerf | 数据中心 AI 基准组织 | 补 dataset-centric AI benchmark 与挑战。 | [DataPerf](https://www.dataperf.org/) |
| MLCommons MLPerf | 系统性能 benchmark 组织 | 补训练、推理与硬件/软件系统性能基准。 | [MLPerf Training](https://mlcommons.org/benchmarks/training/)、[MLPerf Inference](https://mlcommons.org/working-groups/benchmarks/inference/) |
| awesome-ml-experiment-management | 实验管理合集 | 补 experiment tracking、logging、dashboard 和结果管理。 | [awesome-mlops/awesome-ml-experiment-management](https://github.com/awesome-mlops/awesome-ml-experiment-management) |
| awesome-open-mlops | 开源 MLOps 合集 | 补 pipeline、部署、监控和 full-stack MLOps 工具。 | [fuzzylabs/awesome-open-mlops](https://github.com/fuzzylabs/awesome-open-mlops) |
| awesome-reproducible-research | 可复现科研合集 | 补 reproducibility case、平台、教程和工具。 | [leipzig/awesome-reproducible-research](https://github.com/leipzig/awesome-reproducible-research) |

## 七、推荐组合

1. `Jupyter MCP + GitHub MCP + DVC + MLflow + Hydra`
   适合最小可复现实验闭环。
2. `Optuna MCP + Optuna + MLflow + Aim`
   适合做参数搜索、trial 追踪与结果比较。
3. `Papermill / marimo + Quarto + Chart MCP`
   适合把 notebook 实验转成可复验报告。
4. `OpenML / TabArena / AutoMLBenchmark`
   适合做 tabular 与 AutoML 基线和公开对照。
5. `OGB / BEIR / MTEB / RecBole / ADBench / CausalBench`
   适合 AI/ML/data mining 专题评测。
6. `MLE-bench / MLGym / MLR-Bench / FML-bench / ToolSandbox / ML-Dev-Bench`
   适合做研究 agent 与实验自动化系统评测。
7. `LiveCodeBench / BigCodeBench / DS-1000`
   适合做代码能力、数据科学代码和代理编程评测。
8. `PMLB / OpenML-CC18 / YAHPO Gym + Ray Tune / Optuna`
   适合做 tabular、HPO 和多保真搜索实验。

## 八、如果这一页的 Skills / MCP 还不够

- Skills 继续补：优先回看 [91-Skills/科研工程与实验Skills](../91-Skills/科研工程与实验Skills.md) 与 [91-Skills/Skill发现平台与精品合集](../91-Skills/Skill发现平台与精品合集.md)。
- MCP 继续补：优先回看 [92-MCP/实验执行与数据工程MCP](../92-MCP/实验执行与数据工程MCP.md) 与 [92-MCP/MCP标准与发现平台](../92-MCP/MCP标准与发现平台.md)。

## 九、仓库内延伸阅读

- [04-新颖性判断与综述](../04-新颖性判断与综述/README.md)
- [06-写作、审稿与投稿](../06-写作、审稿与投稿/README.md)
- [08-方向专题/AI-ML-DataMining资源](../08-方向专题/AI-ML-DataMining资源.md)
