# 科研常用 MCP 清单

这一页只收“直接能服务科研”的 MCP，优先选择官方或较成熟实现。

## 1. 文献检索与学术数据库

| 资源 | 场景 | 简述 | 链接 |
| --- | --- | --- | --- |
| paper-search-mcp | 多源检索 | 同时覆盖 arXiv、PubMed、Semantic Scholar、Crossref、OpenAlex、Zenodo 等多源搜索。 | [openags/paper-search-mcp](https://github.com/openags/paper-search-mcp) |
| openreview/openreview-mcp | 顶会追踪 | 直接面向 OpenReview 生态，适合追最新投稿、rebuttal 前沿与 novelty 检查。 | [openreview/openreview-mcp](https://github.com/openreview/openreview-mcp) |
| hbiaou/openalex-mcp | 学术图谱 | 适合做引文网络、landscape、作者与主题探索。 | [hbiaou/openalex-mcp](https://github.com/hbiaou/openalex-mcp) |
| blazickjp/arxiv-mcp-server | arXiv 检索 | 面向 arXiv 的 MCP，适合快速拉论文和元数据。 | [blazickjp/arxiv-mcp-server](https://github.com/blazickjp/arxiv-mcp-server) |
| takashiishida/arxiv-latex-mcp | LaTeX 源码抓取 | 对需要精确读公式、读源文件结构的场景特别有用。 | [takashiishida/arxiv-latex-mcp](https://github.com/takashiishida/arxiv-latex-mcp) |
| hy20191108/semantic-scholar-mcp | Semantic Scholar | 适合做论文、作者、引文网络分析。 | [hy20191108/semantic-scholar-mcp](https://github.com/hy20191108/semantic-scholar-mcp) |
| JackKuo666/Google-Scholar-MCP-Server | Google Scholar | 适合补充 Scholar 侧搜索，但要注意 Scholar 抓取稳定性。 | [JackKuo666/Google-Scholar-MCP-Server](https://github.com/JackKuo666/Google-Scholar-MCP-Server) |

## 2. 个人文献资产与知识管理

| 资源 | 场景 | 简述 | 链接 |
| --- | --- | --- | --- |
| 54yyyu/zotero-mcp | Zotero 检索与导出 | 适合把个人文献库、笔记和 BibTeX 直接接给 Agent。 | [54yyyu/zotero-mcp](https://github.com/54yyyu/zotero-mcp) |
| makenotion/notion-mcp-server | 笔记 / 项目管理 | 适合把研究计划、会议纪要、实验记录接进 Agent 工作流。 | [makenotion/notion-mcp-server](https://github.com/makenotion/notion-mcp-server) |
| github/github-mcp-server | 代码与协作 | 对论文配套代码、issue、PR、CI 非常实用。 | [github/github-mcp-server](https://github.com/github/github-mcp-server) |

## 3. 实验、Notebook 与可视化

| 资源 | 场景 | 简述 | 链接 |
| --- | --- | --- | --- |
| datalayer/jupyter-mcp-server | Notebook 控制 | 可对 Jupyter Notebook 做查看、编辑、执行和管理。 | [datalayer/jupyter-mcp-server](https://github.com/datalayer/jupyter-mcp-server) |
| antvis/mcp-server-chart | 图表生成 | 适合把实验结果快速变成可读图表。 | [antvis/mcp-server-chart](https://github.com/antvis/mcp-server-chart) |
| microsoft/playwright-mcp | 网页自动化 | 抓网页实验面板、自动登录平台、浏览论文官网时很有用。 | [microsoft/playwright-mcp](https://github.com/microsoft/playwright-mcp) |

## 4. 搜索与补充信息获取

| 资源 | 场景 | 简述 | 链接 |
| --- | --- | --- | --- |
| exa-labs/exa-mcp-server | AI 原生搜索 | 适合补充网页搜索、最新资料和公开网页抓取。 | [exa-labs/exa-mcp-server](https://github.com/exa-labs/exa-mcp-server) |
| tavily-ai/tavily-mcp | 搜索增强 | 适合做 research assistant 的外部网页检索补充。 | [tavily-ai/tavily-mcp](https://github.com/tavily-ai/tavily-mcp) |

## 5. 对 ResearchOS 最值得优先接入的 MCP

如果你是要服务真实科研工作流，最值得先接入的是：

1. `paper-search-mcp`
2. `openreview/openreview-mcp`
3. `hbiaou/openalex-mcp`
4. `54yyyu/zotero-mcp`
5. `datalayer/jupyter-mcp-server`
6. `github/github-mcp-server`

## 6. 使用提醒

- 社区 MCP 数量多，不代表都适合进主链路。
- 学术检索类 MCP 一定要做“来源可追溯”，不能只保留生成结论。
- 访问 Zotero、GitHub、Notion 等私有资产时，默认采用最小权限配置。
- 网页搜索类 MCP 更适合“补充资料”，不宜替代学术数据库本身。
