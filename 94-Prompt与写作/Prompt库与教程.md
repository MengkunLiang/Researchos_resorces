# Prompt 库与教程

这一页聚焦“可直接复用或二次改写”的 Prompt 资源库、模板集合与教程入口。它更像公开素材层，适合先扫范式、再抽出适合团队沉淀的部分。

## 1. 直接面向科研与学术写作的 Prompt 资源

| 资源 | 类型 | 简述 | 链接 |
| --- | --- | --- | --- |
| awesome-ai-research-writing | Prompt / 资源合集 | 面向 AI 科研写作的公开资源库，覆盖写作、审稿、提纲、改写、文献综述等高频任务。 | [Leey21/awesome-ai-research-writing](https://github.com/Leey21/awesome-ai-research-writing) |
| CARefully prompt your AI | 写作 Prompt 库 | 用 `Collect / Articulate / Refine / Evaluate` 四阶段组织学术写作 Prompt，并强调伦理边界。 | [CARefully prompt your AI](https://olivethree.github.io/carefullyprompt/) |
| chatgpt-prompts-for-academic-writing | 学术写作 Prompt 集 | 覆盖 brainstorm、literature review、research plan、语言润色等任务。 | [LeSinus/chatgpt-prompts-for-academic-writing](https://github.com/LeSinus/chatgpt-prompts-for-academic-writing) |
| ChatGPT-Academic-Prompt | 学术 Prompt 汇总 | 中文社区较常见的学术 Prompt 汇总入口。 | [xuhangc/ChatGPT-Academic-Prompt](https://github.com/xuhangc/ChatGPT-Academic-Prompt) |
| academic_prompts | 中文 Prompt 集 | 小而直接，适合快速抽取中文科研任务 prompt 骨架。 | [Kiteflyingee/academic_prompts](https://github.com/Kiteflyingee/academic_prompts) |
| prompt-library | 学术 Prompt 检索库 | 覆盖 structured extraction、programming、research article indexing 等学术场景。 | [RISE-UNIBAS/prompt-library](https://github.com/RISE-UNIBAS/prompt-library) |
| HKUST-Got-Skills Resources | 课程化资源页 | 把 Skills、MCP、命令行工具、科研自动化材料放在一个入口里。 | [HKUST-Got-Skills Resources](https://giggleliu.github.io/HKUST-Got-Skills/resources) |
| GPT Academic | 中文学术助手平台 | 适合观察“Prompt + 插件 + 学术任务”的组合方式。 | [binary-husky/gpt_academic](https://github.com/binary-husky/gpt_academic) |

## 2. 适合持续扫新的 Prompt 与自定义资源入口

| 资源 | 类型 | 简述 | 链接 |
| --- | --- | --- | --- |
| Awesome GitHub Copilot | prompts / instructions / skills 目录 | 虽然面向 Copilot，但大量 prompt files 与 instructions 可迁移到科研场景。 | [github/awesome-copilot](https://github.com/github/awesome-copilot) |
| GitHub Prompt Files Docs | 可复用 prompt 文件 | 适合把团队内部高频 prompts 变成 `.github/prompts/*.prompt.md`。 | [GitHub Docs](https://docs.github.com/en/copilot/tutorials/customization-library/prompt-files) |
| GitHub Models Prompt Files | prompt 配置与版本化 | 适合把 prompt、模型参数、测试输入保存为 `.prompt.yml`。 | [GitHub Docs](https://docs.github.com/en/github-models/use-github-models/storing-prompts-in-github-repositories) |
| Prompt Engineering Guide | Prompt 学习与案例库 | DAIR.AI 的大型公开指南，覆盖 prompt 技术、工具、论文和应用案例。 | [dair-ai/Prompt-Engineering-Guide](https://github.com/dair-ai/Prompt-Engineering-Guide) |
| LangSmith Prompt Engineering | Prompt Hub 与管理 | 适合把 Prompt 放进版本、标签、测试集和共享流程。 | [LangSmith Docs](https://docs.langchain.com/langsmith/prompt-engineering) |

## 3. 这些 Prompt 资源更适合怎么用

| 用法 | 说明 |
| --- | --- |
| 当作工作流种子 | 更适合借 prompt 的任务拆解方式，而不是直接照抄最终句子。 |
| 当作 schema 灵感来源 | 高价值 Prompt 往往隐含了 output schema、rubric 或 checklist。 |
| 当作评测样例来源 | 适合整理出成功样例、失败样例和边界条件。 |
| 当作内部资产雏形 | 适合升级成 `prompt file / skill / workflow template / artifact schema`。 |

## 4. 按科研任务找 Prompt 素材时，优先看什么

| 任务 | 更适合先扫哪些入口 |
| --- | --- |
| 单篇精读、论文卡片 | `prompt-library`、`academic_prompts`、`HKUST-Got-Skills` |
| 综述、related work、evidence synthesis | `awesome-ai-research-writing`、`chatgpt-prompts-for-academic-writing`、`CARefully prompt your AI` |
| response、rebuttal、审稿 | `awesome-ai-research-writing`、`ChatGPT-Academic-Prompt` |
| 中文科研写作 | `academic_prompts`、`ChatGPT-Academic-Prompt`、`GPT Academic` |
| Prompt 文件与团队资产化 | `GitHub Prompt Files Docs`、`GitHub Models Prompt Files`、`LangSmith Prompt Engineering` |

## 5. 常见误区

1. 把一个超长 Prompt 当作完整科研系统。
2. 只存 Prompt 文本，不存输入结构、输出 schema、引用要求与失败案例。
3. 对引用、结论与 novelty 判断不加人工 gate。
4. 用“可直接投稿”的表述替代真实的写作、证据核对与审稿流程。

## 6. 一条比较稳的升级路线

1. 先用公开 Prompt 库建立任务拆解视角。
2. 再用 [Prompt方法与官方指南](./Prompt方法与官方指南.md) 补齐结构化设计和评测意识。
3. 把高频 Prompt 固化为 `prompt file / rubric / workflow template / artifact schema`。
4. 与 [学术写作与审稿](./学术写作与审稿.md) 或 [系统综述与证据综合](./系统综述与证据综合.md) 里的实际产出链路绑定。

## 7. 相关页面

- [Prompt方法与官方指南](./Prompt方法与官方指南.md)
- [学术写作与审稿](./学术写作与审稿.md)
- [系统综述与证据综合](./系统综述与证据综合.md)
- [98-全局索引/外部导航与合集](../98-全局索引/外部导航与合集.md)
