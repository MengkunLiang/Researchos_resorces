# Graph / Retrieval / Recsys 与 Data Mining

这一页聚焦图学习、知识图谱、检索、embedding、推荐系统和结构化数据挖掘。适合建立图、检索与推荐方向的统一入口，减少在不同框架和 benchmark 之间来回跳转。

## 这一步通常要回答的问题

1. 图学习、检索、推荐和结构化 mining 各自最稳定的 benchmark 是什么。
2. 哪些框架适合做研究原型，哪些适合做标准化评测。
3. 哪些 `Skills`、`MCP` 和工作流最适合图、检索和推荐方向。
4. 哪些公开合集值得继续扫库和补充子方向页面。

## 推荐先看

- [05-实验执行、复现与评测](../05-实验执行、复现与评测/README.md)
- [92-MCP/实验执行与数据工程MCP](../92-MCP/实验执行与数据工程MCP.md)
- [92-MCP/文献检索与知识库MCP](../92-MCP/文献检索与知识库MCP.md)
- [91-Skills/科研工程与实验Skills](../91-Skills/科研工程与实验Skills.md)

## 最小工具栈

1. `PyTorch Geometric / DGL + OGB`
   适合快速建立图学习与图挖掘基线。
2. `Pyserini + BEIR + MTEB`
   适合检索、embedding 与 RAG retrieval 评测。
3. `RecBole / Cornac`
   适合推荐系统算法与评测流程。
4. `Jupyter MCP + GitHub MCP + OpenAlex MCP`
   适合实验、代码基线和论文线索联动。

## 一、相关 Skills

| 资源 | 类型 | 更适合的用途 | 链接 |
| --- | --- | --- | --- |
| 科研工程与实验Skills | 仓库内附录 | 训练、评测、追踪和实验工程的主入口。 | [91-Skills/科研工程与实验Skills](../91-Skills/科研工程与实验Skills.md) |
| 科学计算与领域Skills | 仓库内附录 | `torch-geometric`、科学计算与数据分析相关技能入口。 | [91-Skills/科学计算与领域Skills](../91-Skills/科学计算与领域Skills.md) |
| Claude Scientific Skills | 科研技能总库 | 含 `torch-geometric`、`dask`、`polars` 等数据与图相关技能。 | [K-Dense-AI/claude-scientific-skills](https://github.com/K-Dense-AI/claude-scientific-skills) |
| AI Research SKILLs | 研究工程技能库 | 适合图学习实验、检索 pipeline 和工程执行。 | [Orchestra-Research/AI-Research-SKILLs](https://github.com/Orchestra-Research/AI-Research-SKILLs) |

## 二、相关 MCP

| 资源 | 类型 | 更适合的用途 | 链接 |
| --- | --- | --- | --- |
| Jupyter MCP Server | notebook MCP | 图学习、检索实验与分析主入口。 | [datalayer/jupyter-mcp-server](https://github.com/datalayer/jupyter-mcp-server) |
| GitHub MCP Server / GitMCP | 仓库与代码 MCP | 适合读取 benchmark 仓库、基线代码和 issue。 | [github/github-mcp-server](https://github.com/github/github-mcp-server)、[idosal/git-mcp](https://github.com/idosal/git-mcp) |
| OpenAlex MCP / Paper Search MCP | 文献与 benchmark 检索 MCP | 适合补 benchmark 论文、任务设定与最新工作。 | [hbiaou/openalex-mcp](https://github.com/hbiaou/openalex-mcp)、[openags/paper-search-mcp](https://github.com/openags/paper-search-mcp) |
| Chart MCP Server | 图表 MCP | 适合可视化召回、排序、embedding 和推荐结果。 | [antvis/mcp-server-chart](https://github.com/antvis/mcp-server-chart) |

## 三、高频框架、benchmark 与平台

| 资源 | 类型 | 更适合的用途 | 链接 |
| --- | --- | --- | --- |
| PyTorch Geometric | 图学习框架 | GNN、heterogeneous graph、graph mining 高频底座。 | [pyg-team/pytorch_geometric](https://github.com/pyg-team/pytorch_geometric) |
| DGL | 图学习框架 | 图训练与工程化实验的主流底座之一。 | [dmlc/dgl](https://github.com/dmlc/dgl) |
| OGB | graph benchmark | 图学习 benchmark 主入口。 | [snap-stanford/ogb](https://github.com/snap-stanford/ogb) |
| GRB | graph robustness benchmark | 适合补图鲁棒性与对抗评测。 | [THUDM/grb](https://github.com/THUDM/grb) |
| PyKEEN | 知识图谱表示学习 | KGE、link prediction 与知识图谱研究。 | [pykeen/pykeen](https://github.com/pykeen/pykeen) |
| Pyserini | 检索研究工具箱 | dense / sparse retrieval、reranking 与 IR 实验底座。 | [castorini/pyserini](https://github.com/castorini/pyserini) |
| BEIR | 检索 benchmark | 跨域 IR 和 RAG retriever 评测。 | [beir-cellar/beir](https://github.com/beir-cellar/beir) |
| MTEB | embedding benchmark | 表征学习、语义检索和 embedding 评测。 | [embeddings-benchmark/mteb](https://github.com/embeddings-benchmark/mteb) |
| RecBole | 推荐系统框架 | 推荐算法、数据处理和评测流程的主流底座。 | [RUCAIBox/RecBole](https://github.com/RUCAIBox/RecBole) |
| Cornac | 推荐系统框架 | 更偏研究原型、多模态推荐和对照实验。 | [PreferredAI/cornac](https://github.com/PreferredAI/cornac) |

## 四、外部整合入口

| 资源 | 类型 | 更适合的用途 | 链接 |
| --- | --- | --- | --- |
| awesome-RecSys | 外部合集 | 推荐系统资源、项目与论文入口。 | [wusw14/awesome-recsys](https://github.com/wusw14/awesome-recsys) |
| Toolathlon | 外部合集 | 工具使用 benchmark 和 agent 任务入口。 | [hkust-nlp/Toolathlon](https://github.com/hkust-nlp/Toolathlon) |
| AgentBoard | 外部合集 | agent 评测与任务维度补充。 | [hkust-nlp/AgentBoard](https://github.com/hkust-nlp/AgentBoard) |
| HKUST-Got-Skills Resources | 综合资源页 | 可继续补 literature、Jupyter、CLI 与工具层。 | [HKUST-Got-Skills Resources](https://giggleliu.github.io/HKUST-Got-Skills/resources) |

## 五、推荐组合

1. `PyG / DGL + OGB + MLflow`
   适合图学习、异构图和图挖掘实验。
2. `Pyserini + BEIR + MTEB + Chart MCP`
   适合检索、embedding 与 RAG retrieval 评测。
3. `RecBole / Cornac + GitHub MCP`
   适合推荐系统 baseline 与仓库对照。
4. `OpenAlex MCP + Paper Search MCP + GitMCP`
   适合补 benchmark 论文、代码仓库和最新工作。

## 六、仓库内延伸阅读

- [05-实验执行、复现与评测](../05-实验执行、复现与评测/README.md)
- [98-全局索引/实验与Benchmark索引](../98-全局索引/实验与Benchmark索引.md)
- [08-方向专题/AI-ML-DataMining资源](./AI-ML-DataMining资源.md)
