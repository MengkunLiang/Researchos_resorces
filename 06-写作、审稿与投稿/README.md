# 写作、审稿与投稿

这一模块聚焦初稿形成、证据式写作、同行评审式 critique、rebuttal 与 response、模板迁移、文稿工程和投稿末端。适合在“已有材料，准备成稿、返修或正式投稿”阶段使用。

## 这一步通常要回答的问题

1. 研究笔记、evidence cards、实验结果和图表怎样组织成可投稿文本。
2. 引用、claim 和证据链怎样保持一致，而不是只生成流畅段落。
3. rebuttal、response letter、cover letter 和 revision notes 怎样结构化整理。
4. 会议、期刊、preprint 与 software paper 需要遵循哪些官方模板和投稿系统。
5. 哪些 `Skills`、`MCP`、写作平台、模板工具和 preflight 检查值得优先接入。

## 推荐先看

- [学术写作、审稿与修订工具详表](./学术写作、审稿与修订工具详表.md)
- [模板、Rebuttal与投稿系统](./模板、Rebuttal与投稿系统.md)
- [94-Prompt与写作/学术写作与审稿](../94-Prompt与写作/学术写作与审稿.md)
- [97-模板与投稿/模板迁移与投稿](../97-模板与投稿/模板迁移与投稿.md)
- [98-全局索引/写作与投稿索引](../98-全局索引/写作与投稿索引.md)
- [91-Skills/科研写作与文献Skills](../91-Skills/科研写作与文献Skills.md)
- [92-MCP/写作协作与投稿MCP](../92-MCP/写作协作与投稿MCP.md)

## 一、相关 Skills

| 资源 | 类型 | 适合环节 | 简述 | 链接 |
| --- | --- | --- | --- | --- |
| 科研写作与文献Skills | 仓库内附录 | Skills 总览 | 当前仓库里写作、综述、审稿、基金、海报与投稿相关 Skills 的主归属页。 | [91-Skills/科研写作与文献Skills](../91-Skills/科研写作与文献Skills.md) |
| Claude Scientific Writer | 深研写作工具包 | research to paper | 覆盖 `research-lookup`、`peer-review`、`citation-management`、`venue-templates`、`research-grants` 等核心子技能。 | [K-Dense-AI/claude-scientific-writer](https://github.com/K-Dense-AI/claude-scientific-writer) |
| `academic-paper` | 学术论文写作 Skill | draft 与 revision | 适合把研究材料转换为结构化学术论文，并保留多轮修改。 | [Imbad0202/academic-research-skills](https://github.com/Imbad0202/academic-research-skills) |
| `academic-paper-reviewer` | 审稿 Skill | critique 与 review | 适合做 rubric 化、角色化、多视角审稿。 | [Imbad0202/academic-research-skills](https://github.com/Imbad0202/academic-research-skills) |
| `academic-pipeline` | 学术流程 Skill | write-review-revise | 适合把 research、write、integrity、review 和 revise 串成统一流程。 | [Imbad0202/academic-research-skills](https://github.com/Imbad0202/academic-research-skills) |
| `citation-management` | 引用管理 Skill | BibTeX 与 references | 适合管理 BibTeX、引用条目和参考文献一致性。 | [K-Dense-AI/claude-scientific-writer](https://github.com/K-Dense-AI/claude-scientific-writer) |
| `venue-templates` | venue 约束 Skill | 模板与格式要求 | 适合把不同 venue 的模板约束和写作规范纳入统一流程。 | [K-Dense-AI/claude-scientific-writer](https://github.com/K-Dense-AI/claude-scientific-writer) |
| `hf-paper-publisher` | HF Skill | 发布与联动 | 适合模型、数据集、论文和 Hub 资产同步发布。 | [huggingface/skills](https://github.com/huggingface/skills) |
| Anthropic 文档类 Skills | 官方文档 Skills | 文稿整理与交付 | `pdf`、`docx`、`pptx`、`xlsx`、`doc-coauthoring` 对论文、汇报和 response 文稿都很高频。 | [anthropics/skills](https://github.com/anthropics/skills) |

## 二、相关 MCP

| 资源 | 类型 | 适合环节 | 简述 | 链接 |
| --- | --- | --- | --- | --- |
| 写作协作与投稿MCP | 仓库内附录 | MCP 总览 | 当前仓库里 Overleaf、Zotero、OpenReview、LaTeX / Markdown 转换和投稿末端相关 MCP 的主归属页。 | [92-MCP/写作协作与投稿MCP](../92-MCP/写作协作与投稿MCP.md) |
| OverleafMCP | 协作写作 MCP | LaTeX 与 Overleaf | 适合把 Overleaf 项目接进 agent 工作流。 | [mjyoo2/OverleafMCP](https://github.com/mjyoo2/OverleafMCP) |
| Zotero MCP | 文献库 MCP | 引用与资料回查 | 适合从 Zotero 文库回查条目、笔记、PDF 和 BibTeX。 | [54yyyu/zotero-mcp](https://github.com/54yyyu/zotero-mcp) |
| OpenReview MCP | 投稿与评审 MCP | review 与 rebuttal | 适合追踪 OpenReview 投稿、评论、讨论和审稿脉络。 | [openreview/openreview-mcp](https://github.com/openreview/openreview-mcp) |
| GitHub MCP Server | 代码与文档 MCP | 仓库与配套材料 | 适合查看配套代码、补充材料、issue 和 release。 | [github/github-mcp-server](https://github.com/github/github-mcp-server) |
| GitMCP | 文档型 MCP | 公共模板与 guide | 适合快速抓取模板仓库、README、指南和样例。 | [idosal/git-mcp](https://github.com/idosal/git-mcp) |
| LaTeX MCP Server | 社区 MCP | LaTeX 工作流 | 适合围绕 LaTeX 工程做社区化实验接入。 | [Yeok-c/latex-mcp-server](https://github.com/Yeok-c/latex-mcp-server) |
| markdown2pdf-mcp | 转换 MCP | Markdown to PDF | 适合把 response、supplement 或草稿快速转成 PDF。 | [tigranbs/markdown2pdf-mcp](https://github.com/tigranbs/markdown2pdf-mcp) |

## 三、相关写作、审稿与修订工具

| 资源 | 类型 | 适合环节 | 简述 | 链接 |
| --- | --- | --- | --- | --- |
| 学术写作、审稿与修订工具详表 | 仓库内详表 | 工具总览 | 当前模块里 grounded writing、review、response 和 programmable authoring 的主归属页。 | [学术写作、审稿与修订工具详表](./学术写作、审稿与修订工具详表.md) |
| OpenDraft | 开源写作系统 | thesis / paper draft | 适合 thesis、long-form paper 和多格式导出。 | [federicodeponte/academic-thesis-ai](https://github.com/federicodeponte/academic-thesis-ai) |
| Open Research | 研究工作台 | critique 与 response | 自带 `paper explainer`、`methodology critic`、`reviewer response` 等研究向能力。 | [Open Research](https://www.open-research.info/) |
| ScholarCopilot | research writing assistant | citation-grounded draft | 更强调有引用依据的 academic writing。 | [TIGER-AI-Lab/ScholarCopilot](https://github.com/TIGER-AI-Lab/ScholarCopilot) |
| GPT Academic | 中文学术助手 | 翻译、写作与分析 | 对论文翻译、润色、项目分析和中文科研场景很实用。 | [binary-husky/gpt_academic](https://github.com/binary-husky/gpt_academic) |
| Paperpal | 学术写作平台 | 语言与投稿检查 | 覆盖 write、cite、language check、pre-submission checks 等能力。 | [Paperpal](https://www.web.paperpal.com/) |
| Jenni | 学术写作平台 | 写作与编辑协助 | 提供 write、cite、edit、research chat、autocomplete 等能力。 | [Jenni](https://jenni.ai/) |
| PaperQA2 | 证据问答工具 | claim 与 citation check | 适合对具体段落、claim 和结论回查证据。 | [Future-House/paper-qa](https://github.com/Future-House/paper-qa) |
| AI Peer Review | AI 辅助 review 工具 | critique 与 meta-review | 适合生成 reviewer concerns、meta-review 和对照式 critique。 | [poldrack/ai-peer-review](https://github.com/poldrack/ai-peer-review) |

## 四、模板、排版与投稿系统

| 资源 | 类型 | 适合环节 | 简述 | 链接 |
| --- | --- | --- | --- | --- |
| 模板、Rebuttal与投稿系统 | 仓库内详表 | 投稿总览 | 当前模块里模板、response、submission system 和 preflight 工具的主归属页。 | [模板、Rebuttal与投稿系统](./模板、Rebuttal与投稿系统.md) |
| 模板迁移与投稿 | 仓库内附录 | 类型附录 | 当前仓库里模板迁移、格式要求和投稿末端工具的附录入口。 | [97-模板与投稿/模板迁移与投稿](../97-模板与投稿/模板迁移与投稿.md) |
| Auto-Resubmit | 模板迁移工具 | resubmission | 适合在多个会议模板家族之间做迁移。 | [LilanOvO/Auto-Resubmit](https://github.com/LilanOvO/Auto-Resubmit) |
| Manubot / Manubot AI Editor | 开放出版与编辑 | collaborative writing | 适合 GitHub 驱动写作、引用自动化和 AI assisted editing。 | [manubot/manubot](https://github.com/manubot/manubot)、[manubot-ai-editor](https://github.com/manubot/manubot-ai-editor) |
| MyST / Curvenote / Stencila | programmable authoring | markdown to publication | 适合把可执行文档、模板和多格式发布结合起来。 | [mystmd/mystmd](https://github.com/mystmd/mystmd)、[curvenote/curvenote](https://github.com/curvenote/curvenote)、[stencila/stencila](https://github.com/stencila/stencila) |
| Quarto / Typst / Pandoc | 文稿工程工具 | 结构化写作与转换 | 适合多格式产出、轻量排版和格式转换。 | [Quarto](https://quarto.org/)、[Typst](https://github.com/typst/typst)、[Pandoc](https://pandoc.org/) |
| Tectonic / latexmk / arxiv-latex-cleaner | build 与 preflight | 编译与清理 | 适合构建、检查和提交前清理 LaTeX 包。 | [tectonic-typesetting/tectonic](https://github.com/tectonic-typesetting/tectonic)、[latexmk](https://ctan.org/pkg/latexmk)、[google-research/arxiv-latex-cleaner](https://github.com/google-research/arxiv-latex-cleaner) |

## 五、外部整合入口

| 资源 | 类型 | 更适合的用途 | 链接 |
| --- | --- | --- | --- |
| awesome-ai-research-writing | 写作与研究合集 | 扫学术写作、agent 与工具资源。 | [Leey21/awesome-ai-research-writing](https://github.com/Leey21/awesome-ai-research-writing) |
| arxiv-translator | 翻译与双语阅读工具 | 中英文论文阅读、翻译与分享。 | [Leey21/arxiv-translator](https://github.com/Leey21/arxiv-translator) |
| Overleaf Template Gallery | 官方模板入口 | 扫会议、期刊和出版社模板。 | [Overleaf Templates](https://www.overleaf.com/latex/templates) |
| MyST Templates | 模板生态 | 扫 MyST 下的期刊、preprint 和 PDF 模板。 | [myst-templates](https://github.com/myst-templates) |
| 外部导航与合集 | 仓库内索引 | 继续扫写作与投稿周边资源。 | [98-全局索引/外部导航与合集](../98-全局索引/外部导航与合集.md) |

## 六、推荐组合

1. `PaperQA2 + Zotero MCP + citation-management + OpenDraft / ScholarCopilot`
   适合 evidence-grounded draft。
2. `paper-glance-skill + peer-review + Open Research + OpenReview`
   适合 critique、rebuttal 与 revision。
3. `MyST / Quarto / Manubot + GitHub + Tectonic / latexmk`
   适合 programmable authoring 与可复现出版。
4. `Auto-Resubmit + official template + arxiv-latex-cleaner + venue-specific checker`
   适合 resubmission、camera-ready 和提交前检查。

## 七、仓库内延伸阅读

- [03-知识管理与证据沉淀](../03-知识管理与证据沉淀/README.md)
- [04-新颖性判断与综述](../04-新颖性判断与综述/README.md)
- [05-实验执行、复现与评测](../05-实验执行、复现与评测/README.md)
