# Prompt 与写作（类型附录）

这一组页面不只是收 Prompt 资源，而是回答三个更实际的问题：

1. 科研 Prompt 应该怎样写，才能和证据、表格、日志、引用、模板配合起来。
2. 什么情况下该停留在 `prompt`，什么情况下该升级成 `prompt file / rubric / schema / skill / workflow template`。
3. 怎样把写作、综述、rebuttal、报告生成和 programmable authoring 接回 `01-09` 主任务线。

## 什么时候进入这一组页

- 需要给综述、审稿、结果解释、数据抽取、rebuttal 写一套稳定 Prompt。
- 需要把高频 prompt 从聊天记录里抽出来，做成可复用文件、模板或评测集。
- 需要把写作工具、Prompt 方法、模板系统和投稿链路连成闭环。
- 已经在 [06-写作、审稿与投稿](../06-写作、审稿与投稿/README.md) 或 [09-按科研任务导航/写作、审稿与投稿](../09-按科研任务导航/写作、审稿与投稿.md) 工作，但还想补强 Prompt / prompt file / 文稿工程层。

## 推荐先看

- [Prompt方法与官方指南](./Prompt方法与官方指南.md)
- [学术写作与审稿](./学术写作与审稿.md)
- [系统综述与证据综合](./系统综述与证据综合.md)
- [Prompt库与教程](./Prompt库与教程.md)

## 按任务回查

| 当前任务 | 更适合先看 | 再回查哪些页 |
| --- | --- | --- |
| 设计结构化 Prompt、prompt file、回归测试 | [Prompt方法与官方指南](./Prompt方法与官方指南.md) | [91-Skills/README](../91-Skills/README.md)、[98-全局索引/Skills索引](../98-全局索引/Skills索引.md) |
| 学术写作、response、rebuttal、修订 | [学术写作与审稿](./学术写作与审稿.md) | [06-写作、审稿与投稿](../06-写作、审稿与投稿/README.md)、[97-模板与投稿/README](../97-模板与投稿/README.md) |
| literature review、systematic review、evidence synthesis | [系统综述与证据综合](./系统综述与证据综合.md) | [04-新颖性判断与综述](../04-新颖性判断与综述/README.md)、[95-文献检索与知识管理/README](../95-文献检索与知识管理/README.md) |
| 扫写作 Prompt、教程与公开范例 | [Prompt库与教程](./Prompt库与教程.md) | [98-全局索引/外部导航与合集](../98-全局索引/外部导航与合集.md) |
| 从任务跳到专题，再跳回 Prompt/写作页 | [98-全局索引/任务专题对照索引](../98-全局索引/任务专题对照索引.md) | [98-全局索引/方向专题索引](../98-全局索引/方向专题索引.md) |

## 一组最小闭环

| 环节 | 最小组合 |
| --- | --- |
| Prompt 设计 | `官方 prompting 指南 + structured output / schema + promptfoo / eval tool` |
| 证据综合 | `OpenAlex / Paper Search / PaperQA2 + extraction schema + review template` |
| 学术写作 | `citation-grounded drafting + response / rebuttal rubric + venue template` |
| 文稿工程 | `MyST / Quarto / Jupyter Book / Manubot + PDF/Word/LaTeX 导出` |
| 任务导航 | `09-按科研任务导航 + 98-任务专题对照索引 + 98-方向专题索引` |

## 高频公开资源

| 资源 | 类型 | 简述 | 链接 |
| --- | --- | --- | --- |
| OpenAI Prompting Guide | 官方方法指南 | 适合补 Prompt 设计、结构化输出与评测意识。 | [OpenAI Docs](https://platform.openai.com/docs/guides/prompting) |
| Anthropic Prompt Engineering | 官方方法指南 | 对 XML tags、few-shot、任务拆解和 test/eval 链路讲得很系统。 | [Anthropic Docs](https://docs.anthropic.com/en/docs/prompt-engineering) |
| GitHub Prompt Files | prompt file 体系 | 适合把高频 Prompt 变成 `.prompt.md` 与 `.prompt.yml` 资产。 | [GitHub Docs](https://docs.github.com/en/copilot/tutorials/customization-library/prompt-files) |
| promptfoo | Prompt 回归测试 | 适合给科研 Prompt 做固定样例、自动评分和对比。 | [promptfoo/promptfoo](https://github.com/promptfoo/promptfoo) |
| LangSmith Prompt Engineering | prompt 管理与评测 | 适合把 Prompt 做成可版本化、可回放、可比对资产。 | [LangSmith Docs](https://docs.langchain.com/langsmith/prompt-engineering) |
| MyST Markdown | 科学写作与出版 | 适合 Markdown、引用、交叉引用、Word/PDF/LaTeX 导出。 | [MyST](https://mystmd.org/) |
| Quarto | 科学与技术出版系统 | 适合文章、报告、网站、幻灯与 books 的统一产出。 | [Quarto](https://quarto.org/index.html) |
| Jupyter Book | 计算叙事与知识库 | 适合把 notebook、Markdown 和可复现实验叙事组织成书或知识库。 | [Jupyter Book](https://jupyterbook.org/docs) |
| PRISMA 2020 | 系统综述报告规范 | 适合 systematic review 的 checklist、flow diagram 与报告约束。 | [PRISMA Statement](https://www.prisma-statement.org/prisma-2020) |
| Cochrane Handbook | 系统综述方法标准 | 适合 system review 的搜索、筛选、抽取、偏倚与 synthesis 方法。 | [Cochrane Handbook](https://www.cochrane.org/authors/handbooks-and-manuals/handbook/current) |

## 推荐配合使用的页面

- [06-写作、审稿与投稿](../06-写作、审稿与投稿/README.md)
- [09-按科研任务导航/写作、审稿与投稿](../09-按科研任务导航/写作、审稿与投稿.md)
- [91-Skills/科研写作与文献Skills](../91-Skills/科研写作与文献Skills.md)
- [92-MCP/写作协作与投稿MCP](../92-MCP/写作协作与投稿MCP.md)
- [97-模板与投稿/模板迁移与投稿](../97-模板与投稿/模板迁移与投稿.md)
- [98-全局索引/写作与投稿索引](../98-全局索引/写作与投稿索引.md)
- [98-全局索引/任务专题对照索引](../98-全局索引/任务专题对照索引.md)
- [98-全局索引/方向专题索引](../98-全局索引/方向专题索引.md)
