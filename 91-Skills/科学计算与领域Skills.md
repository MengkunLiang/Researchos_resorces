# 科学计算与领域 Skills

这一页专门补跨学科 scientific skills。对科研团队来说，这类 skills 的真正价值，不是“替代研究”，而是把高频数据库、Python 包、分析流程和领域最佳实践打包成可调用能力。

## 1. 最大的跨学科科学技能库

| 资源 | 类型 | 简述 | 链接 |
| --- | --- | --- | --- |
| Claude Scientific Skills | 大规模科学技能总库 | K-Dense 新一代科学技能库，公开说明显示已覆盖 120+ 到 128+ ready-to-use scientific skills，并支持 Claude Code、Cursor 和 MCP 客户端。 | [K-Dense-AI/claude-scientific-skills](https://github.com/K-Dense-AI/claude-scientific-skills) |
| Scientific Agent Skills | 科学技能总库 | 公开说明显示已覆盖 133 个 scientific / research skills，适合做实验室的科学底座库。 | [K-Dense-AI/scientific-agent-skills](https://github.com/K-Dense-AI/scientific-agent-skills) |
| Materials Simulation Skills | 材料模拟技能包 | 面向 computational materials science，适合 simulation / numerical stability / solver / validation。 | [HeshamFS/materials-simulation-skills](https://github.com/HeshamFS/materials-simulation-skills) |
| my_claude_skills | 小而专的领域技能集 | 包含 `extract_from_pdfs`、`phylo_from_buscos`、`biogeobears`、`think_deeply` 等。 | [brunoasm/my_claude_skills](https://github.com/brunoasm/my_claude_skills) |

## 2. Claude Scientific Skills 为什么值得优先补进来

这个仓库是我这轮补搜里最重要的遗漏之一。根据仓库公开说明，它把技能做得非常像“科研通用超集”：

| 覆盖层 | 公开说明 | 为什么重要 |
| --- | --- | --- |
| Scientific Databases | 26+ 数据库，如 OpenAlex、PubMed、ChEMBL、UniProt、ClinicalTrials.gov | 直接打通文献、知识库和领域数据库访问。 |
| Python Packages | 54+ 科学计算包，如 RDKit、Scanpy、PyTorch Lightning、scikit-learn、Qiskit | 对实验复现和 workflow 组装很实用。 |
| Scientific Integrations | 15+ 平台集成，如 Benchling、DNAnexus、OMERO、Protocols.io | 适合更真实的科研平台协同。 |
| Analysis & Communication | 20+ 分析和沟通 skills，如文献综述、scientific writing、peer review、document processing | 说明它不是纯计算库，而是完整科研工作流能力层。 |

这个仓库尤其适合同时关注 AI/ML / data mining 和更广 scientific computing 场景的团队。

## 3. Scientific Agent Skills 的覆盖面为什么很值得单独收录

根据仓库公开说明，它不只是“几个 prompt”，而是把多层能力一起做进去了：

| 覆盖层 | 公开说明 | 为什么重要 |
| --- | --- | --- |
| Scientific & Financial Databases | 100+ 数据源、统一数据库查询层 | 很适合科研团队做外部知识和公共数据库访问。 |
| Optimized Python Package Skills | 70+ Python 包的高质量用法与范式 | 能明显降低“我知道这个包存在，但不会高质量调用”的问题。 |
| Scientific Integration Skills | 多个科研平台 / 系统集成技能 | 适合搭跨工具科研流程。 |
| Analysis & Communication Tools | literature review、scientific writing、posters、slides、schematics 等 | 说明它不仅覆盖计算，也覆盖输出。 |
| Research & Clinical Tools | hypothesis generation、grant writing、clinical decision support 等 | 对更复杂的科研流程尤其有价值。 |

## 4. Scientific Agent Skills 里最值得重点关注的领域

| 领域 | 代表能力 | 链接 |
| --- | --- | --- |
| Bioinformatics & Genomics | 序列分析、single-cell、variant annotation、gene discovery、network analysis | [K-Dense-AI/scientific-agent-skills](https://github.com/K-Dense-AI/scientific-agent-skills) |
| Clinical Research & Precision Medicine | 临床试验、药物安全、精准治疗、变异解释 | [K-Dense-AI/scientific-agent-skills](https://github.com/K-Dense-AI/scientific-agent-skills) |
| Healthcare AI & Clinical ML | EHR、医疗影像、临床预测模型 | [K-Dense-AI/scientific-agent-skills](https://github.com/K-Dense-AI/scientific-agent-skills) |
| Machine Learning & AI | 深度学习、强化学习、时间序列、Bayesian methods | [K-Dense-AI/scientific-agent-skills](https://github.com/K-Dense-AI/scientific-agent-skills) |
| Materials Science & Chemistry | 晶体结构、相图、计算化学、材料分析 | [K-Dense-AI/scientific-agent-skills](https://github.com/K-Dense-AI/scientific-agent-skills) |
| Physics & Astronomy | 天文数据分析、坐标变换、物理计算、符号数学 | [K-Dense-AI/scientific-agent-skills](https://github.com/K-Dense-AI/scientific-agent-skills) |
| Engineering & Simulation | 离散事件模拟、多目标优化、系统建模、过程优化 | [K-Dense-AI/scientific-agent-skills](https://github.com/K-Dense-AI/scientific-agent-skills) |
| Data Analysis & Visualization | 统计分析、网络分析、时间序列、publication-quality figures | [K-Dense-AI/scientific-agent-skills](https://github.com/K-Dense-AI/scientific-agent-skills) |
| Geospatial Science & Remote Sensing | GIS、遥感、空间统计、地球观测 ML | [K-Dense-AI/scientific-agent-skills](https://github.com/K-Dense-AI/scientific-agent-skills) |
| Research Methodology | hypothesis generation、scientific brainstorming、grant writing、scholar evaluation | [K-Dense-AI/scientific-agent-skills](https://github.com/K-Dense-AI/scientific-agent-skills) |

## 5. 小而强的领域型 community skills

| 资源 / 子技能 | 场景 | 简述 | 链接 |
| --- | --- | --- | --- |
| `extract_from_pdfs` | 科学 PDF 结构化抽取 | 从 scientific PDF 到验证数据库的完整抽取管线，适合做资料数据库化。 | [brunoasm/my_claude_skills](https://github.com/brunoasm/my_claude_skills) |
| `phylo_from_buscos` | 系统发育分析 | 从 genome assemblies / BUSCO 单拷贝直系同源基因出发生成 phylogenomic workflow。 | [brunoasm/my_claude_skills](https://github.com/brunoasm/my_claude_skills) |
| `biogeobears` | 生物地理学分析 | 面向 BioGeoBEARS 的分析与可视化。 | [brunoasm/my_claude_skills](https://github.com/brunoasm/my_claude_skills) |
| `think_deeply` | 防止确认式回答 | 虽然不是学科技能，但对研究推理质量非常有帮助。 | [brunoasm/my_claude_skills](https://github.com/brunoasm/my_claude_skills) |
| Materials Simulation Skills | 计算材料与模拟 | 数值稳定性、时间步长、线性求解器、网格与后处理。 | [HeshamFS/materials-simulation-skills](https://github.com/HeshamFS/materials-simulation-skills) |

## 6. 面向不同研究方向的选择方式

### 如果主要做 AI / ML / data mining

优先：

1. `Claude Scientific Skills`
2. `Scientific Agent Skills` 中的 ML / data analysis / research methodology 部分
3. `AI Research SKILLs`
4. 写作与文献类 skills

### 如果做 computational design science / management + technology

优先：

1. `Claude Scientific Skills`
2. `Scientific Agent Skills` 中的数据分析、网络分析、时间序列、统计与研究方法部分
3. 写作与综述类 skills
4. 面向公开数据库的 skill bundles

### 如果做生物、医工、材料、地学

优先：

1. `Claude Scientific Skills`
2. `Scientific Agent Skills`
3. `my_claude_skills`
4. `materials-simulation-skills`

## 7. 更适合作为公开资源库的维护方式

对领域 skills，不建议只按“仓库名”收。更实用的是按下面三层持续补：

1. 数据库 skills
2. Python 包 / 计算框架 skills
3. 完整领域 workflow skills

这样以后无论是补生物、材料、地理还是社会计算，都能持续往下扩展。
