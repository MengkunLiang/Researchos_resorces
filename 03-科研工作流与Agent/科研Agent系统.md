# 科研 Agent 系统

这一页聚焦“研究型工作流系统”和“科研闭环参考对象”。如果你想搭 `ResearchOS / AutoLab / FlowAssist` 这种系统，这一页是最重要的参考材料之一。

## 1. 直接可用的科研工作台 / 系统

| 资源 | 定位 | 简述 | 链接 |
| --- | --- | --- | --- |
| Open Research | 研究工作台 | 强调 “research director in terminal”，带有 novelty-check、source scout、paper explainer、reviewer response 等能力。 | [open-research.info](https://www.open-research.info/) |
| RTI | 文献工作流系统 | 把“方向输入 -> 检索 -> 摘要点评 -> 选论文 -> 翻译 -> 深度分析”串成完整流程。 | [yrc-better/RTI](https://github.com/yrc-better/RTI) |
| PaperQA2 | 科学文献问答 | 面向科学文献的高精度 RAG，对论文问答、证据引用和总结很实用。 | [Future-House/paper-qa](https://github.com/Future-House/paper-qa) |
| Robin | 科学发现多 Agent | Future House 的科学发现多 Agent 系统，更适合作为“高度自动化”参考对象。 | [Future-House/robin](https://github.com/Future-House/robin) |
| OpenDraft | 学术长文写作系统 | 面向 thesis / paper 的多 Agent 写作框架，适合写作与整理阶段。 | [federicodeponte/academic-thesis-ai](https://github.com/federicodeponte/academic-thesis-ai) |
| AI Co-Scientist | idea 生成系统 | Google Research 的公开系统页面，适合参考“问题提出、反思、排序、证据回查”的架构。 | [Google Research Blog](https://research.google/blog/accelerating-scientific-breakthroughs-with-an-ai-co-scientist/) |

## 2. 闭环自动科研的关键参考对象

| 资源 | 定位 | 简述 | 链接 |
| --- | --- | --- | --- |
| AI-Scientist-v2 | 自主科研闭环 | Sakana AI 的自动科研系统，覆盖从研究方向到实验与写作的完整链路。 | [SakanaAI/AI-Scientist-v2](https://github.com/SakanaAI/AI-Scientist-v2) |
| AI Scientist Nature 页面 | 论文主页 | 更适合从系统级视角理解 AI Scientist 的设计目标和研究叙事。 | [Sakana AI 页面](https://sakana.ai/ai-scientist-nature/) |
| Dolphin | 闭环科研论文 | 强调 `Thinking -> Practice -> Feedback` 的自动科研闭环。 | [ACL Anthology](https://aclanthology.org/2025.acl-long.1056/) |
| ResearchAgent | ideation + reviewing | 在 idea 阶段引入 ReviewingAgents 的思路，适合借鉴审稿人式自纠。 | [ACL Anthology](https://aclanthology.org/2025.naacl-long.342/) |
| VirSci | 多 Agent 研究想法生成 | 强调多 Agent 协作生成、评价、修正 research ideas。 | [ACL Anthology](https://aclanthology.org/2025.acl-long.1368/) |
| HypoGeniC | hypothesis generation | 更偏“从观测数据出发生成并检验假设”的系统范式。 | [项目页](https://chicagohai.github.io/hypogenic-demo/) |
| llm4novelty / NovBench | novelty 评测资源 | 更适合作为 novelty assessment 模块的 benchmark 入口，而不是单纯系统 demo。 | [njust-winchy/llm4novelty](https://github.com/njust-winchy/llm4novelty) |

## 3. novelty / reviewing 这一条线值得单列看

如果你们的核心研究之一是 `idea generation + novelty assessment`，下面这些资源不要只当补充链接，它们本身就可以单独组成一条子系统：

| 资源 | 价值 | 链接 |
| --- | --- | --- |
| llm4novelty | 直接做 novelty assessment benchmark | [njust-winchy/llm4novelty](https://github.com/njust-winchy/llm4novelty) |
| ReviewAdvisor | 审稿与 novelty 结构化参考 | [neulab/ReviewAdvisor](https://github.com/neulab/ReviewAdvisor) |
| NLPeer | 公开 peer review 数据 | [UKPLab/nlpeer](https://github.com/UKPLab/nlpeer) |
| OpenReview | 顶会审稿与讨论入口 | [OpenReview](https://openreview.net/) |

## 4. 适合拆到 ResearchOS 各模块的参考点

| 模块 | 最值得参考的资源 | 为什么 |
| --- | --- | --- |
| 文献普查 | `RTI`、`PaperQA2`、`Open Research` | 这几类项目最能体现“检索 + 精读 + 结构化整理”的实际价值。 |
| idea 与 novelty | `AI Co-Scientist`、`llm4novelty`、`ResearchAgent`、`VirSci` | 更适合借鉴“如何让系统自己找空白、再做审计”的机制。 |
| 自主闭环 | `AI-Scientist-v2`、`Dolphin` | 适合借鉴状态机、反馈回路、实验修正逻辑。 |
| 写作与答辩 | `OpenDraft`、`Open Research` | 更适合后半程的论文输出、review response 和转投辅助。 |

## 5. 我的建议

如果你要做一个真正可落地的 ResearchOS，不建议把某一个现成系统整包照搬，而是更适合这样组合：

1. 用 `RTI + PaperQA2 + arxiv-translator` 搭文献层
2. 用 `OpenReview MCP + OpenAlex MCP` 搭 novelty / latest paper 层
3. 用 `AI-Scientist-v2 / Dolphin / AI Co-Scientist / ResearchAgent / VirSci` 提供闭环机制参考
4. 用 `OpenDraft + Auto-Resubmit` 处理写作与投稿末端

也就是说，比较稳的路线通常不是“找一个全能系统”，而是“拆出最强的几段链路自己拼”。

如果你要继续深挖这个方向，建议同时看专题页：
[科研新颖性与Idea生成](../09-方向专题/科研新颖性与Idea生成.md)
