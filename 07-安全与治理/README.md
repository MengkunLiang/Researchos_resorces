# 安全与治理

这一模块聚焦科研工作流中的权限边界、工具调用风险、研究诚信、数据治理、人工复核、安全评测与软件/模型供应链。适合在把 `agent`、`MCP`、自动化脚本、外部 API 和投稿平台接入研究流程之后，用来补齐可审计、可追溯、可控的治理底座。

## 这一步通常要回答的问题

1. `Skill`、`MCP`、代码执行、网页访问和外部 API 调用应当怎样做最小权限与人机分工。
2. Prompt injection、间接注入、工具越权、敏感数据外泄、confused deputy 等风险应当怎样识别与缓解。
3. 科研场景中的论文初稿、审稿意见、未公开数据、IRB/伦理审批、人类参与者数据和保密材料应当遵循哪些公开规范。
4. 哪些红队框架、benchmark、guardrails、供应链标准与 provenance 工具值得优先接入。
5. 面向 AI/ML、data mining、computational design science 的研究自动化系统，应当怎样建立日志留痕、复核关口与发布前检查。

## 推荐先看

- [安全治理与最佳实践](./安全治理与最佳实践.md)
- [Agent、MCP与工具调用安全](./Agent、MCP与工具调用安全.md)
- [数据治理、科研诚信与合规](./数据治理、科研诚信与合规.md)
- [安全评测、红队与供应链](./安全评测、红队与供应链.md)
- [05-实验执行、复现与评测](../05-实验执行、复现与评测/README.md)
- [06-写作、审稿与投稿](../06-写作、审稿与投稿/README.md)
- [92-MCP/MCP标准与发现平台](../92-MCP/MCP标准与发现平台.md)

## 一、相关 Skills

| 资源 | 类型 | 适合环节 | 简述 | 链接 |
| --- | --- | --- | --- | --- |
| Skills标准与生态 | 仓库内附录 | Skills 总览 | 当前仓库里 `Skill` 标准、生态与宿主实现的主归属页。 | [91-Skills/Skills标准与生态](../91-Skills/Skills标准与生态.md) |
| Skill发现平台与精品合集 | 仓库内附录 | 外部技能库补充 | 适合继续扩充公开 `Skill` 生态、精品合集和多宿主技能资源。 | [91-Skills/Skill发现平台与精品合集](../91-Skills/Skill发现平台与精品合集.md) |
| Anthropic Skills | 官方 Skill 库 | 工具封装与文档处理 | 覆盖 `mcp-builder`、`pdf`、`docx`、`pptx`、`doc-coauthoring` 等高频能力，适合学习权限边界与工具封装方式。 | [anthropics/skills](https://github.com/anthropics/skills) |
| OpenAI Skills | 官方 Skill 库 | 代码、审查与工程治理 | 更适合围绕代码审查、工程诊断、工作流执行和工具编排建立可复核流程。 | [openai/skills](https://github.com/openai/skills) |
| OpenHands Skills Docs | 技能文档与共享注册表 | 开发代理与技能治理 | 适合查看共享技能、公开技能发现与宿主接入方式。 | [OpenHands Skills Docs](https://docs.openhands.dev/overview/skills/overview) |
| AI Research SKILLs | 科研工程技能总库 | 研究工程与实验自动化 | 覆盖训练、评测、实验工程和研究工作流，是补齐科研自动化能力边界时很有价值的公开技能库。 | [Orchestra-Research/AI-Research-SKILLs](https://github.com/Orchestra-Research/AI-Research-SKILLs) |

## 二、相关 MCP 与协议文档

| 资源 | 类型 | 适合环节 | 简述 | 链接 |
| --- | --- | --- | --- | --- |
| MCP标准与发现平台 | 仓库内附录 | MCP 总览 | 当前仓库里 `MCP` 规范、发现平台与生态入口的主归属页。 | [92-MCP/MCP标准与发现平台](../92-MCP/MCP标准与发现平台.md) |
| 科研常用MCP清单 | 仓库内附录 | 常用 MCP 清单 | 适合回查文献、代码、知识库、写作与实验相关 MCP。 | [92-MCP/科研常用MCP清单](../92-MCP/科研常用MCP清单.md) |
| MCP Security Best Practices | 官方规范 | MCP 安全基线 | 面向 `MCP` 客户端、服务器与实现者的官方安全建议。 | [modelcontextprotocol.io](https://modelcontextprotocol.io/specification/2025-06-18/basic/security_best_practices) |
| MCP Authorization | 官方规范 | 认证授权与令牌边界 | 说明 `OAuth`、授权委托与远程服务器场景下的权限边界。 | [modelcontextprotocol.io](https://modelcontextprotocol.io/specification/2025-06-18/basic/authorization) |
| GitHub MCP Server | 官方 MCP Server | 审计、代码与变更留痕 | 适合把代码、Issue、PR、提交和讨论放到可追溯工作流里。 | [github/github-mcp-server](https://github.com/github/github-mcp-server) |
| GitMCP | 只读型仓库 MCP | 公共仓库文档回查 | 适合以低权限方式查阅开源仓库内容、减少直接写操作暴露面。 | [idosal/git-mcp](https://github.com/idosal/git-mcp) |
| Jupyter MCP Server | notebook MCP | 实验执行与隔离 | 适合 notebook 读取、修改和执行，但应与环境隔离、日志留痕和资源配额一起使用。 | [datalayer/jupyter-mcp-server](https://github.com/datalayer/jupyter-mcp-server) |
| OpenReview MCP | 社区 MCP | 审稿流程与讨论回查 | 适合追踪投稿记录与讨论脉络，但应特别注意未公开评审材料的访问控制。 | [openreview/openreview-mcp](https://github.com/openreview/openreview-mcp) |

## 三、治理框架与官方规范

| 资源 | 类型 | 更适合的用途 | 链接 |
| --- | --- | --- | --- |
| NIST AI RMF 1.0 | 官方治理框架 | 建立 AI 风险识别、映射、测量与治理语言。 | [NIST](https://www.nist.gov/publications/artificial-intelligence-risk-management-framework-ai-rmf-10) |
| NIST Generative AI Profile | 官方治理补充 | 把生成式 AI 特有风险映射到 `AI RMF`。 | [NIST](https://www.nist.gov/publications/artificial-intelligence-risk-management-framework-generative-artificial-intelligence-profile) |
| OWASP Top 10 for LLM Applications | 官方安全清单 | 快速识别提示注入、数据泄露、过度权限等常见风险。 | [OWASP](https://owasp.org/www-project-top-10-for-large-language-model-applications/) |
| OWASP Top 10 for Agentic Applications 2026 | 官方安全清单 | 适合补足多工具、多步骤、带副作用 agent 的风险建模。 | [OWASP GenAI Security Project](https://genai.owasp.org/resource/owasp-top-10-for-agentic-applications-for-2026/) |
| Secure AI Framework (SAIF) | 官方安全框架 | 适合把模型、系统、基础设施和软件供应链放在同一安全框架下讨论。 | [Google](https://blog.google/technology/safety-security/introducing-googles-secure-ai-framework/) |
| MITRE ATLAS | 官方对抗知识库 | 适合把 AI 系统威胁映射到 tactics、techniques 与 mitigations。 | [MITRE ATLAS](https://atlas.mitre.org/) |
| Updated Preparedness Framework | 官方风险治理框架 | 适合参考高能力模型的发布前评估与分级治理思路。 | [OpenAI](https://openai.com/index/updating-our-preparedness-framework/) |

## 四、评测、红队与供应链工具

| 资源 | 类型 | 适合环节 | 简述 | 链接 |
| --- | --- | --- | --- | --- |
| 安全评测、红队与供应链 | 仓库内详表 | 安全评测总览 | 当前模块里红队框架、benchmark、guardrails 与供应链标准的主归属页。 | [安全评测、红队与供应链](./安全评测、红队与供应链.md) |
| garak | LLM 漏洞扫描器 | prompt safety 与模型探测 | 面向 LLM 漏洞探测、探针运行与测试报告生成。 | [NVIDIA/garak](https://github.com/NVIDIA/garak) |
| inspect_ai | 评测与红队框架 | 可复现实验与任务化评测 | 适合把安全评测、对抗任务和多轮代理任务纳入结构化评测。 | [UKGovernmentBEIS/inspect_ai](https://github.com/UKGovernmentBEIS/inspect_ai) |
| promptfoo | red teaming 与回归评测框架 | prompt、RAG 与 agent 测试 | 适合做越狱、注入、策略回归与自动化对照测试。 | [promptfoo/promptfoo](https://github.com/promptfoo/promptfoo) |
| PyRIT | AI red teaming 框架 | 风险测试与攻击编排 | 适合围绕生成式 AI 系统组织红队测试。 | [Azure/PyRIT](https://github.com/Azure/PyRIT) |
| HarmBench / JailbreakBench / CyberSec Eval | 安全 benchmark | 攻击与防护对照 | 覆盖越狱、有害输出与网络安全任务评测。 | [HarmBench](https://github.com/centerforaisafety/HarmBench)、[JailbreakBench](https://github.com/JailbreakBench/jailbreakbench)、[PurpleLlama/CybersecurityBenchmarks](https://github.com/meta-llama/PurpleLlama/tree/main/CybersecurityBenchmarks) |
| SLSA / Sigstore / SPDX / CycloneDX / in-toto | 供应链与 provenance 标准 | 构建可验证交付链 | 适合做产物签名、SBOM、来源证明与发布链验证。 | [SLSA](https://slsa.dev/)、[Sigstore](https://www.sigstore.dev/)、[SPDX](https://spdx.dev/)、[CycloneDX](https://cyclonedx.org/)、[in-toto](https://in-toto.io/) |

## 五、外部整合入口

| 资源 | 类型 | 更适合的用途 | 链接 |
| --- | --- | --- | --- |
| 外部导航与合集 | 仓库内索引 | 继续扩展安全与治理周边资源。 | [98-全局索引/外部导航与合集](../98-全局索引/外部导航与合集.md) |
| OWASP GenAI Security Project | 官方项目页 | 扫 LLM、agent、MCP 与 red teaming 最新安全资料。 | [OWASP GenAI Security Project](https://genai.owasp.org/) |
| MITRE ATLAS | 官方知识库 | 扫 AI 对抗技术、攻击矩阵与案例。 | [MITRE ATLAS](https://atlas.mitre.org/) |
| awesome-reproducible-research | 可复现科研合集 | 从 reproducibility 角度补治理与留痕工具。 | [leipzig/awesome-reproducible-research](https://github.com/leipzig/awesome-reproducible-research) |
| awesome-open-mlops | 开源 MLOps 合集 | 补实验平台、部署、监控与供应链相关工具。 | [fuzzylabs/awesome-open-mlops](https://github.com/fuzzylabs/awesome-open-mlops) |

## 六、推荐组合

1. `MCP Security Best Practices + MCP Authorization + GitHub MCP Server + GitMCP`
   适合给公开仓库回查、代码审阅和有限写操作建立最小权限边界。
2. `OWASP LLM Top 10 + OWASP Agentic Top 10 + MITRE ATLAS + SAIF`
   适合把风险识别、攻击面映射和控制措施放到统一框架里。
3. `garak + promptfoo + inspect_ai + PyRIT`
   适合把 prompt 安全、red teaming 与回归评测串成持续测试链。
4. `ORI + OHRP + NIH DMS Policy + FAIR Principles + ICMJE / COPE`
   适合把研究诚信、数据管理、论文写作和同行评审环节纳入同一治理面。
5. `SLSA + Sigstore + SPDX / CycloneDX + in-toto`
   适合把脚本、容器、模型和交付产物的 provenance 与发布链验证补齐。

## 七、仓库内延伸阅读

- [04-新颖性判断与综述](../04-新颖性判断与综述/README.md)
- [05-实验执行、复现与评测](../05-实验执行、复现与评测/README.md)
- [06-写作、审稿与投稿](../06-写作、审稿与投稿/README.md)
- [08-方向专题/AI-ML-DataMining资源](../08-方向专题/AI-ML-DataMining资源.md)
