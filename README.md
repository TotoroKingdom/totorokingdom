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
| 🎯 Direction | LLM 原理 / Agent 工程 |

---

## 学习记录

现在主要做 Agent 相关开发。框架和工具用得越多，越觉得有些问题不能只停留在“会调用 API”上：模型究竟怎么生成回答？长上下文为什么越来越慢？工具调用是模型决定的，还是框架决定的？

所以接下来想认真补一补 LLM 原理。不是准备转机器学习算法岗，也不打算从 CS229 开始把整个机器学习体系刷一遍。先把和 LLM、Agent 关系最直接的部分学明白。

### 先弄懂 LLM 怎么工作

**1. 从一句话到下一个 Token**

Tokenizer、Embedding、Context Window、Logits、Softmax、Temperature、Top-p、自回归生成。

先搞清楚输入是怎么变成 Token 的，模型输出的到底是什么，以及“生成一句话”实际发生了多少次预测。

**2. Transformer 内部是什么样的**

Attention、Q/K/V、Causal Mask、Multi-Head Attention、FFN、残差连接、归一化、RoPE、Decoder-only 架构。

重点是能沿着数据流看懂一层 Transformer：输入进来后经过了什么，每一步起什么作用。数学不够用时再补矩阵、点积和 Softmax。

**3. 模型的能力从哪里来**

Next Token Prediction、训练目标与 Loss、梯度和反向传播、预训练、SFT、LoRA、DPO，以及强化学习后训练的基本思路。

这部分主要想分清楚：预训练学到了什么，后训练改变了什么，推理模型和普通指令模型有什么区别。暂时不追求完整复现训练过程。

### 再理解推理系统

Transformer 看明白后，再看模型是怎么高效跑起来的：

- Prefill、Decode 和 KV Cache
- Prefix Caching、Batching、PagedAttention
- 量化、显存、延迟与吞吐
- TTFT、TPOT，以及 vLLM 等推理框架的设计

这部分和 Agent 很相关。多轮对话、长上下文、频繁工具调用，最后都会反映到速度和成本上。希望能从模型计算和系统设计两方面解释这些现象。

### 最后回到 Agent

Agent Loop、Tool Calling、Context Engineering、Memory、RAG、模型路由、权限与安全、评估和可观测性，这些已经在实际项目里接触过。下一步不是再找一个框架从头学，而是结合 LLM 原理重新理解它们：

- 为什么工具结果要回到模型，由模型决定下一步？
- 为什么上下文不是越长越好，应该保留什么、丢掉什么？
- 长任务里的状态、记忆和模型上下文有什么区别？
- 为什么同一个 Agent 换了模型，工具调用和任务完成情况会有变化？

还有一条平行的学习线：Ontology、Knowledge Graph 和企业知识治理。继续结合实际问题学习，不强行塞进 Transformer 的学习顺序里。

### 数学和机器学习怎么补

之前看 CS229 时，公式和推导跟起来比较吃力。先不硬啃整门课，遇到具体问题再回头补：

| 遇到的问题 | 回头补什么 |
| --- | --- |
| Attention 公式看不懂 | 向量、矩阵乘法、点积、Softmax |
| 训练过程看不懂 | 导数、梯度、链式法则、Cross Entropy |
| 采样和概率看不懂 | 条件概率、概率分布、对数 |
| SFT、DPO、RL 看不懂 | 最大似然、优化目标、奖励与策略 |

传统机器学习里的决策树、SVM、K-Means、PCA 等先了解概念，不作为目前的主线。

### 参考资料

- [Karpathy — Deep Dive into LLMs](https://www.youtube.com/watch?v=7xTGNNLPyMI)：先把整体过程听明白。
- [3Blue1Brown](https://www.3blue1brown.com/)：补数学直觉，特别是 Attention 和神经网络。
- [Hugging Face LLM Course](https://huggingface.co/learn/llm-course/chapter1/1)：Tokenizer、Transformer 和模型使用。
- [Karpathy — Neural Networks: Zero to Hero](https://karpathy.ai/zero-to-hero.html)：需要从代码理解机制时再看。
- [Stanford CS336](https://cs336.stanford.edu/)：后面深入语言模型训练与系统时选读。
- [vLLM 文档](https://docs.vllm.ai/en/latest/)：学习推理优化时查阅。
- [Stanford CS229](https://cs229.stanford.edu/)：暂时作为数学和机器学习的参考，不从头刷课。

不设“几周必须学完”的计划。能用自己的话讲明白一个概念，知道它和现有系统有什么关系，就继续往下学；碰到理解障碍，再看动画、推公式或者写一小段代码。学习本身不是项目交付。

<p align="center">
  See you in the next deployment.
</p>
