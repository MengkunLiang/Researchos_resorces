# MCP（类型附录）

本目录保留为查全型附录，适合系统补 `MCP` 协议、科研工作流常见服务器、学术检索层、实验执行层和投稿协作层的具体实现。

## 这一层适合什么时候进入

1. 已经知道当前任务需要哪类工具协议，但还需要继续扫具体 server 实现。
2. 需要把搜索、知识库、notebook、GitHub、Zotero、OpenReview、Overleaf 等能力接到代理工作流。
3. 需要比较同一类 MCP 的不同实现路线、宿主兼容性和高频使用场景。

## 推荐先看

- [MCP标准与发现平台](./MCP标准与发现平台.md)
- [科研常用MCP清单](./科研常用MCP清单.md)
- [文献检索与知识库MCP](./文献检索与知识库MCP.md)
- [实验执行与数据工程MCP](./实验执行与数据工程MCP.md)
- [写作协作与投稿MCP](./写作协作与投稿MCP.md)
- [生物医药与专利MCP](./生物医药与专利MCP.md)

## 按任务回查

| 当前任务 | 更适合先看 |
| --- | --- |
| 选题、文献检索、趋势扫描 | [文献检索与知识库MCP](./文献检索与知识库MCP.md) |
| 知识管理、个人文库、证据沉淀 | [文献检索与知识库MCP](./文献检索与知识库MCP.md) |
| notebook、pipeline、实验跟踪、benchmark | [实验执行与数据工程MCP](./实验执行与数据工程MCP.md) |
| 成稿、审稿、投稿与文档协作 | [写作协作与投稿MCP](./写作协作与投稿MCP.md) |
| 生物医药、专利、健康与科学数据 | [生物医药与专利MCP](./生物医药与专利MCP.md) |

## 高频公开资源

| 资源 | 类型 | 简述 | 链接 |
| --- | --- | --- | --- |
| Paper Search MCP | 学术检索 MCP | 适合多源论文检索与 PDF 获取。 | [openags/paper-search-mcp](https://github.com/openags/paper-search-mcp) |
| Academia MCP | 学术研究 MCP | 集成论文、数据集、引用、网页与研究报告工作流。 | [IlyaGusev/academia_mcp](https://github.com/IlyaGusev/academia_mcp) |
| OpenReview MCP | 投稿生态 MCP | 适合跟踪 OpenReview 投稿、讨论与审稿信息。 | [openreview/openreview-mcp](https://github.com/openreview/openreview-mcp) |
| OpenAlex Research MCP | research landscape MCP | 适合引文分析、趋势分析和文献 landscape。 | [oksure/openalex-research-mcp](https://github.com/oksure/openalex-research-mcp) |
| Jupyter MCP Server | notebook MCP | 适合执行与检查 notebook。 | [datalayer/jupyter-mcp-server](https://github.com/datalayer/jupyter-mcp-server) |
| GitHub MCP Server | 仓库协作 MCP | 适合仓库、Issue、PR、CI 与 release 读取。 | [github/github-mcp-server](https://github.com/github/github-mcp-server) |

## 推荐配合使用的页面

- [09-按科研任务导航](../09-按科研任务导航/README.md)
- [98-全局索引/MCP索引](../98-全局索引/MCP索引.md)
- [00-总览/任务与资源对照表](../00-总览/任务与资源对照表.md)
