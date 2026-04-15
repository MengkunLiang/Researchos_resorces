# PDF解析与阅读加工

这一页聚焦学术 PDF、扫描文档、公式与表格解析，以及阅读辅助和文献问答相关公开资源。

## 1. 学术文档结构化解析

| 资源 | 类型 | 简述 | 链接 |
| --- | --- | --- | --- |
| GROBID | 学术 PDF 结构化解析 | 将论文 PDF 转成结构化 TEI/XML，是 citation / section 解析的经典底座。 | [kermitt2/grobid](https://github.com/kermitt2/grobid) |
| Marker | PDF 转 Markdown | 适合把论文、技术文档与教材转成 LLM 友好的 Markdown。 | [VikParuchuri/marker](https://github.com/VikParuchuri/marker) |
| Docling | 通用文档解析 | 统一处理 PDF、Office、扫描文档与多种复杂版式。 | [docling-project/docling](https://github.com/docling-project/docling) |
| MinerU | 文档解析引擎 | 对复杂科研 PDF 的公式、表格、版面还原较强，支持 Markdown / JSON。 | [opendatalab/MinerU](https://github.com/opendatalab/MinerU) |
| Nougat | 学术文档 OCR | 面向学术文档与数学公式的 OCR / Markdown 转换模型。 | [facebookresearch/nougat](https://github.com/facebookresearch/nougat) |
| Unstructured | 文档 ETL | 面向多格式文档切分、清洗与结构化抽取的开源底座。 | [Unstructured-IO/unstructured](https://github.com/Unstructured-IO/unstructured) |
| PyMuPDF4LLM | PDF 结构提取 | 适合做本地、快速、程序化的 PDF 结构与文本抽取。 | [PyMuPDF4LLM](https://pymupdf.io/) |

## 2. 阅读辅助与文献问答

| 资源 | 类型 | 简述 | 链接 |
| --- | --- | --- | --- |
| PaperQA2 | 文献问答 | 面向 scientific literature 的高精度问答与证据检索框架。 | [Future-House/paper-qa](https://github.com/Future-House/paper-qa) |
| RTI | 文献研究工作流 | 面向“找方向 -> 找论文 -> 做分析”的研究型工作流。 | [yrc-better/RTI](https://github.com/yrc-better/RTI) |
| arxiv-translator | 中文翻译 | 从 arXiv LaTeX 源码生成中文版本，适合长文精读与教学复用。 | [Leey21/arxiv-translator](https://github.com/Leey21/arxiv-translator) |
| paper-glance-skill | 深读加工 | 对单篇论文生成分析、导图、审稿意见与结构化摘要。 | [CatVinci-Studio/paper-glance-skill](https://github.com/CatVinci-Studio/paper-glance-skill) |

## 3. 选型参考

| 需求 | 更适合先看什么 |
| --- | --- |
| 高质量学术结构化解析 | `GROBID + Docling + Marker` |
| 复杂公式、表格与中文文档 | `MinerU + Nougat` |
| 多格式通用预处理 | `Unstructured + PyMuPDF4LLM` |
| 单篇论文问答与证据抽取 | `PaperQA2` |
| 从 PDF 走向笔记或导图 | `paper-glance-skill + Better Notes / Obsidian / Logseq` |

## 4. 使用提示

- 解析结果适合做索引、粗筛、问答与对比，但公式、图表与附录仍可能需要人工复核。
- 学术 PDF 常见多栏排版、脚注、参考文献回流与表格跨页问题，工具间交叉验证通常更稳。
- 若结果要进入知识库、综述或 novelty 分析，宜保留原文页码、图表编号与出处链接。
