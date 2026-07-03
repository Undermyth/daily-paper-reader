---
title: Stimulus and circuit contributions to the information geometry of neural manifolds
title_zh: 刺激与电路对神经流形信息几何的贡献
authors: "Goedeke, S., Kautz, J. K., Leibold, C."
date: 2026-06-25
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.21.733384v1.full.pdf"
tags: ["query:comp-neuro"]
score: 8.0
evidence: 神经流形的微分几何分析，连接网络连接与信息编码
tldr: 神经网络活动中的低维流形结构如何产生尚不明确。本文发展微分几何框架，推导了率模型递归网络中神经流形的拉回度量，并证明其与Fisher信息矩阵结构一致。通过分析网格细胞空间表示，发现前馈连接足以形成环面流形，而递归连接仅在快速噪声下提升编码。
source: biorxiv
selection_source: fresh_fetch
motivation: 揭示网络连接如何塑造神经表示是系统神经科学的核心问题，但缺乏连接流形几何与网络机制、信息编码的严格框架。
method: 针对速率递归网络，推导神经流形拉回度量的解析表达式，并证明稳态Fisher信息矩阵也具有拉回度量结构。
result: 前馈连接决定性影响表示几何，递归连接在慢噪声下效应抵消；仅前馈连接即可从随机调谐生成网格细胞环形流形。
conclusion: 前馈连接足以生成结构化空间表示，递归连接可在快速噪声下选择性降噪，改善刺激编码。
---

## 摘要
理解网络连接如何塑造神经表征是系统神经科学的核心问题。虽然降维方法在群体记录中发现了低维流形结构，但目前仍缺乏一个严格的框架将流形几何与网络机制及信息编码联系起来。我们开发了一种微分几何方法，用于分析接受调谐前馈输入的基于速率的递归神经网络中的神经流形。我们推导了神经流形拉回度量的表达式，展示了输入调谐曲线以及前馈和递归突触连接如何塑造流形几何。关键的是，我们证明了稳态下的费舍尔信息矩阵也具有拉回度量的结构，直接将内在流形几何与刺激可区分性和信息编码联系起来。对于通过网络传播的具有缓慢时间相关性的噪声，我们表明递归对信息几何的影响被抵消：费舍尔信息仅取决于前馈连接。因此，前馈连接关键地决定了表征几何。我们将该方法应用于六边形网格细胞模块对空间的表征。我们首先证明，对于网格相位的随机分布，表征近似等距。此外，线性前馈变换可以将空间随机的输入调谐曲线映射到一群六边形网格细胞，生成环面神经流形。因此，仅前馈连接就能生成结构化的空间表征，无需精心调整的递归连接或连续吸引子动力学。然而，研究表明递归连接可以改善快速噪声下的刺激编码，从而实现选择性降噪。

## Abstract
Understanding how network connectivity shapes neural representations is central to systems neuroscience. While dimensionality reduction methods uncover low-dimensional manifold structure in population recordings, a rigorous framework connecting manifold geometry to network mechanisms and information encoding remains lacking. We develop a differential geometric approach for analyzing neural manifolds in rate-based recurrent networks receiving tuned feedforward inputs. We derive expressions for the pullback metric of neural manifolds, showing how input tuning curves together with feedforward and recurrent synaptic connectivity shape manifold geometry. Critically, we establish that the Fisher information matrix at steady states also has the structure of a pullback metric, directly linking intrinsic manifold geometry to stimulus discriminability and information encoding. For noise with slow temporal correlations propagated through the network, we show that recurrent effects on information geometry cancel: Fisher information depends only on the feedforward connectivity. Thus, feedforward connectivity critically determines representational geometry. We apply our approach to the representation of space by a module of hexagonal grid cells. We first demonstrate that the representation is approximately isometric for a random distribution of grid phases. Moreover, a linear feedforward transformation can map spatially random input tuning curves into a population of hexagonal grid cells, generating a toroidal neural manifold. Thus, feedforward connectivity alone can generate structured spatial representations without requiring carefully tuned recurrent connectivity or continuous attractor dynamics. Recurrent connectivity, however, is shown to improve stimulus encoding under fast noise, thereby implementing a selective noise reduction.

---

## 论文详细总结（自动生成）

好的，以下是根据您提供的论文内容生成的中文总结。

---

### 1. 论文的核心问题与整体含义（研究动机和背景）
- **核心问题**：神经网络群体活动中常观察到低维的神经流形，但这些流形的几何结构（如距离、曲率）如何由网络内部机制（前馈和递归连接）决定，以及这种几何如何与刺激的编码能力（Fisher信息）相关联，目前缺乏严格的理论框架。
- **整体含义**：该工作旨在建立一个微分几何框架，将神经流形的内在几何与网络连接参数、噪声特性以及信息编码联系起来，从而揭示网络机制如何塑造神经表征。特别地，它试图区分前馈和递归连接在信息几何中的不同角色。

### 2. 论文提出的方法论：核心思想、关键技术细节、公式或算法流程
- **核心思想**：将神经流形视为刺激空间到神经网络活动空间的嵌入，利用“拉回度量”（pullback metric）描述流形的内在几何，并证明该度量与Fisher信息矩阵在结构上等价，从而将几何与编码能力直接挂钩。
- **关键技术细节与公式**：
  - **模型设定**：考虑率模型递归网络，稳态活动满足隐式方程 \(x^* - W\phi(x^*) = M\psi(z)\)，其中 \(z\) 是刺激，\(W\) 是递归权重，\(M\) 是前馈权重。
  - **神经流形度量**：神经流形的拉回度量 \(g_M(z) = (\partial_z x^*)^T \partial_z x^*\)，通过线性化可表达为 \(g_M(z) = (\partial_z\psi)^T M^T [1-W]^{-T} [1-W]^{-1} M \partial_z\psi\)。
  - **Fisher信息与度量的等价**：对于刺激无关的等向高斯噪声，Fisher信息 \(I(z) = \sigma^{-2} g_M(z)\)。更一般地，Fisher信息可视为另一种变换后流形（统计流形）的拉回度量。
  - **噪声传播**：考虑噪声通过网络动态传播，得到连续Lyapunov方程。关键结果是：对于慢噪声（时间相关性长），Fisher信息简化为 \(I(z) = (\partial_z\psi)^T M^T (\Sigma')^{-1} M \partial_z\psi\)，完全不含递归权重 \(W\)，即递归作用被抵消。对于快噪声（如白噪声），递归权重会影响Fisher信息，具体表现为 \(I(z) = (\partial_z\psi)^T M^T \tilde{\Sigma}^{-1} M \partial_z\psi\)，其中 \(\tilde{\Sigma}\) 依赖于 \(W\) 的特征值。
- **算法流程**：推导基于线性化稳定点、谱分解和Lyapunov方程求解，通过解析计算而非迭代算法实现。

### 3. 实验设计：使用了哪些数据集 / 场景，它的 benchmark 是什么，对比了哪些方法
- **数据集/场景**：全部使用合成数据，没有真实神经数据。
  - **场景一**：两个神经元、低秩网络，输入为高斯调谐曲线（1维刺激），演示前馈和递归对度量与Fisher信息的影响（图1）。
  - **场景二**：环形流形，输入为余弦调谐曲线（1维环状刺激），前馈权重设计成将扭曲的环恢复成均匀圆，展示前馈可改变几何（图2）。
  - **场景三**：网格细胞模块，使用叠加三个平面波的网格细胞模型，考察不同相位分布（理想六角晶格、随机扰动、均匀随机）下度量的均匀性（图3）。
  - **场景四**：前馈生成网格细胞，从随机空间调谐输入通过Hebbian学习得到前馈权重，产生网格细胞活动，并分析流形的曲率（图4）。
  - **场景五**：递归网络在快噪声下的作用，构建两种递归权重（全外积 vs 去掉第二大特征模），比较神经流形和统计流形的拓扑与体积元（图5）。
- **Benchmark**：论文本身没有明确的对比方法，主要进行理论推导和数值验证。基准（baseline）为无递归（\(W=0\)）或理想等距条件。
- **对比方法**：对比了不同相位配置（理想、扰动、随机）、不同递归结构（有/无特定特征模）下的度量、Fisher信息、体积元、Ricci标量等指标。

### 4. 资源与算力：如果文中有提到，请总结使用了多少算力（GPU 型号、数量、训练时长等）。若未明确说明，也请指出这一点。
- **未明确说明**。论文专注于理论分析和数值模拟，未提及任何GPU型号、数量或训练时长。数值实验（如Isomap嵌入、网格细胞活动生成）很可能在普通CPU上完成，但具体硬件未交代。

### 5. 实验数量与充分性：大概做了多少组实验（如不同数据集、消融实验等），这些实验是否充分、是否客观、公平
- **实验数量**：
  - 图1：2个样本刺激方向、2种递归设置（有/无）。
  - 图2：1种输入分布（von Mises），1种前馈映射。
  - 图3：N=7~256，每种扰动尺度（0~0.6ℓ）做1000次随机实现，共约10种扰动水平 × 6种神经元数量 × 1000次 = 约60000次模拟（但可并行）。
  - 图4：单次前馈网格细胞生成（K=4000, N=256）。
  - 图5：2种递归矩阵（全/减模式），分析体积元、特征重叠等。
  - 此外，附录中有解析推导与简化情况。
- **充分性与公平性**：
  - **充分**：在不同场景（简单、复杂、网格细胞）、不同噪声假设（慢、快）、不同递归形式下验证了理论预测。对网格细胞相位的随机扰动进行了统计显著性检验。
  - **客观**：所有实验均为合成数据，可完全复现。但未在真实神经数据上验证，理论预测的生物学适用性需进一步检验。
  - **公平性**：对比条件合理（如慢噪声下有/无递归，快噪声下不同特征模的影响），但缺乏与其他同类理论模型（如连续吸引子模型）的定量比较。

### 6. 论文的主要结论与发现
1. **前馈连接决定性作用**：在慢噪声下，递归连接对Fisher信息无贡献，只有前馈连接决定表征几何。前馈连接可以重塑甚至改变流形的拓扑（如从平面环变成环面）。
2. **递归连接在快噪声下改善编码**：对于快噪声（如白噪声），递归可以放大与递归特征向量对齐的信号，实现选择性降噪，提高Fisher信息。
3. **网格细胞等距表征**：即使网格相位随机分布，随着神经元数量增加（约N=100），引入的几何畸变变得很小（~7%），说明精细的相位排列并非必需。
4. **前馈生成网格细胞**：仅通过Hebbian前馈学习，从随机空间调谐输入即可生成六边形网格细胞活动，并形成近似的环面流形，无需递归吸引子机制。

### 7. 优点：方法或实验设计上有哪些亮点
- **理论创新**：建立了神经流形几何与Fisher信息之间的严格数学联系，并给出了递归网络中两者依赖于电路参数的解析表达式。首次区分了慢噪声和快噪声下递归的不同作用。
- **分析方法深入**：不仅分析度量（一阶导数），还计算了Ricci标量（二阶曲率），提供了更丰富的几何信息。
- **实验设计全面**：从简单双神经元到复杂网格细胞模块，系统验证了理论预测，并通过扰动分析评估了鲁棒性。
- **生物学洞察**：解释为何网格细胞模块可以容忍相位随机性，并指出前馈机制足以产生结构化空间表征，挑战了依赖连续吸引子的经典观点。

### 8. 不足与局限：包括实验覆盖、偏差风险、应用限制等
- **实验覆盖**：所有实验基于合成数据，未使用真实神经记录验证，理论预测是否适合生物神经网络存疑。
- **模型假设限制**：假设线性激活函数（或线性化）、固定点吸引子、高斯噪声。真实的神经网络包含非线性、突触可塑性、非平稳动态，可能改变结论。
- **偏差风险**：分析仅限于固定点，未考虑振荡或混沌状态；忽略了神经元的输入-输出非线性（如整流非线性）可能带来的几何效应。
- **应用限制**：结论对慢噪声成立，但真实神经系统中噪声时间尺度多样，可能同时存在慢和快成分，需更复杂模型。另外，仅考虑单层递归网络，未涉及深层或多区域循环连接。

（完）
