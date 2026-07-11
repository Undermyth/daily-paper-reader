---
title: A unified theory of context-conditioned efficient and predictive coding
title_zh: 上下文条件化的高效与预测编码的统一理论
authors: "Tavoni, G."
date: 2026-07-06
pdf: "https://www.biorxiv.org/content/10.1101/2025.02.24.639817v2.full.pdf"
tags: ["query:comp-neuro"]
score: 8.0
evidence: 上下文依赖神经表征的高效与预测编码统一理论
tldr: 感官处理依赖行为与多模态上下文，但缺乏统一理论。本文通过数学推导证明，上下文条件的高效编码等价于预测编码：上下文信号提供输入期望，局部神经元编码预期偏差，递归连接白化残差信号。该理论统一解释了跨模态抑制、多模态感受野等现象，并恢复经典单模态编码结果，为理解分布式系统中上下文如何塑造局部表征提供了原则性框架。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-02-24-639817-v2/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1198, \"height\": 1457, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-02-24-639817-v2/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1358, \"height\": 1303, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-02-24-639817-v2/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1431, \"height\": 1571, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-02-24-639817-v2/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1493, \"height\": 977, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-02-24-639817-v2/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1657, \"height\": 1220, \"label\": \"Figure\"}]"
motivation: 现有理论未揭示多模态上下文如何优化局部感官表征，缺乏统一框架。
method: 通过数学分析建立上下文条件高效编码与预测编码的等价性，推导出可解释的神经算法。
result: 上下文提供期望，局部编码偏差，递归白化残差，高效压缩同时产生预测计算。
conclusion: 理论统一了跨模态抑制等多样现象，为分布式神经系统的上下文依赖编码提供基础。
---

## 摘要
感觉处理并非孤立进行：在特定感觉模态中，神经元所表征的内容会受到来自其他感官、动作及行为背景信号的塑造。这种背景依赖性为神经编码理论提出了一个基本问题：神经回路如何能够在高效编码局部输入的同时，利用大脑其他部位可用的信息？在此，我们发展了一个高效编码与预测编码的统一理论，展示了多模态背景信息如何优化局部感觉回路内的表征。我们通过解析证明，高效编码解可映射为一个可解释的神经算法：背景信号为局部回路提供关于感觉输入的预期，局部神经元编码与这些预期的偏差，而递归交互则对残差信号进行白化。这一结果建立了上下文条件化的高效编码与预测编码之间的数学等价性，揭示了预测计算可以从由背景引导的高效输入压缩中涌现。由此产生的框架既区别于单一模态内的经典冗余减少，也不同于层次贝叶斯推理。该理论解释并统一了多样的实验现象，包括对预测输入的跨模态抑制反应，以及跨感觉运动、视听、视觉-嗅觉和听觉-体感回路的多模态感受野，同时将经典的单模态编码效应恢复为极限情况。通过将编码目标、回路机制与实验观察到的现象联系在单一分析框架内，本研究为理解分布式神经系统如何利用背景来塑造局部表征提供了原理性基础。

## Abstract
Sensory processing does not occur in isolation: what neurons represent in a given sensory modality is shaped by signals from other senses, actions, and behavioral context. This context dependence raises a fundamental question for theories of neural coding: how can circuits efficiently encode their local input while using information available elsewhere in the brain? Here we develop a unified theory of efficient and predictive coding that shows how multimodal contextual information can optimize representations within a local sensory circuit. We demonstrate analytically that the efficient-coding solution maps onto an interpretable neural algorithm: contextual signals provide expectations about the sensory input to the local circuit, local neurons encode deviations from those expectations, and recurrent interactions whiten the residual signals. This result establishes a mathematical equivalence between context-conditioned efficient coding and predictive coding, revealing that predictive computations can emerge from efficient input compression guided by context. The resulting framework is distinct from both classical redundancy reduction within a single modality and hierarchical Bayesian inference. The theory explains and unifies diverse experimental phenomena, including cross-modal suppression of responses to predicted inputs and multimodal receptive fields across sensorimotor, audiovisual, visual-olfactory, and auditory-somatosensory circuits, while recovering classical unimodal coding effects as limiting cases. By linking coding objectives, circuit mechanisms, and experimentally observed phenomena within a single analytical framework, this work provides a principled foundation for understanding how distributed neural systems use context to shape local representations.

---

## 论文详细总结（自动生成）

# 论文详细中文总结

## 1. 核心问题与整体含义（研究动机与背景）

- **核心问题**：感觉处理并非孤立进行，神经元在特定感觉模态中的表征会受到来自其他感官、运动和行为背景信号的塑造。然而，现有理论（如高效编码和预测编码）大多局限于单一模态或层次贝叶斯推理，未能统一解释多模态上下文如何优化局部感觉表征。
- **研究动机**：作者试图回答一个根本性问题——神经回路如何能在高效编码局部输入的同时，利用大脑其他部位可用的上下文信息？现有实验现象（如跨模态抑制、多模态感受野）缺乏统一的规范性解释。
- **整体含义**：本文提出并证明了一个**上下文条件化的高效编码与预测编码的统一理论**，揭示预测计算可以从高效输入压缩中涌现，为理解分布式神经系统如何利用上下文塑造局部表征提供了原理性基础。

## 2. 方法论：核心思想与关键技术细节

- **核心思想**：将高效编码框架推广到多模态场景。局部感觉回路（E-I网络）接收局部输入 **s** 和来自其他模态或运动系统的上下文信号 **k**。编码目标是在最大化响应熵（信息）的同时最小化反应幅度的平方和（能量代价）。
- **数学模型**：
  - 定义多模态输入 **I = (s, k)**，多模态响应 **R = (e, k)**，其中 **e** 是兴奋性神经元响应。
  - 效率函数 **E = h(R) - γ Σ_i ⟨R_i²⟩**，等价于条件熵 **h(e|k) - γ Σ_i ⟨e_i²⟩**（在低噪声有限精度下）。
  - 在输入服从高斯分布的近似下，利用拉格朗日乘子法最大化 **E**，得到最优有效连接：
    - 反馈连接 **F₀ = C_{SK} C_K^{-1}**，实现从上下文 **k** 对局部输入 **s** 的最优线性预测 **ŝ = F₀ k**。
    - 侧向连接 **L₀ = √(2γ) (C_S - C_{SK} C_K^{-1} C_{SK}^T)^{1/2} - 1**，实现残差信号的去相关和缩放（白化）。
  - 最终响应公式：**e₀ = (1 + L₀)^{-1} (s - F₀ k) = (1/√(2γ)) P^{1/2} (s - ŝ)**，其中 **P** 是精度矩阵。
- **算法解释**：
  - 上下文信号提供对局部输入的期望预测。
  - 局部神经元编码预测误差（输入减去预测）。
  - 递归侧向连接（通过抑制性中间神经元实现）对残差信号进行白化，消除冗余。
- **与经典预测编码的区别**：上下文信号是外部提供的条件变量，而非内部推理的隐变量；不要求双向迭代更新，适用于非对称的跨模态交互。

## 3. 实验设计

- **数据集/场景**：论文未使用真实实验数据集，而是通过**数值模拟**复现了多个经典实验现象：
  - 视听实验（Garner & Keller, 2022）：检测小鼠V1对听觉提示视觉刺激的抑制。
  - 听觉-运动实验（Schneider et al., 2018; Audette et al., 2022）：小鼠听觉皮层对运动产生声音的预期抑制。
  - 视觉-嗅觉实验（Mandairon et al., 2014）：嗅球颗粒细胞对配对气味与视觉背景的选择性反应。
  - 单模态实验：习惯化、新颖性偏好、模式分离、范围适应。
- **Benchmark**：理论预测与上述已发表实验数据直接对比（定性趋势及统计显著性标定）。
- **对比方法**：论文未对比其他模型，而是与自身理论的极限情况（无反馈的单模态情形）进行对比，并展示了理论对不同参数（如上下文关联强度、输入频率等）的预测变化。

## 4. 资源与算力

- **未明确说明**：文中没有提及使用的GPU型号、数量、训练时长等具体算力信息。所有数值模拟均基于数学求解（闭式解），计算开销较小，在普通工作站或高性能CPU上即可完成（一次模拟涉及100个神经元、1000-50000个观测样本）。

## 5. 实验数量与充分性

- **实验数量**：
  - 核心数值实验约**5组**（对应图3～图5），每组包含多个子条件（如不同刺激类型、不同训练天数、不同上下文相关性）。
  - 额外进行了**20000次随机Hessian矩阵检验**验证最优解的唯一性（所有特征值为负）。
  - 进行了**参数敏感性分析**（如改变γ、输入频率、上下文强度等），结果稳健。
- **充分性与公平性**：
  - 实验覆盖了主流的跨模态和运动感觉交互现象，以及经典的单模态效应，范围较广。
  - 数值模拟的输入参数（如神经元数量、激活比例、频率等）依据实验文献设置，并进行了随机重复（如50～10000次），统计结果可靠。
  - 论文未与其他理论模型直接比较，可能削弱了公平性对比，但因其目的是提出统一理论框架，而非模型竞赛，此做法可以理解。

## 6. 主要结论与发现

- **高效编码与预测编码等价**：在上下文条件下，最大化信息效率等价于编码预测误差并进行白化。
- **统一解释多模态现象**：视听抑制、运动感觉抑制、选择性嗅觉颗粒细胞等活动均可从该原理推导。
- **恢复经典单模态编码**：无上下文反馈时，理论自然退化为范围适应、习惯化、模式分离等。
- **新预测**：提出“逆有效性”现象——当单模态表征分辨力低时，上下文反馈对模式分离的增益最大；上下文增强新异刺激选择性等可验证预测。

## 7. 优点

- **理论创新**：首次将高效编码与预测编码在多模态背景下统一，并给出闭式解和显式算法映射。
- **可解释性**：电路中每个组件（上下文→预测，E细胞→预测误差，I细胞+侧向连接→白化）功能清晰，便于对接实验。
- **广泛解释力**：对多个模式（视听、体感、运动）和多层次（单模态、多模态）给出统一的规范性解释。
- **生成新预测**：提出可实验验证的逆有效性、上下文依赖性模式分离等新假设。

## 8. 不足与局限

- **假设简化**：线性响应、高斯输入分布、L2代价、高信噪比等假设不严格符合生物现实。虽然作者论证了原理的通用性，但未提供非线性、非高斯、有噪声情况下的严格推导。
- **实验覆盖有限**：主要复现了少数几个特定实验，未覆盖更广泛的跨模态现象（如听觉-视觉在行为中的竞争、注意调节等）；也未与现有其他预测编码模型（如自由能原理）进行定量比较。
- **实验公平性**：由于未公开代码，难以验证数值结果的可复现性；且没有与其他理论模型的模拟直接对比（如仅与自身无反馈情况对比）。
- **应用限制**：当前框架假设上下文信号是固定统计的，未考虑在线学习或动态变化；忽略神经噪声和随机性可能对编码的影响；未扩展到任务导向的优化目标。

（完）
