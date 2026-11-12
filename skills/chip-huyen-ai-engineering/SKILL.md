---
name: chip-huyen-ai-engineering
description: "基于 Chip Huyen《AI Engineering》的逐章学习与应用技能。用于基础模型应用的用例选择、模型与评估、提示、RAG、Agent、微调、数据集、推理优化、架构与用户反馈；可做章节讲解、自测和项目诊断。回答前读取相关章节并区分书中事实、作者判断与应用推演。"
---

# AI Engineering: Building Applications with Foundation Models

作者：Chip Huyen。基于用户提供的本地 OCR 文本，共 10 章。OCR 可见全文已逐段核读；图像、损坏公式与代码不视为已核实。适合逐章学习、概念自测与项目诊断。

## 调用规则

1. 任何具体问题先读对应章节；跨主题读最相关的 2–3 章，并查看术语表或方法库。章节导航在下方。
2. 逐章学习采用“解释一个判断→重构一个例子→提问检查理解→给一个练习”的节奏；等待用户作答再给反馈。
3. 原句、数值、故事细节、代码或争议观点必须用[原文读取工具](scripts/read_source.py)按章节行号核对。工具需要本机匹配的原始 OCR；若系统的 python 命令不可用，可用已安装的 Python 解释器运行。无法访问原文时明确说明不能核验。
4. 区分作者观点、书中引用/案例、本技能推演、今天的事实。OCR图像未读取，不能声称已核对图表或印刷页码。
5. 面对现实项目，以用户目标和现有证据开始；信息不足时标注假设，提出一个可验证的下一步。

## 核心框架

- **评价先行**：定义任务、评估集和业务门槛；单一排行榜分数不足以指导上线。[第1章](chapters/ch01.md)、[第3章](chapters/ch03.md)、[第4章](chapters/ch04.md)
- **适配路径**：按失败原因比较提示、检索、工具和微调，逐层验证收益。[第5章](chapters/ch05.md)、[第6章](chapters/ch06.md)、[第7章](chapters/ch07.md)
- **数据三角**：质量、覆盖、数量同时决定训练价值，合成样本要验证。[第8章](chapters/ch08.md)
- **推理经济性**：分解 TTFT、TPOT、goodput 和单位任务成本，按瓶颈优化。[第9章](chapters/ch09.md)
- **产品反馈循环**：从最小架构出发，建立护栏、可观测性与经授权的反馈回流。[第10章](chapters/ch10.md)

## 章节导航

|章|主题|关键判断|
|---|---|---|
|[01](chapters/ch01.md)|Introduction to Building AI Applications with Foundation Models|先判断基础模型应用是否值得做，再选任务、模型和开发路径。|
|[02](chapters/ch02.md)|Understanding Foundation Models|理解模型能力与训练方式，才能做合理的模型选择。|
|[03](chapters/ch03.md)|Evaluation Methodology|评估设计必须先定义目标任务、数据集和人工判断口径。|
|[04](chapters/ch04.md)|Evaluate AI Systems|系统评价要覆盖任务成功、生成质量、安全、延迟和成本。|
|[05](chapters/ch05.md)|Prompt Engineering|提示工程通过明确任务、上下文、例子和输出结构控制行为。|
|[06](chapters/ch06.md)|RAG and Agents|RAG补充外部证据，Agent调用工具，但多步决策引入新故障。|
|[07](chapters/ch07.md)|Finetuning|微调适用于行为或领域适配有可验证收益的场景。|
|[08](chapters/ch08.md)|Dataset Engineering|数据工程决定模型和评估的上限。|
|[09](chapters/ch09.md)|Inference Optimization|推理优化在质量、吞吐、延迟与单位成本之间取舍。|
|[10](chapters/ch10.md)|AI Engineering Architecture and User Feedback|系统架构与用户反馈把一次性实验变成可持续产品。|

## 资料

- [核心框架细读](references/deep-frameworks.md)
- [术语表](glossary.md)
- [方法库](patterns.md)
- [决策速查](cheatsheet.md)
- [来源质量](references/source-quality.md)
- [章段与哈希清单](references/source-manifest.json)

不同书籍间的内容不可混用作者、命名或案例。若只问“从头学习”，从第1章开始。
