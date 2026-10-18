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
| 🌌 AI World Portal | [Enter My AI World →](https://www.paiguangguang.xyz/)           |
| 📮 Email           | [totorokingdom@foxmail.com](mailto:totorokingdom@foxmail.com)   |
| 🎯 Direction       | AI Applications → Transformer Internals → LLM Inference Systems |

## 🗺️ My AI Learning Roadmap

> ✅ 已掌握 / 已实践　⬜ 待学习

### 学习框架：四层知识体系

机器学习 / 深度学习是**技术体系**，监督学习 / 无监督学习 / 自监督学习 / 强化学习是**学习范式**，两者是不同的分类维度；深度学习可以采用多种学习范式。

| 层次 | 学习重点 | 在路线图中的位置 |
| :--- | :--- | :--- |
| **第一层：机器学习基础** | 数据、特征、训练与评估；监督、无监督、自监督及强化学习的基本区别 | 「正在补 → 数学基础 / 机器学习基础」 |
| **第二层：深度学习** | 神经网络、反向传播、优化、PyTorch、Transformer | 「正在补 → PyTorch / 深度学习」「下一步 → Transformer」 |
| **第三层：LLM 训练** | 自监督预训练、SFT、LoRA、偏好优化、强化学习后训练 | 「后续 → LLM 训练与对齐」 |
| **第四层：AI Agent 工程** | Agent Loop、Tool Calling、规划、记忆、运行时、评估与安全 | 「已掌握 → Agent / Agent 工程」「Agent 深化」 |

> 学习顺序不是从零开始：已有 Agent 工程实践继续保留；补齐底层原理，再反哺 LLM 与 Agent 架构能力。**Agent Loop 不等于强化学习**，只有基于反馈训练或更新策略，才涉及相应的学习过程。

---

## 1. 已掌握

* ✅ **RAG**：文档解析、向量检索、BM25、混合检索、Rerank、权限过滤、评估
* ✅ **Agent**：Agent Loop、ReAct、Tool Calling、MCP、Memory、Planning
* ✅ **Agent 工程**：任务系统、Checkpoint / Resume、HITL、Multi-Agent、Agent 编排
* ✅ **安全与评估**：Trace、LLM Judge、Guardrails、Permission、Sandbox
* ✅ **系统设计**：并发、队列、Worker、Redis、MQ、限流、重试、幂等、高可用、分布式系统

---

## 2. 正在补

### 数学基础

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

### 机器学习基础（第一层）

* [ ] 学习范式：监督学习 / 无监督学习 / 自监督学习 / 强化学习
* [ ] 数据与泛化：特征、标签、训练集 / 验证集 / 测试集
* [ ] 监督学习：回归、分类、线性回归、逻辑回归、决策树
* [ ] 无监督学习：聚类、降维、K-Means、PCA
* [ ] 自监督学习：从原始数据自动构造预测目标，与人工标签的区别
* [ ] 强化学习入门：State / Action / Reward / Policy / Return
* [ ] 模型训练与评估：损失函数、优化目标、Accuracy / Precision / Recall / F1
* [ ] 泛化问题：过拟合、欠拟合、正则化与数据泄漏

#### 实践

* [ ] 用 Scikit-learn 完成一个监督分类任务并评估效果
* [ ] 用 K-Means 完成一个无监督聚类任务，解释聚类结果

### PyTorch（第二层：实现工具）

* ✅ Tensor
* ✅ Shape & Broadcasting
* ✅ Matrix Operations
* [ ] Autograd
* [ ] `nn.Module`
* [ ] Loss Function
* [ ] Optimizer
* [ ] Training Loop
* [ ] GPU / CUDA 基础

#### 实践

* [ ] 独立写出完整 Training Loop
* [ ] 追踪 Tensor Shape 变化

### 深度学习（第二层）

* [ ] Neural Network
* [ ] Forward Propagation
* [ ] Backpropagation
* [ ] Activation Function
* [ ] Gradient Descent
* [ ] Cross Entropy
* [ ] Adam / AdamW
* [ ] Overfitting / Regularization

---

## 3. 下一步

### Transformer（第二层 → LLM）

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

#### 实践

* [ ] 手写 Self-Attention
* [ ] 手写 Transformer Block
* [ ] 手写 Mini GPT
* [ ] Token → Embedding → Attention → FFN → Logits

### LLM 推理

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

#### 实践

* [ ] 部署 vLLM 服务
* [ ] 跑通完整推理过程
* [ ] 分析延迟 / 吞吐 / 显存

---

## 4. Agent 深化（第四层：AI Agent 工程）

* [ ] Workflow / Agent 边界
* [ ] Router / Planner / Executor
* [ ] Supervisor / Handoff
* [ ] Context Engineering
* [ ] 长任务状态保存与恢复
* [ ] Agent Evaluation
* [ ] Tool 权限与安全边界
* [ ] Agent Runtime
* [ ] 区分 Agent 的执行反馈 / 轨迹评估与强化学习中的策略训练

---

## 5. 企业知识

* [ ] Ontology
* [ ] Knowledge Graph
* [ ] Entity / Relation Modeling
* [ ] Graph Retrieval / GraphRAG
* [ ] Metadata / Taxonomy
* [ ] Knowledge Governance
* [ ] 企业知识权限模型

---

## 6. 后续

### LLM 训练与对齐（第三层）

* [ ] 自监督预训练：Next Token Prediction / Causal Language Modeling
* [ ] 训练数据：预训练语料、数据质量、Token 与训练目标
* [ ] SFT：监督微调（Instruction → Response）
* [ ] LoRA / QLoRA：参数高效微调
* [ ] DPO：基于偏好数据的直接偏好优化
* [ ] 强化学习基础：MDP、Policy、Value、Reward、探索与利用
* [ ] 奖励信号：Reward Model / Verifiable Reward
* [ ] PPO / GRPO：策略优化方法及其在 LLM 后训练中的应用
* [ ] 对比 Pretraining / SFT / DPO / RL：数据、反馈信号与优化目标

#### 实践

* [ ] 为一个小模型准备指令数据，跑通 SFT 或 LoRA 微调
* [ ] 分析一条偏好优化 / 强化学习训练链路（奖励信号、策略更新、评估）

### 模型架构与进阶方向

* [ ] MoE
* [ ] DeepSeek Architecture
* [ ] Reasoning Models
* [ ] Multimodal LLM
* [ ] 分布式 LLM Inference

---

## 🎯 当前顺序

```text
Machine Learning Fundamentals
   ↓
PyTorch & Deep Learning
   ↓
Transformer
   ↓
LLM Inference + LLM Training & Alignment
   ↓
Agent Architecture（结合现有 Agent 工程经验）
   ↓
AI Agent Architect
```

<p align="center">
  See you in the next deployment.
</p>