# 实验执行与数据工程 MCP

这一页聚焦“实验能否跑起来、数据能否查得到、结果能否回写成结构化产物”这一层 MCP。

## 1. Notebook、代码与网页执行

| 资源 | 场景 | 简述 | 链接 |
| --- | --- | --- | --- |
| Jupyter MCP Server | Notebook 控制 | 支持查看、编辑、执行和管理 Jupyter Notebook，是科研实验工作流里最核心的执行层之一。 | [datalayer/jupyter-mcp-server](https://github.com/datalayer/jupyter-mcp-server) |
| Jupyter Notebook MCP | Notebook 交互 | 提供另一条较轻量的 notebook 交互实现路线。 | [jjsantos01/jupyter-notebook-mcp](https://github.com/jjsantos01/jupyter-notebook-mcp) |
| GitHub MCP Server | 代码与协作 | 适合读取仓库、Issue、PR、提交记录与 CI 信息。 | [github/github-mcp-server](https://github.com/github/github-mcp-server) |
| Playwright MCP | 网页自动化 | 适合自动登录平台、抓取实验面板、浏览论文官网和交互式网页。 | [microsoft/playwright-mcp](https://github.com/microsoft/playwright-mcp) |
| Chart MCP Server | 图表生成 | 适合把实验结果快速整理成可读图表。 | [antvis/mcp-server-chart](https://github.com/antvis/mcp-server-chart) |
| MarkItDown | 文档与附件预处理 | 适合把附件、表格、截图与 Office 文档转换为 Markdown 进入后续分析链路。 | [microsoft/markitdown](https://github.com/microsoft/markitdown) |
| GitMCP | 公共仓库文档访问 | 适合快速读取 benchmark 仓库、README、配置和示例。 | [idosal/git-mcp](https://github.com/idosal/git-mcp) |
| Optuna MCP Server | HPO 与 study 分析 | 适合发起 study、读取 trial、分析优化结果和可视化。 | [optuna/optuna-mcp](https://github.com/optuna/optuna-mcp) |
| Prefect MCP Server | workflow 观察 | 适合读取 flow run、deployment、日志和调度状态。 | [PrefectHQ/prefect-mcp-server](https://github.com/PrefectHQ/prefect-mcp-server) |
| MCP for ZenML | pipeline 与 artifact | 适合查看 pipeline run、artifact 和触发新运行。 | [zenml-io/mcp-zenml](https://github.com/zenml-io/mcp-zenml) |
| Docker Hub MCP | 容器与镜像发现 | 适合给实验环境与 benchmark 容器选择基础镜像。 | [docker/hub-mcp](https://github.com/docker/hub-mcp) |
| MCP 官方 Servers | 基础能力样例 | 官方参考实现包含 `filesystem`、`fetch`、`memory` 等高频基础能力，适合理解“底层工具层”如何组织。 | [modelcontextprotocol/servers](https://github.com/modelcontextprotocol/servers) |

## 2. 数据库、分析库与检索后端

| 资源 | 场景 | 简述 | 链接 |
| --- | --- | --- | --- |
| PostgreSQL MCP Server | 结构化数据查询 | 适合对实验数据库、标注库、结果库做只读查询。 | [yuru-sha/mcp-server-postgres](https://github.com/yuru-sha/mcp-server-postgres) |
| PGMCP | 自然语言问库 | 对现有 PostgreSQL 数据库做自然语言查询，适合分析型工作流。 | [subnetmarco/pgmcp](https://github.com/subnetmarco/pgmcp) |
| SQLite MCP Server | 轻量本地数据库 | 适合单机分析、原型验证与小型结果库。 | [prayanks/mcp-sqlite-server](https://github.com/prayanks/mcp-sqlite-server) |
| MotherDuck / DuckDB MCP | OLAP 与本地分析 | 适合 SQL analytics、本地数据文件分析与 DuckDB 工作流。 | [motherduckdb/mcp-server-motherduck](https://github.com/motherduckdb/mcp-server-motherduck) |
| DuckDB MCP Extension | SQL 与 MCP 桥接 | 适合把 DuckDB 同时作为 MCP 客户端和服务器理解。 | [teaguesterling/duckdb_mcp](https://github.com/teaguesterling/duckdb_mcp) |
| dbhub | 多数据库 MCP | 适合零依赖访问 Postgres、MySQL 与 SQLite。 | [bytebase/dbhub](https://github.com/bytebase/dbhub) |
| Milvus MCP Server | 向量数据库 | 适合 embedding 检索、语义搜索与 RAG 实验。 | [zilliztech/mcp-server-milvus](https://github.com/zilliztech/mcp-server-milvus) |

## 3. 数据集平台、地理信息与外部实验环境

| 资源 | 场景 | 简述 | 链接 |
| --- | --- | --- | --- |
| Kaggle MCP | 数据集发现与下载 | 适合搜索 Kaggle 数据集，并把 EDA 入口接入 MCP 工作流。 | [arrismo/kaggle-mcp](https://github.com/arrismo/kaggle-mcp) |
| Mapbox MCP Server | 地理信息与空间分析 | 对地理编码、路线、可达性、位置 intelligence 场景很有价值。 | [mapbox/mcp-server](https://github.com/mapbox/mcp-server) |
| GeoServer MCP | 空间数据服务 | 适合连接 GeoServer REST API，对地理信息系统与空间数据服务有帮助。 | [mahdin75/geoserver-mcp](https://github.com/mahdin75/geoserver-mcp) |

## 4. 相关 CLI 与终端工具

| 资源 | 场景 | 简述 | 链接 |
| --- | --- | --- | --- |
| nbconvert | notebook 导出 | 适合把 notebook 转成 PDF、HTML、LaTeX。 | [nbconvert](https://nbconvert.readthedocs.io/) |
| nbstripout | notebook 清理 | 适合去掉输出，保持更干净的 git diff。 | [kynan/nbstripout](https://github.com/kynan/nbstripout) |
| duckdb | 分析型 SQL CLI | 适合直接分析 CSV / Parquet / JSON。 | [DuckDB](https://duckdb.org/) |
| jq | JSON 处理 | 适合切片、过滤、转换实验 JSON 输出。 | [jqlang/jq](https://github.com/jqlang/jq) |
| csvkit | CSV 工具集 | 适合表格数据检查、筛选和格式转换。 | [wireservice/csvkit](https://github.com/wireservice/csvkit) |
| git-lfs | 大文件版本控制 | 适合管理模型权重、数据切片和大附件。 | [git-lfs](https://git-lfs.com/) |
| dvc | 数据版本控制 | 适合把数据与 pipeline 也纳入版本化管理。 | [DVC](https://dvc.org/) |
| tmux / GNU parallel | 远程与并行执行 | 适合长实验保活和批量任务并行。 | [tmux](https://github.com/tmux/tmux)、[GNU parallel](https://www.gnu.org/software/parallel/) |
| hyperfine | 命令行基准测试 | 适合比较脚本与工具链运行耗时。 | [sharkdp/hyperfine](https://github.com/sharkdp/hyperfine) |
| uv / ripgrep / fd / fzf | 开发效率工具 | 适合依赖管理、代码搜索、文件遍历和交互式查找。 | [astral-sh/uv](https://github.com/astral-sh/uv)、[BurntSushi/ripgrep](https://github.com/BurntSushi/ripgrep)、[sharkdp/fd](https://github.com/sharkdp/fd)、[junegunn/fzf](https://github.com/junegunn/fzf) |

## 5. 适合研究型系统的基础 MCP 组合

| 组合 | 适用链路 | 说明 |
| --- | --- | --- |
| `filesystem + fetch + github + jupyter` | 最小实验闭环 | 适合文件、网页、代码与 Notebook 统一接入。 |
| `github + postgres + chart` | 实验结果审查 | 适合把代码、结果库和可视化串起来。 |
| `jupyter + motherduck/duckdb + markitdown` | 数据分析与报告 | 适合 notebook 内分析和文档化输出。 |
| `milvus + postgres + kaggle` | RAG / 数据挖掘原型 | 适合数据集获取、结构化存储与向量检索组合。 |
| `jupyter + optuna + chart + github` | 调参与结果分析 | 适合把试验、调参和可视化串成闭环。 |
| `github + prefect + zenml` | pipeline 观察与诊断 | 适合同时查看代码、workflow、artifact 和运行状态。 |
| `jupyter + duckdb + jq + nbconvert` | 数据分析与报告导出 | 适合从原始结果到结构化分析再到报告输出。 |

## 6. 选择这类 MCP 时的注意点

1. 与数据库相连的 MCP 优先选择只读模式、事务隔离和显式 schema inspection。
2. 与 Notebook 相连的 MCP 需要额外关注执行副作用、内核状态与输出留痕。
3. 浏览器自动化类 MCP 很适合抓交互网页，但应和正式 API / 学术数据库分层使用。
4. 向量数据库与 SQL 数据库往往适合组合使用，一个负责检索，一个负责结构化核验。
