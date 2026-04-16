# 按科研任务导航

这一模块是“真正按任务使用仓库”的入口层。`01-08` 更偏资源正文与专题深挖，`09` 更适合回答另一类问题：当前处在科研流程的哪一步，接下来最应该先看哪些页、先接哪些 `Skills / MCP / agent / benchmark / 模板`，以及完成这一阶段后应当转向哪里。

## 一、先判断当前处在哪一步

| 当前状态 | 更适合先进入 | 主要目标 |
| --- | --- | --- |
| 只有模糊兴趣，还没有清晰问题 | [课题扫描与选题](./课题扫描与选题.md) | 扫方向、缩小问题空间、形成候选切口。 |
| 已经有主题词或几篇 seed paper | [文献检索与单篇精读](./文献检索与单篇精读.md) | 扩展论文池、筛出关键论文、形成结构化精读卡。 |
| 已经有一批论文、笔记和引用 | [知识管理与证据沉淀](./知识管理与证据沉淀.md) | 把资料沉淀成可复用、可追溯资产。 |
| 需要判断 novelty、空白点或 reviewer concern | [新颖性判断与综述](./新颖性判断与综述.md) | 做 novelty check、review mining、系统综述与证据综合。 |
| 已经决定要做，准备把 idea 变成实验 | [实验执行、复现与评测](./实验执行、复现与评测.md) | 搭实验闭环、追踪结果、建立 benchmark 与评测。 |
| 已经有材料和结果，准备成稿或返修 | [写作、审稿与投稿](./写作、审稿与投稿.md) | 形成 grounded draft、response、模板与投稿包。 |

## 二、六步主线

1. [课题扫描与选题](./课题扫描与选题.md)
2. [文献检索与单篇精读](./文献检索与单篇精读.md)
3. [知识管理与证据沉淀](./知识管理与证据沉淀.md)
4. [新颖性判断与综述](./新颖性判断与综述.md)
5. [实验执行、复现与评测](./实验执行、复现与评测.md)
6. [写作、审稿与投稿](./写作、审稿与投稿.md)

如果希望先按“完整研究路线”而不是按单个阶段进入，可直接看：
- [常见研究路径组合](./常见研究路径组合.md)

如果希望先把任务页、正文模块、类型附录和方向专题之间的关系看清，再决定从哪一层进入，可先看：
- [00-总览/任务与资源对照表](../00-总览/任务与资源对照表.md)
- [98-全局索引/任务专题对照索引](../98-全局索引/任务专题对照索引.md)
- [98-全局索引/方向专题索引](../98-全局索引/方向专题索引.md)

## 三、三条最常见的使用路线

### 路线 A：AI / ML / data mining 论文路线

1. [课题扫描与选题](./课题扫描与选题.md)
2. [新颖性判断与综述](./新颖性判断与综述.md)
3. [实验执行、复现与评测](./实验执行、复现与评测.md)
4. [写作、审稿与投稿](./写作、审稿与投稿.md)

重点补看：
- [08-方向专题/AI-ML-DataMining资源](../08-方向专题/AI-ML-DataMining资源.md)
- [08-方向专题/Tabular-AutoML与HPO](../08-方向专题/Tabular-AutoML与HPO.md)
- [08-方向专题/Graph-Retrieval-Recsys与DataMining](../08-方向专题/Graph-Retrieval-Recsys与DataMining.md)

### 路线 B：综述 / evidence synthesis 路线

1. [课题扫描与选题](./课题扫描与选题.md)
2. [文献检索与单篇精读](./文献检索与单篇精读.md)
3. [知识管理与证据沉淀](./知识管理与证据沉淀.md)
4. [新颖性判断与综述](./新颖性判断与综述.md)
5. [写作、审稿与投稿](./写作、审稿与投稿.md)

重点补看：
- [94-Prompt与写作/系统综述与证据综合](../94-Prompt与写作/系统综述与证据综合.md)
- [95-文献检索与知识管理/引文导航与研究地图](../95-文献检索与知识管理/引文导航与研究地图.md)

### 路线 C：开放创新 / 管理技术交叉路线

1. [课题扫描与选题](./课题扫描与选题.md)
2. [开放学术、创新与行为实验资源](../08-方向专题/开放学术、创新与行为实验资源.md)
3. [新颖性判断与综述](./新颖性判断与综述.md)
4. [实验执行、复现与评测](./实验执行、复现与评测.md)
5. [写作、审稿与投稿](./写作、审稿与投稿.md)

重点补看：
- [08-方向专题/Computational-Design-Science与管理技术交叉](../08-方向专题/Computational-Design-Science与管理技术交叉.md)

## 四、最小工具栈建议

| 任务阶段 | 最小组合 |
| --- | --- |
| 选题扫描 | `Paper Search MCP + OpenAlex MCP + OpenReview MCP + Open Research / GPT Researcher` |
| 精读与筛选 | `Paper Search MCP + OpenAlex / Semantic Scholar + GROBID / Marker / Docling + PaperQA2` |
| 知识沉淀 | `Zotero + Better BibTeX + Zotero MCP + Obsidian / Logseq` |
| novelty 与综述 | `OpenReview MCP + OpenAlex MCP + llm4novelty + NLPeer / ReviewAdvisor + scite` |
| 实验与评测 | `Jupyter MCP + GitHub MCP + MLflow + DVC + benchmark suites` |
| 写作与投稿 | `Zotero MCP + OverleafMCP / MyST / Quarto + OpenResearch / ScholarCopilot + template tools` |

## 五、每一步的最小可执行路径

| 任务阶段 | 最短路径 |
| --- | --- |
| 选题扫描 | `方向词 / seed paper -> Paper Search / OpenAlex -> 核心论文池 -> novelty 检查` |
| 精读筛选 | `候选论文池 -> 结构化精读 -> PDF 深解析 -> 精读卡输出` |
| 知识沉淀 | `Zotero / Bib -> 笔记系统 -> 证据卡 -> 写作或综述出口` |
| novelty 与综述 | `相关工作池 -> review mining / novelty -> claim 核验 -> 继续做或停止做` |
| 实验与评测 | `环境与配置 -> benchmark / baseline -> tracking / DVC -> artifact` |
| 写作与投稿 | `证据与图表回收 -> grounded draft -> 内审 / rebuttal -> 投稿包` |

## 六、按角色进入

- 做选题：
  [课题扫描与选题](./课题扫描与选题.md)
- 做文献精读：
  [文献检索与单篇精读](./文献检索与单篇精读.md)
- 做知识沉淀：
  [知识管理与证据沉淀](./知识管理与证据沉淀.md)
- 做 novelty / reviewer 预演：
  [新颖性判断与综述](./新颖性判断与综述.md)
- 做实验与 benchmark：
  [实验执行、复现与评测](./实验执行、复现与评测.md)
- 做成稿与投稿：
  [写作、审稿与投稿](./写作、审稿与投稿.md)

## 七、横向补充入口

- [07-安全与治理](../07-安全与治理/README.md)
  适合在任何阶段补权限边界、数据治理、评测安全与供应链要求。
- [08-方向专题](../08-方向专题/README.md)
  适合按研究方向继续深挖 AI/ML、data mining、computational design science 和开放创新资源。
- [98-全局索引/任务专题对照索引](../98-全局索引/任务专题对照索引.md)
  适合从“当前阶段”直接跳到最值得补看的方向专题。
- [98-全局索引/方向专题索引](../98-全局索引/方向专题索引.md)
  适合从“当前方向”反查最该回去的任务页、附录页与 benchmark 入口。
- [98-全局索引/外部导航与合集](../98-全局索引/外部导航与合集.md)
  适合继续扫外部公开合集并补库。

## 八、每一步继续补 Skills / MCP 时优先回查

| 任务阶段 | Skills 优先回查 | MCP 优先回查 |
| --- | --- | --- |
| 课题扫描与选题 | [91-Skills/科研向Skills合集](../91-Skills/科研向Skills合集.md)、[91-Skills/Skill发现平台与精品合集](../91-Skills/Skill发现平台与精品合集.md) | [92-MCP/文献检索与知识库MCP](../92-MCP/文献检索与知识库MCP.md)、[92-MCP/MCP标准与发现平台](../92-MCP/MCP标准与发现平台.md) |
| 文献检索与单篇精读 | [91-Skills/科研写作与文献Skills](../91-Skills/科研写作与文献Skills.md)、[91-Skills/Skill发现平台与精品合集](../91-Skills/Skill发现平台与精品合集.md) | [92-MCP/文献检索与知识库MCP](../92-MCP/文献检索与知识库MCP.md)、[92-MCP/MCP标准与发现平台](../92-MCP/MCP标准与发现平台.md) |
| 知识管理与证据沉淀 | [91-Skills/科研写作与文献Skills](../91-Skills/科研写作与文献Skills.md)、[91-Skills/Skill发现平台与精品合集](../91-Skills/Skill发现平台与精品合集.md) | [92-MCP/文献检索与知识库MCP](../92-MCP/文献检索与知识库MCP.md)、[92-MCP/MCP标准与发现平台](../92-MCP/MCP标准与发现平台.md) |
| 新颖性判断与综述 | [91-Skills/科研写作与文献Skills](../91-Skills/科研写作与文献Skills.md)、[91-Skills/Skill发现平台与精品合集](../91-Skills/Skill发现平台与精品合集.md) | [92-MCP/文献检索与知识库MCP](../92-MCP/文献检索与知识库MCP.md)、[92-MCP/MCP标准与发现平台](../92-MCP/MCP标准与发现平台.md) |
| 实验执行、复现与评测 | [91-Skills/科研工程与实验Skills](../91-Skills/科研工程与实验Skills.md)、[91-Skills/Skill发现平台与精品合集](../91-Skills/Skill发现平台与精品合集.md) | [92-MCP/实验执行与数据工程MCP](../92-MCP/实验执行与数据工程MCP.md)、[92-MCP/MCP标准与发现平台](../92-MCP/MCP标准与发现平台.md) |
| 写作、审稿与投稿 | [91-Skills/科研写作与文献Skills](../91-Skills/科研写作与文献Skills.md)、[91-Skills/Skill发现平台与精品合集](../91-Skills/Skill发现平台与精品合集.md) | [92-MCP/写作协作与投稿MCP](../92-MCP/写作协作与投稿MCP.md)、[92-MCP/MCP标准与发现平台](../92-MCP/MCP标准与发现平台.md) |
