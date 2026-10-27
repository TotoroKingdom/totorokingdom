# TotoroKingdom

**LLM · Agent Runtime · Knowledge Systems**

平时写后端和 Agent，也读一些框架源码。这里放技术笔记、项目，以及正在追的问题。

[技术主页](https://www.paiguangguang.xyz/) · [Learn Codex](https://github.com/TotoroKingdom/paiguangguang-ai/blob/dev/docs/README.zh.md) · [GitHub](https://github.com/TotoroKingdom) · [联系我](mailto:totorokingdom@foxmail.com)

---

## 文章与项目

### [Learn Codex：从一次提问，读懂一套 Agent 系统](https://github.com/TotoroKingdom/paiguangguang-ai/blob/dev/docs/README.zh.md)

一套沿着 Codex 运行链路读源码的教程。从用户输入到模型请求、工具执行和结果回传，重点看 Agent Loop、会话状态、权限和执行环境如何配合。

### [ChatGPT-Harness](https://github.com/TotoroKingdom/ChatGPT-Harness)

一个连接 ChatGPT 与本地工作区的实验项目。MCP 负责工具入口，Runtime 处理工作区限制、权限策略与审批。关注点不只是“让模型能操作文件”，还有**谁允许它操作、操作后留下什么记录**。

### [Codex Agent Lab](https://github.com/TotoroKingdom/codex-rollout-trace)

整理 Codex 会话和运行轨迹的实验仓库。分析模型轮次、工具调用、执行过程和上下文消耗，看看 Agent 的时间与 Token 究竟花在哪里。

---

## 技术路线

目前主要沿着两条线往深处读：一条是 **LLM 自身的计算与训练机制**，另一条是 **Agent 如何把模型接入真实系统**。企业知识系统则是长期关注的方向。

### 01 / LLM：从文本到下一个 Token

先看一次生成具体发生了什么：

```text
文本 → Tokenizer → Token IDs → Embedding
                                ↓
                     Transformer Blocks
                                ↓
                           Logits
                                ↓
                        Sampling → 下一个 Token
                                ↖_____________|
```

这条链路里有几个需要真正弄清楚的地方：

- **Tokenizer / Embedding**：为什么模型看到的不是“字”或“词”，不同切分方式又会带来什么差异？
- **Attention**：Q、K、V 是怎么来的？为什么要除以 √d？Causal Mask 在挡什么？
- **Transformer**：Attention、FFN、残差、归一化和位置编码如何组合？
- **Sampling**：模型给出的是 logits。Temperature、Top-k、Top-p 改变的是选择下一个 Token 的方式。

数学跟不上时就往回查矩阵运算、点积、Softmax 和概率分布。暂时不从传统机器学习课程的第一章顺序往下刷。

### 02 / 训练：模型的能力从哪里来

看懂前向计算之后，再去理解参数是怎么学出来的：

```text
预训练（Next Token Prediction）
          ↓
指令微调（SFT）
          ↓
偏好优化 / 强化学习后训练
          ↓
面向用户的模型行为
```

这里重点读交叉熵、梯度和反向传播、AdamW、LoRA、DPO，以及 PPO / GRPO 的基本思路。不是为了立刻训练一个大模型，而是弄清楚**训练目标不同，模型行为为什么会不同**。

Tool Calling、结构化输出、指令遵循和推理能力，都可以放回这条训练与后训练的脉络里理解。

### 03 / 推理：一个 Token 的成本

模型的前向计算只是起点。真正上线后还会碰到延迟、吞吐和显存的问题。

- **Prefill / Decode**：处理输入和逐 Token 生成，是两种不同的计算负载。
- **KV Cache**：缓存了什么，节省了什么计算，又占用了多少显存？
- **Prefix Caching / Continuous Batching**：请求之间如何复用和调度计算？
- **FlashAttention / PagedAttention**：它们分别解决哪类内存访问或缓存管理问题？
- **量化与推理服务**：参数精度、显存、吞吐和输出质量之间怎么取舍？

接着再读 vLLM 等推理框架。希望能把 TTFT、TPOT、TPS 这些指标和底层实际发生的计算联系起来，而不是只看压测数字。

### 04 / Agent：模型之外的那一半

模型负责预测下一步输出；文件读写、网络请求、权限校验和任务状态都属于模型之外的系统。

这里继续研究：

- **Agent Loop / Harness**：模型输出、工具结果和下一轮模型请求怎样接起来；工具执行成功为什么不等于任务完成。
- **Context Engineering**：上下文窗口有限时，历史、工具结果、检索内容应该怎么取舍。
- **Memory / Checkpoint**：会话上下文、长期记忆和运行时状态不是一回事。
- **MCP / Tool Security**：执行前的权限检查、上游数据权限、工具输出的信任边界。
- **Tracing / Evaluation**：不能只看最终回答，还要能还原模型决策、工具耗时和失败原因。

这一部分会继续结合 Codex 源码和自己的 Harness 项目来写。相比框架的 API 用法，更关心背后的状态流转与架构取舍。

### 05 / 企业知识：让 Agent 用对数据

RAG 不止是切块、Embedding 和向量检索。实际业务里还会遇到文档版本、元数据、组织权限、撤权以及检索结果是否可信的问题。

这条线主要关注 Hybrid Retrieval、Rerank、Knowledge Governance、Ontology、Knowledge Graph 和 GraphRAG。重点是**哪些信息适合语义检索，哪些关系需要显式建模，权限又该在什么边界上生效**。

---

## 阅读资料

这些是长期会翻的资料，不是按顺序必须刷完的课程表。

| 资料 | 用来读什么 |
| --- | --- |
| [Karpathy · Deep Dive into LLMs](https://www.youtube.com/watch?v=7xTGNNLPyMI) | LLM 的全貌：数据、训练、推理、后训练 |
| [3Blue1Brown](https://www.3blue1brown.com/) | 线性代数、Attention、神经网络的直观解释 |
| [Hugging Face LLM Course](https://huggingface.co/learn/llm-course/chapter1/1) | Tokenizer、Transformer、生成过程 |
| [Karpathy · Zero to Hero](https://karpathy.ai/zero-to-hero.html) | 顺着代码理解梯度、神经网络和 GPT |
| [Stanford CS336](https://cs336.stanford.edu/) | 语言模型训练与系统的深入内容 |
| [vLLM Documentation](https://docs.vllm.ai/en/latest/) | KV Cache、调度、推理服务 |
| [Stanford CS229](https://cs229.stanford.edu/) | 数学和机器学习基础，遇到缺口时选读 |

当前更看重 **LLM 原理 → 推理系统 → Agent 架构** 这条阅读顺序。训练与后训练穿插着学；数学够用就继续往下，不把某门课学完当成前提。

---

<details>
<summary>GitHub Stats</summary>

<p align="center">
  <img src="https://github-profile-summary-cards.vercel.app/api/cards/stats?username=TotoroKingdom&theme=github" width="420" />
  <img src="https://github-profile-summary-cards.vercel.app/api/cards/most-commit-language?username=TotoroKingdom&theme=github" width="420" />
</p>
</details>

<details>
<summary>🎮 Genshin Signal</summary>

<p align="center">
  <img src="https://genshin-card-kallka.vercel.app/rand/310652688.png" width="420" />
</p>
</details>
