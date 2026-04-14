# Computational Design Science 与管理技术交叉

这一页面向你特别强调的方向：`AI / analytics / data mining` 和 `management / IS / digital innovation / decision support` 的交叉研究。这里的重点不是单一算法库，而是那些能支撑“问题发现、机制识别、实验设计、创新测量、证据组织”的公共资源。

## 1. 这类研究通常最需要的四层资源

1. 开放学术与创新数据
2. 因果识别与解释工具
3. 行为实验与在线实验工具
4. 文献到创新再到结果变量的跨源拼接能力

## 2. 开放学术、创新与社会技术数据源

| 资源 | 类型 | 为什么值得收录 | 链接 |
| --- | --- | --- | --- |
| OpenAlex | 学术图谱 API | 做研究主题演化、引用网络、作者机构合作、领域扩散很实用。 | [OpenAlex](https://openalex.org/) |
| Semantic Scholar API | 学术 API | 对 citation、paper metadata、embedding 辅助任务很有价值。 | [Semantic Scholar API](https://www.semanticscholar.org/product/api) |
| Crossref REST API | DOI / 元数据 | 适合补论文元数据、引用信息、出版信息。 | [Crossref REST API](https://www.crossref.org/documentation/retrieve-metadata/rest-api/) |
| OpenReview | 会议过程数据 | 如果你研究 AI 社区、审稿机制、idea 演化、学术组织行为，这个非常重要。 | [OpenReview](https://openreview.net/) |
| OSF API | 开放科学平台 | 适合接 preregistration、开放材料、项目结构化元数据。 | [developer.osf.io](https://developer.osf.io/) |
| PatentsView / USPTO PatentSearch API | 专利与创新数据 | 做创新扩散、知识重组、技术融合、发明人网络时非常重要。注意 PatentsView 已在 2025-05-01 停用 Legacy API，并计划于 2026-03-20 迁移到 USPTO Open Data Portal。 | [PatentsView APIs](https://patentsview.org/apis/api-endpoints) |
| The Lens | 专利 + 学术联动平台 | 做“论文到专利”的知识流动、技术转化和创新映射很实用。 | [The Lens](https://www.lens.org/) |
| GDELT Project | 全球事件与媒体数据 | 如果研究数字平台、政策冲击、AI 舆情、产业事件扩散，这个是常见外部数据层。 | [GDELT Project](https://www.gdeltproject.org/) |

## 3. 机制识别与解释性方法工具

| 资源 | 类型 | 简述 | 链接 |
| --- | --- | --- | --- |
| DoWhy | 因果推断 | 最适合把识别假设、估计、refutation 写成可追溯流程。 | [py-why/dowhy](https://github.com/py-why/dowhy) |
| EconML | 异质性效应 | 适合研究不同用户、组织或平台情境下的 treatment heterogeneity。 | [py-why/EconML](https://github.com/py-why/EconML) |
| causal-learn | 因果发现 | 适合探索变量结构和潜在机制图。 | [py-why/causal-learn](https://github.com/py-why/causal-learn) |
| statsmodels | 统计建模 | 经典、稳健、论文里最容易解释。 | [statsmodels](https://www.statsmodels.org/) |
| linearmodels | panel / IV / DID | 做面板、工具变量、固定效应、事件研究时非常常见。 | [linearmodels](https://bashtage.github.io/linearmodels/) |
| PyMC | 贝叶斯建模 | 适合机制不确定、层级模型、多源先验融合。 | [PyMC](https://www.pymc.io/) |

## 4. 文本、主题、网络与知识结构分析

| 资源 | 类型 | 简述 | 链接 |
| --- | --- | --- | --- |
| BERTopic | 主题建模 | 很适合做研究主题演化、专利主题聚类、评论主题归纳。 | [MaartenGr/BERTopic](https://github.com/MaartenGr/BERTopic) |
| Gensim | 文本挖掘 | 经典 topic modeling / vector space 工具。 | [piskvorky/gensim](https://github.com/piskvorky/gensim) |
| sentence-transformers | 表征学习 | 做 semantic similarity、clustering、idea/patent/paper 匹配都很实用。 | [UKPLab/sentence-transformers](https://github.com/UKPLab/sentence-transformers) |
| NetworkX | 网络分析 | 对引文网络、合作网络、创新扩散网络很方便。 | [networkx/networkx](https://github.com/networkx/networkx) |
| igraph | 大规模网络 | 数据更大时常比 NetworkX 更稳。 | [igraph/python-igraph](https://github.com/igraph/python-igraph) |

## 5. 行为实验、在线实验与设计科学原型

| 资源 | 类型 | 简述 | 链接 |
| --- | --- | --- | --- |
| oTree | 在线实验平台 | 做行为实验、平台机制实验、激励设计实验时很常用。 | [oTree](https://www.otree.org/)、[oTree-org/oTree](https://github.com/oTree-org/oTree) |
| jsPsych | Web 实验框架 | 做用户行为、认知实验、人机交互实验都很轻便。 | [jsPsych](https://www.jspsych.org/)、[jspsych/jsPsych](https://github.com/jspsych/jsPsych) |
| lab.js | 浏览器实验工具 | 偏设计实验原型和可视化构建，适合快速试验。 | [lab.js](https://lab.js.org/)、[FelixHenninger/lab.js](https://github.com/FelixHenninger/lab.js) |
| PsychoPy | 心理/行为实验 | 更偏本地实验与可控实验流程。 | [psychopy/psychopy](https://github.com/psychopy/psychopy) |

## 6. 如果你们做 UTD 风格管理技术交叉研究，可以重点关注的三条链

### 链路 A：创新与知识重组

1. `OpenAlex + Lens + PatentsView`
2. `BERTopic + sentence-transformers + NetworkX`
3. `DoWhy / linearmodels`

适合研究：

- 技术融合与知识重组
- 论文到专利的知识转移
- 创新扩散、组织学习、领域收敛

### 链路 B：平台治理与用户行为

1. 平台日志 / 用户行为数据
2. `jsPsych / oTree / lab.js`
3. `statsmodels + DoWhy + EconML`

适合研究：

- AI 辅助决策
- 平台激励与治理
- 推荐、排序、解释对用户行为的影响

### 链路 C：开放科学与科研组织

1. `OpenReview + OpenAlex + OSF`
2. `llm4novelty + NLPeer + ReviewAdvisor`
3. `NetworkX + topic modeling + causal inference`

适合研究：

- 审稿机制与创新筛选
- 学术社区协作网络
- AI 如何改变科研生产流程

## 7. 对 design science 团队更实用的仓库建设建议

不要只收算法库，建议把专题资源按下面三层维护：

1. `Data Layer`
   OpenAlex、OpenReview、PatentsView、Lens、GDELT、OSF
2. `Method Layer`
   BERTopic、DoWhy、EconML、NetworkX、linearmodels
3. `Intervention Layer`
   oTree、jsPsych、lab.js、PsychoPy、MCP/Agent 工具链

这样以后无论你们研究的是 AI 采纳、数字平台、创新扩散还是科研组织行为，都能很快拼出一条可执行 pipeline。
