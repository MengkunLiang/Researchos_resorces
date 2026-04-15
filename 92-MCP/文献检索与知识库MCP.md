# 文献检索与知识库 MCP

这一页聚焦科研工作流中最常见的一条链路：发现论文、追踪投稿、整理文库、回到全文与元数据。

## 1. 学术检索与研究情报的核心 MCP

| 资源 | 场景 | 简述 | 链接 |
| --- | --- | --- | --- |
| Paper Search MCP | 多源学术检索 | 同时覆盖 arXiv、PubMed、Semantic Scholar、Crossref、OpenAlex、Zenodo 等多个公开来源，适合做统一入口。 | [openags/paper-search-mcp](https://github.com/openags/paper-search-mcp) |
| OpenReview MCP | 投稿与评审生态 | 直接面向 OpenReview，适合跟踪最新投稿、评审流程、rebuttal 语境与顶会前沿。 | [openreview/openreview-mcp](https://github.com/openreview/openreview-mcp) |
| OpenAlex MCP | 学术图谱 | 面向 OpenAlex API，适合做作者、机构、主题、引文网络与文献 landscape。 | [hbiaou/openalex-mcp](https://github.com/hbiaou/openalex-mcp) |
| OpenAlex Research MCP | 文献综述与 landscape | 功能更偏 literature review、citation analysis 与 research landscaping。 | [oksure/openalex-research-mcp](https://github.com/oksure/openalex-research-mcp) |
| arXiv MCP Server | arXiv 检索 | 适合快速获取预印本与基础元数据。 | [blazickjp/arxiv-mcp-server](https://github.com/blazickjp/arxiv-mcp-server) |
| arXiv LaTeX MCP | LaTeX 源码抓取 | 对公式、伪代码、表格结构和附录材料的精读场景特别有价值。 | [takashiishida/arxiv-latex-mcp](https://github.com/takashiishida/arxiv-latex-mcp) |
| Semantic Scholar MCP | 引文网络与作者分析 | 适合做论文、作者、引用关系与主题网络分析。 | [zongmin-yu/semantic-scholar-fastmcp-mcp-server](https://github.com/zongmin-yu/semantic-scholar-fastmcp-mcp-server) |
| Crossref MCP | DOI 与出版元数据 | 适合 DOI 查询、出版信息补全与元数据核对。 | [botanicastudios/crossref-mcp](https://github.com/botanicastudios/crossref-mcp) |

## 2. 个人文库、知识库与文档资产

| 资源 | 场景 | 简述 | 链接 |
| --- | --- | --- | --- |
| Zotero MCP | 个人文献库 | 适合检索个人 Zotero 文库、读取条目、笔记、PDF 与 BibTeX 资产。 | [54yyyu/zotero-mcp](https://github.com/54yyyu/zotero-mcp) |
| Zotero MCP Server | 本地 API 集成 | 直接对接 Zotero Local API，适合本地全文抽取与库内检索。 | [masaki39/zotero-mcp](https://github.com/masaki39/zotero-mcp) |
| Zotero MCP Server（Python SDK） | 文库管理 | 支持条目、馆藏与 group library 操作，是另一条值得关注的实现线。 | [cr625/zotero-mcp-server](https://github.com/cr625/zotero-mcp-server) |
| Notion MCP Server | 笔记与项目知识库 | 适合连接研究计划、会议纪要、任务页与知识卡片。 | [makenotion/notion-mcp-server](https://github.com/makenotion/notion-mcp-server) |
| GitHub MCP Server | 代码与配套文档 | 适合读取配套代码、Issue、PR、Actions 与 release 信息。 | [github/github-mcp-server](https://github.com/github/github-mcp-server) |
| MarkItDown | 文档转换 | 对 PDF、Word、Excel、图片、音频等附件转换为 Markdown 非常实用，适合进入检索与摘要链路前的预处理。 | [microsoft/markitdown](https://github.com/microsoft/markitdown) |

## 3. 网页搜索与补充信息层

| 资源 | 场景 | 简述 | 链接 |
| --- | --- | --- | --- |
| Exa MCP Server | AI 原生搜索 | 适合补充开放网页、项目页、新闻稿、实验主页和最新资料。 | [exa-labs/exa-mcp-server](https://github.com/exa-labs/exa-mcp-server) |
| Tavily MCP | 搜索增强 | 适合做 research assistant 的外部信息补充层。 | [tavily-ai/tavily-mcp](https://github.com/tavily-ai/tavily-mcp) |

## 4. 适合公开资源库保留的组合方式

| 组合 | 适用链路 | 说明 |
| --- | --- | --- |
| `paper-search + openalex + semantic scholar` | 综述与 landscape | 适合做 broad search、citation network 与主题演化分析。 |
| `openreview + openalex + github` | 顶会追踪 | 适合把投稿、作者、机构和配套代码串起来看。 |
| `zotero + markitdown + notion` | 私有文库与知识库 | 适合把本地文献库、附件与笔记整理到统一工作流。 |
| `arxiv-latex + crossref + zotero` | 精读与引用核对 | 适合公式精读、引用补全与正式元数据校验。 |

## 5. 选择这类 MCP 时的注意点

1. 文献类 MCP 优先选择返回 DOI、ArXiv ID、PMID、OpenAlex ID、OpenReview Note ID 等可验证标识符的实现。
2. Google Scholar 类接口波动较大，适合做补充层，不宜作为主数据源。
3. 本地文库类 MCP 通常涉及个人笔记和全文资产，建议默认采用只读或最小权限配置。
4. 文档转换工具适合作为前处理层，不应替代正式文献元数据源。
