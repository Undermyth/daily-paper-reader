---
title: A geometric and dynamical theory of latent computations in biological neural networks
title_zh: 生物神经网络中潜在计算的几何与动力学理论
authors: "Dinc, F., Blanco-Pozo, M., Klindt, D., Acosta, F., Sylber, C., Jiang, Y., Ebrahimi, S., Shai, A., Tanaka, H., Yuan, P., Miolane, N., Schnitzer, M. J."
date: 2026-07-15
pdf: "https://www.biorxiv.org/content/10.64898/2026.07.10.737763v1.full.pdf"
tags: ["query:comp-neuro"]
score: 8.0
evidence: 生物神经网络中潜在计算的几何与动力理论
tldr: 神经记录揭示低维行为变量，但降维无法解释网络稳定计算。本文提出架构无关的潜在处理单元（LPU）概念，并建立六个定理。定理表明低维编码变量可生成高维神经动力学；许多神经元虽表征行为变量但对下游影响微弱；线性读出可实现近最优解码；神经表征漂移但计算保持完整。LPU理论统一了几何与动力学视角，为大脑可靠计算提供因果解释。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-10-737763-v1/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1654, \"height\": 1615, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-10-737763-v1/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1699, \"height\": 972, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-10-737763-v1/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1405, \"height\": 1280, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-10-737763-v1/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1685, \"height\": 744, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-10-737763-v1/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1709, \"height\": 1494, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-10-737763-v1/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1753, \"height\": 1760, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-10-737763-v1/fig-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 1489, \"height\": 1022, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-10-737763-v1/fig-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 1731, \"height\": 2018, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-10-737763-v1/fig-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 1725, \"height\": 851, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-10-737763-v1/fig-010.webp\", \"caption\": \"\", \"page\": 0, \"index\": 10, \"width\": 1747, \"height\": 909, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-10-737763-v1/fig-011.webp\", \"caption\": \"\", \"page\": 0, \"index\": 11, \"width\": 1507, \"height\": 514, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-10-737763-v1/fig-012.webp\", \"caption\": \"\", \"page\": 0, \"index\": 12, \"width\": 1751, \"height\": 1381, \"label\": \"Figure\"}]"
tables_json: "[{\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-07-10-737763-v1/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 2036, \"height\": 2104, \"label\": \"Table\"}, {\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-07-10-737763-v1/table-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1771, \"height\": 512, \"label\": \"Table\"}]"
motivation: 解释生物神经网络如何在高维噪声下实现稳定的低维计算，弥补降维分析因果解释的不足。
method: 提出潜在处理单元（LPU）概念，基于六个定理构建描述低维计算与高维动力学的理论框架。
result: 六个定理揭示了低维编码生成高维动力学、神经元活动与下游影响分离、线性读出近最优、表征漂移但计算不变等关键规律。
conclusion: LPU理论统一神经网络计算的几何与动力学观点，为系统神经科学提供了计算稳定性的因果机制。
---

## 摘要
许多神经记录揭示了在大规模神经活动模式中编码的行为相关变量的低维集合。然而，仅靠降维分析无法为网络如何稳定地执行对单神经元动力学显著变异具有鲁棒性的计算提供因果解释。此外，现有的降维方法通常依赖于关于网络结构的简化假设，这限制了它们的适用性和解释力。为了提供一个描述高维神经网络中低维计算动力学的理论框架，我们在此引入潜在处理单元（LPU）的概念，这是一种在生物神经回路中运行的与架构无关的计算元素。关于LPU编码和计算的六个定理共同为一系列常见的生物学发现提供了解释：低维编码变量集可以生成高维神经动力学；许多神经元的活动模式代表行为相关变量，但对下游回路影响甚微；神经群体活动的线性读出通常允许接近最优的解码；即使网络计算保持完整，神经表征的漂移也往往很大。总体而言，我们对LPU（在网络动力学中实现）的处理将神经计算的几何视角和动力学视角统一在一个联合框架下，并为系统神经科学提供了大脑如何执行可靠计算的因果解释。

## Abstract
Many neural recordings have revealed low-dimensional sets of behaviorally relevant variables encoded within large-scale neural activity patterns. However, dimensionality reduction analyses alone cannot yield causal explanations for how networks stably implement computations that are resilient to the substantial variability of single neuron dynamics. Further, existing methods for dimensionality reduction often rely on simplifying assumptions about network structure that limit their applicability and explanatory power. To provide a theoretical framework describing the dynamics of low-dimensional computation in high-dimensional neural networks, here we introduce the concept of latent processing units (LPUs), which are architecture-agnostic computational elements operating within biological neural circuitry. Six theorems governing coding and computation by LPUs collectively provide explanations for a range of common biological findings: low-dimensional sets of coding variables can generate high-dimensional neural dynamics; many neurons have activity patterns that represent behaviorally relevant variables but exert little influence on downstream circuits; linear readouts of neural population activity commonly permit near-optimal decoding; the drift of neural representations is often substantial even while network computations remain intact. Overall, our treatment of LPUs, as enacted in network dynamics, unifies the geometric and dynamical views of neural computation under a joint framework and provides systems neuroscience with a causal account of how the brain executes reliable computations.

---

## 论文详细总结（自动生成）

以下是根据论文《A geometric and dynamical theory of latent computations in biological neural networks》生成的详细中文总结。

## 1. 论文的核心问题与整体含义（研究动机和背景）

- **核心问题**：生物神经网络由大量噪声、异质的神经元组成，却能集体、稳定地执行复杂的计算。然而，单个神经元的调谐特性会随时间发生“表征漂移”，而整体编码和行为输出却保持稳定。过去的第一代降维方法（如PCA）只提供了几何描述，缺乏因果机制；第二代动力学方法（如低秩RNN、rSLDS）依赖过强的线性假设，无法解释高维神经活动、非线性调谐、冗余编码和漂移鲁棒性等现象。
- **整体含义**：本文提出**潜在处理单元（Latent Processing Unit, LPU）** 的概念，将低维潜在动力学与高维神经活动统一在编码-嵌入框架下，并通过六个数学定理解释了上述看似矛盾的生物学发现，为系统神经科学提供了因果性的理论基石。

## 2. 论文提出的方法论

### 核心思想
- **LPU** 是架构无关的计算单元，由四个基本原则（P1-P4）定义：
  - **P1（线性编码）**：潜在变量 $\boldsymbol{\kappa}(t) = \boldsymbol{N}\boldsymbol{r}(t)$，即神经活动的线性组合。
  - **P2（非线性嵌入）**：神经动力学 $\tau\dot{\boldsymbol{r}} = -\boldsymbol{r} + \boldsymbol{\varphi}(\boldsymbol{\kappa}(t), \boldsymbol{u}(t))$，嵌入函数 $\boldsymbol{\varphi}$ 是非线性的。
  - **P3（低维潜在动力学）**：行为相关的计算由低维潜在向量场 $\dot{\boldsymbol{\kappa}} = \boldsymbol{G}(\boldsymbol{\kappa}, \boldsymbol{u})$ 驱动。
  - **P4（生物学实现）**：嵌入和编码权重通过低秩突触连接 $\boldsymbol{W} \approx \boldsymbol{M}\boldsymbol{N}$ 实现，即突触权重由嵌入矩阵 $\boldsymbol{M}$ 和编码矩阵 $\boldsymbol{N}$ 的乘积近似。

### 关键技术细节
- **六个定理**：
  1. **Theorem 1（通用计算）**：在足够大的网络中，LPU 可以任意逼近任意连续 $K$ 维向量场。
  2. **Theorem 2（跨时间尺度计算）**：LPU 可支持远长于神经时间常数的计算，但所需神经元数量随时间尺度分离度 $\beta$ 平方增长，误差 $O(\beta^2/N)$。
  3. **Theorem 3（线性读出最优性）**：在 $N\to\infty$ 时，任何可微潜在函数均可由线性读出从神经活动中逼近，无需显式识别潜在变量。
  4. **Theorem 4（神经流形）**：当潜在动力学比神经动力学慢得多时，神经活动近似位于低维流形上，但流形的外在维度可达 $N$（由非线性嵌入引起）。
  5. **Theorem 5（无因果影响的编码）**：只要扰动方向正交于因果编码子空间（由 $\boldsymbol{N}$ 的行空间张成），即使扰动在调谐方向上，也不会改变 LPU 动力学，偏差指数衰减。
  6. **Theorem 6（表征漂移鲁棒性）**：当嵌入权重的改变是随机的或正交于因果编码维度时，潜在动力学保持一阶不变（误差 $O(\|\Delta\boldsymbol{m}\|_2^2/N^2)$）。

- **公式流程**：从神经动力学方程出发，通过低秩分解得到潜在变量，推导出自洽的潜在动力学。定理 1 证明了通用逼近性，定理 2 给出了有限尺度下的误差缩放，定理 3 建立了线性读出的最优性，定理 4-6 分别解释了高维外在维度、因果与非因果编码、漂移鲁棒性。

## 3. 实验设计

### 使用的数据集/场景
- **合成任务**：
  - $K$位翻转触发器（flip-flop）任务（图1、6）。
  - 双稳态动力系统（图2）。
  - 延迟加法任务（图5）。
  - 序列排序任务（图4）。
  - 随机连接的低秩混沌RNN（图S5）。
- **真实神经数据**：从已发表数据集（Ebrahimi et al., Nature 2022）中重新分析的小鼠皮层大尺度钙成像记录，涉及8个皮层区域（V1, LV, MV, PPC, A, S, M, RSC），每个小鼠记录约3595个神经元，共6只小鼠30个成像会话。

### 基准与对比方法
- **对比线性 vs. 非线性解码器**：逻辑回归/LDA vs. 随机森林/QDA，在不同维度瓶颈下评估正确/错误试验分类准确率（图3、S2）。
- **扰动实验**：对比沿编码方向、读出方向、嵌入方向、随机方向等的扰动效果（图5）。
- **漂移类型对比**：完全随机漂移 vs. 正交于因果编码的漂移 vs. 切向于因果编码的漂移（图6）。

## 4. 资源与算力

- **文中未明确说明**训练所使用的GPU型号、数量及训练时长。仅提到训练RNN时使用了Adam优化器、学习率调度、梯度裁剪等标准技术，并提及“训练了51个rank-1 RNNs”等。对于大尺度仿真（如1,000,000神经元网络），未给出具体硬件资源。因此，**无法获知确切的计算资源细节**。

## 5. 实验数量与充分性

- **实验覆盖面**：
  - 多种任务（翻转触发器、延迟加法、序列排序、双稳态、混沌网络）。
  - 多种网络架构（基本RNN、增益调制RNN、低秩RNN、全秩RNN）。
  - 多种漂移类型和扰动方向。
  - 神经元数量从几百到百万级别。
  - 真实数据包含6只小鼠、30个会话、多个脑区、不同任务时期。
- **重复性**：大部分仿真结果基于多随机种子、多网络实例（如50个网络、10次重复等），并报告均值与标准差。
- **公平性**：对比方法（线性 vs. 非线性解码器）在相同的数据划分和维度缩减下进行；扰动实验严格保持扰动幅度一致。
- **充分性**：理论结果（六个定理）均有配套数值实验支撑，实验设计考虑了静态嵌入、动态训练、随机初始化和噪声注入等多种情况，较全面地验证了理论预测。但缺乏对真实神经数据中LPU因果编码子空间的直接验证（文中提到需要新一代单细胞调控工具）。

## 6. 论文的主要结论与发现

1. **通用计算能力**：LPU 可在生物合理网络中实现任意连续潜在动力学。
2. **长时计算需要大网络**：维持秒级时间尺度的计算需要百万级神经元，否则误差会毁坏动力学稳定性。
3. **线性读出最优**：在足够大的网络中，线性解码器可以逼近任意可微潜在变量的函数，解释了为什么大脑使用简单的线性通信子空间。
4. **高维神经活动源于非线性嵌入**：即使潜在维度很低，非线性嵌入也能产生外在的高维线性维度，这解释了近期大规模记录中的高维方差谱。
5. **因果编码分离**：神经元的调谐不一定代表其对下游的因果影响；只有具有编码权重的神经元才对LPU动力学有持续影响。
6. **漂移鲁棒性源于编码子空间**：随机或正交于编码方向的漂移几乎不影响潜在动力学，而切向漂移则会破坏计算；增加网络规模可以增强鲁棒性。

## 7. 优点

- **理论框架统一**：首次将几何与动力学视角统一在一个编码-嵌入框架下，并提供了六个可验证的定理。
- **生物合理性**：LPU 基于线性编码和非线性嵌入，符合现实神经元的线性-非线性性质，支持树突计算。
- **解释范了围广泛**：同时解释了低维编码、高维活动、冗余神经元、线性解码最优性、表征漂移、量子扰动敏感性等关键实验现象。
- **实验可检验**：每个定理都产生了明确的、可实验验证的预测（例如，有效扰动应限于低维线性子空间、神经流形应是弯曲的等）。
- **对比全面**：在多个任务、多种网络规模、多种扰动/漂移类型下进行了系统性测试。

## 8. 不足与局限

- **实验覆盖缺失**：
  - 缺乏对真实生物网络中因果编码子空间的直接实验验证（需要新工具）。
  - 未将LPU框架扩展到脉冲神经网络（SNN）或更复杂的生物细节（如抑制性神经元、突触可塑性）。
- **应用限制**：
  - 理论主要考虑弱标度（权重 $O(1/N)$），未覆盖混沌标准标度（权重 $O(1/\sqrt{N})$）。
  - 对漂移源头的建模抽象（仅改变嵌入权重），未深入生物学习规则。
  - 部分观察下重构LPU的困难：除非记录几乎所有神经元，否则潜在动力学和因果子空间难以准确估计。
- **偏差风险**：
  - 所有仿真均基于监督训练（BPTT），不保证生物可实现。
  - 解码分析仅涉及正确试验，未考虑错误试验的完整解码表现。
- **算力与可重复性**：未提供训练资源细节，可能影响可复现性。

（完）
