# 评测与 Benchmark

科研智能体不只要“看起来很聪明”，还要能被评估。下面这些资源适合用来搭建 benchmark、回归测试与持续评测体系。

## 1. 科研 / 研究工程相关 Benchmark

| 资源 | 类型 | 简述 | 链接 |
| --- | --- | --- | --- |
| MLE-bench | ML engineering benchmark | 强调真实 ML 工程任务与 Kaggle 风格问题，对科研实验能力评估很有价值。 | [OpenAI - MLE-bench](https://openai.com/index/mle-bench/) |
| MLGym | ML research benchmark | 更直接面向机器学习研究任务与 research agent，对 AI/ML 团队很值得单独跟进。 | [MLGym 项目页](https://sites.google.com/view/mlgym) |
| Aviary | Agent 环境基座 | Future House 的 language agent gym，含科学文献搜索与 notebook 环境。 | [Future-House/aviary](https://github.com/Future-House/aviary) |
| LAB-Bench | 科学研究 benchmark | 面向生物科学研究能力的评测集，也适合作为科研 agent 评测参考。 | [Future-House/LAB-Bench](https://github.com/Future-House/LAB-Bench) |
| OpenML | 开放 benchmark 平台 | 提供标准化数据集、任务、runs 和 suites，适合建立可复现对照基线。 | [OpenML](https://openml.io/) |

## 2. 通用模型 / RAG / Agent 评测资源

| 资源 | 类型 | 简述 | 链接 |
| --- | --- | --- | --- |
| OpenCompass | 大模型评测平台 | 中文社区比较常用，适合做基准评估与任务对比。 | [open-compass/opencompass](https://github.com/open-compass/opencompass) |
| lm-evaluation-harness | 语言模型评测 | 经典的 LLM benchmark 执行框架。 | [EleutherAI/lm-evaluation-harness](https://github.com/EleutherAI/lm-evaluation-harness) |
| Ragas | RAG 评测 | 对文献问答、知识库检索和 RAG 系统评测很有参考价值。 | [explodinggradients/ragas](https://github.com/explodinggradients/ragas) |
| HELM | 评测框架 | 更适合理解综合评测设计和多任务基线。 | [stanford-crfm/helm](https://github.com/stanford-crfm/helm) |
| Papers with Code SOTA | 公开榜单 | 适合做外部 baseline 对照和任务标准追踪。 | [Papers with Code SOTA](https://paperswithcode.com/sota) |

## 3. AI / ML / Data Mining 常用 benchmark 入口

| 方向 | 资源 | 为什么值得收录 | 链接 |
| --- | --- | --- | --- |
| 图学习 | OGB | graph ML 最通用的 benchmark 入口之一。 | [snap-stanford/ogb](https://github.com/snap-stanford/ogb) |
| 图鲁棒性 | GRB | 适合做 graph robustness / adversarial 评测。 | [THUDM/grb](https://github.com/THUDM/grb) |
| 检索 / RAG | BEIR | 对检索器、reranker、RAG retrieval 都很重要。 | [beir-cellar/beir](https://github.com/beir-cellar/beir) |
| 推荐系统 | RecBole | 除了训练框架，本身也适合做 recommender benchmark 基线复现。 | [RUCAIBox/RecBole](https://github.com/RUCAIBox/RecBole) |
| 治疗科学 / AI for Science | TDC | 如果有 health / drug / bio 方向，这个值得优先收录。 | [mims-harvard/TDC](https://github.com/mims-harvard/TDC) |

## 4. novelty / 审稿 / idea generation 的评测入口

| 资源 | 类型 | 简述 | 链接 |
| --- | --- | --- | --- |
| llm4novelty / NovBench | novelty benchmark | 专门针对学术新颖性判断，适合做 idea / novelty 系统基线与评测。 | [njust-winchy/llm4novelty](https://github.com/njust-winchy/llm4novelty) |
| ReviewAdvisor | scientific reviewing | 可作为 novelty、significance、weakness 等 review 维度的参考基线。 | [neulab/ReviewAdvisor](https://github.com/neulab/ReviewAdvisor) |
| NLPeer | peer review dataset | 公开 peer review 数据资源，适合做 review mining 和审稿结构分析。 | [UKPLab/nlpeer](https://github.com/UKPLab/nlpeer) |
| OpenReview | 公开审稿平台 | 顶会审稿过程和版本演化的真实数据入口。 | [OpenReview](https://openreview.net/) |

## 5. 科研工作流的评测建议

### 至少做三类评测

1. 文献理解质量
2. 研究工程执行质量
3. Agent 工作流稳定性
4. novelty 判断与 reviewer-style critique 质量

### 对应可以参考的资源

- 文献理解：`PaperQA2` 风格问答、人工标注 claim 集
- 工程执行：`MLE-bench`、`MLGym`
- 工作流稳定性：`Aviary`
- novelty / 审稿：`llm4novelty`、`NLPeer`、`OpenReview`

## 6. 更实用的落地方式

不要一开始就想做一个巨大的 benchmark 平台，建议按下面顺序来：

1. 先做 10 到 20 个内部黄金任务
2. 再引入 `MLE-bench / MLGym / Aviary / Ragas`
3. 如果目标包含 idea / novelty，再补 `llm4novelty / NLPeer / OpenReview`
4. 对 AI/ML/data mining 方向，再逐步补 `OpenML / OGB / BEIR / RecBole`
5. 最后再把 benchmark 和 CI、回归测试绑起来

这样最容易真正形成持续迭代的评测闭环。

补充专题页：
[AI-ML-DataMining资源](../09-方向专题/AI-ML-DataMining资源.md)
