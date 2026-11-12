# 关键术语

以下为学习用工作定义；具体论证请读对应章节。

|术语|含义|章节|
|---|---|---|
|Foundation model|经广泛预训练、可适配多种下游任务的基础模型|[2](chapters/ch02.md)|
|SFT / preference finetuning|用指令—期望回答学习行为；用偏好比较调整相对优劣|[2](chapters/ch02.md)、[7](chapters/ch07.md)|
|Evaluation set|代表目标任务、用于比较模型或系统的样本与判分规则|[3](chapters/ch03.md)、[4](chapters/ch04.md)|
|LLM-as-a-judge|让模型辅助评价输出，需校准一致性、位置与长度等偏差|[4](chapters/ch04.md)|
|Prompt engineering|通过指令、上下文、示例和输出约束引导模型|[5](chapters/ch05.md)|
|RAG|检索外部内容并将相关证据放入生成上下文|[6](chapters/ch06.md)|
|Agent|让模型在多步任务中规划、调用工具并处理结果的系统|[6](chapters/ch06.md)|
|LoRA / QLoRA|低秩可训练增量；在量化冻结底座上训练增量|[7](chapters/ch07.md)|
|Data leakage / contamination|训练、提示、检索或评价之间的信息交叉污染，导致评测失真|[3](chapters/ch03.md)、[8](chapters/ch08.md)|
|Synthetic data|由规则、仿真或 AI 合成以补规模或覆盖的数据，需核验|[8](chapters/ch08.md)|
|TTFT / TPOT|用户等待首个 token 的时间；后续每输出 token 的时间|[9](chapters/ch09.md)|
|Goodput|在服务目标内完成的请求吞吐|[9](chapters/ch09.md)|
|KV cache|推理中缓存历史 token 的 key/value 以免重复计算|[9](chapters/ch09.md)|
|Model gateway / router|统一模型访问、安全与限额的网关；按任务选择路径的路由器|[10](chapters/ch10.md)|
|Explicit / implicit feedback|用户主动评分；从纠错、编辑、接受、停止等行为推测的反馈|[10](chapters/ch10.md)|
