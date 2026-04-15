# 科研工程与实验 Skills

这一页收“真正能帮助科研团队跑实验、做训练、做评测、搭研究工程底座”的 skills。它们不一定都写着 `research`，但只要能显著增强科研实验链路，都值得收录。

## 1. 研究工程主力技能包

| 资源 | 类型 | 简述 | 链接 |
| --- | --- | --- | --- |
| AI Research SKILLs | AI 研究工程总库 | 目前最强的 AI/ML 研究工程 skills 库之一，公开信息显示已覆盖 22 个类别、87 个 skills。 | [Orchestra-Research/AI-Research-SKILLs](https://github.com/Orchestra-Research/AI-Research-SKILLs) |
| OpenAI Skills | Codex 官方技能目录 | 虽然不是专门做科研的，但如果团队用 Codex 做实验工程、review、CI、计划拆解，这个官方目录非常值得长期跟。 | [openai/skills](https://github.com/openai/skills) |
| Hugging Face Skills | AI/ML 官方技能包 | 适合数据集构建、训练、评测、Hub 操作和论文发布。 | [huggingface/skills](https://github.com/huggingface/skills) |
| Anthropic Skills | 官方通用技能包 | `pdf/docx/pptx/xlsx` 对科研团队高频，`mcp-builder` 和 `skill-creator` 对平台建设也很重要。 | [anthropics/skills](https://github.com/anthropics/skills) |
| Development Methodology | 方法论技能库 | `test-driven-development`、`systematic-debugging`、`verification-before-completion` 这类方法论技能对实验代码、复现与排错很关键。 | [obra/superpowers](https://github.com/obra/superpowers) |
| Azure Skills | 云端与 AI 平台技能包 | 对需要云训练、推理、资源诊断、成本分析、Foundry/MCP 集成的团队很有帮助。 | [microsoft/azure-skills](https://github.com/microsoft/azure-skills) |
| Vercel Agent Skills | 研发辅助技能包 | 不直接面向科学实验，但对研究网站、demo、可视化页面、实验展示前端很实用。 | [vercel-labs/agent-skills](https://github.com/vercel-labs/agent-skills) |
| OpenHands Skills | 技能文档与注册表 | 适合把技能化执行扩展到软件代理与实验代理。 | [OpenHands Skills Docs](https://docs.openhands.dev/overview/skills/overview) |
| skills CLI / skillkit | 安装与分发工具 | 适合批量发现、安装与迁移公开技能包。 | [vercel-labs/skills](https://github.com/vercel-labs/skills)、[rohitg00/skillkit](https://github.com/rohitg00/skillkit) |
| HKUST-Got-Skills Resources | 综合资源页 | 同时覆盖 `Skills`、`MCP`、CLI 和研究场景推荐，适合继续补库。 | [HKUST-Got-Skills Resources](https://giggleliu.github.io/HKUST-Got-Skills/resources) |

## 2. AI Research SKILLs 最值得关注的覆盖面

根据仓库公开说明，`AI-Research-SKILLs` 已经把技能拆到很细，特别适合 AI/ML 团队：

| 类别 | 代表内容 | 为什么重要 |
| --- | --- | --- |
| Autoresearch / Ideation | `autoresearch`、brainstorming、creative thinking | 让 agent 不只是写代码，而是能串研究流程。 |
| Model Architecture | LitGPT、Mamba、RWKV、NanoGPT、TorchTitan | 适合原型复现和结构理解。 |
| Fine-Tuning / Post-Training | Axolotl、LLaMA-Factory、PEFT、TRL、OpenRLHF、SimPO、verl | 训练和对齐链路最常用。 |
| Distributed / Optimization | DeepSpeed、FSDP、Accelerate、Megatron、Flash Attention、bitsandbytes | 大模型实验工程核心。 |
| Evaluation / Inference | lm-eval-harness、vLLM、TensorRT-LLM、SGLang | 做 benchmark、部署和评测都离不开。 |
| MLOps / Observability | W&B、MLflow、TensorBoard、LangSmith、Phoenix | 很适合实验追踪与 agent 运行观测。 |
| RAG / Agents / Prompt Engineering | LangChain、LlamaIndex、Qdrant、FAISS、DSPy、Instructor、Guidance | 适合科研助理、文献问答和 agent 开发。 |
| Multimodal / Emerging | CLIP、Whisper、LLaVA、SAM、Stable Diffusion、Distillation、Pruning | 适合扩展前沿研究。 |

## 3. Hugging Face Skills 里最适合科研团队先装的

| Skill | 用途 | 链接 |
| --- | --- | --- |
| `hf-cli` | 用 `hf` CLI 操作 Hub、仓库、作业、上传下载模型/数据。 | [HF Skills Docs](https://huggingface.co/docs/hub/agents-skills) |
| `hf_dataset_creator` | 训练数据集设计、模板和脚本。 | [huggingface/skills](https://github.com/huggingface/skills) |
| `hf_model_evaluation` | 跑评测、出评测报告、整理 metrics。 | [huggingface/skills](https://github.com/huggingface/skills) |
| `hf-llm-trainer` | 模型训练、微调、资源估算、脚本示例。 | [huggingface/skills](https://github.com/huggingface/skills) |
| `hf-paper-publisher` | 论文与模型/数据仓库联动、paper 发布。 | [huggingface/skills](https://github.com/huggingface/skills) |

## 4. Anthropic 官方技能里最值得科研团队长期保留的

| Skill | 为什么值钱 | 链接 |
| --- | --- | --- |
| `pdf` | 文献、supplement、审稿意见、报告都离不开。 | [anthropics/skills](https://github.com/anthropics/skills) |
| `docx` | 写项目文档、基金草稿、合作版文件时很实用。 | [anthropics/skills](https://github.com/anthropics/skills) |
| `pptx` | 组会、答辩、投稿汇报、展示材料高频。 | [anthropics/skills](https://github.com/anthropics/skills) |
| `xlsx` | 表格、指标、实验结果整理很高频。 | [anthropics/skills](https://github.com/anthropics/skills) |
| `mcp-builder` | 搭 MCP 工具层时尤其重要。 | [anthropics/skills](https://github.com/anthropics/skills) |
| `skill-creator` | 适合把团队方法论沉淀成内部 skills。 | [anthropics/skills](https://github.com/anthropics/skills) |

## 5. Azure Skills 为什么对科研团队也值得关注

`microsoft/azure-skills` 不是纯学术技能包，但它有两个很现实的价值：

1. 它把 `skills + MCP + cloud workflow` 做成了一体化插件。
2. 对需要云 GPU、部署、资源检查、成本优化、AI 平台实验的团队特别有帮助。

公开说明里比较值得科研团队关注的 skills 包括：

- `azure-prepare`
- `azure-validate`
- `azure-deploy`
- `azure-diagnostics`
- `azure-observability`
- `azure-cost-optimization`
- `azure-ai`
- `microsoft-foundry`

链接：
[microsoft/azure-skills](https://github.com/microsoft/azure-skills)

## 6. 对实验执行和 benchmark 更直接有帮助的 Skill 入口

| 资源 | 类型 | 更适合的用途 | 链接 |
| --- | --- | --- | --- |
| `hf_model_evaluation` | HF Skill | 跑模型评测、汇总指标和结果。 | [huggingface/skills](https://github.com/huggingface/skills) |
| `hf-llm-trainer` | HF Skill | 搭建训练、微调和资源估算流程。 | [huggingface/skills](https://github.com/huggingface/skills) |
| `hf_dataset_creator` | HF Skill | 数据集草案、字段规划和 Hub 对接。 | [huggingface/skills](https://github.com/huggingface/skills) |
| `hf-cli` | HF Skill | 模型、数据和 artifact 管理。 | [Hugging Face Agents Skills](https://huggingface.co/docs/hub/agents-skills) |
| `mcp-builder` | Anthropic Skill | 把实验平台和脚本包装成 MCP。 | [anthropics/skills](https://github.com/anthropics/skills) |
| `xlsx` | Anthropic Skill | 把大量实验结果整理成表格。 | [anthropics/skills](https://github.com/anthropics/skills) |
| `test-driven-development` | 方法论 Skill | 适合先写测试再实现，减少实验代码边改边坏。 | [obra/superpowers](https://github.com/obra/superpowers) |
| `systematic-debugging` | 方法论 Skill | 适合先定位根因，再修改训练脚本、评测脚本和 pipeline。 | [obra/superpowers](https://github.com/obra/superpowers) |
| `verification-before-completion` | 方法论 Skill | 适合在“任务完成”前强制跑验证命令和回归检查。 | [obra/superpowers](https://github.com/obra/superpowers) |
| `dispatching-parallel-agents` | 方法论 Skill | 适合把数据准备、训练、评测、结果整理拆成并行子任务。 | [obra/superpowers](https://github.com/obra/superpowers) |
| skills.sh | Skill 发现平台 | 快速扫公开 skill 包和能力目录。 | [skills.sh](https://skills.sh/) |
| awesome-agent-skills | Skill 合集 | 继续补充公开 skill 生态和案例。 | [VoltAgent/awesome-agent-skills](https://github.com/VoltAgent/awesome-agent-skills) |

## 7. 面向 AI/ML / data mining 团队的安装顺序建议

1. `anthropics/skills`
2. `obra/superpowers`
3. `Orchestra-Research/AI-Research-SKILLs`
4. `openai/skills`
5. `huggingface/skills`
6. `skills` / `skillkit`
7. 再按具体框架栈追加专门 skills

## 8. 对科研场景更实用的一个判断标准

要优先保留那些能直接增强下面这些环节的 skills：

1. 环境与数据准备
2. 模型训练与推理
3. 评测与实验追踪
4. 结果整理与图表输出
5. 失败排查与复现实验

如果一个 skill 很酷，但对真实实验流水线没有稳定价值，就不必优先放进主链路。
