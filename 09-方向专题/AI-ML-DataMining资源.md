# AI / ML / Data Mining 资源

这一页专门补 AI、ML、data mining 方向的高频开源资源。目标不是做“全领域百科”，而是挑那些最适合接进科研团队日常工作流的公共资源、框架、benchmark 和数据入口。

## 1. 研究自动化与 ML 研究 Agent

| 资源 | 类型 | 简述 | 链接 |
| --- | --- | --- | --- |
| MLE-bench | ML engineering benchmark | 真实感很强的 ML 工程 benchmark，适合评估 agent 是否真的能做实验、调参、修 bug、提分。 | [OpenAI - MLE-bench](https://openai.com/index/mle-bench/) |
| MLGym | AI research agent benchmark | 专门面向机器学习研究任务的评测框架，适合对比不同 research agent。 | [MLGym 项目页](https://sites.google.com/view/mlgym) |
| OpenML | 开放 ML 平台 | 提供开放数据、任务、runs 和 benchmark suites，特别适合做可复现实验和基线复用。 | [OpenML](https://openml.io/)、[OpenML Docs](https://docs.openml.org/) |
| AutoGluon | AutoML 框架 | 对 tabular、multimodal 等任务很友好，适合快速建一个可靠 baseline。 | [autogluon/autogluon](https://github.com/autogluon/autogluon) |

## 2. 图学习、知识图谱与结构化数据挖掘

| 资源 | 类型 | 简述 | 链接 |
| --- | --- | --- | --- |
| PyTorch Geometric | 图学习框架 | 做 GNN、graph mining、heterogeneous graph 实验时最常用的底座之一。 | [pyg-team/pytorch_geometric](https://github.com/pyg-team/pytorch_geometric) |
| DGL | 图学习框架 | 另一个主流图学习框架，工程化和生态也很完整。 | [dmlc/dgl](https://github.com/dmlc/dgl) |
| Open Graph Benchmark | 图学习 benchmark | 标准化 graph benchmark、数据加载器和 evaluator，做 graph ML 几乎绕不开。 | [snap-stanford/ogb](https://github.com/snap-stanford/ogb) |
| GRB | graph robustness benchmark | 更偏图模型鲁棒性与对抗评测，适合做高质量 graph benchmark 扩展。 | [THUDM/grb](https://github.com/THUDM/grb) |
| PyKEEN | 知识图谱表示学习 | 做 knowledge graph embeddings、link prediction 时很常见。 | [pykeen/pykeen](https://github.com/pykeen/pykeen) |

## 3. 推荐系统、检索与用户行为建模

| 资源 | 类型 | 简述 | 链接 |
| --- | --- | --- | --- |
| RecBole | 推荐系统框架 | 中文社区和学术界都很常用，覆盖大量推荐算法与评测流程。 | [RUCAIBox/RecBole](https://github.com/RUCAIBox/RecBole) |
| Cornac | 推荐系统框架 | 更偏研究原型和多模态推荐，适合快速做对比实验。 | [PreferredAI/cornac](https://github.com/PreferredAI/cornac) |
| Pyserini | 检索研究工具箱 | 信息检索、dense/sparse retrieval、reranking 实验很常用。 | [castorini/pyserini](https://github.com/castorini/pyserini) |
| BEIR | 检索 benchmark | 通用 IR benchmark，适合做跨域检索和 RAG retriever 对比。 | [beir-cellar/beir](https://github.com/beir-cellar/beir) |

## 4. 异常检测、风险识别与图异常

| 资源 | 类型 | 简述 | 链接 |
| --- | --- | --- | --- |
| PyOD | 异常检测工具箱 | 经典 outlier / anomaly detection 工具箱，做 data mining 基线非常高效。 | [yzhao062/pyod](https://github.com/yzhao062/pyod) |
| PyGOD | 图异常检测 | 把 anomaly detection 扩展到 graph / relational setting，很适合图数据风控、欺诈、社区异常等任务。 | [pygod-team/pygod](https://github.com/pygod-team/pygod) |

## 5. 因果推断与机制识别

这部分对 `management + technology`、`digital innovation`、`平台治理`、`A/B test`、`政策冲击` 研究尤其重要。

| 资源 | 类型 | 简述 | 链接 |
| --- | --- | --- | --- |
| DoWhy | 因果推断框架 | 强调因果图、假设显式化、识别与 refutation，适合把“研究设计”写进代码。 | [py-why/dowhy](https://github.com/py-why/dowhy) |
| causal-learn | 因果发现 | 更偏从观测数据中学习 causal structure，适合做 exploratory discovery。 | [py-why/causal-learn](https://github.com/py-why/causal-learn) |
| EconML | CATE / treatment effect | 偏异质性处理效应与双重机器学习，在政策评估、用户干预、个性化决策里很实用。 | [py-why/EconML](https://github.com/py-why/EconML) |

## 6. 领域数据与 benchmark 入口

| 资源 | 类型 | 简述 | 链接 |
| --- | --- | --- | --- |
| OpenML Tasks / Suites | benchmark 平台 | tabular ML 做复现实验时非常合适。 | [OpenML](https://openml.io/) |
| OGB | graph benchmark | 图学习 benchmark 入口。 | [OGB](https://github.com/snap-stanford/ogb) |
| TDC | 治疗科学 benchmark | 如果团队有 AI for Science / health / drug discovery 方向，这个非常值得系统收录。 | [mims-harvard/TDC](https://github.com/mims-harvard/TDC) |
| Papers with Code | 任务与榜单 | 适合追 benchmark、任务定义、SOTA baseline 和论文代码。 | [Papers with Code](https://paperswithcode.com/) |

## 7. 适合你们团队的三条组合路线

### 路线 A：经典 AI/ML 实验链

1. `OpenML + AutoGluon + MLflow + DVC`
2. 先做稳定 baseline
3. 再把 agent 接进调参、复现、结果汇总

### 路线 B：data mining / 图 / 推荐链

1. `PyG / DGL + OGB`
2. `RecBole / PyKEEN / PyGOD`
3. 用 `MLGym / MLE-bench` 做 agent 化评测

### 路线 C：管理技术交叉的机制识别链

1. `OpenML / 行为数据 / 平台日志`
2. `DoWhy + causal-learn + EconML`
3. 再接 `OpenAlex / PatentsView / Lens` 做知识与创新外部数据拼接

## 8. 收录时我特别建议优先看的标准

1. 有没有标准化 evaluator 和 benchmark split
2. 有没有长期维护的文档和 examples
3. 能不能和 `MLflow / DVC / Jupyter / Hydra` 接起来
4. 对 agent 来说，能不能转成稳定的“工具调用接口”

对科研团队来说，真正高价值的资源不是“功能最多”，而是“更容易做复现、评测、对照和持续积累”。
