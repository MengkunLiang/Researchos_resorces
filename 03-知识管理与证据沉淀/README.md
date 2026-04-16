# 知识管理与证据沉淀

这一模块聚焦文献库、Bib、证据卡片、项目笔记、引用资产与长期知识沉淀。重点不是“存文献”，而是把检索结果转成可复用、可追溯、可迁移的研究资产。

## 这一步通常要回答的问题

1. 文献条目、PDF、批注、摘录、卡片和项目笔记应该怎样分层保存。
2. 怎样把 DOI、BibTeX、网页来源、页码和实验记录保持可追溯。
3. 哪些工具更适合长期迁移，哪些更适合短期协作。
4. 怎样把文献资产与代码仓库、草稿、审稿回复和实验结果连接起来。

## 推荐先看

- [知识管理工具、MCP与知识载体详表](./知识管理工具、MCP与知识载体详表.md)
- [95-文献检索与知识管理/知识管理与引用](../95-文献检索与知识管理/知识管理与引用.md)
- [91-Skills/科研写作与文献Skills](../91-Skills/科研写作与文献Skills.md)
- [02-文献检索与单篇精读](../02-文献检索与单篇精读/README.md)
- [06-写作、审稿与投稿](../06-写作、审稿与投稿/README.md)

## 一、相关 Skills

| 资源 | 类型 | 适合环节 | 简述 | 链接 |
| --- | --- | --- | --- | --- |
| 科研写作与文献Skills | 仓库内附录 | Skills 总览 | 当前仓库里阅读、综述、写作与知识沉淀相关 Skills 的主归属页。 | [91-Skills/科研写作与文献Skills](../91-Skills/科研写作与文献Skills.md) |
| NotebookLM Skill | 知识库技能 | 项目级问答 | 适合在已有资料库基础上做 source-grounded 问答和复查。 | [PleasePrompto/notebooklm-skill](https://github.com/PleasePrompto/notebooklm-skill) |
| `citation-management` | 子技能 | 引用与证据管理 | 适合把 Bib、引用键和 references 一致性纳入长期资产管理。 | [K-Dense-AI/claude-scientific-writer](https://github.com/K-Dense-AI/claude-scientific-writer) |
| Claude Scientific Writer | 写作与深研技能库 | 引用与证据资产 | 其中 `citation-management`、`literature-review`、`research-lookup` 对长期知识沉淀很有帮助。 | [K-Dense-AI/claude-scientific-writer](https://github.com/K-Dense-AI/claude-scientific-writer) |
| `academic-pipeline` | 子技能 | 项目资产贯通 | 适合把检索、精读、写作、审稿和修订沉成统一项目资产链。 | [Imbad0202/academic-research-skills](https://github.com/Imbad0202/academic-research-skills) |
| Academic Research Skills | 学术流程技能库 | 项目资产贯通 | `academic-pipeline` 适合把检索、写作、评审和修订产物串成完整学术资产链。 | [Imbad0202/academic-research-skills](https://github.com/Imbad0202/academic-research-skills) |
| Anthropic Skills | 官方技能库 | 附件资料处理 | `pdf`、`docx`、`pptx`、`xlsx` 适合处理文档、附录和资料包。 | [anthropics/skills](https://github.com/anthropics/skills) |
| OpenAI Skills | 官方技能库 | 代码与文档协同 | 适合把代码、结果、文档和说明放在统一工作流里。 | [openai/skills](https://github.com/openai/skills) |

## 二、相关 MCP

| 资源 | 类型 | 适合环节 | 简述 | 链接 |
| --- | --- | --- | --- | --- |
| 文献检索与知识库MCP | 仓库内附录 | MCP 总览 | 当前仓库里文献库、知识库和资料接入类 MCP 的主归属页。 | [92-MCP/文献检索与知识库MCP](../92-MCP/文献检索与知识库MCP.md) |
| Zotero MCP | 文献库 MCP | 私有文库接入 | 适合读取条目、笔记、Bib 和附件，连接精读结果与文献库。 | [54yyyu/zotero-mcp](https://github.com/54yyyu/zotero-mcp) |
| Academic RAG MCP | 学术问答 MCP | 证据回查 | 适合围绕项目论文池做来源约束问答和多篇证据整合。 | [Jackela/mcp-academic-rag-server](https://github.com/Jackela/mcp-academic-rag-server) |
| Notion MCP Server | 笔记与任务 MCP | 协作知识页 | 适合研究计划、会议纪要、项目页与待办任务。 | [makenotion/notion-mcp-server](https://github.com/makenotion/notion-mcp-server) |
| GitHub MCP Server | 代码与项目 MCP | 代码文档关联 | 适合连接 Issue、PR、实验日志、release 和写作资产。 | [github/github-mcp-server](https://github.com/github/github-mcp-server) |
| Obsidian MCP Server | 本地知识库 MCP | 双链笔记 | 适合把本地 Markdown 知识库接入问答和自动整理流程。 | [MarkusPfundstein/obsidian-mcp-server](https://github.com/MarkusPfundstein/obsidian-mcp-server) |
| Zotero MCP Server（其他实现） | 文库接入 MCP | 多实现对比 | 适合比较本地 API、Python SDK 和 group library 支持差异。 | [masaki39/zotero-mcp](https://github.com/masaki39/zotero-mcp) |

## 三、相关工具与知识载体

| 资源 | 类型 | 适合环节 | 简述 | 链接 |
| --- | --- | --- | --- | --- |
| 知识管理与引用 | 仓库内附录 | 总览 | 当前仓库里文献管理、引用和知识库工具的主归属页。 | [95-文献检索与知识管理/知识管理与引用](../95-文献检索与知识管理/知识管理与引用.md) |
| Zotero | 文献管理器 | 文献底座 | 当前最常见的开源文献管理底座之一。 | [Zotero](https://www.zotero.org/) |
| Better BibTeX | Zotero 插件 | 稳定引用键 | 适合 BibTeX / BibLaTeX 写作链和可重复引用键管理。 | [retorquere/zotero-better-bibtex](https://github.com/retorquere/zotero-better-bibtex) |
| JabRef | Bib 管理器 | LaTeX 工作流 | 适合 BibTeX / BibLaTeX 优先的写作环境。 | [JabRef](https://www.jabref.org/) |
| Papis | CLI 文献管理 | 脚本化路线 | 适合终端优先、本地文件优先的工作流。 | [papis/papis](https://github.com/papis/papis) |
| Obsidian | Markdown 知识库 | 本地笔记 | 适合双链、插件式和长期研究笔记系统。 | [Obsidian](https://obsidian.md/) |
| Logseq | 开源知识库 | 双链与白板 | 适合做本地优先的知识卡片、白板和论文笔记。 | [logseq/logseq](https://github.com/logseq/logseq) |
| Joplin | 开源笔记系统 | 通用归档 | 适合做通用项目记录与多端同步。 | [Joplin](https://joplinapp.org/) |
| Zettlr | 写作工作台 | 长文写作 | 适合从笔记直接走向长文草稿和投稿稿件。 | [Zettlr](https://www.zettlr.com/) |
| Org-roam | Emacs 知识管理 | 深度定制 | 适合纯文本和 Zettelkasten 工作流。 | [org-roam/org-roam](https://github.com/org-roam/org-roam) |
| NotebookLM | 知识问答平台 | source-grounded QA | 适合对项目资料包和论文池进行来源约束问答。 | [NotebookLM](https://notebooklm.google.com/) |

## 四、相关工作流与集成工具

| 资源 | 类型 | 适合环节 | 简述 | 链接 |
| --- | --- | --- | --- | --- |
| 科研工作流设计模式 | 仓库内附录 | 流程设计 | 适合把 evidence card、project note、draft 和 repo 串成流程。 | [93-科研工作流与Agent/科研工作流设计模式](../93-科研工作流与Agent/科研工作流设计模式.md) |
| Better Notes for Zotero | Zotero 插件 | 笔记模板与导出 | 适合把文献条目与结构化卡片连接起来。 | [windingwind/zotero-better-notes](https://github.com/windingwind/zotero-better-notes) |
| Obsidian Zotero Integration | Obsidian 插件 | 引文与批注导入 | 适合把 Zotero 的批注和文献信息同步到 Obsidian。 | [mgmeyers/obsidian-zotero-integration](https://github.com/mgmeyers/obsidian-zotero-integration) |
| Manubot | 开源写作流水线 | 可追溯写作 | 适合把引用、版本和协作写作放在 Git 上管理。 | [manubot/manubot](https://github.com/manubot/manubot) |
| Fidus Writer | 协作写作平台 | 文稿协作 | 适合多人协作写作和评论。 | [fiduswriter/fiduswriter](https://github.com/fiduswriter/fiduswriter) |

## 五、推荐组合

1. `Zotero + Better BibTeX + Zotero MCP`
   适合作为文献条目、PDF、Bib 和引用键的稳定底座。
2. `Obsidian / Logseq + Better Notes + Obsidian Zotero Integration`
   适合把文献卡片、主题笔记和项目笔记串起来。
3. `GitHub MCP / Notion MCP / NotebookLM Skill`
   适合作为项目级知识沉淀、代码关联和问答层。
4. `Manubot / Zettlr / Quarto`
   适合作为面向公开稿件与长期维护的写作出口。

## 六、如果这一页的 Skills / MCP 还不够

- Skills 继续补：优先回看 [91-Skills/科研写作与文献Skills](../91-Skills/科研写作与文献Skills.md) 与 [91-Skills/Skill发现平台与精品合集](../91-Skills/Skill发现平台与精品合集.md)。
- MCP 继续补：优先回看 [92-MCP/文献检索与知识库MCP](../92-MCP/文献检索与知识库MCP.md) 与 [92-MCP/MCP标准与发现平台](../92-MCP/MCP标准与发现平台.md)。

## 七、仓库内延伸阅读

- [02-文献检索与单篇精读](../02-文献检索与单篇精读/README.md)
- [04-新颖性判断与综述](../04-新颖性判断与综述/README.md)
- [06-写作、审稿与投稿](../06-写作、审稿与投稿/README.md)
