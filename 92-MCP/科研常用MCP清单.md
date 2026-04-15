# 科研常用 MCP 清单

这一页作为 `92-MCP` 的总入口，收录“直接服务科研工作流”的 MCP，并按任务链路进行组织。相比按仓库名堆叠，按工作流拆分更适合持续维护。

## 1. 文献、知识库与学术情报

代表性资源：

- [openags/paper-search-mcp](https://github.com/openags/paper-search-mcp)
- [openreview/openreview-mcp](https://github.com/openreview/openreview-mcp)
- [hbiaou/openalex-mcp](https://github.com/hbiaou/openalex-mcp)
- [oksure/openalex-research-mcp](https://github.com/oksure/openalex-research-mcp)
- [zongmin-yu/semantic-scholar-fastmcp-mcp-server](https://github.com/zongmin-yu/semantic-scholar-fastmcp-mcp-server)
- [botanicastudios/crossref-mcp](https://github.com/botanicastudios/crossref-mcp)
- [54yyyu/zotero-mcp](https://github.com/54yyyu/zotero-mcp)
- [microsoft/markitdown](https://github.com/microsoft/markitdown)

专题页：

- [文献检索与知识库MCP](./文献检索与知识库MCP.md)

## 2. 实验执行、Notebook 与数据工程

代表性资源：

- [datalayer/jupyter-mcp-server](https://github.com/datalayer/jupyter-mcp-server)
- [github/github-mcp-server](https://github.com/github/github-mcp-server)
- [microsoft/playwright-mcp](https://github.com/microsoft/playwright-mcp)
- [antvis/mcp-server-chart](https://github.com/antvis/mcp-server-chart)
- [yuru-sha/mcp-server-postgres](https://github.com/yuru-sha/mcp-server-postgres)
- [motherduckdb/mcp-server-motherduck](https://github.com/motherduckdb/mcp-server-motherduck)
- [zilliztech/mcp-server-milvus](https://github.com/zilliztech/mcp-server-milvus)
- [arrismo/kaggle-mcp](https://github.com/arrismo/kaggle-mcp)

专题页：

- [实验执行与数据工程MCP](./实验执行与数据工程MCP.md)

## 3. 生物医药、生命科学与专利情报

代表性资源：

- [grll/pubmedmcp](https://github.com/grll/pubmedmcp)
- [Augmented-Nature/PubMed-MCP-Server](https://github.com/Augmented-Nature/PubMed-MCP-Server)
- [Augmented-Nature/ClinicalTrials-MCP-Server](https://github.com/Augmented-Nature/ClinicalTrials-MCP-Server)
- [Augmented-Nature/OpenTargets-MCP-Server](https://github.com/Augmented-Nature/OpenTargets-MCP-Server)
- [Augmented-Nature/GTEx-MCP-Server](https://github.com/Augmented-Nature/GTEx-MCP-Server)
- [Augmented-Nature/PubChem-MCP-Server](https://github.com/Augmented-Nature/PubChem-MCP-Server)
- [riemannzeta/patent_mcp_server](https://github.com/riemannzeta/patent_mcp_server)

专题页：

- [生物医药与专利MCP](./生物医药与专利MCP.md)

## 4. 第一梯队 MCP 组合

对于通用科研工作流，第一梯队 MCP 组合通常包括：

1. 文献聚合：`paper-search-mcp`
2. 投稿与评审生态：`openreview/openreview-mcp`
3. 学术图谱：`openalex-mcp` 或 `openalex-research-mcp`
4. 个人文库：`zotero-mcp`
5. 文档转换：`markitdown`
6. Notebook 执行：`jupyter-mcp-server`
7. 代码与协作：`github-mcp-server`

## 5. 使用提醒

- 社区 MCP 数量多，不等于都适合进入主链路。
- 学术检索类 MCP 更适合返回可验证的来源、标识符和元数据，而不是只给摘要结论。
- 访问 Zotero、GitHub、Notion、数据库等私有资产时，公开资源整理应默认强调最小权限与只读优先。
- 网页搜索类 MCP 适合做补充信息层，不宜替代学术数据库与正式文献源。
- 对涉及专利、临床、医学数据的 MCP，额外关注 API 条款、数据许可与引用规范。
