# Causal / Anomaly 与 Data-Centric AI

这一页聚焦因果推断、因果发现、异常检测以及 `data-centric AI`。适合处理“机制识别是否可信”“异常模式是否稳健”“数据质量与性能如何评估”这类问题。

## 这一步通常要回答的问题

1. 异常检测、图异常与鲁棒性任务应当从哪些 benchmark 开始。
2. 因果推断、因果发现和异质性效应估计应当优先采用哪些框架。
3. 数据质量、数据选择和系统性能应当如何纳入实验评测。
4. 哪些 `Skills`、`MCP` 和公开数据平台最适合这一子方向。

## 推荐先看

- [05-实验执行、复现与评测](../05-实验执行、复现与评测/README.md)
- [08-方向专题/Computational-Design-Science与管理技术交叉](./Computational-Design-Science与管理技术交叉.md)
- [92-MCP/实验执行与数据工程MCP](../92-MCP/实验执行与数据工程MCP.md)
- [91-Skills/科研工程与实验Skills](../91-Skills/科研工程与实验Skills.md)

## 最小工具栈

1. `PyOD / PyGOD + ADBench`
   适合异常检测与图异常基线。
2. `DoWhy / causal-learn / EconML / DoubleML`
   适合因果推断、因果发现和异质性效应估计。
3. `DataPerf / MLPerf`
   适合把数据质量和系统性能维度加进评测。
4. `Jupyter MCP + dbhub + Chart MCP`
   适合分析、查询和结果展示。

## 一、相关 Skills

| 资源 | 类型 | 更适合的用途 | 链接 |
| --- | --- | --- | --- |
| 科研工程与实验Skills | 仓库内附录 | 训练、评测、追踪和实验工程主入口。 | [91-Skills/科研工程与实验Skills](../91-Skills/科研工程与实验Skills.md) |
| 科学计算与领域Skills | 仓库内附录 | 统计、分析、科学计算与领域数据技能入口。 | [91-Skills/科学计算与领域Skills](../91-Skills/科学计算与领域Skills.md) |
| Claude Scientific Skills | 科研技能总库 | `statsmodels`、`dask`、`polars` 等分析型技能适合数据中心实验。 | [K-Dense-AI/claude-scientific-skills](https://github.com/K-Dense-AI/claude-scientific-skills) |
| obra/superpowers | 方法论技能库 | 适合把验证、debug 与实验回归变成固定工作流。 | [obra/superpowers](https://github.com/obra/superpowers) |

## 二、相关 MCP

| 资源 | 类型 | 更适合的用途 | 链接 |
| --- | --- | --- | --- |
| Jupyter MCP Server | notebook MCP | 因果与异常实验的主执行入口。 | [datalayer/jupyter-mcp-server](https://github.com/datalayer/jupyter-mcp-server) |
| dbhub | 数据库 MCP | 适合读写实验结果表、日志表和分析数据。 | [bytebase/dbhub](https://github.com/bytebase/dbhub) |
| GitHub MCP Server | 仓库协作 MCP | 适合读取 benchmark 仓库、实现与 CI。 | [github/github-mcp-server](https://github.com/github/github-mcp-server) |
| Chart MCP Server | 图表 MCP | 适合展示 ROC、PR、ATE/CATE 和 ablation 结果。 | [antvis/mcp-server-chart](https://github.com/antvis/mcp-server-chart) |
| OpenAlex MCP / Paper Search MCP | 文献检索 MCP | 适合补因果、异常与 data-centric AI 的论文线索。 | [hbiaou/openalex-mcp](https://github.com/hbiaou/openalex-mcp)、[openags/paper-search-mcp](https://github.com/openags/paper-search-mcp) |

## 三、高频框架、benchmark 与平台

| 资源 | 类型 | 更适合的用途 | 链接 |
| --- | --- | --- | --- |
| PyOD | 异常检测工具箱 | 建立 outlier / anomaly detection 稳定 baseline。 | [yzhao062/pyod](https://github.com/yzhao062/pyod) |
| PyGOD | 图异常检测 | 图异常、欺诈、风控与 relational anomaly 研究入口。 | [pygod-team/pygod](https://github.com/pygod-team/pygod) |
| ADBench | 异常检测 benchmark | 适合比较异常检测算法、噪声设置和鲁棒性。 | [Minqi824/ADBench](https://github.com/Minqi824/ADBench) |
| DoWhy | 因果推断框架 | 适合把识别、估计和 refutation 写成可追溯流程。 | [py-why/dowhy](https://github.com/py-why/dowhy) |
| causal-learn | 因果发现 | 适合探索变量结构与机制图。 | [py-why/causal-learn](https://github.com/py-why/causal-learn) |
| EconML / DoubleML | 异质性效应与双重机器学习 | 适合 treatment heterogeneity、政策评估与高维因果。 | [py-why/EconML](https://github.com/py-why/EconML)、[DoubleML](https://github.com/DoubleML/doubleml-for-py) |
| CausalBench | 因果 benchmark | 因果发现与因果机制比较的公开 benchmark。 | [ravivanpong/CausalBench](https://github.com/ravivanpong/CausalBench) |
| DataPerf | data-centric AI | 适合补数据质量、数据选择与 dataset-centric 评测。 | [DataPerf](https://www.dataperf.org/) |
| MLPerf | 系统性能 benchmark | 适合补训练与推理性能维度。 | [MLPerf Training](https://mlcommons.org/benchmarks/training/)、[MLPerf Inference](https://mlcommons.org/working-groups/benchmarks/inference/) |

## 四、外部整合入口

| 资源 | 类型 | 更适合的用途 | 链接 |
| --- | --- | --- | --- |
| awesome-causal-inference | 外部合集 | 因果推断论文、工具和资源入口。 | [matteocourthoud/awesome-causal-inference](https://github.com/matteocourthoud/awesome-causal-inference) |
| awesome-data-agents | 外部合集 | data-centric agent、数据处理与分析工作流入口。 | [HKUSTDial/awesome-data-agents](https://github.com/HKUSTDial/awesome-data-agents) |
| HKUST-Got-Skills Resources | 综合资源页 | 可继续补 Jupyter、数据库、CLI、Git 和实验工具。 | [HKUST-Got-Skills Resources](https://giggleliu.github.io/HKUST-Got-Skills/resources) |

## 五、推荐组合

1. `PyOD / PyGOD + ADBench + MLflow`
   适合异常检测、图异常与可比评测。
2. `DoWhy + causal-learn + EconML / DoubleML`
   适合因果机制、因果发现和异质性效应研究。
3. `DataPerf + MLPerf + DVC`
   适合把数据与系统性能维度纳入实验闭环。
4. `Jupyter MCP + dbhub + Chart MCP`
   适合分析、查询和结果可视化。

## 六、仓库内延伸阅读

- [05-实验执行、复现与评测](../05-实验执行、复现与评测/README.md)
- [08-方向专题/Computational-Design-Science与管理技术交叉](./Computational-Design-Science与管理技术交叉.md)
- [98-全局索引/实验与Benchmark索引](../98-全局索引/实验与Benchmark索引.md)
