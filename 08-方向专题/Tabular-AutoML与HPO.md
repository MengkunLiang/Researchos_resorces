# Tabular / AutoML 与 HPO

这一页聚焦表格任务、`AutoML`、超参搜索和多保真优化。适合建立稳定 baseline、做公开 benchmark 比较，以及把搜索实验接到可复现流水线里。

## 这一步通常要回答的问题

1. 表格任务优先从哪些公开任务集与 suite 开始。
2. AutoML 系统与手工 pipeline 应该如何做公平对照。
3. 超参搜索、预算约束与多保真优化应当如何接到实验流水线。
4. 哪些 `Skills`、`MCP` 和框架最适合构成这一子方向的最小工具栈。

## 推荐先看

- [05-实验执行、复现与评测](../05-实验执行、复现与评测/README.md)
- [05-实验执行、复现与评测/AI-ML-DataMining-Benchmark与公开评测集](../05-实验执行、复现与评测/AI-ML-DataMining-Benchmark与公开评测集.md)
- [92-MCP/实验执行与数据工程MCP](../92-MCP/实验执行与数据工程MCP.md)
- [91-Skills/科研工程与实验Skills](../91-Skills/科研工程与实验Skills.md)

## 最小工具栈

1. `OpenML + OpenML-CC18 + PMLB`
   适合快速拿到标准 tabular 任务集。
2. `AutoGluon / FLAML / auto-sklearn`
   适合建立 AutoML 与手工 baseline 的第一组对照。
3. `Optuna / Ray Tune + YAHPO Gym`
   适合把超参搜索和多保真优化接进实验流程。
4. `MLflow / DVC + Jupyter MCP + GitHub MCP`
   适合记录 runs、数据版本、notebook 与代码变更。

## 一、相关 Skills

| 资源 | 类型 | 更适合的用途 | 链接 |
| --- | --- | --- | --- |
| 科研工程与实验Skills | 仓库内附录 | 训练、评测、追踪与工程自动化主入口。 | [91-Skills/科研工程与实验Skills](../91-Skills/科研工程与实验Skills.md) |
| AI Research SKILLs | 研究工程技能库 | `evaluation`、`mlops`、`observability`、`rag/agents` 等子类适合实验编排。 | [Orchestra-Research/AI-Research-SKILLs](https://github.com/Orchestra-Research/AI-Research-SKILLs) |
| Hugging Face Skills | 官方技能包 | `hf_model_evaluation`、`hf_dataset_creator`、`hf-llm-trainer` 对建立实验闭环很直接。 | [huggingface/skills](https://github.com/huggingface/skills) |
| obra/superpowers | 方法论技能库 | `test-driven-development`、`verification-before-completion` 适合减少实验脚本回归。 | [obra/superpowers](https://github.com/obra/superpowers) |

## 二、相关 MCP

| 资源 | 类型 | 更适合的用途 | 链接 |
| --- | --- | --- | --- |
| Jupyter MCP Server | notebook MCP | 适合运行数据探索、训练、错误分析和结果导出。 | [datalayer/jupyter-mcp-server](https://github.com/datalayer/jupyter-mcp-server) |
| Optuna MCP Server | HPO MCP | 适合 study 管理、trial 查询和优化分析。 | [optuna/optuna-mcp](https://github.com/optuna/optuna-mcp) |
| GitHub MCP Server | 仓库协作 MCP | 适合读取 benchmark 仓库、配置和 CI。 | [github/github-mcp-server](https://github.com/github/github-mcp-server) |
| dbhub | 数据库 MCP | 适合查询 SQLite / Postgres / MySQL 中的实验记录和中间结果。 | [bytebase/dbhub](https://github.com/bytebase/dbhub) |
| Chart MCP Server | 图表 MCP | 适合把搜索轨迹、ablation 和 leaderboard 快速图表化。 | [antvis/mcp-server-chart](https://github.com/antvis/mcp-server-chart) |
| Kaggle MCP | 数据平台 MCP | 适合补比赛数据、tabular 数据和原型任务。 | [arrismo/kaggle-mcp](https://github.com/arrismo/kaggle-mcp) |

## 三、高频框架、benchmark 与平台

| 资源 | 类型 | 更适合的用途 | 链接 |
| --- | --- | --- | --- |
| OpenML | 开放任务平台 | 提供数据、task、run 和 benchmark suite。 | [OpenML](https://openml.io/) |
| OpenML-CC18 | tabular benchmark suite | 经典中小规模分类 benchmark 套件。 | [OpenML Benchmarking Suites](https://docs.openml.org/benchmark/) |
| PMLB | tabular benchmark 数据库 | 适合传统 ML 与 tabular baseline 对照。 | [EpistasisLab/pmlb](https://github.com/EpistasisLab/pmlb) |
| TabArena | living tabular benchmark | 更适合持续维护和追踪 tabular leaderboard。 | [autogluon/tabarena](https://github.com/autogluon/tabarena) |
| AutoMLBenchmark | benchmarking 框架 | 适合系统比较 AutoML workflow。 | [openml/automlbenchmark](https://github.com/openml/automlbenchmark) |
| YAHPO Gym | HPO benchmark gym | 适合多保真搜索与预算敏感优化实验。 | [slds-lmu/yahpo_gym](https://github.com/slds-lmu/yahpo_gym) |
| AutoGluon | AutoML 框架 | 适合 tabular、multimodal、time series 快速 baseline。 | [autogluon/autogluon](https://github.com/autogluon/autogluon) |
| FLAML | 轻量 AutoML 框架 | 适合成本敏感搜索与快速迭代。 | [microsoft/FLAML](https://github.com/microsoft/FLAML) |
| auto-sklearn | AutoML 框架 | 经典 tabular AutoML 基线。 | [automl/auto-sklearn](https://github.com/automl/auto-sklearn) |

## 四、推荐组合

1. `OpenML + OpenML-CC18 + AutoGluon + MLflow`
   适合快速建立第一轮可复现实验。
2. `PMLB + FLAML / auto-sklearn + DVC`
   适合做传统 ML 与 AutoML 对照。
3. `YAHPO Gym + Optuna / Ray Tune + Chart MCP`
   适合做预算约束下的 HPO 分析。
4. `Jupyter MCP + GitHub MCP + dbhub`
   适合做 notebook、代码和结果表联动检查。

## 五、仓库内延伸阅读

- [05-实验执行、复现与评测](../05-实验执行、复现与评测/README.md)
- [98-全局索引/实验与Benchmark索引](../98-全局索引/实验与Benchmark索引.md)
- [98-全局索引/CLI与终端工具索引](../98-全局索引/CLI与终端工具索引.md)
