# 实验执行与数据工程 MCP

这一页聚焦“实验能否跑起来、数据能否查得到、结果能否回写成结构化产物”这一层 MCP。

## 1. Notebook、代码与网页执行

| 资源 | 场景 | 简述 | 链接 |
| --- | --- | --- | --- |
| Jupyter MCP Server | Notebook 控制 | 支持查看、编辑、执行和管理 Jupyter Notebook，是科研实验工作流里最核心的执行层之一。 | [datalayer/jupyter-mcp-server](https://github.com/datalayer/jupyter-mcp-server) |
| GitHub MCP Server | 代码与协作 | 适合读取仓库、Issue、PR、提交记录与 CI 信息。 | [github/github-mcp-server](https://github.com/github/github-mcp-server) |
| Playwright MCP | 网页自动化 | 适合自动登录平台、抓取实验面板、浏览论文官网和交互式网页。 | [microsoft/playwright-mcp](https://github.com/microsoft/playwright-mcp) |
| Chart MCP Server | 图表生成 | 适合把实验结果快速整理成可读图表。 | [antvis/mcp-server-chart](https://github.com/antvis/mcp-server-chart) |
| MarkItDown | 文档与附件预处理 | 适合把附件、表格、截图与 Office 文档转换为 Markdown 进入后续分析链路。 | [microsoft/markitdown](https://github.com/microsoft/markitdown) |
| MCP 官方 Servers | 基础能力样例 | 官方参考实现包含 `filesystem`、`fetch`、`memory` 等高频基础能力，适合理解“底层工具层”如何组织。 | [modelcontextprotocol/servers](https://github.com/modelcontextprotocol/servers) |

## 2. 数据库、分析库与检索后端

| 资源 | 场景 | 简述 | 链接 |
| --- | --- | --- | --- |
| PostgreSQL MCP Server | 结构化数据查询 | 适合对实验数据库、标注库、结果库做只读查询。 | [yuru-sha/mcp-server-postgres](https://github.com/yuru-sha/mcp-server-postgres) |
| PGMCP | 自然语言问库 | 对现有 PostgreSQL 数据库做自然语言查询，适合分析型工作流。 | [subnetmarco/pgmcp](https://github.com/subnetmarco/pgmcp) |
| SQLite MCP Server | 轻量本地数据库 | 适合单机分析、原型验证与小型结果库。 | [prayanks/mcp-sqlite-server](https://github.com/prayanks/mcp-sqlite-server) |
| MotherDuck / DuckDB MCP | OLAP 与本地分析 | 适合 SQL analytics、本地数据文件分析与 DuckDB 工作流。 | [motherduckdb/mcp-server-motherduck](https://github.com/motherduckdb/mcp-server-motherduck) |
| DuckDB MCP Extension | SQL 与 MCP 桥接 | 适合把 DuckDB 同时作为 MCP 客户端和服务器理解。 | [teaguesterling/duckdb_mcp](https://github.com/teaguesterling/duckdb_mcp) |
| Milvus MCP Server | 向量数据库 | 适合 embedding 检索、语义搜索与 RAG 实验。 | [zilliztech/mcp-server-milvus](https://github.com/zilliztech/mcp-server-milvus) |

## 3. 数据集平台、地理信息与外部实验环境

| 资源 | 场景 | 简述 | 链接 |
| --- | --- | --- | --- |
| Kaggle MCP | 数据集发现与下载 | 适合搜索 Kaggle 数据集，并把 EDA 入口接入 MCP 工作流。 | [arrismo/kaggle-mcp](https://github.com/arrismo/kaggle-mcp) |
| Mapbox MCP Server | 地理信息与空间分析 | 对地理编码、路线、可达性、位置 intelligence 场景很有价值。 | [mapbox/mcp-server](https://github.com/mapbox/mcp-server) |
| GeoServer MCP | 空间数据服务 | 适合连接 GeoServer REST API，对地理信息系统与空间数据服务有帮助。 | [mahdin75/geoserver-mcp](https://github.com/mahdin75/geoserver-mcp) |

## 4. 适合研究型系统的基础 MCP 组合

| 组合 | 适用链路 | 说明 |
| --- | --- | --- |
| `filesystem + fetch + github + jupyter` | 最小实验闭环 | 适合文件、网页、代码与 Notebook 统一接入。 |
| `github + postgres + chart` | 实验结果审查 | 适合把代码、结果库和可视化串起来。 |
| `jupyter + motherduck/duckdb + markitdown` | 数据分析与报告 | 适合 notebook 内分析和文档化输出。 |
| `milvus + postgres + kaggle` | RAG / 数据挖掘原型 | 适合数据集获取、结构化存储与向量检索组合。 |

## 5. 选择这类 MCP 时的注意点

1. 与数据库相连的 MCP 优先选择只读模式、事务隔离和显式 schema inspection。
2. 与 Notebook 相连的 MCP 需要额外关注执行副作用、内核状态与输出留痕。
3. 浏览器自动化类 MCP 很适合抓交互网页，但应和正式 API / 学术数据库分层使用。
4. 向量数据库与 SQL 数据库往往适合组合使用，一个负责检索，一个负责结构化核验。
