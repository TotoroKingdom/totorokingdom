<!-- 🌌 TotoroKingdom GitHub Profile -->

<h1 align="center">🌌 TotoroKingdom</h1>

<p align="center">
  <b>AI Engineer · Full-Stack Developer · LLM Systems Explorer</b>
</p>
<p align="center">
  <b>Vibe Coding</b>
</p>

## 🎮 Genshin Signal

<p align="center">
  <img src="https://genshin-card-kallka.vercel.app/rand/310652688.png" width="420" />
</p>

<p align="center">
  <i>愿派蒙与你同在 ✨</i>
</p>

---

## 📊 GitHub Stats

<p align="center">
  <img
    src="https://github-profile-summary-cards.vercel.app/api/cards/stats?username=TotoroKingdom&theme=github"
    width="420"
  />
</p>

## 💻 Most Used Languages

<p align="center">
  <img
    src="https://github-profile-summary-cards.vercel.app/api/cards/most-commit-language?username=TotoroKingdom&theme=github"
    width="420"
  />
  <img
  src="https://github-profile-summary-cards.vercel.app/api/cards/repos-per-language?username=TotoroKingdom&theme=github"
  width="420"
/>
</p>
---

## 🧭 Navigation

| Module | Entry |
| :--- | :--- |
| 🌌 AI World Portal | [Enter My AI World →](https://www.paiguangguang.xyz/) |
| 📮 Email | [Contact](mailto:totorokingdom@foxmail.com) |
| 🎯 Direction | **LLM Fundamentals → LLM Inference → Agent Systems** |

---

## 🗺️ My AI Learning Roadmap

> **学习目标：理解 LLM 为什么能生成语言、如何获得能力、为什么会有局限，以及这些原理如何影响 Agent 系统设计。**
>
> 职业方向：AI / Agent Engineer → Agent Runtime / Platform → Agentic Architect。  
> 这是**知识学习地图**，不是项目开发计划。没有固定工期、代码交付门槛或阶段验收；可根据理解程度调整顺序和深度。

### 🧭 学习的主线

```text
认识 LLM：Token 是怎样一步步生成的？
                ↓
理解 Transformer：模型内部发生了什么？
                ↓
理解训练与对齐：模型的能力从哪里来？
                ↓
理解推理系统：为什么推理会慢、贵、占显存？
                ↓
理解 LLM 的能力边界：为什么 Agent 需要工具、记忆与外部控制？
                ↓
回到 Agent 工程：用模型原理指导架构取舍
```

**学习原则**

- **先直觉，后公式，再源码**：先听懂“是什么、为什么”，再逐渐研究数学与实现。
- **按需补基础**：数学、PyTorch 和传统机器学习是辅助工具，不是必须全部学完才能进入 LLM。
- **主线学原理，实践帮助理解**：小实验是可选的理解手段，不把“写完代码、通过测试、部署服务”当成学会知识的前提。
- **Agent 工程与理论互相印证**：已有的工程经验用于提出问题；不要求每个理论知识点都立即改造成项目功能。

### 📍 当前起点

| 已有基础 | 接下来希望弄懂 |
| :--- | :--- |
| Agent Loop、Tool Calling、MCP、Memory、RAG 等工程实践 | LLM 的生成、推理、规划与工具调用能力究竟来自哪里 |
| 后端、并发、缓存、分布式系统经验 | Prefill、Decode、KV Cache、Batching、显存与吞吐背后的原理 |
| 向量 / 矩阵、基础微积分概念；PyTorch Tensor 等入门知识 | Attention 的数学意义、损失函数、梯度与训练过程 |

以上是根据已有学习记录整理的起点，不表示每个主题都已经达到同一熟练程度。

---

## 第一部分 · 从整体上理解 LLM

**核心问题：大模型到底在做什么？**

- [ ] LLM、Language Model、Foundation Model、Chat Model 的概念与关系
- [ ] Token、Tokenizer、Vocabulary、Embedding
- [ ] Context Window 与自回归生成（Autoregressive Generation）
- [ ] Logits、Softmax、Temperature、Top-k / Top-p、停止条件
- [ ] Base Model、Instruct Model、Reasoning Model 的区别
- [ ] Prompt、System Instruction、Tool Call 在输入 / 输出层面是什么

**理解重点：**能用自然语言讲清楚“输入一句话之后，模型怎样一步步预测并生成下一个 Token”；知道模型产生的是预测结果，而不是直接执行系统操作。

**推荐入门：**[Karpathy — Deep Dive into LLMs](https://www.youtube.com/watch?v=7xTGNNLPyMI)；[Hugging Face LLM Course](https://huggingface.co/learn/llm-course/chapter1/1)。

## 第二部分 · Transformer 的内部机制

**核心问题：Transformer 为什么能够利用上下文？**

- [ ] Embedding 与位置表示
- [ ] Dot Product、Q / K / V 的直觉含义
- [ ] Self-Attention 与 Scaled Dot-Product Attention
- [ ] Causal Mask：为什么不能“偷看”未来 Token
- [ ] Multi-Head Attention：为什么有多个注意力头
- [ ] Feed-Forward Network、Residual Connection、LayerNorm / RMSNorm
- [ ] RoPE 等位置编码机制
- [ ] Decoder-only Transformer 的完整数据流

**理解重点：**不仅记住“Attention = QKᵀ / √d”，还要知道每一步解决什么问题，矩阵的维度如何变化，以及 Attention 如何把上下文信息混合进表示。

**可选辅助：**看动画、画一张 Transformer 结构图，或用 NumPy / PyTorch 算一次极小的 Attention。**不要求先手写完整 GPT。**

**推荐资源：**[3Blue1Brown](https://www.3blue1brown.com/)；[Karpathy — Zero to Hero](https://karpathy.ai/zero-to-hero.html)。

## 第三部分 · 模型是怎样训练和对齐的

**核心问题：为什么预训练模型能学会语言？为什么指令模型会遵循要求？**

- [ ] 自监督学习与 Next Token Prediction
- [ ] 训练数据、训练 / 验证、Loss、Cross Entropy 与 Perplexity
- [ ] Forward、Backward、Gradient、Optimizer、AdamW 的基本作用
- [ ] Pretraining 与 Post-training 的区别
- [ ] SFT：示例如何影响模型行为
- [ ] 偏好优化与强化学习后训练：Reward Model、DPO、PPO / GRPO 的基本思想
- [ ] LoRA / QLoRA：为什么可以低成本微调
- [ ] Tool Calling 与结构化输出：训练行为、模型输出格式和外部执行之间的关系
- [ ] Hallucination、泛化、训练分布和模型能力边界

**理解重点：**分清“模型参数怎样被训练更新”和“Agent 运行时怎样通过提示词、工具及反馈组织任务”；**Agent Loop 不等于强化学习**。

这里重点掌握训练过程和方法之间的区别，**暂不以完整训练大模型、推导 PPO/GRPO 论文细节为目标**。

## 第四部分 · LLM 推理原理与系统

**核心问题：为什么模型推理既慢又贵？优化究竟发生在哪里？**

- [ ] Training vs. Inference；自回归推理中的计算过程
- [ ] Prefill 与 Decode：两种阶段的工作负载有什么不同
- [ ] KV Cache：复用了什么、为什么能提速、代价是什么
- [ ] Prompt Length / Output Length 与延迟的关系
- [ ] TTFT、TPOT、TPS、Throughput 与 Latency 的区别
- [ ] Batching、Continuous Batching、Prefix Caching
- [ ] FlashAttention、PagedAttention 的问题背景和核心思想
- [ ] Quantization、模型参数量、显存占用的基本关系
- [ ] vLLM 与推理服务的基本架构；本地部署和 API 服务的差异

**理解重点：**能解释“长上下文为什么增加计算与缓存压力”“KV Cache 与 Prefix Caching 有何不同”“吞吐和单请求延迟为何会冲突”。

**推荐资源：**[vLLM Docs](https://docs.vllm.ai/en/latest/)；[Stanford CS336](https://cs336.stanford.edu/)（选读相关章节，作为进阶参考）。

## 第五部分 · 用 LLM 原理理解 Agent

**核心问题：模型本身不执行外部操作，Agent 为什么能完成任务？**

- [ ] LLM 与 Agent 的边界：模型推断、工具执行、外部控制循环
- [ ] Tool Calling：模型怎样表达调用意图，谁真正执行工具
- [ ] Reasoning / Planning 的能力与局限；为什么“想得更久”不必然做得更对
- [ ] Context Engineering：上下文位置、长度、噪声、裁剪和压缩的影响
- [ ] Memory、RAG、长期任务状态：参数知识与外部信息的区别
- [ ] 多轮调用中的延迟、成本、缓存与错误累积
- [ ] Model Routing：能力、成本、上下文长度、延迟如何影响选型
- [ ] Tool 失败、权限边界、可信 / 不可信内容与 Prompt Injection
- [ ] Agent Evaluation：最终结果、执行轨迹、工具调用、模型判断分别评估什么

**理解重点：**能从模型特性解释 Agent 的系统设计，而不是只会描述框架 API。已有工程实践继续作为理解这些问题的参照，不另设代码交付目标。

## 第六部分 · 按兴趣与职业方向深化（非必修顺序）

| 专题 | 值得研究的问题 | 学习建议 |
| :--- | :--- | :--- |
| Reasoning Models | 推理时计算、长思考、测试时扩展如何影响能力和成本？ | 优先 |
| MoE / 大模型架构 | 稀疏激活为什么能改变参数规模与计算成本的关系？ | 选学 |
| 分布式推理 | Tensor / Pipeline Parallelism、模型切分、通信开销怎样相互影响？ | 选学 |
| Multimodal LLM | 视觉、语音等非文本信息如何进入模型？ | 选学 |
| Ontology / Knowledge Graph / GraphRAG | 外部结构化知识何时优于纯向量检索？ | 与企业知识经验结合 |
| 模型训练研究 | 预训练数据工程、Scaling Laws、优化稳定性 | 有进一步研究目标时深入 |

---

## 🧮 数学与机器学习：作为随学随查的辅助线

**不要求先完成 Stanford CS229。**先掌握能够支撑 LLM 原理理解的最小知识集合：

| 学 LLM 时遇到的问题 | 按需补充 |
| :--- | :--- |
| 看不懂 QKᵀ、Embedding 或张量形状 | 向量、矩阵乘法、点积、维度、线性变换 |
| 看不懂 Softmax、采样或 Cross Entropy | 概率分布、条件概率、对数、期望 |
| 看不懂 Backpropagation 和训练 | 导数、偏导、链式法则、梯度下降 |
| 看不懂 SFT / DPO / RL | 最大似然、优化目标、奖励与策略的基本概念 |

已有基础：✅ 向量与矩阵、矩阵乘法、线性变换、导数、偏导、梯度、链式法则等已有学习经历；概率与优化相关内容继续补充。

传统机器学习的回归、分类、SVM、K-Means、PCA 等可以了解基本概念，**不作为 LLM 学习的必经前置课程**。

## 📚 课程怎么选

| 课程 / 材料 | 适合解决的问题 | 使用方式 |
| :--- | :--- | :--- |
| [Karpathy — Deep Dive into LLMs](https://www.youtube.com/watch?v=7xTGNNLPyMI) | 先建立完整的 LLM 认知 | **从这里开始** |
| [Hugging Face LLM Course](https://huggingface.co/learn/llm-course/chapter1/1) | Tokenizer、Transformer、生成机制的结构化学习 | 边看边查概念 |
| [3Blue1Brown](https://www.3blue1brown.com/) | Attention、神经网络和数学直觉 | 看不懂公式时使用 |
| [Karpathy — Zero to Hero](https://karpathy.ai/zero-to-hero.html) | 从直觉走向代码层机制 | 选看，不必完成所有项目 |
| [Stanford CS336](https://cs336.stanford.edu/) | 从语言建模延伸到训练与系统 | 进阶选读，难度较高 |
| [Stanford CS229](https://cs229.stanford.edu/) | 系统学习机器学习与数学方法 | 工具书性质，**暂不作为主课** |

## 📝 怎样判断自己学懂了

不使用工期、Gate 或代码测试来衡量学习进度。每学一个主题，可以循序渐进地问自己：

1. **直觉层**：不用术语，能向别人讲明白它是什么、为什么存在吗？
2. **机制层**：能画出过程，说明输入、输出、关键步骤和限制吗？
3. **关联层**：能解释它与 LLM 推理、上下文或 Agent 设计有什么关系吗？
4. **深入层（可选）**：是否有必要看公式、论文、源码或做小实验？

如果某门课程听不懂，先判断是数学符号、概念、前置知识还是讲授节奏的问题，换一种讲法或补一个知识点，**不必因此推翻整条学习路线**。

> **North Star:** Understand how LLMs work, why they behave as they do, and how that understanding leads to better Agent systems.

<p align="center">
  See you in the next deployment.
</p>
