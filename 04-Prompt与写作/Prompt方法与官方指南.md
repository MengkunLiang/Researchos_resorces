# Prompt 方法与官方指南

这一页聚焦 Prompt 方法论本身，包括官方 prompting 文档、Prompt 版本化、Prompt 评测与可复用 prompt 文件体系。相比“Prompt 库与教程”，这里更关注如何把 prompt 从一次性输入升级成可维护资产。

## 1. 官方 Prompt 方法指南

| 资源 | 类型 | 简述 | 链接 |
| --- | --- | --- | --- |
| Anthropic Prompt Engineering Overview | 官方 prompting 指南 | 系统整理清晰指令、few-shot、思维链、XML tags、角色设定、复杂 prompt chaining 等方法。 | [Anthropic Docs](https://docs.anthropic.com/en/docs/prompt-engineering) |
| OpenAI Prompting / Prompt Engineering | 官方 prompting 入口 | 提供 prompting 与 prompt engineering 概览，并强调固定模型版本与建立 evals。 | [OpenAI Docs](https://platform.openai.com/docs/guides/prompting) |
| Gemini Prompt Design Strategies | 官方 prompt 设计指南 | Google 官方的 prompt design 入门页，适合对比不同模型家族的 prompt 风格。 | [Google AI for Developers](https://ai.google.dev/guide/prompt_best_practices) |
| Azure OpenAI Prompt Engineering Techniques | 官方 techniques 文档 | 对 prompt construction 的基本概念、模式和注意事项做了系统梳理。 | [Microsoft Learn](https://learn.microsoft.com/en-us/azure/ai-foundry/openai/concepts/prompt-engineering?context=%2Fazure%2Fai-foundry%2Fcontext%2Fcontext) |
| Prompt Engineering Guide | 开放学习指南 | DAIR.AI 的大型公开指南，覆盖 techniques、applications、papers、tools 与 datasets。 | [dair-ai/Prompt-Engineering-Guide](https://github.com/dair-ai/Prompt-Engineering-Guide) |

## 2. Prompt 文件、共享与版本化

| 资源 | 类型 | 简述 | 链接 |
| --- | --- | --- | --- |
| GitHub Prompt Files | `.prompt.md` 文件 | 适合把任务型 prompts 做成可调用文件，支持输入变量和工作区上下文。 | [GitHub Docs](https://docs.github.com/en/copilot/tutorials/customization-library/prompt-files) |
| GitHub Models Prompt Configs | `.prompt.yml` 配置 | 适合保存 prompt、模型、参数和测试输入，便于版本化与复现。 | [GitHub Docs](https://docs.github.com/en/github-models/use-github-models/storing-prompts-in-github-repositories) |
| GitHub Customization Cheat Sheet | 定制化对照表 | 用一张表对比 custom instructions、prompt files、skills、agents 的定位与文件位置。 | [GitHub Docs](https://docs.github.com/en/copilot/reference/customization-cheat-sheet) |
| GitHub Copilot Response Customization | 自定义指南 | 适合理解 repository instructions、organization instructions 与 prompt files 的分层。 | [GitHub Docs](https://docs.github.com/en/copilot/concepts/prompting/response-customization) |
| Agent Skills | 从 prompt 走向 skill | 当 prompt 稳定到足以复用时，适合进一步升级为 `SKILL.md` 结构。 | [agentskills.io](https://agentskills.io/) |

## 3. Prompt 评测与回归测试

| 资源 | 类型 | 简述 | 链接 |
| --- | --- | --- | --- |
| promptfoo | Prompt 评测工具 | 支持对 prompts 和模型做测试、对比、自动评分与回归检查。 | [promptfoo/promptfoo](https://github.com/promptfoo/promptfoo) |
| GitHub Models | prompt 比较与评测 | 提供 prompt management、model comparison、evaluators 与 repository-native 协作。 | [GitHub Docs](https://docs.github.com/en/github-models/about-github-models) |
| Anthropic Eval 指南入口 | prompt 与 eval 联动 | Anthropic 文档在 prompting 之前就强调 success criteria 与 empirical evaluations。 | [Anthropic Docs](https://docs.anthropic.com/en/docs/prompt-engineering) |

## 4. 对科研 Prompt 最有价值的几个设计点

| 设计点 | 说明 |
| --- | --- |
| 任务边界显式化 | 先说明任务、输出对象、受众、禁区和证据要求，通常比“帮我写一篇”更稳。 |
| 输出结构化 | 对综述、审稿、结果解释、数据抽取等任务，优先要求表格、要点、schema 或 rubric。 |
| 引用与证据约束 | 对科研文本，prompt 最好明确要求来源、引文、原文片段或可回查标识。 |
| 分阶段生成 | `检索 -> 摘要 -> 提纲 -> 草稿 -> critique -> 修改` 通常优于一步到位。 |
| 失败样例回灌 | 把 hallucination、漏引、过度自信等失败案例纳入 prompt regression，效果通常最好。 |

## 5. Prompt 不该只停留在文本层

在科研场景里，较成熟的 prompt 往往会演化成下面几种资产：

1. `prompt file`：可调用、可传参、可版本化。
2. `rubric`：如 novelty 检查表、review checklist、systematic review screening criteria。
3. `artifact schema`：如 paper card、evidence card、experiment spec、review response table。
4. `skill`：把 prompt 与脚本、资源、模板、工具调用边界一起打包。

## 6. 相关页面

- [Prompt库与教程](./Prompt库与教程.md)
- [学术写作与审稿](./学术写作与审稿.md)
- [系统综述与证据综合](./系统综述与证据综合.md)
