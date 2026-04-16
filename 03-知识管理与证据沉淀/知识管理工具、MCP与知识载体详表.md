# 知识管理工具、MCP 与知识载体详表

这一页把“知识沉淀”里最关键的部分拆成三层：`文献底座`、`知识库载体`、`项目级连接层`。适合在论文池已经建立之后，把资产沉成长期可复用结构。

## 一、文献底座层

| 资源 | 更适合的用法 | 核心价值 | 链接 |
| --- | --- | --- | --- |
| Zotero | 文献条目、附件和分组管理 | 最适合做公开资源里默认推荐的第一层文献底座。 | [Zotero](https://www.zotero.org/) |
| Better BibTeX | 稳定 citation key 和 Bib 导出 | 适合把文献管理和 LaTeX / Quarto / Pandoc 写作链打通。 | [retorquere/zotero-better-bibtex](https://github.com/retorquere/zotero-better-bibtex) |
| JabRef | BibTeX / BibLaTeX 工作流 | 适合 Bib 优先、终端或 LaTeX 较重的写作环境。 | [JabRef](https://www.jabref.org/) |
| Papis | CLI 文献管理 | 适合脚本化、本地文件优先的研究工作流。 | [papis/papis](https://github.com/papis/papis) |

## 二、知识库载体层

| 资源 | 更适合的用法 | 核心价值 | 链接 |
| --- | --- | --- | --- |
| Obsidian | 文献卡片、主题笔记、项目笔记 | 适合做本地优先、双链化的长期知识管理。 | [Obsidian](https://obsidian.md/) |
| Logseq | 卡片、白板、研究草图 | 适合做双链笔记和研究白板。 | [logseq/logseq](https://github.com/logseq/logseq) |
| Joplin | 通用资料归档 | 适合做多端同步和项目记录归档。 | [Joplin](https://joplinapp.org/) |
| Zettlr | 从笔记到稿件 | 适合将文献笔记直接衔接到长文写作。 | [Zettlr](https://www.zettlr.com/) |
| Org-roam | 纯文本 Zettelkasten | 适合高度定制和 Emacs 生态。 | [org-roam/org-roam](https://github.com/org-roam/org-roam) |
| NotebookLM | 来源约束问答 | 适合把资料包变成 source-grounded QA 入口。 | [NotebookLM](https://notebooklm.google.com/) |

## 三、MCP 与连接层

| 资源 | 更适合的用法 | 核心价值 | 链接 |
| --- | --- | --- | --- |
| Zotero MCP | 连接文献库 | 把文献条目、批注、Bib 和附件暴露给 Agent。 | [54yyyu/zotero-mcp](https://github.com/54yyyu/zotero-mcp) |
| Academic RAG MCP | 连接学术问答层 | 适合围绕多篇论文和资料包做来源约束问答。 | [Jackela/mcp-academic-rag-server](https://github.com/Jackela/mcp-academic-rag-server) |
| Notion MCP Server | 连接项目协作页 | 适合研究计划、待办、协作文档和会议纪要。 | [makenotion/notion-mcp-server](https://github.com/makenotion/notion-mcp-server) |
| GitHub MCP Server | 连接代码与 Issue | 适合把知识条目和代码、PR、实验记录关联起来。 | [github/github-mcp-server](https://github.com/github/github-mcp-server) |
| Obsidian MCP Server | 连接本地知识库 | 适合把 Markdown 知识库直接接入问答与整理流程。 | [MarkusPfundstein/obsidian-mcp-server](https://github.com/MarkusPfundstein/obsidian-mcp-server) |

## 四、常见资产分层

1. 原始资产层：PDF、附录、网页快照、DOI、BibTeX、截图和数据说明。
2. 结构化资产层：文献卡片、摘录、claim list、comparison table、主题标签。
3. 项目资产层：研究问题、假设、实验计划、复现记录、写作提纲、投稿版本。
4. 输出资产层：论文、补充材料、海报、slides、rebuttal、project page。

## 五、常见使用顺序

1. 先用 `Zotero + Better BibTeX` 管条目和 Bib。
2. 再用 `Better Notes / Obsidian Zotero Integration` 把文献卡片转入知识库。
3. 用 `Obsidian / Logseq / NotebookLM` 维持主题级与项目级资产。
4. 用 `GitHub MCP / Notion MCP / Obsidian MCP` 把知识层与代码、任务和资料层打通。
5. 最后把成熟资产输出到 [06-写作、审稿与投稿](../06-写作、审稿与投稿/README.md)。

## 六、继续补 Skills / MCP 时优先回查

- Skills：先回到 [../91-Skills/科研写作与文献Skills.md](../91-Skills/科研写作与文献Skills.md) 和 [../91-Skills/Skill发现平台与精品合集.md](../91-Skills/Skill发现平台与精品合集.md)。
- MCP：先回到 [../92-MCP/文献检索与知识库MCP.md](../92-MCP/文献检索与知识库MCP.md) 和 [../92-MCP/MCP标准与发现平台.md](../92-MCP/MCP标准与发现平台.md)。
