# Prompt 方法与官方指南

这一页不收“现成句子”，而是收 Prompt 方法论本身。目标是把科研 Prompt 从一次性输入升级成可维护资产。

## 1. 官方方法、结构化输出与评测入口

| 资源 | 类型 | 简述 | 链接 |
| --- | --- | --- | --- |
| Anthropic Prompt Engineering Overview | 官方 prompting 指南 | 系统讲清晰指令、few-shot、XML tags、prompt chaining 与任务拆解。 | [Anthropic Docs](https://docs.anthropic.com/en/docs/prompt-engineering) |
| Anthropic XML Tags Guide | 结构化提示 | 对多段上下文、指令、样例和输出段落分区很有帮助。 | [Anthropic Docs](https://docs.anthropic.com/en/docs/build-with-claude/prompt-engineering/use-xml-tags) |
| Anthropic Eval Design | 评测设计指南 | 强调 success criteria、测试集设计和 empirical evals。 | [Anthropic Docs](https://docs.anthropic.com/en/docs/build-with-claude/develop-tests) |
| Anthropic Evaluation Tool | Console 评测工具 | 适合给 Prompt 做变量化测试、对比和版本迭代。 | [Anthropic Docs](https://docs.anthropic.com/en/docs/test-and-evaluate/eval-tool) |
| OpenAI Prompting Guide | 官方 prompting 指南 | 适合和 eval、结构化输出、系统消息设计一起看。 | [OpenAI Docs](https://platform.openai.com/docs/guides/prompting) |
| OpenAI Structured Outputs | 结构化输出 | 适合把 extraction、paper card、review table 做成稳定 JSON schema。 | [OpenAI Docs](https://platform.openai.com/docs/guides/structured-outputs?lang=javascript) |
| GitHub Prompt Files | `.prompt.md` 文件 | 适合把任务型 Prompt 做成仓库内可调用文件。 | [GitHub Docs](https://docs.github.com/en/copilot/tutorials/customization-library/prompt-files) |
| GitHub Models Prompt Configs | `.prompt.yml` 配置 | 适合保存 prompt、模型参数、样例输入和测试配置。 | [GitHub Docs](https://docs.github.com/en/github-models/use-github-models/storing-prompts-in-github-repositories) |
| GitHub Customization Cheat Sheet | 定制化对照表 | 适合理解 instructions、prompt files、skills、agents 的边界。 | [GitHub Docs](https://docs.github.com/en/copilot/reference/customization-cheat-sheet) |
| promptfoo | Prompt 回归工具 | 适合固定样例集、自动评分和 prompt 版本对比。 | [promptfoo/promptfoo](https://github.com/promptfoo/promptfoo) |
| LangSmith Prompt Engineering | Prompt 管理与版本化 | 适合做 prompt 提交、标签、测试集、版本比对和 GitHub 同步。 | [LangSmith Docs](https://docs.langchain.com/langsmith/prompt-engineering) |
| Agent Skills | 从 Prompt 升级到 Skill | 当任务边界、输入输出和资源引用稳定后，适合升级为 `SKILL.md`。 | [agentskills.io](https://agentskills.io/) |

## 2. 科研 Prompt 最值得固定的五个槽位

| 槽位 | 应该写什么 |
| --- | --- |
| 任务边界 | 负责什么，不负责什么；哪些内容必须停下来交人工判断。 |
| 输入结构 | 论文、表格、日志、Bib、review comments、章节草稿分别如何传入。 |
| 输出结构 | 提纲、rubric、JSON schema、evidence card、response table、draft skeleton。 |
| 证据要求 | 是否必须引用原文、页码、DOI、表格编号、日志片段或实验 ID。 |
| 失败模式 | hallucination、漏引、编造 SOTA、把 reviewer 意见误判成事实等。 |

## 3. 一个可直接迁移的科研 Prompt 最小模板

```text
任务：
你要完成的是 {task_name}，目标产物是 {artifact_name}。

输入：
- 文献材料：{papers_or_notes}
- 结构化数据：{tables_or_logs}
- 约束：{venue_or_style_constraints}

必须遵守：
1. 只根据已给材料判断，不补造事实。
2. 所有结论都要标注来源或证据状态。
3. 信息不足时显式写“未知 / 待核验 / 仅基于摘要”。

输出格式：
- 部分 A：{section_a}
- 部分 B：{section_b}
- 部分 C：{section_c}

质量检查：
- 是否遗漏关键证据？
- 是否把推测写成事实？
- 是否给出了可继续人工检查的结构？
```

## 4. 按科研任务写 Prompt 时最常见的结构

| 任务 | 更稳的 Prompt 结构 |
| --- | --- |
| 单篇精读 | `输入覆盖范围 -> 论文卡 schema -> 优势/局限/复现难点 -> 是否值得继续读` |
| 多篇综述 | `主题边界 -> 对比维度 -> 分类法 -> 代表路线 -> 开放问题 -> 待读清单` |
| novelty / reviewer 预演 | `候选 claim -> 相关工作池 -> concern taxonomy -> 支持与反证 -> 风险判断` |
| rebuttal / response | `reviewer concern 分组 -> 补实验/澄清分类 -> response tone -> 风险表述提醒` |
| benchmark 抽取 | `paper list -> extraction schema -> unknown policy -> table-ready output` |
| 实验总结 | `run ids / logs / metrics -> best run -> failure modes -> next-step hypotheses` |

## 5. Prompt 不该只停留在文本层

在科研场景里，成熟 Prompt 往往会继续演化成下面几种资产：

1. `prompt file`
   适合稳定复用、参数化调用和仓库化管理。
2. `rubric`
   适合 novelty check、review checklist、screening criteria、response quality gate。
3. `artifact schema`
   适合 paper card、evidence card、benchmark row、review table、revision roadmap。
4. `eval set`
   适合把失败案例、边界条件和固定样例做成回归测试。
5. `skill`
   当 Prompt 已经明确依赖模板、脚本、引用文件和工具边界时，适合升级成 `SKILL.md`。

## 6. 一个比较稳的 Prompt 版本化与回归流程

1. 先把任务拆成最小 artifact。
2. 给 artifact 定 schema，而不是先追求漂亮措辞。
3. 把成功样例和失败样例都收进固定测试集。
4. 用 `promptfoo / LangSmith / Anthropic Eval Tool / GitHub prompt configs` 做对比。
5. 当 prompt 已经稳定到“任务边界 + 输入输出 + 失败模式”都清楚时，再升级成 `prompt file / skill`。

## 7. 对科研 Prompt 最有价值的判断标准

1. 能不能稳定地产出可复查结构，而不是只产出顺滑段落。
2. 能不能在信息不足时明确暴露缺口，而不是硬补。
3. 能不能和 `paper card / evidence card / benchmark table / review response table` 这些 artifact 接起来。
4. 能不能被固定样例集持续回归测试。

## 8. 相关页面

- [Prompt库与教程](./Prompt库与教程.md)
- [学术写作与审稿](./学术写作与审稿.md)
- [系统综述与证据综合](./系统综述与证据综合.md)
- [91-Skills/科研写作与文献Skills](../91-Skills/科研写作与文献Skills.md)
- [98-全局索引/写作与投稿索引](../98-全局索引/写作与投稿索引.md)
