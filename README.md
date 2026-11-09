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

| Module            | Entry                                                        |
| :---------------- | :----------------------------------------------------------- |
| 🌌 AI World Portal | [Enter My AI World →](https://www.paiguangguang.xyz/)        |
| 📮 Email           | [totorokingdom@foxmail.com](mailto:totorokingdom@foxmail.com) |
| 🎯 Direction       | AI Applications → Transformer Internals → LLM Inference Systems |

## 🗺️ My AI Learning Roadmap

> ✅ 已掌握 / 已实践　⬜ 待学习

### 学习框架：四层知识体系

机器学习 / 深度学习是**技术体系**，监督学习 / 无监督学习 / 自监督学习 / 强化学习是**学习范式**，两者是不同的分类维度；深度学习可以采用多种学习范式。

| 层次                      | 学习重点                                                     | 在路线图中的位置                                        |
| :------------------------ | :----------------------------------------------------------- | :------------------------------------------------------ |
| **第一层：机器学习基础**  | 数据、特征、训练与评估；监督、无监督、自监督及强化学习的基本区别 | 「正在补 → 数学基础 / 机器学习基础」                    |
| **第二层：深度学习**      | 神经网络、反向传播、优化、PyTorch、Transformer               | 「正在补 → PyTorch / 深度学习」「下一步 → Transformer」 |
| **第三层：LLM 训练**      | 自监督预训练、SFT、LoRA、偏好优化、强化学习后训练            | 「后续 → LLM 训练与对齐」                               |
| **第四层：AI Agent 工程** | Agent Loop、Tool Calling、规划、记忆、运行时、评估与安全     | 「已掌握 → Agent / Agent 工程」「Agent 深化」           |

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

> 脑图主线：以现代 Decoder-only（仅解码器）自回归 LLM 为例。节点按“整体 → Block → 子层 → 操作”展开；不同模型的 Norm、位置编码和 FFN 实现可能不同。

- [ ] **01 整体架构**
  - [ ] Token IDs → Token Embedding（词嵌入）→ Hidden States（隐藏状态）
  - [ ] Transformer Block × N（多层堆叠，逐层更新 Hidden States）
  - [ ] Final Norm（最终归一化）→ LM Head（词表投影）→ Logits（各候选 Token 的未归一化分数）
  - [ ] 位置信息：例如 RoPE（旋转位置编码），通常施加在 Attention 的 Q、K 上，并非所有 Transformer 都使用 RoPE
- [ ] **02 Transformer Block × N（以常见 Pre-Norm 结构为例）**
  - [ ] **A. Self-Attention（自注意力）子层**
    - [ ] Norm：先对输入 Hidden States 归一化
    - [ ] Q / K / V Projection：将当前层输入投影为 Query、Key、Value
    - [ ] Attention Heads：MHA（多头注意力）/ GQA（分组查询注意力，多个 Q 头共享一组 K/V 头）/ MQA（多查询注意力）
    - [ ] Position：如使用 RoPE，对 Q、K 施加位置旋转
    - [ ] Scaled Dot-Product Attention（缩放点积注意力）
      - [ ] Attention Scores：Q × Kᵀ / √d_head
      - [ ] Causal Mask：阻止当前位置关注未来 Token（Decoder-only 因果注意力）
      - [ ] Softmax：将分数转换为注意力权重
      - [ ] Weighted Sum of V：用注意力权重对 V 加权求和
    - [ ] Head Merge + Output Projection：合并各头输出并线性投影
    - [ ] Residual Connection：与本子层输入做残差相加
  - [ ] **B. FFN / MLP（前馈网络）子层**
    - [ ] Norm：对 Attention 子层输出归一化
    - [ ] FFN：线性变换 → 非线性激活 / 门控（如 SwiGLU）→ 线性变换
    - [ ] Residual Connection：与本子层输入做残差相加
  - [ ] **C. Block Output**
    - [ ] 产生更新后的 Hidden States，传入下一层 Block
    - [ ] 说明：以上是 Pre-Norm 的概念示意；Post-Norm、并行残差、MoE 等模型实现会有差异
- [ ] **03 关键概念及边界**
  - [ ] Forward Pass（前向计算）：输入经过 Embedding、各层 Transformer、Final Norm、LM Head 后得到 Logits
  - [ ] Hidden States：每层传递的中间表示，不是独立于 Transformer 的额外计算步骤
  - [ ] KV Cache：推理时缓存每层 Attention 历史 Token 的 K、V；缓存的读写发生在 Attention 内部
  - [ ] Transformer 其他结构：Encoder-only 可用双向注意力；Encoder-Decoder 还包含 Cross-Attention（交叉注意力）
- [ ] **04 实践**
  - [ ] 手写 Scaled Dot-Product / Causal Self-Attention，验证 Mask 和张量形状
  - [ ] 手写 Multi-Head Attention 和 Transformer Block（包含 Norm、Residual、FFN）
  - [ ] 手写 Mini GPT：Token IDs → Embedding → Blocks → Final Norm → LM Head → Logits

### LLM 推理

> 脑图主线：以 Decoder-only 自回归文本生成、启用 KV Cache 为例。**Prefill 和 Decode 都会执行模型 Forward Pass；Sampling 发生在 Forward Pass 产生 Logits 之后。**

- [ ] **01 请求准备与输入**
  - [ ] Prompt / Messages：系统指令、用户消息和历史上下文
  - [ ] Chat Template（聊天模板）：按模型格式组织消息和特殊 Token
  - [ ] Tokenizer：文本 → Token IDs
  - [ ] Token Embedding：Token IDs → 向量 / Tensor（张量是数据结构，不是单独的推理阶段）
- [ ] **02 Prefill（预填充：处理输入上下文）**
  - [ ] 对输入 Prompt Token 执行一次批量 Forward Pass（因果 Mask 保证不看未来）
  - [ ] Transformer Block × N：逐层计算 Self-Attention、FFN 等
    - [ ] 每层 Attention 计算该层的 Q / K / V
    - [ ] 将当前 Prompt 的 K、V 写入对应层 KV Cache
  - [ ] Final Norm → LM Head → 最后位置的 Logits
  - [ ] 对最后位置的 Logits 进行 Sampling / Greedy，得到**第一个输出 Token**
- [ ] **03 Decode（增量解码：逐 Token 生成）**
  - [ ] 将上一步选出的 Token ID 输入 Embedding
  - [ ] 对**新 Token** 执行一次增量 Forward Pass，仍然经过全部 Transformer 层
    - [ ] 当前层仅计算新 Token 的 Q、K、V（不重算历史 Token 的 K、V）
    - [ ] 当前 Q 与“历史缓存 K + 当前 K”计算 Attention，并对对应 V 加权求和
    - [ ] 将新 K、V 加入当前层 KV Cache，然后继续 FFN / 后续 Transformer 层
  - [ ] Final Norm → LM Head → 新位置的 Logits → Sampling / Greedy → 下一个 Token
  - [ ] 重复 Decode，直到 EOS、Stop Sequence、最大生成长度等停止条件触发
- [ ] **04 KV Cache（贯穿 Prefill / Decode 的注意力缓存）**
  - [ ] 缓存内容：**每个 Transformer 层各自的历史 K、V**，而不是整套 Transformer 输出或全部 Q
  - [ ] Prefill：建立初始缓存；Decode：复用历史 K、V，并更新新 Token 的 K、V
  - [ ] 作用：避免重复计算历史 Token 的 K、V 及其前序层表示；新 Token 仍需经过各层计算
  - [ ] 成本：常规 KV Cache 的显存占用通常随上下文长度、并发请求数、层数、KV 头数及数值精度等增长；滑动窗口等策略可限制缓存长度
  - [ ] 优化方向：GQA / MQA、Paged KV Cache、Prefix Caching（按模型和推理框架支持情况）
- [ ] **05 Logits、Sampling 与输出**
  - [ ] Logits：LM Head 输出的词表分数，尚非概率
  - [ ] Sampling：按生成策略对 Logits 做 Temperature 缩放、Top-k / Top-p 等过滤及概率归一化，再选出 Token；也可采用 Greedy（具体处理顺序依框架而异）
  - [ ] Temperature / Top-p 主要影响 Token 选择策略，不直接改变已完成的 Transformer 前向计算；选出不同 Token 会影响后续 Decode 的输入
  - [ ] Detokenization：将生成的 Token ID 逐步还原为文本
  - [ ] Stream：服务端可增量发送生成文本；流式传输不等于提前完成整次推理
- [ ] **06 推理性能与工程**
  - [ ] Prefill：重点关注输入长度、计算量与 TTFT（首 Token 延迟）
  - [ ] Decode：重点关注单 Token 延迟（TPOT / ITL）、KV Cache 读写与显存带宽
  - [ ] 服务指标：吞吐（Tokens/s）、并发、显存占用、排队延迟与端到端时延
  - [ ] 优化方向：Continuous Batching（连续批处理）、量化、KV Cache 管理与缓存复用
- [ ] **07 实践**
  - [ ] 部署 vLLM 服务，观察 Prefill、Decode 与 KV Cache
  - [ ] 跑通 Prompt → Token IDs → Prefill → 首 Token → Decode 循环 → Stream
  - [ ] 比较不同输入长度、输出长度、并发数下的 TTFT、TPOT、吞吐和显存

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
