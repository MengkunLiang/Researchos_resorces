# 文献检索与单篇精读

这一模块聚焦多源检索、单篇论文精读、PDF 解析、引文回查与结构化摘要。核心目标不是“多找几篇论文”，而是把检索结果稳定转成可复查的论文池、精读卡片和证据条目。

## 这一步通常要回答的问题

1. 哪些数据库和平台最适合作为第一轮检索入口。
2. 怎样从一批搜索结果里筛出真正值得精读的论文。
3. 怎样把 PDF、LaTeX 源码、图表和附录内容转成便于分析的结构化材料。
4. 怎样把单篇论文拆成 `问题 - 方法 - 数据 - 结果 - 局限 - 可延伸点` 的可复用卡片。

## 推荐先看

- [精读用Skills、MCP与解析工具详表](./精读用Skills、MCP与解析工具详表.md)
- [91-Skills/Skill发现平台与精品合集](../91-Skills/Skill发现平台与精品合集.md)
- [95-文献检索与知识管理/文献检索与阅读](../95-文献检索与知识管理/文献检索与阅读.md)
- [95-文献检索与知识管理/PDF解析与阅读加工](../95-文献检索与知识管理/PDF解析与阅读加工.md)
- [03-知识管理与证据沉淀](../03-知识管理与证据沉淀/README.md)

## 一、相关 Skills

| 资源 | 类型 | 适合环节 | 简述 | 链接 |
| --- | --- | --- | --- | --- |
| 科研写作与文献Skills | 仓库内附录 | 总览 | 当前仓库里文献阅读、综述、写作与审稿相关 Skills 的主归属页。 | [91-Skills/科研写作与文献Skills](../91-Skills/科研写作与文献Skills.md) |
| Skill发现平台与精品合集 | 仓库内附录 | Skills 扩容 | 适合继续找 PDF 处理、论文问答和 research reading 相关 skill。 | [91-Skills/Skill发现平台与精品合集](../91-Skills/Skill发现平台与精品合集.md) |
| paper-glance-skill | 单篇精读技能 | 单篇拆解 | 适合把论文快速拆成 contribution、method、experiment、weakness。 | [CatVinci-Studio/paper-glance-skill](https://github.com/CatVinci-Studio/paper-glance-skill) |
| Claude Scientific Writer | 写作与深研技能库 | 检索与综述 | 其中 `research-lookup`、`literature-review`、`scientific-critical-thinking` 很适合精读前后处理。 | [K-Dense-AI/claude-scientific-writer](https://github.com/K-Dense-AI/claude-scientific-writer) |
| Academic Research Skills | 学术流程技能库 | deep research | `deep-research` 和 `academic-paper-reviewer` 适合做精读后的系统核验与批判阅读。 | [Imbad0202/academic-research-skills](https://github.com/Imbad0202/academic-research-skills) |
| Anthropic Skills | 官方技能库 | 文档加工 | `pdf`、`docx`、`pptx`、`xlsx` 适合处理论文、补充材料和数据表。 | [anthropics/skills](https://github.com/anthropics/skills) |
| OpenAI Skills | 官方技能库 | 资料处理与代码核验 | 适合把代码、文档、表格和检索结果并到同一工作流。 | [openai/skills](https://github.com/openai/skills) |
| Claude Skills 中文镜像 | 中文学习镜像 | skill 学习与迁移 | 适合中文环境下快速扫 `pdf`、`research`、`documentation` 相关技能范式。 | [LeastBit/Claude_skills_zh-CN](https://github.com/LeastBit/Claude_skills_zh-CN) |
| NotebookLM Skill | 知识库技能 | 长文问答 | 适合把课程资料、组会文件、项目文档和论文池放进统一问答入口。 | [PleasePrompto/notebooklm-skill](https://github.com/PleasePrompto/notebooklm-skill) |

## 二、相关 MCP

| 资源 | 类型 | 适合环节 | 简述 | 链接 |
| --- | --- | --- | --- | --- |
| 文献检索与知识库MCP | 仓库内附录 | MCP 总览 | 当前仓库里文献检索、个人文库和知识库 MCP 的主归属页。 | [92-MCP/文献检索与知识库MCP](../92-MCP/文献检索与知识库MCP.md) |
| Paper Search MCP | 学术检索 MCP | broad search | 聚合 arXiv、PubMed、Semantic Scholar、Crossref、OpenAlex 等来源。 | [openags/paper-search-mcp](https://github.com/openags/paper-search-mcp) |
| OpenReview MCP | 投稿与评审 MCP | 顶会补充检索 | 适合补最新投稿、审稿讨论与 workshop / conference 线索。 | [openreview/openreview-mcp](https://github.com/openreview/openreview-mcp) |
| OpenAlex MCP | 学术图谱 MCP | 论文池扩展 | 适合从 seed paper 往作者、机构和引文网络扩展。 | [hbiaou/openalex-mcp](https://github.com/hbiaou/openalex-mcp) |
| Semantic Scholar MCP | 学术图谱 MCP | 引文与作者分析 | 适合在初筛后做论文家族和影响路径扩展。 | [zongmin-yu/semantic-scholar-fastmcp-mcp-server](https://github.com/zongmin-yu/semantic-scholar-fastmcp-mcp-server) |
| Hugging Face MCP Server | 模型与数据生态 MCP | 模型卡与数据卡回查 | 适合在论文配套模型、数据集和 demo 之间做交叉核验。 | [huggingface/hf-mcp-server](https://github.com/huggingface/hf-mcp-server) |
| Academic RAG MCP | 学术问答 MCP | 论文池问答 | 适合围绕多篇论文做来源约束问答与证据回查。 | [Jackela/mcp-academic-rag-server](https://github.com/Jackela/mcp-academic-rag-server) |
| Zotero MCP | 文献库 MCP | 私有文库接入 | 适合把已有文献库、批注和笔记纳入精读流程。 | [54yyyu/zotero-mcp](https://github.com/54yyyu/zotero-mcp) |
| arXiv LaTeX MCP | LaTeX 源码 MCP | 公式与表格精读 | 对公式、伪代码、附录和表格结构的细读很有帮助。 | [takashiishida/arxiv-latex-mcp](https://github.com/takashiishida/arxiv-latex-mcp) |
| Crossref MCP | 元数据 MCP | DOI 核验 | 适合核对正式出版信息、DOI 与基础元数据。 | [botanicastudios/crossref-mcp](https://github.com/botanicastudios/crossref-mcp) |

## 三、相关 Agent 与研究工作流

| 资源 | 类型 | 适合环节 | 简述 | 链接 |
| --- | --- | --- | --- | --- |
| PaperQA2 | 证据问答框架 | 单篇问答 | 适合围绕论文内容做 claim 级问答与证据回查。 | [PaperQA2](https://github.com/Future-House/paper-qa) |
| Open Deep Research | 开源 deep research 系统 | 多篇阅读归并 | 适合把检索、网页资料和论文阅读整合成持续更新 dossier。 | [langchain-ai/open_deep_research](https://github.com/langchain-ai/open_deep_research) |
| RTI | 文献研究工作流 | 检索到精读 | 适合把方向输入、检索、筛选、翻译和深读接成流程。 | [RTI](https://github.com/yrc-better/RTI) |
| Open Research | 研究工作台 | 论文解释与核验 | 适合做 source scout、paper explainer、novelty check。 | [Open Research](https://www.open-research.info/) |
| STORM | 结构化调研 | 精读后归并 | 适合把多篇论文归并成提纲、问题树和长报告。 | [STORM](https://github.com/stanford-oval/storm) |
| GPT Researcher | deep research agent | 多轮资料整合 | 适合把单篇精读放回 broader dossier 中继续整理。 | [GPT Researcher](https://github.com/assafelovic/gpt-researcher) |

## 四、相关数据源与解析工具

| 资源 | 类型 | 适合环节 | 简述 | 链接 |
| --- | --- | --- | --- | --- |
| 文献检索与阅读 | 仓库内附录 | 检索入口 | 当前仓库里学术检索平台和阅读工具的主归属页。 | [95-文献检索与知识管理/文献检索与阅读](../95-文献检索与知识管理/文献检索与阅读.md) |
| PDF解析与阅读加工 | 仓库内附录 | 解析工具总览 | 当前仓库里 PDF 结构化解析与阅读加工工具的主归属页。 | [95-文献检索与知识管理/PDF解析与阅读加工](../95-文献检索与知识管理/PDF解析与阅读加工.md) |
| Semantic Scholar | 学术搜索平台 | 初筛 | 适合做 relevance、citation 和 author graph 级筛选。 | [Semantic Scholar](https://www.semanticscholar.org/) |
| OpenAlex | 开放学术图谱 | 扩展与核验 | 更适合做 citation network、topic 和 venue 扩展。 | [OpenAlex](https://openalex.org/) |
| DBLP | 计算机领域索引 | CS 方向补检 | 对 AI/ML、data mining、IR、database 方向尤其有价值。 | [DBLP](https://dblp.org/) |
| GROBID | 学术 PDF 解析 | 结构化抽取 | 适合把论文 PDF 转成 TEI/XML 与结构化 section/citation。 | [kermitt2/grobid](https://github.com/kermitt2/grobid) |
| Marker | PDF 转 Markdown | LLM 友好文本 | 适合快速转成 Markdown 并进入问答或摘要流程。 | [VikParuchuri/marker](https://github.com/VikParuchuri/marker) |
| Docling | 文档解析框架 | 多格式抽取 | 适合统一处理 PDF、Office、扫描件和复杂版式。 | [docling-project/docling](https://github.com/docling-project/docling) |
| MinerU | 文档解析引擎 | 复杂版面与公式 | 对复杂科研 PDF 的版面、表格、公式还原较强。 | [opendatalab/MinerU](https://github.com/opendatalab/MinerU) |
| Nougat | 学术文档 OCR | 公式型文档 | 适合数学公式、扫描论文和复杂学术版式。 | [facebookresearch/nougat](https://github.com/facebookresearch/nougat) |
| Unstructured | 文档 ETL | 前处理 | 适合做切分、清洗和进入知识库前的统一预处理。 | [Unstructured-IO/unstructured](https://github.com/Unstructured-IO/unstructured) |

## 五、外部整合入口

| 资源 | 类型 | 适合用途 | 简述 | 链接 |
| --- | --- | --- | --- | --- |
| awesome-ai-research-writing | 写作与研究合集 | 后链路补充 | 可继续补综述、写作、翻译、审稿与研究型 prompts/skills。 | [Leey21/awesome-ai-research-writing](https://github.com/Leey21/awesome-ai-research-writing) |
| Awesome LLM Scientific Discovery | 科学发现合集 | broad scan | 适合从 scientific discovery 视角继续找工具和系统。 | [HKUST-KnowComp/Awesome-LLM-Scientific-Discovery](https://github.com/HKUST-KnowComp/Awesome-LLM-Scientific-Discovery) |
| SurveyX | survey automation | 多篇归并 | 更适合在精读后把论文池转成 survey outline 与初稿。 | [IAAR-Shanghai/SurveyX](https://github.com/IAAR-Shanghai/SurveyX) |
| 外部导航与合集 | 仓库内索引 | 继续扫库 | 当前仓库里的外部公开合集总入口。 | [98-全局索引/外部导航与合集](../98-全局索引/外部导航与合集.md) |

## 六、推荐组合

1. `paper-search-mcp + OpenAlex / Semantic Scholar + OpenReview`
   适合做 broad search、论文池初筛与会议信息补充。
2. `GROBID / Marker / Docling / MinerU`
   适合把 PDF 与补充材料转成结构化阅读材料。
3. `PaperQA2 + paper-glance-skill + Zotero MCP`
   适合把单篇精读变成证据卡片和长期可复用材料。
4. `arXiv LaTeX MCP + Crossref MCP + OpenAlex`
   适合做公式、表格和正式出版信息的二次核验。

## 七、如果这一页的 Skills / MCP 还不够

- Skills 继续补：优先回看 [91-Skills/科研写作与文献Skills](../91-Skills/科研写作与文献Skills.md) 与 [91-Skills/Skill发现平台与精品合集](../91-Skills/Skill发现平台与精品合集.md)。
- MCP 继续补：优先回看 [92-MCP/MCP标准与发现平台](../92-MCP/MCP标准与发现平台.md) 与 [92-MCP/文献检索与知识库MCP](../92-MCP/文献检索与知识库MCP.md)。

## 八、仓库内延伸阅读

- [03-知识管理与证据沉淀](../03-知识管理与证据沉淀/README.md)
- [04-新颖性判断与综述](../04-新颖性判断与综述/README.md)
- [05-实验执行、复现与评测](../05-实验执行、复现与评测/README.md)
