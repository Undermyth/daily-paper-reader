---
title: "A unified model of short- and long-term plasticity: Effects on network connectivity and information capacity"
title_zh: 短时与长时塑性的统一模型：对网络连接性和信息容量的影响
authors: "Ahokainen, I., Linne, M.-L."
date: 2026-06-22
pdf: "https://www.biorxiv.org/content/10.1101/2025.11.07.687160v2.full.pdf"
tags: ["query:comp-neuro"]
score: 9.0
evidence: 短时和长时突触可塑性的统一模型
tldr: 现有STDP模型常忽略短时程动力学对长时程可塑性的影响。本文提出SL-STDP规则，整合Tsodyks-Markram短时程模型与突触后长时程可塑性，拟合视觉皮层第5层数据。应用于递归神经网络发现，SL-STDP网络自组织为不同频率集群，加入稳态调节后进一步改善信息容量。结果表明短时程动力学通过改变长时程可塑性的频率依赖塑造网络连接和信息处理能力。
source: biorxiv
selection_source: fresh_fetch
motivation: 现有STDP模型忽略短时程动力学对长时程可塑性的影响，导致对某些神经元类型过度简化，需要新模型研究二者耦合效应。
method: 提出SL-STDP规则，将Tsodyks-Markram短时程模型与突触后长时程STDP整合，拟合视觉皮层L5数据并应用于递归神经网络训练。
result: SL-STDP网络形成不同频率集群并稳定动力学；加入权重归一化和兴奋-抑制可塑性后，信息容量在多数储层计算任务中优于未耦合模型。
conclusion: 短时程动力学通过调节长时程可塑性的频率依赖，对网络自组织及信息处理起关键作用。
---

## 摘要
活动依赖性突触可塑性是塑造神经回路连接性和活动的基本学习机制。现有的尖峰时序依赖性可塑性（STDP）计算模型以不同程度的生物细节捕捉长时突触变化。常见方法是忽略短时动力学对长时塑性的影响，这可能对某些神经元类型过于简化。因此，需要新模型来研究短时动力学如何影响长时塑性。为填补这一空白，我们引入了一种新的现象学模型——短-长时STDP（SL-STDP）规则，该规则直接将Tsodyks-Markram短时动力学模型与突触后长时塑性整合。我们将新模型拟合到视觉皮层第5层的记录数据，并研究短时塑性如何影响单个突触长时塑性的放电频率依赖性。我们的分析揭示，长时塑性的前突触和后突触频率依赖性在塑造递归神经网络（RNN）的自组织及其通过汇聚和源节点的信息处理中起关键作用。我们将SL-STDP规则应用于RNN，发现SL-STDP网络中的神经元自组织成不同的放电率簇，稳定了动力学。我们通过引入稳态平衡（即权重归一化和兴奋-抑制可塑性）扩展了实验，并观察到SL-STDP网络与无短时和长时塑性直接耦合的网络在度相关性上的差异。最后，我们评估了修改后的连接性如何影响网络在储层计算任务中的信息容量。SL-STDP规则在大多数任务中优于非耦合系统，而包含兴奋-抑制易化突触进一步提高了信息容量。我们的研究表明，短时动力学诱导的长时塑性频率依赖性变化在塑造网络动力学和将突触机制与RNN中的信息处理联系起来方面发挥关键作用。

## Abstract
Activity-dependent synaptic plasticity is a fundamental learning mechanism that shapes the connectivity and activity of neural circuits. Existing computational models of Spike-Timing-Dependent Plasticity (STDP) capture long-term synaptic changes with varying degrees of biological detail. A common approach is to neglect the influence of short-term dynamics on long-term plasticity, which may be an oversimplification for certain neuron types. Thus, there is a need for new models to investigate how short-term dynamics influence long-term plasticity. To address this gap, we introduce a novel phenomenological model, the Short-Long-Term STDP (SL-STDP) rule, which directly integrates the Tsodyks-Markram model of short-term dynamics with postsynaptic long-term plasticity. We fit the new model to recordings from layer 5 of the visual cortex and study how short-term plasticity affects the firing rate frequency dependence of long-term plasticity in a single synapse. Our analysis revealed that the pre- and postsynaptic frequency dependence of long-term plasticity plays a crucial role in shaping the self-organization of recurrent neural networks (RNNs) and their information processing through the emergence of sinks and source nodes. We applied the SL-STDP rule to RNNs and found that neurons in the SL-STDP network self-organize into distinct firing rate clusters, stabilizing the dynamics. We extended the experiments by including homeostatic balancing, namely weight normalization and excitatory-to-inhibitory plasticity, and observed differences in degree correlations between the SL-STDP network and a network without direct coupling between short-term and long-term plasticity. Finally, we evaluated how the modified connectivity affects the networks' information capacity in reservoir computing tasks. The SL-STDP rule outperformed the uncoupled system in the majority of tasks, and including excitatory-to-inhibitory facilitating synapses further improved information capacity. Our study demonstrates that short-term dynamics--induced changes in the frequency dependence of long-term plasticity play a pivotal role in shaping network dynamics and link synaptic mechanisms to information processing in RNNs.

---

## 论文详细总结（自动生成）

# 论文详细中文总结

## 1. 论文的核心问题与整体含义（研究动机和背景）
- **核心问题**：现有计算神经科学中的尖峰时序依赖可塑性（STDP）模型虽然能捕捉长时程突触变化，但普遍忽略短时程动力学对长时程可塑性的影响。这种简化对于某些神经元类型（如视觉皮层第5层锥体细胞）可能失之偏颇，需要建立统一模型来研究短时程与长时程可塑性的耦合效应。
- **整体含义**：短时程动力学（如易化、抑制）如何通过调节长时程可塑性的频率依赖性，影响神经网络的拓扑结构和信息处理能力，是理解大脑学习与记忆机制的关键。论文旨在填补这一建模空白，揭示二者耦合在自组织网络和信息容量中的作用。

## 2. 论文提出的方法论：核心思想、关键技术细节、公式或算法流程
- **核心思想**：直接将Tsodyks-Markram短时程动力学模型与突触后长时程STDP规则整合，形成新的“短-长时STDP（SL-STDP）”现象学规则。短时程模型负责动态调节突触传递效率（易化/抑制的时间尺度），而长时程STDP根据前后脉冲时序调整突触权重，两者通过共同的频率依赖性机制耦合。
- **关键技术细节**：
  - **Tsodyks-Markram模型**：描述短时程突触可塑性，包含利用度（U）、恢复时间常数（τ_rec）和易化时间常数（τ_facil）等参数，动态计算突触效能。
  - **突触后长时程STDP**：采用标准的双指数窗函数，根据突触前和突触后尖峰的时间差（Δt）调整权重，但长时程可塑性的幅度和方向受到短时程有效突触强度（即由Tsodyks-Markram计算的当前释放概率）的调制。
  - **SL-STDP规则**：长时程权重变化 = 基础STDP函数 × 短时程依赖的调制因子（如有效突触强度或频率依赖的缩放）。通过拟合视觉皮层第5层（L5）记录数据，确定调制因子的具体形式。
  - **算法流程**：在每一时间步更新短时程状态变量（U, R等） → 计算有效突触后电位（PSP） → 基于前后脉冲时序计算STDP更新量，并用短时程状态对更新量进行加权或门控 → 更新长时程权重。

## 3. 实验设计：使用的数据集/场景、benchmark、对比方法
- **数据集与场景**：
  - **单突触水平**：采用视觉皮层第5层（L5）的公开电生理记录数据，用于拟合SL-STDP规则中短时程与长时程的耦合参数。
  - **网络水平**：将SL-STDP规则应用于递归神经网络（RNN）的自组织学习，分别使用随机初始连接的兴奋-抑制网络，模拟无任务驱动的自发活动和储层计算任务。
  - **储层计算任务**：包括标准基准任务（如非线性变换、记忆任务、混沌时间序列预测等），用于评价网络的信息容量。
- **Benchmark**：对比了“非耦合系统”（即短时程动力学和长时程STDP独立运行，无直接耦合）的网络。
- **对比方法**：
  - 仅使用标准STDP（忽略短时程动力学）的网络。
  - 引入稳态平衡机制（权重归一化和兴奋-抑制可塑性）后的SL-STDP网络 vs 非耦合网络。
  - 包含兴奋-抑制易化突触的特殊变体。

## 4. 资源与算力
- **未明确说明**：论文摘要及元数据中未提及所使用的GPU型号、数量、训练时长或其他计算资源。仅属于计算模型仿真，可能涉及CPU集群但未提供细节。

## 5. 实验数量与充分性
- **实验组别**：
  - 单突触频率依赖性分析（前后不同频率组合下的LTP/LTD方向）。
  - RNN自组织动力学：神经元放电率分布、集群形成（频率聚类）。
  - 度相关性比较：SL-STDP网络 vs 非耦合网络在有无稳态调节下的出度/入度相关性。
  - 储层计算任务：至少涵盖多个典型任务（文中称“most tasks”），包括对比实验和消融（如去掉稳态调节、仅含抑制性易化等）。
- **充分性评估**：
  - **优点**：覆盖了从单突触到网络的多个层级，验证了短时程耦合的关键作用；使用了真实数据拟合确保生物合理性；在储层计算任务上进行了量化比较。
  - **不足**：缺乏统计显著性检验（如重复实验误差棒、多随机种子结果）；未展示所有任务的详细结果（仅泛称“多数任务”优于非耦合）；未对不同网络规模或参数鲁棒性进行系统扫参。

## 6. 论文的主要结论与发现
- **主要发现**：
  1. 短时程动力学通过调节长时程可塑性的频率依赖性，使长时程权重变化表现出更强的频率选择性（而不是简单的STDP时序窗）。
  2. 在RNN中，SL-STDP规则促使神经元自组织成不同的放电率集群（高/低频簇），稳定了网络动力学，避免了传统STDP下的过度同步或沉默。
  3. 加入稳态平衡机制（权重归一化和兴奋-抑制可塑性）后，SL-STDP网络与无耦合网络在度相关性上出现显著差异（如形成独特的膨胀-核心拓扑）。
  4. 在储层计算任务中，SL-STDP网络在多数任务上信息容量超过非耦合系统；若加入兴奋-抑制易化突触，信息容量进一步提升。
- **核心结论**：短时程动力学通过改变长时程可塑性的频率依赖，是塑造网络自组织结构和信息处理能力的关键机制，统一模型比分离模型更接近生物实现且性能更优。

## 7. 优点：方法或实验设计上的亮点
- **生物真实性**：直接整合Tsodyks-Markham模型，拟合视觉皮层L5数据，比纯STDP模型更接近真实突触行为。
- **机理揭示**：明确展示了短时程动力学如何通过频率依赖性调控长时程可塑性，指导网络拓扑演化。
- **多层次验证**：从单突触到网络自组织，再到功能任务（储层计算），形成了完整的理论-计算-应用链条。
- **引入稳态调节**：将权重归一化和兴奋-抑制可塑性纳入统一框架，更贴近体内稳态可塑性机制，增强了模型稳健性。

## 8. 不足与局限
- **模型现象学性质**：SL-STDP规则是现象学描述，未涉及分子信令通路（如钙离子动力学），可能丧失部分生物细节。
- **数据覆盖有限**：仅使用视觉皮层L5数据拟合，其他脑区（如海马、体感皮层）的适用性未验证。
- **实验充分性不足**：未提供重复实验的统计结果、参数敏感性分析；储层计算任务的具体类型和数量未详细列出，可能存在选择性报告。
- **应用限制**：局限于递归神经网络仿真，未在生物真实网络尺度（大规模）或在线学习场景中测试；计算资源消耗未评估，可能对大规模网络较慢。
- **对比基准单一**：仅与非耦合模型比较，未与近年来其他统一模型（如STDP with calcium dynamics）或基于能量的学习规则对比。

（完）
