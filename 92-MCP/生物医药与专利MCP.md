# 生物医药与专利 MCP

这一页聚焦生命科学、医学研究、药物发现与专利情报相关的 MCP。对于 biomedical informatics、drug discovery、innovation analytics 这类方向，这一组资源的价值尤其明显。

## 1. 生物医学文献与临床研究

| 资源 | 场景 | 简述 | 链接 |
| --- | --- | --- | --- |
| PubMed MCP | 医学文献检索 | 适合基于 PubMed 做检索与文章抓取。 | [grll/pubmedmcp](https://github.com/grll/pubmedmcp) |
| PubMed MCP Server（Augmented Nature） | 生物医学深检索 | 提供更完整的 PubMed / PMC 工具集，适合高级检索、分析与研究辅助。 | [Augmented-Nature/PubMed-MCP-Server](https://github.com/Augmented-Nature/PubMed-MCP-Server) |
| PubMed MCP Server（cyanheads） | 生产型实现 | 强调 research workflow、分析与可视化能力，是另一条值得关注的实现线。 | [cyanheads/pubmed-mcp-server](https://github.com/cyanheads/pubmed-mcp-server) |
| ClinicalTrials MCP Server | 临床试验检索 | 适合检索试验、比较研究设计、做趋势与资格条件分析。 | [Augmented-Nature/ClinicalTrials-MCP-Server](https://github.com/Augmented-Nature/ClinicalTrials-MCP-Server) |

## 2. 靶点、组学与生物数据库

| 资源 | 场景 | 简述 | 链接 |
| --- | --- | --- | --- |
| Open Targets MCP Server | 靶点与疾病关联 | 适合基因、疾病、药物靶点、证据评分与优先级分析。 | [Augmented-Nature/OpenTargets-MCP-Server](https://github.com/Augmented-Nature/OpenTargets-MCP-Server) |
| GTEx MCP Server | 组织表达与 eQTL | 适合做组织表达、遗传调控与表达比较分析。 | [Augmented-Nature/GTEx-MCP-Server](https://github.com/Augmented-Nature/GTEx-MCP-Server) |
| PubChem MCP Server | 化学与生物活性 | 适合化合物检索、分子属性、结构相似性与 bioassay 信息读取。 | [Augmented-Nature/PubChem-MCP-Server](https://github.com/Augmented-Nature/PubChem-MCP-Server) |

## 3. 专利与技术情报

| 资源 | 场景 | 简述 | 链接 |
| --- | --- | --- | --- |
| USPTO Patent MCP Server | 专利检索与文本 | 连接 USPTO Patent Public Search API、ODP API 与 Google Patents Public Datasets，适合做专利检索、全文获取与技术情报分析。 | [riemannzeta/patent_mcp_server](https://github.com/riemannzeta/patent_mcp_server) |
| Patent MCP Server Config | 多数据源配置示例 | 面向 EPO、WIPO、USPTO 等多专利源的配置型整合项目，更适合作为参考样例。 | [myownipgit/mcp-server-patent](https://github.com/myownipgit/mcp-server-patent) |

配套公开数据源：

- [PatentsView](https://github.com/PatentsView)
- [USPTO](https://github.com/USPTO)

## 4. 适合科研与创新分析的组合方式

| 组合 | 适用链路 | 说明 |
| --- | --- | --- |
| `pubmed + clinicaltrials + open targets` | 转化医学与药物发现 | 适合把文献、试验与靶点证据串起来看。 |
| `pubchem + open targets + pubmed` | 化学与生物活性研究 | 适合从化合物走到靶点和文献证据。 |
| `patent-mcp + openalex/openreview` | 新颖性与技术情报 | 适合把学术文献与专利布局放在同一分析框架中。 |
| `gtex + pubmed + clinicaltrials` | 组学到临床 | 适合从表达模式走到疾病和试验线索。 |

## 5. 选择这类 MCP 时的注意点

1. 医学与临床类 MCP 优先选择基于官方公开 API 或官方数据库的数据源。
2. PubMed、ClinicalTrials、Open Targets 这类资源适合返回可验证标识符，如 PMID、NCT ID、Ensembl / target ID。
3. 专利类 MCP 需要特别关注 API 限流、检索语法与全文许可边界。
4. 对生物医学场景，最好把“文献层、临床层、靶点层、化学层”分开看，再通过 MCP 在工作流中串联。
