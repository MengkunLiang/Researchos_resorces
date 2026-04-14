# 通用 Agent 框架

这一页收录“不是专为科研而生，但很适合搭科研智能体”的通用框架。它们更像底座层，负责状态管理、工具调用、工作流编排、结构化输出和生产化部署。

## 1. 编排与工作流内核

| 资源 | 定位 | 适合关注的点 | 链接 |
| --- | --- | --- | --- |
| LangGraph | 图式工作流编排 | 状态机、检查点、回退、人工 gate、多阶段产物管理。 | [langchain-ai/langgraph](https://github.com/langchain-ai/langgraph) |
| Microsoft Agent Framework | 新一代微软代理底座 | 图式 workflow、MCP/A2A 互操作、Python/.NET 双栈、生产级状态管理。 | [microsoft/agent-framework](https://github.com/microsoft/agent-framework) |
| AutoGen | 多 Agent 协作 | 经典多代理消息模式，适合角色分工和快速多代理原型。 | [microsoft/autogen](https://github.com/microsoft/autogen) |
| Google ADK | 代码优先 Agent SDK | 工具注册、评测、部署与可组合代理模块。 | [google/adk-python](https://github.com/google/adk-python) |
| Semantic Kernel | 企业级 AI 编排 | 插件、memory、workflow、连接器和较成熟的工程化能力。 | [microsoft/semantic-kernel](https://github.com/microsoft/semantic-kernel) |
| OpenHands Software Agent SDK | 代码代理 SDK | 本地或远程工作区、文件/终端工具、面向软件与实验实现的执行环境。 | [OpenHands/software-agent-sdk](https://github.com/OpenHands/software-agent-sdk) |

## 2. 结构化与生产化框架

| 资源 | 定位 | 适合关注的点 | 链接 |
| --- | --- | --- | --- |
| PydanticAI | 结构化 Agent | schema 驱动输出、类型安全、工具调用与可测试性。 | [pydantic/pydantic-ai](https://github.com/pydantic/pydantic-ai) |
| Agno | 多 Agent 与运行时 | agent/team/workflow 一体化，带知识、记忆、guardrails 与运行时。 | [agno-agi/agno](https://github.com/agno-agi/agno) |
| Semantic Kernel | 插件与连接器生态 | 更适合需要 memory、插件系统和企业连接器的场景。 | [microsoft/semantic-kernel](https://github.com/microsoft/semantic-kernel) |
| Microsoft Agent Framework | 长流程与可观测性 | checkpoint、telemetry、workflow 分支控制。 | [microsoft/agent-framework](https://github.com/microsoft/agent-framework) |

## 3. 轻量原型与多角色模拟

| 资源 | 定位 | 适合关注的点 | 链接 |
| --- | --- | --- | --- |
| smolagents | 轻量级代理 | 上手快，适合课程 demo、小型实验和工具调用原型。 | [huggingface/smolagents](https://github.com/huggingface/smolagents) |
| CrewAI | 角色协作框架 | `Scout / Reader / Writer / Reviewer` 这类角色式流程很容易搭建。 | [crewAIInc/crewAI](https://github.com/crewAIInc/crewAI) |
| CAMEL | 多代理研究平台 | 社会化代理、任务分工和协作研究实验较活跃。 | [camel-ai/camel](https://github.com/camel-ai/camel) |
| AutoGen | 角色式协作实验 | 群聊、代理角色和对话驱动协作仍然非常常用。 | [microsoft/autogen](https://github.com/microsoft/autogen) |

## 4. 检索增强、优化与 Agentic RAG 底座

| 资源 | 定位 | 适合关注的点 | 链接 |
| --- | --- | --- | --- |
| DSPy | 程序化提示与优化 | 程序化 prompt、模块组合、自动优化、评测驱动改进。 | [stanfordnlp/dspy](https://github.com/stanfordnlp/dspy) |
| DeepAgents | 深度代理模板 | LangGraph 团队推出的深度代理模式与范式参考。 | [langchain-ai/deepagents](https://github.com/langchain-ai/deepagents) |
| LlamaIndex | 数据与 RAG 工作流 | 文档索引、检索、工具、知识工作流和 agentic RAG。 | [run-llama/llama_index](https://github.com/run-llama/llama_index) |
| Haystack | 检索与评测管线 | 检索、生成、评测和 pipeline 组装能力较成熟。 | [deepset-ai/haystack](https://github.com/deepset-ai/haystack) |
| LDP | Agent / 环境 / 优化器解耦 | 更适合作为科研型代理训练与评测实验底座。 | [Future-House/ldp](https://github.com/Future-House/ldp) |

## 5. 面向科研工作流的选型视角

| 关注点 | 更适合优先看的框架 | 说明 |
| --- | --- | --- |
| 严谨状态机与长流程控制 | `LangGraph`、`Microsoft Agent Framework`、`Semantic Kernel` | 适合有明显阶段边界、需要 checkpoint 和人工审核的系统。 |
| 角色化多 Agent 原型 | `AutoGen`、`CrewAI`、`CAMEL` | 适合快速验证“检索员、阅读员、写作者、审稿员”这类角色分工。 |
| 结构化 artifact 与类型安全 | `PydanticAI`、`Microsoft Agent Framework` | 适合强调 schema、实验记录、证据卡片与结果对象化输出。 |
| 代码执行与实验落地 | `OpenHands SDK`、`Google ADK`、`Agno` | 适合需要文件系统、终端、远程工作区和工具链整合的场景。 |
| prompt 程序化优化 | `DSPy`、`LDP` | 适合把 research agent 的子模块做成可调优、可评测组件。 |
| 检索与知识工作流 | `LlamaIndex`、`Haystack`、`DSPy` | 更贴近文献检索、知识库问答和 agentic RAG 链路。 |

## 6. 与科研系统搭配时最常见的误区

1. 只选编排框架，不选学术数据源。科研代理常见瓶颈往往在 `OpenAlex / OpenReview / Semantic Scholar / Zotero / PDF parser`，而不是工作流图本身。
2. 把所有逻辑都塞进单轮 prompt。更稳的路线通常是把检索、证据抽取、novelty 审计、实验执行、写作整理拆成多个 artifact。
3. 过早追求全自动。对于科研任务，很多系统在“半自动 + 显式证据链 + 人工 gate”时比完全自动更可靠。

## 7. 相关页面

- [科研Agent系统](./科研Agent系统.md)
- [自动科研与闭环系统](./自动科研与闭环系统.md)
- [Deep Research与研究工作台](./Deep%20Research与研究工作台.md)
- [科研工作流设计模式](./科研工作流设计模式.md)
- [MCP标准与发现平台](../02-MCP/MCP标准与发现平台.md)
