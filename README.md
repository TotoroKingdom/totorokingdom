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
| 🎯 Direction | **LLM Internals → Agent Runtime / Harness → Agentic Architect** |

---

## 🗺️ My AI Learning Roadmap

> **目标：理解 LLM 的工作机制，并将原理转化为可验证的 Agent 工程能力。**  
> 职业方向：AI Agent Engineer → Agent Runtime / Platform Engineer → Agentic Architect。  
> 不以传统机器学习算法研究或从零预训练大模型为当前主线。

### 01 · 学习策略：两条主线，并行推进

| 主线 | 关注的问题 | 最终要证明的能力 |
| :--- | :--- | :--- |
| **A. LLM 原理与推理（30%）** | Token 如何生成？Attention、KV Cache、Prefill / Decode 如何工作？ | 能解释机制、写简化实现、分析推理性能 |
| **B. Agent 工程与架构（50%）** | Agent 如何可靠调用工具、治理上下文、恢复任务、管理权限与模型？ | 能设计可测试、可观测、可恢复的 Runtime / Harness |
| **C. 评估与技术表达（20%）** | 怎样证明改动提升了质量、延迟、成本和可靠性？ | 可复现实验、架构文档、面试级案例分析 |

学习方式：**工程问题 → 原理解释 → 最小实验 → 集成验证 → 指标复盘**。以上是时间分配建议，不是固定排课。

**优先级**

- **P0（必修）**：Tokenizer、Embedding、Self-Attention、Transformer、Sampling、KV Cache、推理指标、Context Engineering、Agent Loop、Tool Calling、权限边界、Trace / Eval。
- **P1（选修深化）**：SFT / LoRA / DPO / RL 基本机制、vLLM / Continuous Batching、MoE、分布式推理、Ontology / Knowledge Graph / GraphRAG。
- **P2（按需查询）**：SVM、K-Means、PCA、完整传统机器学习推导、从零大规模预训练。**CS229 是参考资料，不是前置关卡。**

### 02 · 已有工程基础（有实践 ≠ 所有方向均已精通）

- ✅ **Agent / RAG**：Agent Loop、ReAct、Tool Calling、MCP、Memory、Planning；文档解析、Hybrid Search、Rerank、权限过滤与评估。
- ✅ **Agent 工程**：Task、Checkpoint / Resume、HITL、Multi-Agent / 编排、Permission、Sandbox、Trace 与 Guardrails 等实践。
- ✅ **分布式后端**：并发、消息队列、Worker、Redis、限流、重试、幂等与系统设计。
- ✅ **数学 / PyTorch 起点**：向量、矩阵及基本微分概念；Tensor、Shape / Broadcasting、矩阵运算。
- ⬜ **待补齐的关键缺口**：从源码解释 Transformer、从指标解释推理性能、端到端证明 Agent 优化效果。

### 03 · 16 周核心路线（每阶段都有可验收产物）

| 阶段 | 时间 | 学习主题 | 验收 Gate |
| :--- | :--- | :--- | :--- |
| **M1：理解 LLM 生成** | W1–W3 | Tokenizer / Embedding / QKV / Causal Mask / Transformer / Logits / Sampling | 最小 GPT 实现 + 关键张量形状与输出解释 |
| **M2：理解推理系统** | W4–W6 | Prefill / Decode、KV Cache、TTFT / TPOT / TPS、Prefix Caching、Batching | 无缓存 vs 有缓存对照实验 + 延迟报告 |
| **M3：深化 Agent Runtime** | W7–W10 | Context Engineering、Tool / MCP、State、Checkpoint、权限与恢复、模型路由 | 一个可恢复、可追踪、权限受控的 Agent 执行链 |
| **M4：企业知识与 Agent** | W11–W13 | Hybrid RAG、ACL、撤权复验、Ontology / GraphRAG 适用边界 | 带权限与失败场景的知识问答 E2E 评估 |
| **M5：工程证据与求职** | W14–W16 | Evaluation、可靠性、成本、架构取舍、系统设计表达 | 可公开演示 + 基准数据 + 架构决策文档 |

#### M1 · LLM 工作机制

- [ ] 理解 BPE / Tokenizer、Embedding、位置编码、Logits、Temperature / Top-p；能解释自回归生成。
- [ ] 手写简化 Self-Attention，跟踪 Q / K / V 与 Attention Score 的形状。
- [ ] 用 PyTorch 拼出最小 Decoder-only Transformer / Mini GPT，验证 Causal Mask。
- [ ] **Gate：**能从输入 Token 逐步解释到下一个 Token 的采样；实验可运行、关键形状有断言。

#### M2 · LLM Inference Systems

- [ ] 区分 Prefill / Decode；理解 KV Cache 的计算节省与显存代价。
- [ ] 理解 Prefix Caching、Continuous Batching、PagedAttention、量化的适用边界。
- [ ] 做一次无 KV Cache / 有 KV Cache 的小模型对照；记录 Prompt 长度、TTFT、TPOT、吞吐与环境。
- [ ] **Gate：**写一页推理性能分析，说明瓶颈、测量方法与至少一种优化取舍。
- [ ] 可选：具备合适 GPU 时体验 vLLM；无 GPU 时用小模型或已有模型服务完成原理与指标实验，**不以部署 vLLM 为通关条件**。

#### M3 · Agent Runtime / Harness

- [ ] 梳理 Agent Loop / Tool Result / Model Decision / Task State 的边界：工具返回 ≠ 任务成功。
- [ ] 实现或完善 Context Budget、裁剪 / 摘要、上下文溯源与长任务恢复。
- [ ] 明确 Tool / MCP 调用前授权、上游授权与返回数据校验边界；覆盖撤权、超时、失败与重试场景。
- [ ] 将 Model Routing / Fallback、Trace、Token / Cost、Latency、Tool Error 纳入统一观测。
- [ ] **Gate：**以已有 Agent 工程做集成验证；保留正常、权限拒绝、工具异常、中断恢复等场景的运行证据。

#### M4 · Knowledge / Ontology × Agent

- [ ] 巩固 Hybrid Retrieval（BM25 + Vector + Rerank）与引用溯源、召回质量评估。
- [ ] 理解 Entity / Relation、Taxonomy、Ontology 与 Knowledge Graph 的差异和取舍。
- [ ] 验证租户 / 组织 / 文档 ACL、密级、撤权后的召回与输出复验。
- [ ] **Gate：**用脱敏或合成数据完成多角色 E2E 测试；给出失败样例与改进前后结果。不得公开企业私有数据。

#### M5 · Job-ready Engineering Evidence

- [ ] **Case Study A — LLM 推理性能**：实验方法、基线、优化、结果和限制。
- [ ] **Case Study B — Agent Runtime 可靠性**：状态机、工具失败、权限模型、恢复机制、Trace。
- [ ] **Case Study C — 企业知识问答**：检索、ACL、Evaluation 与知识治理边界。
- [ ] **Gate：**每个案例至少有架构图、可复现的最小 Demo / 测试、指标或断言证据、取舍说明；能在面试中独立讲清楚。

### 04 · 数学 / ML：遇到问题再补，不走 CS229 全量先修

| 当前问题 | 只补所需基础 | 立即应用 |
| :--- | :--- | :--- |
| 看不懂 Attention | 向量点积、矩阵乘法、Softmax | 手写 QKᵀ / √d 与 Attention |
| 看不懂训练损失 | 对数、概率、Cross Entropy、梯度与链式法则 | 小样本 next-token loss / Autograd |
| 看不懂模型输出 | 条件概率、Logits、采样分布 | Temperature / Top-p 实验 |
| 看不懂 SFT / RL | 最大似然、优化目标、Policy / Reward 基础 | 比较 SFT、DPO、RL 的目标和反馈信号 |

暂时不把线性回归、决策树、SVM、聚类、PCA 的完整课程学习或刷题作为通往 LLM 的必经路径。

### 05 · 学习资源（按需选章节，不以刷完课程为目标）

| 资源 | 何时使用 | 策略 |
| :--- | :--- | :--- |
| [Hugging Face LLM Course](https://huggingface.co/learn/llm-course/chapter1/1) | M1 入门 | 选 Tokenizer、Transformer、生成相关内容 |
| [Karpathy — Neural Networks: Zero to Hero](https://karpathy.ai/zero-to-hero.html) | M1 代码实现 | 优先看 GPT 构建，缺反向传播再补前置章节 |
| [vLLM Documentation](https://docs.vllm.cc/en/latest/) | M2 推理系统 | 阅读 KV Cache、Prefix Caching、Serving / 性能文档 |
| [Stanford CS336 — Language Modeling from Scratch](https://cs336.stanford.edu/) | M1/M2 深化；后续持续参考 | 选择 Transformer、推理与评估内容；不强制完成高计算成本的训练作业 |
| [PyTorch Tutorials](https://pytorch.org/tutorials/) | 代码卡点时 | Tensor、Autograd、Module、训练循环按需查阅 |

### 06 · 执行与复盘规则

- **每周节奏**：约 3 小时原理、4 小时实验 / 工程、1 小时复盘；时间不足时优先完成本阶段 Gate。
- **每周只交付一个主成果**：一个最小实验、一份性能报告或一条真实 E2E 证据，避免多项目并行分散注意力。
- **Done 的定义**：不是“看完视频”或“运行成功”，而是能 **解释原理、展示可复现证据、说清设计取舍**。
- **学习与项目双向驱动**：现有 Agent / RAG / Harness 代码优先作为实验场；缺什么原理，就学习什么原理。
- **四周复盘一次**：如果当前阶段阻碍工程产出，就缩小任务和补对应前置知识；不因一门大学课程过难而整体停摆。

---

> **North Star:** Understand LLMs deeply enough to engineer reliable, observable, secure, and efficient Agent systems.

<p align="center">
  See you in the next deployment.
</p>
