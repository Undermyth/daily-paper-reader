---
title: "BraiNN: A Modern Simulator for Clinically Feasible Personalized Whole-Brain Network Modeling"
title_zh: "BraiNN: 一种面向临床可行性个性化全脑网络建模的现代模拟器"
authors: "Fasse, A., Billi, C., Garvalov, V., Morvan, M., Newton, T., Kuster, N., Neufeld, E."
date: 2026-07-13
pdf: "https://www.biorxiv.org/content/10.64898/2026.07.08.737156v1.full.pdf"
tags: ["query:comp-neuro"]
score: 9.0
evidence: 用于临床的全脑网络模拟器
tldr: 个性化全脑网络建模需要快速拟合患者数据，但现有神经质量模型框架计算缓慢。BraiNN利用JAX和GPU加速，结合区域Jansen-Rit网络与皮层网格，实现EEG正向建模。在单消费级GPU上约2-3小时完成八维参数空间拟合，速度提升2-3个数量级，且准确复现标准动力学。该工具将高细节全脑模型个性化从数天缩短至数小时，为临床数字孪生和神经调控规划奠定基础。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-08-737156-v1/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 891, \"height\": 571}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-08-737156-v1/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1664, \"height\": 907}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-08-737156-v1/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 894, \"height\": 534}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-08-737156-v1/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 904, \"height\": 517}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-08-737156-v1/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 901, \"height\": 518}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-08-737156-v1/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 901, \"height\": 518}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-08-737156-v1/fig-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 896, \"height\": 518}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-08-737156-v1/fig-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 1842, \"height\": 915}]"
tables_json: "[{\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-07-08-737156-v1/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 867, \"height\": 556}, {\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-07-08-737156-v1/table-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 898, \"height\": 297}]"
motivation: 现有神经质量模型框架无法在临床相关时间内实现高分辨率全脑网络个性化拟合。
method: 基于JAX构建可微分计算图，利用GPU/TPU加速和XLA编译，结合区域网络、皮层网格和互易性EEG正演，采用贝叶斯优化与梯度优化混合策略。
result: 在单GPU上2-3小时完成8维参数空间谱拟合，速度比传统工具快2-3个数量级，数值验证复现Jansen-Rit网络动力学。
conclusion: BraiNN将高细节全脑表面模型个性化时间从数天降至数小时，使临床可行的个性化脑网络建模成为可能。
---

## 摘要
个性化全脑建模旨在通过实现患者特异性的脑网络动力学模拟，来革新神经系统疾病的治疗规划。神经质量模型（NMM）在生物物理细节与计算成本之间提供了易于处理的折衷，并可直接与脑电图（EEG）等宏观观测指标关联。然而，将NMM扩展到具有真实连接、传导延迟和皮层表面分辨率的全脑网络，并将其拟合到个体患者数据上，所施加的计算需求是现有框架在临床相关时间尺度上无法满足的。在此，我们介绍BraiNN，一个基于JAX的Python框架，用于大规模神经质量建模，通过利用GPU/TPU加速和XLA编译的数组计算，相比现有工具实现了高达两到三个数量级的加速。BraiNN将区域级Jansen-Rit网络与受试者特异性的耦合神经质量模型皮层表面网格以及基于互易性导联场的生物物理基础EEG正演建模相结合。其完全可微的计算图支持一种混合个性化流程，将用于全局参数探索的贝叶斯优化与基于梯度的精化相结合，在单个消费级GPU上约2-3小时内完成八维参数空间的EEG驱动频谱拟合——而传统神经质量建模软件则需要数天时间。针对已建立基准的数值验证确认BraiNN能够忠实再现Jansen-Rit网络的典型同步和分岔动力学。

通过将高细节全脑表面模型个性化的时间需求从数天减少到消费级硬件上的数小时，BraiNN使个性化脑网络建模更接近临床实际应用。我们预期BraiNN将作为患者特异性数字孪生和EEG引导神经调控规划的基础。

## Abstract
Personalized whole-brain modeling aims to transform treatment planning for neurological disorders by enabling patient-specific simulations of brain network dynamics. Neural mass models (NMMs) offer a tractable compromise between biophysical detail and computational cost and can be directly linked to macroscopic observables such as EEG. However, scaling NMMs to whole-brain networks with realistic connectivity, conduction delays, and cortical surface resolution--and fitting them to individual patient data--imposes computational demands that existing frameworks cannot meet at clinically relevant timescales. Here we introduce BraiNN, a JAX-based Python framework for large-scale neural mass modeling that achieves speedups of up to two to three orders of magnitude over existing tools by leveraging GPU/TPU-accelerated, XLA-compiled array computation. BraiNN combines a region-level Jansen-Rit network with a subject-specific cortical surface mesh of coupled neural mass models and biophysically grounded EEG forward modeling via reciprocity-based lead fields. Its fully differentiable computational graph enables a hybrid personalization pipeline that pairs Bayesian optimization for global parameter exploration with gradient-based refinement, completing EEG-driven spectral fitting of an eight-dimensional parameter space in approximately 2-3 hours on a single consumer GPU--compared to multiple days with conventional neural mass modeling software. Numerical verification against established benchmarks confirms that BraiNN faithfully reproduces canonical synchronization and bifurcation dynamics of Jansen-Rit networks.

By reducing the time requirements for personalizing a high-detail whole-brain surface model from days to a few hours on consumer-grade hardware, BraiNN brings personalized brain network modeling closer to practical use in clinical contexts. We anticipate that BraiNN will serve as a foundation for patient-specific digital twins and EEG-guided neuromodulation planning.

---

## 论文详细总结（自动生成）

# 论文详细总结

## 1. 核心问题与整体含义（研究动机和背景）

- **问题**：个性化全脑网络建模能通过患者仿真优化神经调控治疗，但现有神经质量模型（NMM）框架（如TVB）在扩展到高分辨率皮层表面、真实连接延迟时，计算成本极高，无法在临床时间窗口（数小时至数天）内完成模型拟合。
- **含义**：需要一种兼顾生物物理精度与计算效率的模拟器，使个性化数字孪生和EEG引导的神经调控规划成为临床可行方案。

## 2. 方法论：核心思想、关键技术细节

- **核心思想**：利用现代AI硬件加速和可微分编程，将NMM模拟转化为GPU/TPU友好的张量计算，并构建完全可微的计算图，支持混合优化。
- **模型架构**：
  - **神经质量模型**：采用标准Jansen–Rit模型（6维状态变量，包含突触动力学和Sigmoid非线性，式1）。
  - **两尺度全脑网络**：
    - **区域级**：每个ROI为一个Jansen–Rit节点，通过结构连接矩阵和延迟矩阵耦合（式2）。
    - **表面级**：每个皮层网格顶点对应一个NMM，局部通过稀疏几何连接耦合，区域长程耦合由所属ROI的平均输出提供（式3-4）。
  - **EEG正演**：基于互易性定理预计算导联场矩阵，将皮层顶点偶极子源线性投影到头皮电极电压。
- **数值实现**：
  - 全部基于JAX，使用`lax.scan`编译完整积分循环，支持多种ODE/SDE求解器。
  - **延迟处理**：采用固定大小环形缓冲区存放耦合变量，避免时间序列移位，保持可微分。
  - **自动微分与优化**：整个仿真、特征提取、损失函数构成可微图，支持梯度下降（Adam等）和贝叶斯优化（高斯过程代理，多样采集函数）。
  - **混合个人化流程**：先用高斯过程贝叶斯优化进行全局探索，再用梯度优化局部精化，克服损失景观的噪声和非凸性。
- **关键公式**：Jansen–Rit动力学方程（式1）、区域耦合输入（式2）、表面耦合输入（式4）。

## 3. 实验设计

- **数据集/场景**：
  - **验证实验**：基于Kazemi & Jamali (2022)的合成网络同步研究，使用256×256参数网格（耦合强度与随机输入水平），128次重复，共约840万次仿真。
  - **性能基准**：使用来自Karimi et al. (2025)的结构连接组和延迟矩阵，改变ROI数（10–250）、表面顶点数（最高约19,000）、最大延迟（0–12.4 s）、批大小（1–32）。
  - **参数恢复实验**：合成数据，8维参数（A,a,B,b,p0,G,G_surf,λ_diff），基于PSD Wasserstein距离损失。
- **基准方法**：对比库包括TVB (tvb-root)、vbjax、cuBNM、brainmass，分别在不同硬件（CPU/GPU）上运行。
- **实验设计**：性能测试每个条件15个随机实例×5次重复；参数恢复实验10次独立初始化，各自250次优化迭代，比较BO与Adam。

## 4. 资源与算力

- **硬件**：AMD Ryzen Threadripper 3970X 32核CPU + 256 GB DDR4；NVIDIA GeForce RTX 3090 GPU。
- **时间**：
  - 单次区域级仿真（N=250）GPU约5.5 s，CPU约59 s。
  - 表面级4,392顶点仿真GPU约12.9 s；20,000顶点GPU约31.6 s。
  - 批处理32个并行仿真GPU约6.0 s。
  - 个人化总时间：BO约140 min ± 1.7 min，Adam约266 min ± 45 min（单GPU）。
- **资源结论**：全部实验在单消费级GPU上完成；最大表面模型约19,000节点，个性化可在2–3小时内完成。

## 5. 实验数量与充分性

- **数量**：验证实验覆盖840万仿真；性能基准覆盖4种参数维度（区域数、表面点数、延迟、批量），共约4×15×5=300次运行；参数恢复实验10次独立初始化，各250次迭代。
- **充分性**：
  - 验证实验复现了文献已知的同步图，确认动力学正确。
  - 性能基准全面，覆盖了主要可变维度，并与5个第三方库对比（TVB、vbjax、cuBNM、brainmass）。
  - 参数恢复实验对比了两种优化器，给出均值和标准差，统计显著。
- **公平性**：所有基准均使用相同积分参数、仿真时间；编译开销包含在测量中（保守）。但所有参数恢复仅使用合成数据，缺乏真实EEG验证。

## 6. 主要结论与发现

- BraiNN实现了2–3个数量级的加速（区域级GPU 215× over TVB，表面级79.5× over TVB）。
- 准确再现Jansen–Rit网络的同步与分岔动力学。
- 混合贝叶斯优化+梯度优化在8维参数空间稳定恢复目标PSD，而纯Adam陷入局部最优且变异大。
- 在单消费级GPU上约2–3小时完成全脑表面模型个性化，远低于传统数天时间，使临床可行性成为可能。
- 支持区域级、表面级、延迟耦合、随机噪声、EEG导联场、可微优化等全面功能。

## 7. 优点

- **性能与可扩展性**：基于JAX/XLA实现，GPU加速，编译为单核，线性或亚线性扩展。
- **功能丰富**：同时支持区域级和表面级仿真；内置延迟、噪声、EEG正演；提供多种优化器（BO、梯度法）；监控可稀疏采样。
- **生物物理保真度**：使用互易性导联场，基于有限元真实头模型；结构连接从DWI获取。
- **与AI生态集成**：完全可微分，可嵌入机器学习流程；代码开源（规划中）。
- **数值验证充分**：在大规模网格上复现文献结果，提供变异性分析。

## 8. 不足与局限

- **模型扩展性**：当前仅实现Jansen–Rit模型，虽宣称易扩展，但尚未展示其他NMM。
- **缺乏真实数据验证**：所有个人化实验基于同一类模型产生的合成数据，未在真实EEG/MEG数据、患者队列中验证。
- **目标函数局限**：仅使用静态PSD（功率谱密度），可能无法捕捉瞬态网络状态、动态功能连接等信息，影响模型辨识力。
- **临床应用限制**：未进行真实临床场景测试（如刺激规划、疗效预测）；模型偏差、噪声鲁棒性未知。
- **梯度优化在长期延迟系统中的挑战**：虽然混合BO缓解，但梯度反向传播计算成本高（Adam步时比BO评估多2.25倍），且可能受梯度不稳定限制。
- **封闭回路与实时控制**：当前仅支持开环优化，尚未集成闭环仿真。

（完）
