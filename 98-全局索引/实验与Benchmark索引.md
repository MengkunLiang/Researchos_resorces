# 实验与 Benchmark 索引

## 先看哪些任务模块

- [05-实验执行、复现与评测](../05-实验执行、复现与评测/README.md)
- [04-新颖性判断与综述](../04-新颖性判断与综述/README.md)
- [07-安全与治理](../07-安全与治理/README.md)

## 类型附录详细页

- [96-实验与评测/实验执行与复现](../96-实验与评测/实验执行与复现.md)
- [96-实验与评测/评测与Benchmark](../96-实验与评测/评测与Benchmark.md)
- [05-实验执行、复现与评测/实验框架、追踪与复现工具详表](../05-实验执行、复现与评测/实验框架、追踪与复现工具详表.md)
- [05-实验执行、复现与评测/AI-ML-DataMining-Benchmark与公开评测集](../05-实验执行、复现与评测/AI-ML-DataMining-Benchmark与公开评测集.md)

## 高频公开资源

| 资源 | 类型 | 简述 | 链接 |
| --- | --- | --- | --- |
| MLE-bench | ML engineering benchmark | 适合评测 AI 代理的 ML 工程能力。 | [OpenAI - MLE-bench](https://openai.com/index/mle-bench/) |
| MLGym | ML research benchmark | 适合评测开放式机器学习研究任务。 | [facebookresearch/MLGym](https://github.com/facebookresearch/MLGym) |
| MLR-Bench | open-ended ML research benchmark | 适合评测 idea、proposal、experiment 到 paper 的开放研究能力。 | [chchenhui/mlrbench](https://github.com/chchenhui/mlrbench) |
| FML-bench | automatic ML research benchmark | 适合评测自动 ML 研究代理的探索广度。 | [qrzou/FML-bench](https://github.com/qrzou/FML-bench) |
| LiveDRBench | deep research benchmark | 适合评测 deep research 与 claim discovery。 | [microsoft/livedrbench](https://github.com/microsoft/livedrbench) |
| OpenHands Benchmarks | 评测 harness | 适合补软件代理与执行类评测。 | [OpenHands/benchmarks](https://github.com/OpenHands/benchmarks) |
| OpenCompass / lm-eval-harness / LightEval | 通用评测框架 | 适合多模型、多数据集、RAG 和 agent eval 统一执行。 | [open-compass/opencompass](https://github.com/open-compass/opencompass)、[EleutherAI/lm-evaluation-harness](https://github.com/EleutherAI/lm-evaluation-harness)、[huggingface/lighteval](https://github.com/huggingface/lighteval) |
| OpenML / OpenML-CC18 / PMLB / TabArena | tabular benchmark | 适合 tabular、AutoML、dataset suite 和可复现实验对照。 | [OpenML](https://openml.io/)、[OpenML Benchmarking Suites](https://docs.openml.org/benchmark/)、[EpistasisLab/pmlb](https://github.com/EpistasisLab/pmlb)、[autogluon/tabarena](https://github.com/autogluon/tabarena) |
| YAHPO Gym / AutoMLBenchmark | HPO 与 AutoML benchmark | 适合做多保真 HPO、AutoML 系统对照和复现实验。 | [slds-lmu/yahpo_gym](https://github.com/slds-lmu/yahpo_gym)、[openml/automlbenchmark](https://github.com/openml/automlbenchmark) |
| OGB | graph benchmark | 图学习 benchmark 主入口之一。 | [snap-stanford/ogb](https://github.com/snap-stanford/ogb) |
| BEIR / MTEB / RecBole | retrieval / embedding / recommender benchmark | 适合检索、表示学习、RAG retrieval 与推荐系统评测。 | [beir-cellar/beir](https://github.com/beir-cellar/beir)、[embeddings-benchmark/mteb](https://github.com/embeddings-benchmark/mteb)、[RUCAIBox/RecBole](https://github.com/RUCAIBox/RecBole) |
| LiveCodeBench / BigCodeBench / DS-1000 | 代码与数据科学 benchmark | 适合评测 coding、数据科学代码和代理执行能力。 | [LiveCodeBench/LiveCodeBench](https://github.com/LiveCodeBench/LiveCodeBench)、[bigcode-project/bigcodebench](https://github.com/bigcode-project/bigcodebench)、[xlang-ai/DS-1000](https://github.com/xlang-ai/DS-1000) |
| ADBench / CausalBench | anomaly / causal benchmark | 适合异常检测与因果发现方向的可比评测。 | [Minqi824/ADBench](https://github.com/Minqi824/ADBench)、[ravivanpong/CausalBench](https://github.com/ravivanpong/CausalBench) |
| DataPerf / MLPerf | data-centric 与系统性能 benchmark | 适合补 dataset-centric AI、训练性能和推理性能维度。 | [DataPerf](https://www.dataperf.org/)、[MLPerf Training](https://mlcommons.org/benchmarks/training/)、[MLPerf Inference](https://mlcommons.org/working-groups/benchmarks/inference/) |

## 按子方向快查

| 子方向 | 更适合先看 | 高频资源 |
| --- | --- | --- |
| Tabular / AutoML / HPO | [08-方向专题/Tabular-AutoML与HPO](../08-方向专题/Tabular-AutoML与HPO.md) | `OpenML`、`OpenML-CC18`、`PMLB`、`TabArena`、`YAHPO Gym` |
| Graph / Retrieval / Recsys | [08-方向专题/Graph-Retrieval-Recsys与DataMining](../08-方向专题/Graph-Retrieval-Recsys与DataMining.md) | `OGB`、`PyG`、`BEIR`、`MTEB`、`RecBole` |
| Causal / Anomaly / Data-Centric AI | [08-方向专题/Causal-Anomaly与Data-Centric-AI](../08-方向专题/Causal-Anomaly与Data-Centric-AI.md) | `PyOD`、`ADBench`、`DoWhy`、`CausalBench`、`DataPerf` |
| 研究代理与自动化实验 | [05-实验执行、复现与评测](../05-实验执行、复现与评测/README.md) | `MLE-bench`、`MLGym`、`MLR-Bench`、`FML-bench`、`OpenHands Benchmarks` |

## 常用配套入口

- [92-MCP/实验执行与数据工程MCP](../92-MCP/实验执行与数据工程MCP.md)
- [98-全局索引/CLI与终端工具索引](./CLI与终端工具索引.md)
- [91-Skills/科研工程与实验Skills](../91-Skills/科研工程与实验Skills.md)

## 推荐配合使用

- [98-全局索引/Agent与工作流索引](./Agent与工作流索引.md)
- [92-MCP/实验执行与数据工程MCP](../92-MCP/实验执行与数据工程MCP.md)
- [09-按科研任务导航/实验执行、复现与评测](../09-按科研任务导航/实验执行、复现与评测.md)
