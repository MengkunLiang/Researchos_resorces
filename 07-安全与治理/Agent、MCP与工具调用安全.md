# Agent、MCP与工具调用安全

这一页聚焦 `agent`、`MCP`、工具调用与外部动作链路的安全问题。重点不是把所有风险都推给模型本身，而是把协议、提示词、工具描述、认证授权、日志留痕与人工审批放到同一张图里。

## 一、优先参考的官方资料

| 资源 | 类型 | 更适合的用途 | 链接 |
| --- | --- | --- | --- |
| MCP Security Best Practices | 官方规范 | 建立 `MCP` 客户端、服务器与宿主的共同安全基线。 | [modelcontextprotocol.io](https://modelcontextprotocol.io/specification/2025-06-18/basic/security_best_practices) |
| MCP Authorization | 官方规范 | 处理 `OAuth`、token delegation、远程服务器与权限委托。 | [modelcontextprotocol.io](https://modelcontextprotocol.io/specification/2025-06-18/basic/authorization) |
| A Practical Guide for Secure MCP Server Development | 官方安全指南 | 面向 `MCP server` 的常见风险与开发检查项。 | [OWASP GenAI Security Project](https://genai.owasp.org/resource/a-practical-guide-for-secure-mcp-server-development/) |
| OWASP Top 10 for LLM Applications | 官方安全清单 | 用于盘点提示注入、数据泄露、供应链与过度权限等基础风险。 | [OWASP](https://owasp.org/www-project-top-10-for-large-language-model-applications/) |
| OWASP Top 10 for Agentic Applications 2026 | 官方安全清单 | 适合盘点多工具、多步骤、长上下文 agent 的风险。 | [OWASP GenAI Security Project](https://genai.owasp.org/resource/owasp-top-10-for-agentic-applications-for-2026/) |
| Mitigate jailbreaks and prompt injections | 官方开发文档 | 适合理解提示注入、越狱与不可信内容隔离。 | [Anthropic Docs](https://docs.anthropic.com/en/docs/test-and-evaluate/strengthen-guardrails/mitigate-jailbreaks) |
| Reduce prompt leak | 官方开发文档 | 适合补 prompt 隐私、系统提示泄露和上下文隔离。 | [Anthropic Docs](https://docs.anthropic.com/en/docs/test-and-evaluate/strengthen-guardrails/reduce-prompt-leak) |
| Secure AI Framework (SAIF) | 官方安全框架 | 适合从更高层看模型、系统、基础设施与供应链安全。 | [Google](https://blog.google/technology/safety-security/introducing-googles-secure-ai-framework/) |
| MITRE ATLAS | 官方攻击知识库 | 适合把 `agent` 风险映射到攻击 tactics 与 techniques。 | [MITRE ATLAS](https://atlas.mitre.org/) |

## 二、科研场景中最常见的工具调用风险

| 风险 | 常见触发面 | 更稳妥的做法 |
| --- | --- | --- |
| 直接 prompt injection | 用户输入、issue、聊天记录、指令模板。 | 系统提示与工具策略分层保存；关键安全规则不与普通上下文混写。 |
| 间接 prompt injection | 网页、PDF、README、表格、网页脚本和补充材料。 | 把抓取内容视为不可信数据；读取层与执行层分离。 |
| Confused deputy | 一个安全工具被诱导替另一方执行高权限操作。 | 工具层做显式授权确认，并把调用主体、项目和作用域写入日志。 |
| 过度权限 | 一个工具同时可读写仓库、云盘、知识库和外部系统。 | 按任务拆分 token、目录、仓库和项目作用域；能只读就不授写。 |
| 长上下文污染 | 早期恶意指令在后续多轮任务中持续生效。 | 做上下文窗口切分、阶段性清空和工具前置检查。 |
| 非预期外部动作 | 直接发邮件、发评审意见、提交 PR、触发发布。 | 对外动作统一走审批或 `two-step confirmation`。 |
| 工具描述不清 | 模型误解工具作用，调用错误函数或错误参数。 | 用清晰 schema、强约束参数和失败时的拒绝策略。 |

## 三、围绕 MCP 的具体设计建议

| 设计点 | 建议 |
| --- | --- |
| Server 暴露面 | 只暴露完成当前任务所需的最小工具集，不把“未来可能用到”的工具一起开放。 |
| Credential | 尽量使用项目级、只读、短期、可撤销的 credential；避免复用主账号长期令牌。 |
| Remote MCP | 远程 `MCP` 优先配合正式认证授权、来源校验、速率限制和审计日志。 |
| Tool schema | 参数名、危险参数、写操作和外部副作用都应在 schema 与说明里显式标注。 |
| Resource 与 Tool 区分 | 只读资源与带副作用工具分开设计，便于审计与授权。 |
| 日志留痕 | 至少记录调用时间、调用者、工具名、参数摘要、返回状态和关联项目。 |
| Sandbox | notebook、shell、Python、浏览器与抓取工具优先放在隔离运行环境里。 |
| Human gate | 写仓库、对外提交、触发部署、发邮件、写数据库等动作放入人工审批。 |

## 四、适合科研工作流的权限分层

| 层级 | 能力范围 | 典型工具 |
| --- | --- | --- |
| `L0` 公开只读 | 网页、公开论文、公开仓库、公开 benchmark。 | 搜索、只读 GitHub、只读文献库。 |
| `L1` 私有只读 | 私有笔记、私有文献库、项目文档。 | Zotero、知识库、私有仓库只读访问。 |
| `L2` 受控执行 | notebook、脚本、图表生成、实验追踪。 | Jupyter、Python、Chart、tracking 平台。 |
| `L3` 高风险写操作 | 写仓库、改配置、提交结果、更新数据库。 | GitHub 写入、数据库写入、对象存储写入。 |
| `L4` 对外动作 | 发投稿、发邮件、发消息、触发 release 或部署。 | 投稿系统、邮件、消息平台、CI/CD 发布。 |

科研场景中，`L0-L2` 更适合自动化，`L3-L4` 更适合审批驱动或半自动化。

## 五、适合落地的安全测试工具

| 资源 | 类型 | 更适合的用途 | 链接 |
| --- | --- | --- | --- |
| promptfoo | red teaming 与回归框架 | 测 prompt、RAG、agent、工具调用与策略回归。 | [promptfoo/promptfoo](https://github.com/promptfoo/promptfoo) |
| evil-mcp-server | MCP 风险演示 | 适合做 `MCP` 服务器威胁建模与防护演练。 | [promptfoo/evil-mcp-server](https://github.com/promptfoo/evil-mcp-server) |
| garak | LLM 漏洞扫描 | 用探针批量测试注入、有害输出和模型行为。 | [NVIDIA/garak](https://github.com/NVIDIA/garak) |
| PyRIT | red teaming 框架 | 适合做更系统的攻击编排与风险测试。 | [Azure/PyRIT](https://github.com/Azure/PyRIT) |
| inspect_ai | 可复现实验与评测框架 | 适合把工具安全与 agent 任务写成可回放评测。 | [UKGovernmentBEIS/inspect_ai](https://github.com/UKGovernmentBEIS/inspect_ai) |
| NeMo Guardrails | guardrail 框架 | 适合给对话和工具流程增加规则层。 | [NVIDIA/NeMo-Guardrails](https://github.com/NVIDIA/NeMo-Guardrails) |
| LLM Guard | 输入输出过滤工具 | 适合补输入、输出和提示词方向的防护层。 | [protectai/llm-guard](https://github.com/protectai/llm-guard) |

## 六、最常用的检查清单

1. 对外抓取内容是否按“不可信输入”处理。
2. 是否把只读资源、执行工具和对外动作分成不同权限层。
3. 高风险工具是否使用独立 token、最小作用域和短期 credential。
4. 是否保留了调用日志、失败日志与参数摘要。
5. notebook、shell 与浏览器是否在隔离环境中运行。
6. 是否为 `PR`、邮件、投稿、数据库写入等动作设置审批门。
7. 是否已经用 `promptfoo`、`garak`、`PyRIT` 或 `inspect_ai` 做过基本安全测试。

## 七、延伸阅读

- [安全治理与最佳实践](./安全治理与最佳实践.md)
- [安全评测、红队与供应链](./安全评测、红队与供应链.md)
- [92-MCP/MCP标准与发现平台](../92-MCP/MCP标准与发现平台.md)
