# MCP 标准与发现平台

MCP（Model Context Protocol）是这类科研智能体最关键的外部能力接入层之一。你可以把它理解成“让模型安全、结构化地连外部工具和数据源”的标准接口。

## 1. 官方标准与参考实现

| 资源 | 类型 | 简述 | 链接 |
| --- | --- | --- | --- |
| Model Context Protocol 官方文档 | 官方文档 | MCP 的总入口，先看这里理解概念、客户端、服务器、工具与资源模型。 | [modelcontextprotocol.io](https://modelcontextprotocol.io/docs/getting-started/intro) |
| MCP 规范仓库 | 官方规范 | 官方规范与文档源码仓库，适合跟协议演进。 | [modelcontextprotocol/modelcontextprotocol](https://github.com/modelcontextprotocol/modelcontextprotocol) |
| MCP 官方 Servers 仓库 | 参考实现 | 官方参考服务器集合，包含 `filesystem`、`fetch`、`memory` 等经典示例。 | [modelcontextprotocol/servers](https://github.com/modelcontextprotocol/servers) |
| MCP Registry | 官方注册表 | 官方注册表入口，适合做标准化发现与安装。 | [registry.modelcontextprotocol.io](https://registry.modelcontextprotocol.io/) |

## 2. MCP 发现与索引平台

| 资源 | 类型 | 简述 | 链接 |
| --- | --- | --- | --- |
| Awesome MCP Servers | Awesome 列表 | 一个覆盖面很广的 MCP Server 汇总仓库，适合扫全局生态。 | [TensorBlock/awesome-mcp-servers](https://github.com/TensorBlock/awesome-mcp-servers) |
| Glama MCP Servers | 发现平台 | 面向 MCP Server 的可浏览目录，适合按分类找活跃项目。 | [Glama MCP Servers](https://glama.ai/mcp/servers) |
| MCPIndex | 发现平台 | 另一个比较实用的 MCP 索引站，适合查具体服务器页面。 | [mcpindex.net](https://mcpindex.net/en) |
| Smithery | 安装与发现平台 | 社区里常用的 MCP 安装与分发入口之一。 | [smithery.ai](https://smithery.ai/) |
| MCP.so | 目录平台 | 适合浏览热门 MCP 服务和快速对比。 | [mcp.so](https://mcp.so/) |

## 3. 与 Skills 的桥接资源

| 资源 | 类型 | 简述 | 链接 |
| --- | --- | --- | --- |
| skill-to-mcp | 桥接思路 | 把 Skills 暴露成 MCP 资源的思路，适合做统一能力层。 | [biocontext-ai/skill-to-mcp](https://github.com/biocontext-ai/skill-to-mcp) |
| SkillPort | SkillOps / MCP 结合 | 更偏“规模化管理 Skill”的方向，适合平台化建设。 | [gotalab/skillport](https://github.com/gotalab/skillport) |
| mcp.science | 科研 MCP 工作台 | 面向科研场景组织 MCP 的开源项目，适合继续跟踪 science-native 的 MCP 用法。 | [pathintegral-institute/mcp.science](https://github.com/pathintegral-institute/mcp.science) |

## 4. 选型建议

### 如果你现在还没用过 MCP

推荐顺序：

1. 先读 `modelcontextprotocol.io`
2. 再看 `modelcontextprotocol/servers`
3. 然后去 `Awesome MCP Servers`、`Glama`、`MCPIndex` 找科研相关实现

### 如果你在做 ResearchOS 这类平台

建议把 MCP 资源分成三层：

- 基础设施层：`filesystem`、`fetch`、`github`、`notion`、`playwright`
- 科研数据层：`paper-search`、`OpenReview`、`OpenAlex`、`Zotero`
- 实验执行层：`Jupyter`、`数据库`、`图表`、`远程执行`

## 5. 一个很重要的现实问题

MCP 生态增长很快，但科研相关 MCP 的社区实现往往很多、质量差异也很大。选型时建议优先用下面的顺序：

1. 官方实现
2. 官方组织维护的实现
3. 活跃社区实现
4. 只在确有需求时使用个人仓库版本

尤其是会访问私人论文库、代码仓库、云端文档的 MCP，必须先做权限分级。
