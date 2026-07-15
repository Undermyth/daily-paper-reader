---
title: A geometric and dynamical theory of latent computations in biological neural networks
title_zh: 生物神经网络中潜在计算的几何与动力学理论
authors: "Dinc, F., Blanco-Pozo, M., Klindt, D., Acosta, F., Sylber, C., Jiang, Y., Ebrahimi, S., Shai, A., Tanaka, H., Yuan, P., Miolane, N., Schnitzer, M. J."
date: 2026-07-15
pdf: "https://www.biorxiv.org/content/10.64898/2026.07.10.737763v1.full.pdf"
tags: ["query:comp-neuro"]
score: 8.0
evidence: 生物神经网络中潜在计算的几何与动力学理论，计算神经科学核心
tldr: 神经记录表明大规模活动蕴含低维变量，但降维分析难以解释网络稳定计算的机制。本文提出潜在处理单元（LPUs），一种架构无关的计算元素，通过六个定理揭示了低维编码可生成高维动态、多数神经元表型变量但影响小、线性读码近最优、表征漂移而计算不变等现象。该理论统一了几何与动力学视角，提供大脑可靠计算的因果解释。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-10-737763-v1/fig-001.webp\", \"caption\": \"\", \"page\": 39, \"index\": 1, \"width\": 1583, \"height\": 2048}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-10-737763-v1/fig-002.webp\", \"caption\": \"\", \"page\": 43, \"index\": 2, \"width\": 1583, \"height\": 2048}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-10-737763-v1/fig-003.webp\", \"caption\": \"\", \"page\": 48, \"index\": 3, \"width\": 1583, \"height\": 2048}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-10-737763-v1/fig-004.webp\", \"caption\": \"\", \"page\": 51, \"index\": 4, \"width\": 1583, \"height\": 2048}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-10-737763-v1/fig-005.webp\", \"caption\": \"\", \"page\": 54, \"index\": 5, \"width\": 1583, \"height\": 2048}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-10-737763-v1/fig-006.webp\", \"caption\": \"\", \"page\": 59, \"index\": 6, \"width\": 1583, \"height\": 2048}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-10-737763-v1/fig-007.webp\", \"caption\": \"\", \"page\": 64, \"index\": 7, \"width\": 1583, \"height\": 2048}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-10-737763-v1/fig-008.webp\", \"caption\": \"\", \"page\": 66, \"index\": 8, \"width\": 1583, \"height\": 2048}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-10-737763-v1/fig-009.webp\", \"caption\": \"\", \"page\": 68, \"index\": 9, \"width\": 1583, \"height\": 2048}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-10-737763-v1/fig-010.webp\", \"caption\": \"\", \"page\": 69, \"index\": 10, \"width\": 1583, \"height\": 2048}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-10-737763-v1/fig-011.webp\", \"caption\": \"\", \"page\": 70, \"index\": 11, \"width\": 1583, \"height\": 2048}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-10-737763-v1/fig-012.webp\", \"caption\": \"\", \"page\": 71, \"index\": 12, \"width\": 1824, \"height\": 1484}]"
motivation: 现有降维方法假设过多，无法解释生物网络稳定实现低维计算，需要统一理论框架。
method: 引入潜在处理单元（LPUs），并通过六个定理统一描述编码与计算的几何与动力学。
result: LPU理论解释了低维编码生成高维动态、神经元冗余性、线性读码最优性及表征漂移等现象。
conclusion: LPU框架整合了几何与动力学观点，为系统神经科学提供大脑可靠计算的因果机制。
---

## 摘要
许多神经记录已揭示，大规模神经活动模式中编码了低维的行为相关变量集合。然而，仅凭降维分析无法提供因果解释，说明网络如何稳定地实现对单个神经元动力学巨大变异具有鲁棒性的计算。此外，现有的降维方法通常依赖于对网络结构的简化假设，这限制了其适用性和解释力。为提供描述高维神经网络中低维计算动力学的理论框架，本文引入潜在处理单元（LPU）的概念，这是一种在生物神经回路中运作的、与架构无关的计算元素。关于LPU编码与计算的六个定理共同为一系列常见生物学发现提供了解释：低维编码变量集能够生成高维神经动力学；许多神经元的活性模式代表了行为相关变量，但对下游回路影响甚微；神经群体活动的线性读出通常允许接近最优的解码；即使在网络计算保持完整的情况下，神经表征的漂移也常常很大。总体而言，我们对LPU的处理（在网络动力学中实现）统一了神经计算的几何观和动力学观于一个联合框架下，并为系统神经科学提供了关于大脑如何执行可靠计算的因果解释。

## Abstract
Many neural recordings have revealed low-dimensional sets of behaviorally relevant variables encoded within large-scale neural activity patterns. However, dimensionality reduction analyses alone cannot yield causal explanations for how networks stably implement computations that are resilient to the substantial variability of single neuron dynamics. Further, existing methods for dimensionality reduction often rely on simplifying assumptions about network structure that limit their applicability and explanatory power. To provide a theoretical framework describing the dynamics of low-dimensional computation in high-dimensional neural networks, here we introduce the concept of latent processing units (LPUs), which are architecture-agnostic computational elements operating within biological neural circuitry. Six theorems governing coding and computation by LPUs collectively provide explanations for a range of common biological findings: low-dimensional sets of coding variables can generate high-dimensional neural dynamics; many neurons have activity patterns that represent behaviorally relevant variables but exert little influence on downstream circuits; linear readouts of neural population activity commonly permit near-optimal decoding; the drift of neural representations is often substantial even while network computations remain intact. Overall, our treatment of LPUs, as enacted in network dynamics, unifies the geometric and dynamical views of neural computation under a joint framework and provides systems neuroscience with a causal account of how the brain executes reliable computations.

---

## 论文详细总结（自动生成）

# 生物神经网络中潜在计算的几何与动力学理论 - 结构化总结

## 1. 核心问题与整体含义（研究动机和背景）

- **背景**：神经记录揭示大规模神经活动隐藏着低维的行为相关变量，但现有降维方法（如PCA、线性动力系统、低秩RNN）存在根本局限：
  - 第一代静态方法（PCA等）无法提供因果性解释。
  - 第二代动力系统方法（如rSLDS、低秩RNN）依赖简化假设（如线性映射），不能全面解释生物网络中的冗余性、高维性、漂移鲁棒性等现象。
- **核心问题**：如何从理论上统一几何与动力学视角，解释生物神经网络如何在单个神经元持续变异和漂移的情况下，稳定地执行低维、可靠的计算？
- **整体含义**：论文提出**潜在处理单元（LPU）** 作为架构无关的计算元素，通过六个定理系统解释了低维编码生成高维动态、神经元冗余编码、线性读码最优性、表征漂移下计算不变性等经典现象，为系统神经科学提供了因果性理论框架。

## 2. 方法论：核心思想、关键技术细节

- **核心思想**：LPU将神经计算分解为**线性编码**和**非线性嵌入**两个独立过程：
  - **P1**：潜变量是神经活动的线性组合：𝜿(𝑡) = 𝑵𝒓(𝑡)
  - **P2**：神经动力学是潜变量的非线性函数：τ𝒓̇(𝑡) = −𝒓(𝑡) + 𝝋(𝜿(𝑡), 𝒖(𝑡))
  - **P3**：行为相关计算由低维潜变量动力学驱动。
  - **P4**：生物网络通过低秩突触权重实现上述映射：𝑾 ≈ 𝑴𝑵

- **关键技术细节**：
  - 线性编码保证了潜变量的自洽性与可识别性（GL_K(R)对称性）。
  - 非线性嵌入（由神经元非线性变换实现）赋予LPU**通用逼近能力**（定理1）。
  - 通过引入**编码矩阵**和**嵌入矩阵**的独立性，实现了因果编码维度与声学编码维度的分离。
  - 六个定理分别覆盖：通用计算（定理1）、长时间尺度计算（定理2）、线性读码最优性（定理3）、高维外部表征（定理4）、因果与非因果编码分离（定理5）、表征漂移鲁棒性（定理6）。

- **公式流程（文字）**：
  - LPU动力学：τ𝜿̇ = −𝜿 + 𝑵𝝋(𝜿, 𝒖)
  - 神经元动力学：τ𝒓̇ = −𝒓 + 𝝋(𝜿, 𝒖)
  - 读码：线性读出可通过投影到因果编码子空间直接解码潜变量函数（定理3）。

## 3. 实验设计：数据集、场景、基准与对比方法

- **模拟实验**：
  - **K位Flip-Flop任务**：训练全秩/低秩RNN（基础RNN、增益调制RNN）以记忆和切换2^K个状态。分析潜变量相位平面、扰动效应。
  - **双稳态动力学设计实验**：基于高斯采样构建一维双稳态LPU，考察有限神经元下有效时间常数的误差缩放（定理2）。
  - **序列排序任务**：训练低秩RNN排序数字序列，测量外部维度如何随神经元数增加而增长（定理4）。
  - **延迟加法任务**：训练秩-1 RNN实现连续变量积分与控制，测试编码方向与读码方向对计算的因果影响（定理5）。
  - **表征漂移实验**：在3-bit Flip-Flop任务中向嵌入权重添加随机/正交/切向扰动，测量状态估计准确率（定理6）。

- **实际神经数据（公开数据集）**：
  - 来源：Ebrahimi et al. (2022) Nature，小鼠皮层大规模钙成像数据。
  - 8个皮层区域（V1, LV, MV, PPC, A, S, M, RSC），6只小鼠，30个成像session，总计约2万个神经元。
  - **任务**：视觉Go/NoGo判别任务。
  - **解码分析**：对比线性解码器（Logistic回归、LDA）与非线性解码器（随机森林、QDA）在PLS降维后解码试次类型（Hit vs CR）的准确率。

- **基准与对比**：
  - 与现有方法比较（见表S1）：低秩RNN、rSLDS、深度学习模型。
  - 在解码实验中，线性与非线性解码器在低维潜子空间中表现一致，支持定理3。
  - 在扰动实验中，比较编码方向、读码方向、随机方向等干预效果。
  - 在漂移实验中，比较三种漂移方向（随机、正交、切向）的耐受阈值。

## 4. 资源与算力

- **文中未明确说明**具体GPU型号、数量或总训练时长。
- **使用的框架**：PyTorch（用于训练RNN）和scikit-learn（用于神经数据解码）。
- **训练规模**：部分RNN训练使用Adam优化器，批量大小至多5000，训练步数5000~20000 epoch。大规模模拟（如百万级神经元）通过重采样方式生成，非直接训练。
- **注意**：由于论文重点为理论研究，训练计算量相对较小，主要计算消耗在蒙特卡洛模拟（多次重复抽样）上。

## 5. 实验数量与充分性

- **仿真实验数量**：
  - Flip-Flop任务：训练了多个网络（如50个网络用于3-bit Flip-Flop漂移实验）。
  - 双稳态设计：每个参数组合重复30次模拟。
  - 序列排序：10次不同随机种子。
  - 延迟加法：训练了51个成功网络。
  - 漂移实验：每个配置（网络大小×漂移类型×强度）使用50个网络。
- **实际数据实验**：6只小鼠×共30个session，每区域每时间段使用100次随机训练/测试划分。
- **消融与变体**：
  - 编码/嵌入架构对比（基本RNN vs 增益调节RNN）。
  - 不同非线性函数（tanh, ReLU, sin）。
  - 网络大小从100到1e6变化。
  - 漂移方向、强度扫描。
  - 读码方向对比（编码、读码、随机、最优等）。
- **充分性评价**：实验覆盖了所有定理的关键预测，并通过统计量（均值和标准差/标准误）展示，结果可靠。结论具有广泛的敏感性分析支撑，公平性较好（如解码实验中线性/非线性公平比较）。

## 6. 主要结论与发现

- **定理1（通用计算）**：当神经元足够多且激活函数多样性足够时，LPU可以任意逼近任何连续潜动力学系统。
- **定理2（长时间尺度）**：为实现毫秒级神经时间常数到秒级行为时间常数的分离，网络规模必须满足 β²/N 误差缩放，大约需要百万级神经元。
- **定理3（线性读码最优性）**：任何平滑的潜变量函数均可通过线性读码从神经活动中逼近，且误差随神经元数增加而消失。实验证实了在小鼠皮层数据中线性与非线性解码性能一致。
- **定理4（低维潜变量→高维神经流形）**：非线性嵌入可使外部线性维度随神经元数线性增长，即使潜变量维度固定。实验表明行为不相关的高维成分可能来自流形曲率而非高维编码。
- **定理5（因果与非因果编码分离）**：只有位于因果编码子空间（编码矩阵行空间）的扰动才能持久影响潜动力学；调谐与因果参与无关。
- **定理6（表征漂移鲁棒性）**：如果漂移是随机的或正交于因果编码维度，潜动力学仅受二阶影响，可被网络规模抑制；切向漂移则破坏计算。
- **总体**：LPU框架统一了几何与动力学视角，解释了神经表征中的冗余性、鲁棒性与高维性。

## 7. 优点：方法和实验设计的亮点

- **理论创新**：
  - 引入编码/嵌入的**独立性**，为因果与声学编码、线性读码最优性、漂移鲁棒性提供了统一解释。
  - 定理2给出了长时间计算需要大网络的定量缩放关系，超越经典容量理论。
  - 定理4证明高维神经活动可由低维潜变量+非线性嵌入产生，挑战了“高维活动=高维编码”的观点。
  - 定理5/6提供了可验证的扰动预测（因果编码子空间）和漂移模式（正交 vs 切向）。

- **实验设计亮点**：
  - 使用多类任务测试不同定理，涵盖离散（Flip-Flop）、连续（延迟加法）和序列（排序）计算。
  - 在大规模实际数据上验证线性读码最优性（6只小鼠，8个皮层区域）。
  - 系统扫描网络规模、漂移类型、扰动方向，并与理论预测定量比较。
  - 展示了连接组信息不足以识别因果编码维度（图5b），突出了理论预测的实用性。

## 8. 不足与局限

- **理论假设**：
  - 主要分析基于弱缩放（权重缩放~1/N），不涵盖强混沌动力学（权重缩放~1/√N）情况。
  - 假设线性编码，可能限制某些生物场景（如非线性树突计算下的编码）。
  - 证明依赖概率分布假设（如自平均性、有限协方差），部分定理要求特殊结构（如正交漂移）。

- **实验覆盖**：
  - 实际数据解码仅用了试次类型（Hit vs CR），未测试更复杂的认知变量。
  - 扰动和漂移实验仅限于仿真，缺乏动物实验验证（如光遗传干预因果编码方向）。
  - 部分观察下LPU重建问题仅用理想化估算（已知真实权重），未在真实数据中测试。
  - 没有训练生物物理可执行模型（如LIF或Hodgkin-Huxley网络）。

- **偏差风险**：
  - 解码实验中选择PLS降维维度（最大15维）可能偏向线性模型，但非线性模型也使用了相同潜变量，比较相对公平。
  - 漂移实验仅用瞬时漂移，未模拟连续学习过程。

- **应用限制**：
  - 实际识别LPU需要知道编码矩阵N，这通常不可直接观测。
  - 定理主要针对“平均”计算，未处理单试次变异性与动态任务切换。
  - 未提供学习算法（如如何从数据中推断LPU）。

（完）
