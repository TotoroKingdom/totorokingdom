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

| Module             | Entry                                                           |
| :----------------- | :-------------------------------------------------------------- |
| 🌌 AI World Portal | [Enter My AI World →](https://www.paiguangguang.xyz/)                  |
| 📮 Email           | [totorokingdom@foxmail.com](mailto:totorokingdom@foxmail.com)   |
| 🎯 Direction       | AI Applications → Transformer Internals → LLM Inference Systems |

## 🗺️ My AI Learning Roadmap

> 目标：**AI Agent 工程师 → AI Agent 架构师**
>
> 不追求把所有 AI 名词学一遍。工作里继续做 Agent，学习时间主要用来补模型底层。
>
> ✅ 已掌握 / 已实践　⬜ 待学习

---

## 1. 已经会的

这些内容已经在项目里做过，后面以实践和深化为主，不再当成“从零学习”的课程。

* ✅ **RAG 工程**：文档解析、向量检索、BM25、混合检索、Rerank、权限过滤、评估
* ✅ **Agent 基础**：Agent Loop、ReAct、Tool Calling、MCP、Memory、Planning
* ✅ **Agent 工程**：任务系统、Checkpoint / Resume、HITL、Multi-Agent、Agent 编排
* ✅ **安全与评估**：Trace、LLM Judge、Guardrails、Permission、Sandbox
* ✅ **系统设计**：并发、队列、Worker、Redis、MQ、限流、重试、幂等、高可用、分布式系统

---

## 2. 现在正在补的

### 数学基础

数学只学到能够看懂深度学习和 Transformer，不走纯数学路线。

* ✅ 向量与矩阵
* ✅ 矩阵乘法
* ✅ 线性变换
* ✅ 特征值 / 特征向量
* ✅ 导数 / 偏导数 / 梯度
* ✅ 链式法则
* [ ] 概率分布
* [ ] 期望 / 方差
* [ ] 条件概率
* [ ] 最大似然估计
* [ ] Softmax / Cross Entropy

### PyTorch

* ✅ Tensor
* ✅ Shape & Broadcasting
* ✅ Matrix Operations
* [ ] Autograd
* [ ] `nn.Module`
* [ ] Loss Function
* [ ] Optimizer
* [ ] Training Loop
* [ ] GPU / CUDA 基础

目标：

* [ ] 独立写出一个完整训练循环
* [ ] 能看懂 Tensor Shape 在网络里的变化

### 深度学习

* [ ] Neural Network
* [ ] Forward Propagation
* [ ] Backpropagation
* [ ] Activation Function
* [ ] Gradient Descent
* [ ] Cross Entropy
* [ ] Adam / AdamW
* [ ] Overfitting / Regularization

---

## 3. 接下来重点学

### Transformer

这是当前模型原理学习的核心。

* [ ] Tokenization
* [ ] Embedding
* [ ] Q / K / V
* [ ] Self-Attention
* [ ] Multi-Head Attention
* [ ] Causal Mask
* [ ] FFN
* [ ] Residual Connection
* [ ] LayerNorm / RMSNorm
* [ ] RoPE
* [ ] Transformer Block
* [ ] Decoder-only Transformer

目标：

* [ ] 手写 Self-Attention
* [ ] 手写 Transformer Block
* [ ] 手写 Mini GPT
* [ ] 能从 Token 一路追踪到最终 Logits

### LLM 推理

重点理解“大模型到底是怎么跑起来的”。

* [ ] 自回归生成
* [ ] Prefill / Decode
* [ ] KV Cache
* [ ] Sampling
* [ ] FlashAttention
* [ ] PagedAttention
* [ ] Continuous Batching
* [ ] Quantization
* [ ] vLLM
* [ ] TTFT / TPOT / TPS
* [ ] GPU 显存分析

目标：

* [ ] 部署一个 vLLM 服务
* [ ] 看懂一次完整推理过程
* [ ] 能分析延迟、吞吐和显存瓶颈

---

## 4. Agent 继续往深处学

这条线和模型学习并行，不停掉实际 Agent 工程。

接下来不再重点学习“某个框架怎么调用”，而是学习**怎么做系统判断**。

* [ ] Workflow 和 Agent 的边界
* [ ] Router / Planner / Executor
* [ ] Supervisor / Handoff
* [ ] Context Engineering
* [ ] 长任务的状态保存与恢复
* [ ] Agent Evaluation
* [ ] Tool 权限与安全边界
* [ ] Agent Runtime

我希望最后能回答这些问题：

* 什么场景应该用 Agent，什么场景普通 Workflow 就够了？
* Context 应该放什么，不应该放什么？
* Tool 应该怎么设计，权限边界在哪里？
* Agent 中途失败后怎么恢复？
* Multi-Agent 什么时候真的有价值？
* 怎么证明一次改动让 Agent 变好了，而不是“感觉更好了”？

---

## 5. 企业知识方向

RAG 已经不是下一阶段的重点，下一步是理解企业知识本身怎么组织。

* [ ] Ontology
* [ ] Knowledge Graph
* [ ] Entity / Relation Modeling
* [ ] Graph Retrieval / GraphRAG
* [ ] Metadata / Taxonomy
* [ ] Knowledge Governance
* [ ] 企业知识权限模型

目标：把 **知识 → 权限 → 检索 → Agent** 串成完整系统。

---

## 6. 以后再学

这些内容重要，但暂时不挡当前主线。

* [ ] SFT
* [ ] LoRA / QLoRA
* [ ] DPO
* [ ] PPO / GRPO
* [ ] MoE
* [ ] DeepSeek Architecture
* [ ] Reasoning Models
* [ ] Multimodal LLM
* [ ] 更深入的分布式 LLM Inference

---

## 🎯 当前顺序

```text
PyTorch
   ↓
Deep Learning
   ↓
Transformer
   ↓
LLM Inference
   ↓
Agent Architecture
   ↓
AI Agent Architect
```

Agent / RAG / 系统设计不会等上面全部学完才继续，而是在真实项目里同步推进。

<p align="center">
  🌌 Build things. Understand how they work. Keep going deeper.
</p>

<p align="center">
  See you in the next deployment.
</p>