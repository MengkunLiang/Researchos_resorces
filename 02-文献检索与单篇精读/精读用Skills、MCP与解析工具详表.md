# 精读用 Skills、MCP 与解析工具详表

这一页把“检索到精读”的常用能力拆成三层：`Skills`、`MCP`、`解析与问答工具`。适合在已经形成候选论文池之后，继续做单篇深读和证据加工。

## 一、优先级最高的 Skills

| 资源 | 更适合的用法 | 为什么对精读有效 | 链接 |
| --- | --- | --- | --- |
| paper-glance-skill | 单篇论文结构化拆解 | 适合把论文拆成 contribution、method、experiment、weakness 与延伸点。 | [CatVinci-Studio/paper-glance-skill](https://github.com/CatVinci-Studio/paper-glance-skill) |
| Claude Scientific Writer | `research-lookup`、`literature-review`、`scientific-critical-thinking` | 适合在精读时补背景文献、写 reading note 和做批判阅读。 | [K-Dense-AI/claude-scientific-writer](https://github.com/K-Dense-AI/claude-scientific-writer) |
| Academic Research Skills | `deep-research`、`academic-paper-reviewer` | 更适合把单篇论文放回 broader literature context 中重新判断价值。 | [Imbad0202/academic-research-skills](https://github.com/Imbad0202/academic-research-skills) |
| Anthropic Skills | `pdf`、`docx`、`xlsx` | 适合处理论文正文、附录、实验表和补充材料。 | [anthropics/skills](https://github.com/anthropics/skills) |
| Claude Skills 中文镜像 | `pdf`、`research`、`documentation` 学习入口 | 适合中文环境下快速理解和迁移常用 skill 模式。 | [LeastBit/Claude_skills_zh-CN](https://github.com/LeastBit/Claude_skills_zh-CN) |
| NotebookLM Skill | 项目资料库问答 | 适合把精读对象与内部笔记、课程包、项目说明一起查。 | [PleasePrompto/notebooklm-skill](https://github.com/PleasePrompto/notebooklm-skill) |

## 二、优先级最高的 MCP

| 资源 | 适合阶段 | 核心价值 | 链接 |
| --- | --- | --- | --- |
| Paper Search MCP | 追加检索 | 适合在单篇论文精读时继续补相关工作。 | [openags/paper-search-mcp](https://github.com/openags/paper-search-mcp) |
| OpenAlex MCP | 论文家族扩展 | 适合沿作者、主题、引文链扩展相关论文。 | [hbiaou/openalex-mcp](https://github.com/hbiaou/openalex-mcp) |
| Semantic Scholar MCP | 作者与引文网络 | 适合把单篇论文放入 citation network 中观察影响路径。 | [zongmin-yu/semantic-scholar-fastmcp-mcp-server](https://github.com/zongmin-yu/semantic-scholar-fastmcp-mcp-server) |
| Hugging Face MCP Server | 模型与数据卡回查 | 适合核对论文配套模型、数据集和 demo。 | [huggingface/hf-mcp-server](https://github.com/huggingface/hf-mcp-server) |
| Academic RAG MCP | 多文档学术问答 | 适合对小型论文池做来源约束问答和证据整合。 | [Jackela/mcp-academic-rag-server](https://github.com/Jackela/mcp-academic-rag-server) |
| arXiv LaTeX MCP | 公式和附录精读 | 对公式、表格、伪代码、算法框架精读特别有帮助。 | [takashiishida/arxiv-latex-mcp](https://github.com/takashiishida/arxiv-latex-mcp) |
| Zotero MCP | 精读资产沉淀 | 适合把阅读结果直接回存到个人文献库。 | [54yyyu/zotero-mcp](https://github.com/54yyyu/zotero-mcp) |
| Crossref MCP | 元数据核验 | 适合 DOI、出版状态和正式引用信息核验。 | [botanicastudios/crossref-mcp](https://github.com/botanicastudios/crossref-mcp) |

## 三、优先级最高的解析与问答工具

| 资源 | 更适合的用法 | 核心价值 | 链接 |
| --- | --- | --- | --- |
| PaperQA2 | 论文问答与证据抽取 | 适合 claim 级问答和来源追溯。 | [PaperQA2](https://github.com/Future-House/paper-qa) |
| GROBID | 学术 PDF 结构化解析 | 适合 section、citation、参考文献与版面结构抽取。 | [kermitt2/grobid](https://github.com/kermitt2/grobid) |
| Marker | PDF 转 Markdown | 适合快速转成 LLM 友好的文本。 | [VikParuchuri/marker](https://github.com/VikParuchuri/marker) |
| Docling | 多格式解析 | 适合把 PDF、Word、PPT、扫描件放到同一解析框架。 | [docling-project/docling](https://github.com/docling-project/docling) |
| MinerU | 复杂科研 PDF 解析 | 对复杂版式、公式和表格处理能力较强。 | [opendatalab/MinerU](https://github.com/opendatalab/MinerU) |
| Nougat | 学术 OCR | 适合扫描稿、数学公式和复杂版面文档。 | [facebookresearch/nougat](https://github.com/facebookresearch/nougat) |

## 四、常见使用顺序

1. 先用 `Paper Search MCP / OpenAlex MCP / Semantic Scholar MCP` 扩展论文家族。
2. 对目标论文使用 `GROBID / Marker / Docling / MinerU` 取结构化内容。
3. 结合 `paper-glance-skill / PaperQA2 / research-lookup` 生成精读卡片。
4. 用 `Zotero MCP / NotebookLM Skill` 把精读结果纳入长期资产层。
5. 再进入 [03-知识管理与证据沉淀](../03-知识管理与证据沉淀/README.md) 或 [04-新颖性判断与综述](../04-新颖性判断与综述/README.md)。

## 五、继续补 Skills / MCP 时优先回查

- Skills：先回到 [../91-Skills/科研写作与文献Skills.md](../91-Skills/科研写作与文献Skills.md) 和 [../91-Skills/Skill发现平台与精品合集.md](../91-Skills/Skill发现平台与精品合集.md)。
- MCP：先回到 [../92-MCP/MCP标准与发现平台.md](../92-MCP/MCP标准与发现平台.md) 和 [../92-MCP/文献检索与知识库MCP.md](../92-MCP/文献检索与知识库MCP.md)。
