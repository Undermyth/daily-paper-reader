---
title: "BraiNN: A Modern Simulator for Clinically Feasible Personalized Whole-Brain Network Modeling"
title_zh: BraiNN：面向临床可行的个性化全脑网络建模的现代模拟器
authors: "Fasse, A., Billi, C., Garvalov, V., Morvan, M., Newton, T., Kuster, N., Neufeld, E."
date: 2026-07-13
pdf: "https://www.biorxiv.org/content/10.64898/2026.07.08.737156v1.full.pdf"
tags: ["query:comp-neuro"]
score: 8.0
evidence: 全脑网络模拟器用于神经科学
tldr: 个性化全脑建模对神经疾病治疗规划至关重要，但现有工具在临床时间尺度上难以满足计算需求。BraiNN采用JAX框架与GPU/TPU加速，实现比现有工具快2-3个数量级的仿真速度。其混合个性化流程结合贝叶斯优化与梯度优化，在约2-3小时内拟合EEG频谱，完成高细节全脑表面模型个性化。该工作将个性化脑网络建模推向临床应用，为患者数字孪生和EEG引导神经调控奠定基础。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-08-737156-v1/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 891, \"height\": 571, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-08-737156-v1/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1664, \"height\": 907, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-08-737156-v1/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 894, \"height\": 534, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-08-737156-v1/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 904, \"height\": 517, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-08-737156-v1/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 901, \"height\": 518, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-08-737156-v1/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 901, \"height\": 518, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-08-737156-v1/fig-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 896, \"height\": 518, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-08-737156-v1/fig-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 1842, \"height\": 915, \"label\": \"Figure\"}]"
tables_json: "[{\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-07-08-737156-v1/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 867, \"height\": 556, \"label\": \"Table\"}, {\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-07-08-737156-v1/table-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 898, \"height\": 297, \"label\": \"Table\"}]"
motivation: 现有全脑建模工具计算成本过高，难以在临床时间尺度内实现患者个性化拟合。
method: 采用JAX与GPU/TPU加速，结合Jansen-Rit模型与皮层表面网格，通过混合贝叶斯与梯度优化拟合EEG数据。
result: 速度提升达2-3个数量级，在消费级GPU上约2-3小时完成8维参数空间拟合，准确再现动力学特性。
conclusion: 将高细节全脑表面模型个性化从数天降至数小时，为临床数字孪生和神经调控奠定基础。
---

## 摘要
个性化全脑建模旨在通过实现患者特定的脑网络动力学模拟来改变神经系统疾病的治疗规划。神经质量模型（NMMs）在生物物理细节和计算成本之间提供了可处理的折衷，并可直接与宏观可观测量（如EEG）关联。然而，将NMMs扩展到具有真实连接性、传导延迟和皮层表面分辨率的全脑网络，并将其拟合到个体患者数据上，对现有框架提出了在临床相关时间尺度上无法满足的计算需求。本文介绍BraiNN，一个基于JAX的Python框架，用于大规模神经质量建模，通过利用GPU/TPU加速的XLA编译数组计算，相比现有工具实现了高达两到三个数量级的加速。BraiNN将区域级Jansen-Rit网络与受试者特定的耦合神经质量模型皮层表面网格以及基于互易性导联场的生物物理EEG正演建模相结合。其完全可微的计算图实现了混合个性化流水线，将贝叶斯优化用于全局参数探索与基于梯度的精调相结合，在单个消费级GPU上大约2-3小时内完成EEG驱动的八维参数空间谱拟合——而使用传统神经质量建模软件则需要数天。针对已有基准的数值验证确认，BraiNN忠实地再现了Jansen-Rit网络的典型同步和分岔动力学。通过将高细节全脑表面模型的个性化时间从数天减少到消费级硬件上的几小时，BraiNN使个性化脑网络建模更接近临床实际应用。我们预期BraiNN将作为患者特定数字孪生和EEG引导的神经调控规划的基础。

## Abstract
Personalized whole-brain modeling aims to transform treatment planning for neurological disorders by enabling patient-specific simulations of brain network dynamics. Neural mass models (NMMs) offer a tractable compromise between biophysical detail and computational cost and can be directly linked to macroscopic observables such as EEG. However, scaling NMMs to whole-brain networks with realistic connectivity, conduction delays, and cortical surface resolution - and fitting them to individual patient data - imposes computational demands that existing frameworks cannot meet at clinically relevant timescales. Here we introduce BraiNN, a JAX-based Python framework for large-scale neural mass modeling that achieves speedups of up to two to three orders of magnitude over existing tools by leveraging GPU/TPU-accelerated, XLA-compiled array computation. BraiNN combines a region-level Jansen-Rit network with a subject-specific cortical surface mesh of coupled neural mass models and biophysically grounded EEG forward modeling via reciprocity-based lead fields. Its fully differentiable computational graph enables a hybrid personalization pipeline that pairs Bayesian optimization for global parameter exploration with gradient-based refinement, completing EEG-driven spectral fitting of an eight-dimensional parameter space in approximately 2-3 hours on a single consumer GPU - compared to multiple days with conventional neural mass modeling software. Numerical verification against established benchmarks confirms that BraiNN faithfully reproduces canonical synchronization and bifurcation dynamics of Jansen-Rit networks. By reducing the time requirements for personalizing a high-detail whole-brain surface model from days to a few hours on consumer-grade hardware, BraiNN brings personalized brain network modeling closer to practical use in clinical contexts. We anticipate that BraiNN will serve as a foundation for patient-specific digital twins and EEG-guided neuromodulation planning.

---

## 论文详细总结（自动生成）

# 论文总结

## 1. 论文的核心问题与整体含义（研究动机与背景）

- **背景**：个性化全脑建模是神经调控和癫痫手术规划等临床干预的关键前沿技术。神经质量模型（NMMs）在生物物理合理性与计算开销之间提供了良好折中，并能直接与EEG等宏观观测关联。然而，将NMMs扩展到带真实结构连接、传导延迟、皮层表面分辨率的全脑网络，并拟合到患者数据，计算需求极高。现有框架（如The Virtual Brain, TVB）主要基于CPU，缺乏GPU加速与自动微分支持，导致模拟与参数拟合在临床时间尺度（数天）内不可行。
- **核心问题**：缺少一个同时具备高生物物理保真度、大规模可扩展性、自动微分能力并能在消费级硬件上实现快速个性化拟合的全脑建模工具。
- **整体含义**：该论文旨在填补这一空白，通过引入BraiNN—基于JAX的现代模拟器，将个性化全脑网络建模从“数天”缩短至“数小时”，向临床数字孪生和个性化神经调控迈出关键一步。

## 2. 方法论：核心思想、关键技术细节与算法流程

### 核心思想
- 利用JAX框架的XLA编译、GPU/TPU加速、自动微分和向量化变换（`vmap`、`jit`），将全脑NMM模拟、EEG正演、特征提取与优化统一为单个可微计算图。
- 采用**双尺度架构**：区域级（ROI）Jansen-Rit网络 + 受试者特定皮层表面网格（每个顶点一个NMM），实现空间细节与计算效率的平衡。

### 关键技术细节
- **神经质量模型**：每个节点采用经典的Jansen-Rit模型，状态为6维向量（三个子群膜电位及其导数）。通过非线性Sigmoid映射输出。
- **区域级网络**：基于扩散MRI获取的结构连接矩阵 \(W_{region} \in \mathbb{R}^{N\times N}\) 和延迟矩阵 \(D\)，外部驱动加上由全局耦合强度 \(G\) 加权的延迟耦合输入。
- **表面级网络**：每个皮层顶点一个NMM，通过最近邻映射分配至所属ROI。短期连接由稀疏几何矩阵 \(W_{surf}\) 表达，长期连接继承区域级信号并广播至顶点。
- **EEG正演**：采用互易性方法预计算导联场矩阵 \(L \in \mathbb{R}^{N_{eeg} \times M}\)，将皮层顶点叠加偶极子投影到EEG电极电压。转换系数 \(g\) 在个性化中估计。
- **延迟实现**：编译循环内使用固定大小循环缓冲区存储耦合变量，延迟索引由纤维长度与传导速度确定。
- **混合个性化流水线**：
    1. **全局探索**：使用贝叶斯优化（BO）与高斯过程（GP）代理模型，采用Matérn-5/2核，配合多种采集函数（EI, LogEI, CEI等）。在每次迭代中，通过Sobol采样全局搜索再使用Adam局部优化采集函数。
    2. **局部精调**：BO识别有希望的区域后，利用Adam梯度优化（基于Optax库）进行微调。
- **目标函数**：提取EEG功率谱密度（PSD，6–30Hz），采用Wasserstein距离衡量目标与模拟PSD之间的差异。

## 3. 实验设计：数据集、场景、基准与方法对比

### 数据集与场景
- **验证实验**：采用Kazemi和Jamali（2022）的随机驱动Jansen-Rit网络参数扫描协议，使用网格状参数组合（256×256），每个点128次重复，共约840万次模拟。耦合强度0–19.5，随机输入0–330Hz。
- **性能基准**：使用来自Karimi等（2025）的受试者特定结构连接矩阵，在区域数（10–250）、表面顶点数（最多约19000）、最大延迟（0–12.4s）、批处理规模（1–32）等维度上测量运行时。
- **个性化恢复实验**：合成数据，从8维参数空间（\(A, a, B, b, p_0, G, G_{surf}, \lambda_{diff}\)）生成真实EEG，然后尝试恢复。每个真实配置10次独立运行，不同初始化与随机种子。

### 基准对比方法
- **模拟器对比**：TVB（CPU）、vbjax（GPU）、cuBNM（CPU/GPU）、brainmass（CPU/GPU）。特征比较表（Table 2）表明仅BraiNN同时支持区域级、延迟、表面级、EEG导联场、优化和稀疏监测。
- **优化对比**：将混合BO+Adam与仅Adam梯度下降进行对比。

### 评价指标
- 运行时（wall-clock time）、加速比。
- PSD恢复质量：Wasserstein距离。
- 动力学验证：同步化程度、主导峰值频率与参考结果定性比对。

## 4. 资源与算力

- **硬件平台**：单台工作站，配置AMD Ryzen Threadripper 3970X（32核CPU）、256GB DDR4 RAM、NVIDIA GeForce RTX 3090 GPU（24GB显存）。
- **仿真时长**：
    - 区域级模拟（250 ROI）：GPU上约5.5秒；CPU上约58.8秒；TVB CPU上约1182.5秒（加速比约215×）。
    - 表面级模拟（约19000顶点）：GPU上约31.6秒；最大CPU基准4392顶点需1025.1秒（加速比约79.5×）。
    - 延迟敏感模拟：最大延迟12.4s时GPU约5.4秒。
    - 批处理32次并行仿真：GPU约6.0秒。
- **个性化拟合时长**：
    - 混合BO（250次迭代）：约140分钟（2.3小时）。
    - 仅Adam（250次迭代）：约266分钟（4.4小时），且质量更差。
    - 每次BO评估成本约28.9秒（≈一次正向模拟），每次Adam梯度步成本约63.9秒（含自动微分）。

## 5. 实验数量与充分性

- **验证实验**：单节点与小型网络轨迹与TVB独立实现逐点比对；大规模参数扫描（256×256网格，128重复）定性验证同步与分岔行为，共计约840万次模拟。该复现实验展示了大规模并行能力。
- **性能基准**：在5个维度（ROI数量、表面顶点数、延迟、批大小、库对比）上分别测试，每条件15个随机实例，每个实例重复5次，统计稳健。
- **个性化恢复实验**：8维参数空间，每个真实目标10次独立运行（不同初始化、不同随机噪声种子），对比BO与Adam。仅进行合成数据实验，无真实EEG数据验证。
- **充分性评估**：
    - 性能基准覆盖了临床相关规模，实验设计较为系统、公平（相同数值配置，包含编译开销）。
    - 个性化实验在合成数据上展示了方法的可行性，但缺乏真实噪声、伪影和模型失配考验，且仅使用PSD作为唯一特征，不能充分证明在真实患者数据上的有效性。
    - 未进行不同被试、不同连接组、不同优化超参数的系统性消融研究。

## 6. 主要结论与发现

- BraiNN能正确复现Jansen-Rit网络的典型动力学（同步转变、峰值频率）。
- 在区域级、表面级、延迟耦合、批处理场景下，BraiNN在GPU上相比TVB实现2–3个数量级的加速，在CPU上也优于或持平于其他GPU加速库。
- 混合BO+Adam流水线实现了8维参数空间的高质量谱拟合，在约2.3小时内完成，而仅Adam方法不仅耗时更长（4.4小时），且拟合质量更差（Wasserstein距离翻倍，方差大一个数量级）。
- 将高细节全脑表面模型个性化从数天降至数小时，使基于消费级GPU的临床数字孪生成为可能。
- 结论：BraiNN弥合了生物物理可解释NMM与临床实用需求之间的鸿沟，为个性化神经调控奠定了基础。

## 7. 优点

- **性能飞跃**：JAX + GPU/TPU带来2–3个数量级加速，使大规模模拟和优化从学术探索变为临床可行工具。
- **功能丰富且统一**：在一个框架内同时支持区域级/表面级、延迟、随机噪声、EEG正演（互易性导联场）、自动微分及多种优化器，集成度高。
- **混合优化策略创新**：结合贝叶斯优化（全局稳健）与梯度精调（局部高效），针对NMM的非凸、噪声损失函数设计巧妙。
- **延迟处理高效**：循环缓冲区避免数据复制，与编译加速兼容，开销极低。
- **原生并行**：`vmap`实现近乎恒定的边际批处理成本，适合BO的批量模拟需求。
- **可扩展与可微分**：计算图完全可微，便于未来集成到强化学习或控制框架。
- **开放科学**：计划开源（论文已承诺），有助于社区复现与扩展。

## 8. 不足与局限

- **模型支持单一**：目前仅实现Jansen-Rit NMM，未包含丘脑、基底节等其他常见NMM或皮层场模型，扩展性受限于作者后续工作。
- **仅合成数据验证**：个性化实验完全基于同一模型类生成的合成数据，未在真实EEG记录上测试。真实环境中的噪声、伪影、模型失配、电极位置误差等问题尚未评估，可能存在过拟合或泛化风险。
- **特征空间狭窄**：仅使用静态PSD（6–30Hz）作为目标，忽略了动态功能连接、时变谱、互信息等更丰富特征，可能丢失对神经调控关键信息的捕捉。
- **BO超参数敏感**：文中对BO的超参数（核函数、采集函数类型、寻优策略）调优描述有限，未进行敏感性分析。
- **未评估真实临床场景**：未进行患者分层、多种疾病类型、不同电极布局的测试，临床适用性仍有待证明。
- **自动微分局限性**：延迟递推、长时间序列导致梯度爆炸/消失，文中采用BO规避但仍限制了纯梯度法的应用，未来可能需要梯度截断、代理梯度或可逆求解器。
- **编译开销**：首次编译耗时未报告（虽然对长时拟合可摊销），变模型结构时需重新编译，可能影响迭代探索效率。

（完）
