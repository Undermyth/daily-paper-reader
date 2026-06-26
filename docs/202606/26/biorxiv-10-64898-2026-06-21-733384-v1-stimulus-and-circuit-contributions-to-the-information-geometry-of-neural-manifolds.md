---
title: Stimulus and circuit contributions to the information geometry of neural manifolds
title_zh: 刺激与回路对神经流形信息几何的贡献
authors: "Goedeke, S., Kautz, J. K., Leibold, C."
date: 2026-06-25
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.21.733384v1.full.pdf"
tags: ["query:comp-neuro"]
score: 8.0
evidence: 发展了循环网络中神经流形的微分几何分析，将连接性与信息编码联系起来，属于计算神经科学核心。
tldr: 神经系统呈现低维流形结构，但其与网络机制的关系缺乏严格框架。本文用微分几何分析率模型网络，推导出神经流形的拉回度量，并证明稳态Fisher信息矩阵也具有拉回度量结构，从而直接联系几何与编码。慢噪声下递归效应抵消，前馈连接决定几何；例如模块化六边形网格细胞的空间表示近似等距，线性前馈变换可将随机调谐映射为六边形网格细胞。该工作表明前馈连接可生成结构化空间表示，无需递归吸引子，递归仅在快噪声下选择性降噪提高编码。
source: biorxiv
selection_source: fresh_fetch
motivation: 理解网络连接如何塑造神经表示，特别是流形几何与网络机制的关系。
method: 用微分几何推导神经流形的拉回度量，建立与Fisher信息的联系。
result: 前馈连接决定慢噪声下的流形几何，快噪声下递归改善编码；线性前馈可生成六边形网格细胞。
conclusion: 神经流形几何主要由前馈连接决定，递归仅用于选择性降噪，挑战了吸引子观点。
---

## 摘要
理解网络连接如何塑造神经表征是系统神经科学的核心问题。虽然降维方法揭示了群体记录中的低维流形结构，但将流形几何与网络机制及信息编码联系起来的严谨框架仍然缺乏。我们发展了一种微分几何方法，用于分析接收调谐前馈输入的基于速率的递归网络中的神经流形。我们推导了神经流形拉回度量的表达式，展示了输入调谐曲线、前馈和递归突触连接如何塑造流形几何。关键的是，我们证明稳态下的费希尔信息矩阵也具有拉回度量的结构，直接将内在流形几何与刺激可分辨性和信息编码联系起来。对于通过网络传播的具有慢时间相关性的噪声，我们显示递归效应对信息几何的影响相互抵消：费希尔信息仅取决于前馈连接。因此，前馈连接关键地决定了表征几何。作为例子，我们证明六边形网格细胞模块对空间的表征对于随机分布的网格相位近似等距。此外，线性前馈变换可以将空间随机输入调谐曲线映射到一群六边形网格细胞，形成环面流形。因此，仅前馈连接就能生成结构化空间表征，而无需精心调谐的递归连接或连续吸引子动力学。然而，递归连接被证明能在快噪声下改善刺激编码，从而实现选择性降噪。

## Abstract
Understanding how network connectivity shapes neural representations is central to systems neuroscience. While dimensionality reduction methods uncover low-dimensional manifold structure in population recordings, a rigorous framework connecting manifold geometry to network mechanisms and information encoding remains lacking. We develop a differential geometric approach for analyzing neural manifolds in rate-based recurrent networks receiving tuned feedforward inputs. We derive expressions for the pullback metric of neural manifolds, showing how input tuning curves, feedforward and recurrent synaptic connectivity shape manifold geometry. Critically, we establish that the Fisher information matrix at steady states also has the structure of a pullback metric, directly linking intrinsic manifold geometry to stimulus discriminability and information encoding. For noise with slow temporal correlations propagated through the network, we show that recurrent effects on information geometry cancel: Fisher information depends only on the feedforward connectivity. Thus, feedforward connectivity critically determines representational geometry. As an example, we demonstrate that the representation of space by a module of hexagonal grid cells is approximately isometric for random distribution of grid phases. Moreover, a linear feedforward transformation can map spatially random input tuning curves into a population of hexagonal grid cells, forming a toroidal manifold. Thus, feedforward connectivity alone can generate structured spatial representations without requiring carefully tuned recurrent connectivity or continuous attractor dynamics. Recurrent connectivity, however, is shown to improve stimulus encoding under fast noise, thereby implementing a selective noise reduction.

---

## 论文详细总结（自动生成）

## 论文详细中文总结

### 1. 论文的核心问题与整体含义
- **研究动机**：系统神经科学中，群体神经活动常呈现低维流形结构，但现有降维方法（如PCA、t-SNE）仅描述现象，缺乏将流形几何与网络连接机制、信息编码联系起来的形式化理论框架。
- **核心问题**：神经流形的几何形状（如曲率、度量）如何由前馈输入调谐、递归突触连接以及噪声传播共同决定？特别是递归连接是否必要？
- **整体含义**：该工作为理解网络连接如何塑造神经表征提供了微分几何基础，挑战了“连续吸引子”必须依赖精心调谐的递归连接的传统观点，指出前馈连接足以生成规则的空间表示（如六边形网格细胞）。

### 2. 论文提出的方法论
- **核心思想**：将神经群体活动视为由刺激参数（如空间位置）参数化的低维流形，采用微分几何中的**拉回度量（pullback metric）** 来描述流形上的距离与角度，并证明稳态下**费希尔信息矩阵（Fisher Information Matrix, FIM）** 也具有拉回度量结构，从而直接关联几何与编码精度。
- **关键技术细节**：
  - 模型：基于速率的递归网络，神经元接收调谐的前馈输入 \( \mathbf{h}(s) \)，递归连接矩阵 \( \mathbf{W} \)，噪声项 \( \xi \)。
  - 稳态活动 \( \mathbf{r} = \phi(\mathbf{h}(s) + \mathbf{W} \mathbf{r} + \xi) \)（\( \phi \) 为非线性）。
  - 推导流形切向量 \( \frac{\partial \mathbf{r}}{\partial s} \) 与拉回度量 \( g_{\mu\nu} = \left( \frac{\partial \mathbf{r}}{\partial s^\mu} \right)^T \mathbf{C}^{-1} \left( \frac{\partial \mathbf{r}}{\partial s^\nu} \right) \)，其中 \( \mathbf{C} \) 为噪声协方差矩阵。
  - 关键发现：对于慢时间相关噪声（协方差矩阵在网络中传播时满足 \( \mathbf{C} \propto (\mathbf{I} - \mathbf{W})^{-2} \)），递归对费希尔信息的贡献相互抵消，最终 \( \text{FIM} \) 仅取决于前馈连接矩阵 \( \mathbf{W}^{\text{ff}} \) 和输入调谐曲线。
- **公式流程（文字说明）**：
  1. 写出网络稳态方程并线性化。
  2. 计算流形切向量（活动对刺激的导数）。
  3. 代入噪声协方差，得到拉回度量/费希尔信息表达式。
  4. 利用慢噪声假设简化，证明递归项消去。
  5. 以六边形网格细胞为例，展示前馈连接可产生环面流形且等距于均匀分布相位。

### 3. 实验设计
- **使用场景**：纯理论推导 + 数学示例分析，无传统实验数据集或基准方法。
- **示例**：
  - **六边形网格细胞模块**：假设前馈连接将随机相位输入映射为六边形网格细胞，证明其空间表示近似等距（即拉回度量与欧几里得空间一致）。
  - **前馈线性变换**：展示任意随机调谐曲线可通过线性前馈连接转化为六边形网格细胞群体，形成环面流形。
- **对比方法**：无直接对比，但隐含与“连续吸引子模型”对比，说明递归并非构建规则空间表示所必需。

### 4. 资源与算力
- **未提及**：论文为理论计算神经科学工作，无数值模拟或深度学习训练，故未报告任何GPU、训练时长等算力信息。

### 5. 实验数量与充分性
- **实验数量**：不涉及传统实验，只有2个数学示例（六边形网格细胞近似等距、线性前馈生成环面流形）。无消融实验、不同噪声条件下的系统性数值验证。
- **充分性评价**：理论推导逻辑严密，但示例偏少且未提供实际神经数据验证。结论依赖于慢噪声假设的成立，缺乏对快速噪声场景下递归作用的数值量化。作为理论框架提出可行，但作为实验验证不够充分。

### 6. 论文的主要结论与发现
- **核心结论**：在慢时间相关噪声下，神经流形的信息几何（费希尔信息）由前馈连接完全决定，递归连接仅起到选择性降噪作用（只在快噪声下改善编码）。
- **具体发现**：
  - 前馈连接足以生成结构化的空间表示（如六边形网格细胞形成的环面流形），无需递归吸引子。
  - 随机分布的网格相位即可使流形近似等距于物理空间（即空间编码的度量保持）。
  - 递归连接在快噪声下可抑制噪声方差，提高刺激可分辨性。

### 7. 优点
- **理论创新性**：首次将微分几何中的拉回度量与神经群体编码的费希尔信息统一，建立连接几何与编码的桥梁。
- **简洁性**：推导出慢噪声下递归抵消的简洁结论，为此后实验验证提供可检验预测。
- **挑战传统观点**：通过反例（线性前馈可生成六边形网格细胞）削弱了连续吸引子模型的必要性，具有理论颠覆性。

### 8. 不足与局限
- **缺乏数值验证**：未通过计算机模拟验证理论预测在不同网络参数、噪声特性下的鲁棒性。
- **假设限制**：慢时间相关噪声假设可能不适用于所有脑区（如感觉皮层常见快速噪声）；非线性网络（如阈值非线性）下的推导是否依然成立未讨论。
- **应用范围**：主要针对速率模型，未扩展到尖峰神经元或突触可塑性；示例仅涉及空间编码，未推广到其他认知功能（如方向、颜色）。
- **偏差风险**：所选示例（六边形网格细胞）可能具有特殊性质（如周期性、低维性），结论能否推广到更复杂的流形（如视觉皮层中的对象表示）存疑。

（完）
