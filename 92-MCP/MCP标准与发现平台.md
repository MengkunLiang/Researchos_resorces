# MCP 标准与发现平台

MCP（Model Context Protocol）是模型连接工具、数据库、知识库与外部服务的开放接口层。对于科研型 Agent 而言，MCP 的价值主要体现在三点：

1. 让外部能力以统一协议暴露给模型
2. 让工具调用、资源读取与提示模板具备结构化边界
3. 让“文献检索、实验执行、数据分析、知识管理”这类工作流可以在同一套接口下组合

## 1. 官方标准、规范与参考实现

| 资源 | 类型 | 简述 | 链接 |
| --- | --- | --- | --- |
| Model Context Protocol 官方文档 | 官方文档 | MCP 总入口，适合先理解客户端、服务器、工具、资源与提示的基本模型。 | [modelcontextprotocol.io](https://modelcontextprotocol.io/docs/getting-started/intro) |
| MCP 规范仓库 | 官方规范 | 官方规范与文档源码仓库，适合持续跟踪协议演化。 | [modelcontextprotocol/modelcontextprotocol](https://github.com/modelcontextprotocol/modelcontextprotocol) |
| MCP 官方 Servers 仓库 | 官方参考实现 | 官方参考服务器集合，包含 `filesystem`、`fetch`、`memory` 等经典示例，是理解“标准服务器应如何组织”的最佳入口之一。 | [modelcontextprotocol/servers](https://github.com/modelcontextprotocol/servers) |
| MCP Registry | 官方注册表 | 官方注册表入口，适合按标准化元数据发现、安装和比较 MCP 服务。 | [registry.modelcontextprotocol.io](https://registry.modelcontextprotocol.io/) |
| MCP Registry GitHub | 官方目录镜像 | GitHub 侧的 Registry 展示入口，适合快速浏览近期热门与高安装量项目。 | [github.com/mcp](https://github.com/mcp) |
| GitHub MCP Server 文档 | 官方宿主文档 | 展示宿主侧如何配置和使用 MCP，适合理解“平台如何消费 MCP”。 | [GitHub Docs](https://docs.github.com/en/copilot/how-tos/provide-context/use-mcp/set-up-the-github-mcp-server) |

## 2. 发现、索引与安装平台

| 资源 | 类型 | 简述 | 链接 |
| --- | --- | --- | --- |
| Awesome MCP Servers | Awesome 列表 | 覆盖面广，适合快速扫全局生态与常见分类。 | [TensorBlock/awesome-mcp-servers](https://github.com/TensorBlock/awesome-mcp-servers) |
| Glama MCP Servers | 发现平台 | 适合按类别和活跃度浏览 MCP 服务。 | [Glama MCP Servers](https://glama.ai/mcp/servers) |
| MCPIndex | 索引站 | 适合快速查询具体服务器页面与安装信息。 | [mcpindex.net](https://mcpindex.net/en) |
| Smithery | 安装与分发平台 | 社区常用的安装与分发入口之一。 | [smithery.ai](https://smithery.ai/) |
| MCP.so | 目录平台 | 适合浏览热门 MCP 服务并进行横向比较。 | [mcp.so](https://mcp.so/) |
| Omedia MCP Servers | 参考集合 | 除官方实现外，还收录了更多参考服务器与扩展资源。 | [Omedia/mcp-servers](https://github.com/Omedia/mcp-servers) |

## 3. 与 Skills、科研工作台和平台化建设的连接点

| 资源 | 类型 | 简述 | 链接 |
| --- | --- | --- | --- |
| skill-to-mcp | 桥接思路 | 把 Skills 暴露为 MCP 资源的思路，适合统一“能力层”和“工具层”。 | [biocontext-ai/skill-to-mcp](https://github.com/biocontext-ai/skill-to-mcp) |
| SkillPort | SkillOps / MCP 结合 | 更偏规模化管理 Skill 与能力分发的方向。 | [gotalab/skillport](https://github.com/gotalab/skillport) |
| mcp.science | 科研 MCP 工作台 | 面向科研场景组织 MCP 的开源项目，适合继续跟踪 science-native 的 MCP 使用方式。 | [pathintegral-institute/mcp.science](https://github.com/pathintegral-institute/mcp.science) |
| Jupyter AI Agents | MCP 工作台 | JupyterLab 内嵌 Agent 与 MCP 工具，是实验型数据分析界面与 MCP 结合的代表项目。 | [datalayer/jupyter-ai-agents](https://github.com/datalayer/jupyter-ai-agents) |

## 4. 面向科研场景的选型框架

科研相关 MCP 数量增长很快，但可维护性、权限边界和数据质量差异很大。公开资源整理时，通常可以从以下六个维度评估：

1. 标准成熟度：是否遵循 MCP 官方规范，是否提供清晰的工具 / 资源 / 提示边界。
2. 维护信号：是否来自官方组织、领域机构或活跃维护者，是否有近期更新记录。
3. 权限模型：是否支持最小权限、只读模式、环境变量隔离、密钥管理。
4. 证据可追溯性：是否直接返回来源、标识符、元数据、原始链接或可验证日志。
5. 传输与部署方式：是否支持 `stdio`、SSE、HTTP，是否适合本地、服务器或容器部署。
6. 数据许可与合规：是否涉及私人文库、私有仓库、受限 API、受版权约束的全文数据。

## 5. 公开资源仓库里的常见分类方式

按照科研工作流整理 MCP，通常比单纯按“仓库名”堆叠更有用。较常见的分类方式包括：

- 标准与注册表：协议、文档、参考实现、发现平台
- 文献与知识库：OpenReview、OpenAlex、arXiv、Crossref、Zotero、Notion
- 实验与数据工程：Jupyter、GitHub、浏览器自动化、SQL、DuckDB、向量库
- 生命科学与专利：PubMed、ClinicalTrials、Open Targets、GTEx、PubChem、USPTO / Google Patents

专题页：

- [科研常用MCP清单](./科研常用MCP清单.md)
- [文献检索与知识库MCP](./文献检索与知识库MCP.md)
- [实验执行与数据工程MCP](./实验执行与数据工程MCP.md)
- [生物医药与专利MCP](./生物医药与专利MCP.md)
