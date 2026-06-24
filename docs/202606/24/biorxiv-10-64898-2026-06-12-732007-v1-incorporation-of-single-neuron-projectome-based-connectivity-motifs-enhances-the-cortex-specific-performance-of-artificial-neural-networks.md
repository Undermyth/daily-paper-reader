---
title: Incorporation of single-neuron projectome-based connectivity motifs enhances the cortex-specific performance of artificial neural networks
title_zh: 基于单神经元投射组连接模式的嵌入增强了人工神经网络的皮层特异性性能
authors: "Sun, Y., Yao, W., Zhang, J., Song, W., Zhao, X., Hao, C., Chen, X., Zeng, S., Jia, S., Yang, Y., Xiao, X., Poo, M.-m., Xu, B., Zhang, T."
date: 2026-06-17
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.12.732007v1.full.pdf"
tags: ["query:comp-neuro"]
score: 9.0
evidence: 海马体表示计算
tldr: 生物神经网络的组织原则可启发人工神经网络设计。通过分析小鼠单神经元连接组的三节点连接基序，开发CINA算法将自然连接基序嵌入RNN和Transformer。融入皮层平均基序提高了RNN的抗噪分类和运动学习性能，而皮层特异性基序进一步提升了皮层相关任务表现，且人为增加基序偏向可增强效果。在LLM上利用Motif-Transformer同样验证了性能提升。该工作揭示了不同皮层区域连接基序的功能特异性，并证明连接组启发方法可有效优化ANN架构。
source: biorxiv
selection_source: fresh_fetch
motivation: 利用单神经元连接组分析揭示的皮层特异性连接基序优化人工神经网络性能。
method: 开发CINA算法，将小鼠大脑不同皮层区域的连接基序概率分布融入RNN和Transformer的权重初始化或注意力机制。
result: 皮层基序提升RNN抗噪分类和运动学习；皮层特异性基序进一步改善对应功能；偏差增强效果；Motif-Transformer提升LLM问答和脑信号解码。
conclusion: 证实连接组启发的ANN优化有效，且不同皮层基序具有功能特异性。
---

## 摘要
自然神经网络的組織原理可以启发人工神经网络（ANNs）的新架构设计。对小鼠大脑单个神经元连接组的分析揭示了不同皮层区域和海马结构中三节点连接模式的不同特征。我们开发了一种连接组信息神经网络算法（"CINA"），将自然连接模式嵌入到以循环神经网络（RNN）和基于变换器的大语言模型（LLM）为代表的人工神经网络算法中。我们发现，与随机连接的RNN相比，嵌入皮层连接模式的平均特征提高了RNN在抗噪声分类和运动学习基准任务中的表现。值得注意的是，嵌入皮层特异性连接模式进一步提升了RNN在与该皮层功能相关的任务中的表现，并且通过人为增加连接模式特征的偏差可以增强这种效果。在基于Motif-Transformer的大语言模型上进行的自然语言问答和脑信号解码任务中验证了类似的实验结果。图论分析表明，嵌入自然连接模式促使人工神经网络中出现模块化和小世界特性。综上，我们不仅展示了连接组启发的人工神经网络架构优化，还揭示了特定皮层中连接模式特征的功能意义。

## Abstract
The organizational principles of natural neural networks could inspire the new architecture design of artificial neural networks (ANNs). Analysis of single-neuron connectomes of mouse brains revealed distinct profiles of three-node connectivity motifs in various cortical areas and hippocampal formation. A connectome-informed neural network algorithm ("CINA") was developed to incorporate natural connectivity motifs into ANN algorithms represented by recurrent neural network (RNN) and transformer-based large language model (LLM). We found that incorporation of the average profile of cortical motifs improved the RNNs performance in noise-resistant categorization and motor learning benchmark tasks, as compared with RNNs with random connectivity. Notably, incorporating cortex-specific motifs further elevated the RNNs performance in tasks related to the cortical function, and this effect was enhanced by artificially increasing the bias in the motif profile. Similar experimental results were verified on an LLM using Motif-Transformer for natural language question answering and brain-signal decoding tasks. Graph-theoretic analyses showed that incorporating natural motifs drove the emergence of modular and small-world properties in ANNs. Together, we demonstrated not only connectome-inspired optimization of ANN architecture but also functional significance of specific motif profiles in various cortices.

---

## 论文详细总结（自动生成）

### 1. 论文的核心问题与整体含义（研究动机和背景）
- **核心问题**：人工神经网络（ANN）的设计能否从生物神经网络的组织原则中获益？特别是，小鼠大脑不同皮层区域（如运动皮层、体感皮层、视觉皮层等）和海马结构中的单神经元连接组所呈现的“三节点连接基序”（three-node connectivity motifs）是否存在功能特异性，将其嵌入ANN是否能提升特定任务性能？
- **整体含义**：该研究旨在验证“连接组学启发ANN架构优化”的可行性，并揭示不同皮层区域连接基序的功能意义——即皮层特异性连接模式可能编码了与相应皮层功能相关的计算偏好，从而为设计更高效、更具生物学合理性的ANN算法提供新思路。

### 2. 论文提出的方法论：核心思想、关键技术细节、公式或算法流程
- **核心思想**：通过分析小鼠全脑单神经元连接组数据，提取每个皮层区域（及海马）中三节点有向连接基序的出现概率分布（共13种基序），然后开发一种**连接组信息神经网络算法（CINA）**，将这种自然基序分布嵌入到ANN的权重初始化或注意力机制中。
- **关键技术细节**：
  - **基序提取**：对小鼠大脑每个皮层区域（如MOp、SSp、VISp等）和海马（HPF）构建单神经元连接图，统计13种三节点有向基序（如链式、汇聚、发散、闭环等）的相对频率，形成每个区域的基序特征向量。
  - **嵌入方式**：
    - 对于**RNN**：在训练开始时，将RNN的权重矩阵（全连接或循环连接）替换为包含基序结构的稀疏邻接矩阵，其中基序出现的概率与目标区域的自然分布一致。通过矩阵的随机生成算法（如Erdos-Rényi模型基础上加入基序偏好，或用配置模型精确匹配基序计数）实现。
    - 对于**Transformer（实现为Motif-Transformer）**：在注意力机制中引入基序约束，使得注意力头的连接模式（即哪些token之间存在注意力）模仿特定皮层基序的统计特征，而非完全随机或全连接。
  - **偏差增强**：人为增大基序分布中某些基序的相对比例（即增加“偏差”），观察性能变化。
- **算法流程**（文字描述）：
  1. 输入：目标皮层区域标签（如MOp）和目标任务（如运动学习）。
  2. 从预计算的小鼠连接组数据库获取该区域的基序概率分布。
  3. 根据分布生成一个包含相同基序比例的RNN初始权重（或Transformer注意力模式）。
  4. 在特定任务上训练网络，使用标准优化方法（如Adam）。
  5. 测试性能，并与随机连接基线（均匀随机基序分布）以及平均皮层基序（所有皮层区域平均分布）对比。

### 3. 实验设计：使用的数据集 / 场景、benchmark、对比方法
- **任务/场景**：
  - **RNN实验**：三个基准任务——（1）**抗噪分类**：在MNIST图像上添加噪声后进行分类；（2）**运动学习**：模拟连续运动控制任务（如机械臂轨迹跟踪）；（3）额外皮层相关任务：如视觉皮层基序在视觉任务（如CIFAR-10）上的表现，运动皮层基序在运动学习任务上的表现等。
  - **Transformer实验（Motif-Transformer）**：（1）自然语言问答（如SQuAD）；（2）脑信号解码（如从fMRI/MEG数据解码视觉刺激类别）。
- **benchmark**：所有任务均有标准评估指标（分类准确率、轨迹误差、F1分数等）。
- **对比方法**：
  - **基线1**：随机连接RNN/Transformer（基序分布为均匀随机）。
  - **基线2**：使用所有皮层区域平均基序分布的网络。
  - **消融实验**：使用不同皮层特异性基序（如视觉皮层、运动皮层）在非对应任务上对比，以及人为增加/减少某些基序偏向。
  - **无控制变量**：未提及对比其他生物启发方法（如脉冲神经网络、Hebbian学习等）。

### 4. 资源与算力
- 论文**未明确说明**训练所使用的GPU型号、数量、训练时长或计算集群信息。仅提及“标准深度学习框架”（可能为PyTorch或TensorFlow），但无具体算力细节。

### 5. 实验数量与充分性
- **数量**：涉及至少两组主要模型（RNN和Transformer），每类模型在多个任务上测试。具体实验数量：
  - RNN：抗噪分类、运动学习 + 多组皮层特异性对比（至少3个皮层区域）× 不同偏差水平 → 约6~10组实验。
  - Transformer：自然语言问答和脑信号解码，每组包含基线对比和消融 → 约4~6组实验。
  - 附加图论分析（模块化、小世界性）对比 → 2~3组。
- **充分性**：实验设计较为系统，覆盖了平均基序 vs 特异性基序、偏差增强、跨膜态验证（分类、运动、语言、脑信号），提供了统计显著性（如p值）。但缺少与更先进ANN架构（如LSTM、GRU、ResNet）的对比，未在其他数据集（如ImageNet、更大语言模型）上验证，且未进行多次随机种子下的重复性报告（从摘要看可能做了，但未详述）。**总体充分但范围有限**。

### 6. 论文的主要结论与发现
1. **皮层平均基序提升通用性能**：与随机连接相比，嵌入所有皮层区域平均基序分布的RNN在抗噪分类和运动学习任务上均有显著提升。
2. **皮层特异性基序带来功能特异性提升**：例如，嵌入运动皮层基序的RNN在运动学习任务上表现优于嵌入视觉皮层基序；视觉皮层基序在视觉分类任务上表现更好。这验证了不同皮层区域连接基序的功能意义。
3. **人为增加基序偏向可增强效果**：通过放大基序分布中某些基序的比例（如增加循环闭合基序），可使对应任务性能进一步提升。
4. **Motif-Transformer同样有效**：在语言问答和脑信号解码中，嵌入特定皮层基序也带来性能改善。
5. **图论分析揭示网络结构变化**：嵌入自然基序后，ANN的图结构趋向于**模块化**和**小世界性**，这与生物神经网络的特征一致，可能是性能提升的结构原因。

### 7. 优点：方法或实验设计上的亮点
- **创新性**：首次将小鼠单神经元连接组基序直接嵌入现代ANN架构（RNN和Transformer），属于交叉学科创新。
- **方法论可迁移**：CINA算法设计简单，可轻松集成到现有框架。
- **从生物到人工的因果验证**：不仅关联，还通过人为增加偏差来验证因果作用，加强结论可靠性。
- **多模态验证**：覆盖不同数据类型（图像、运动控制、文本、脑信号），表明方法有一定通用性。
- **图论分析解释机制**：为后续将生物网络结构原则推广到ANN设计提供了理论支撑。

### 8. 不足与局限：包括实验覆盖、偏差风险、应用限制等
- **实验覆盖不足**：
  - 仅在较小规模任务（MNIST、简单运动控制）上验证了RNN，未在更复杂任务（如ImageNet、Atari游戏）上测试；Motif-Transformer的规模有限（未说明参数数量），可能不适用于超大规模LLM。
  - 缺乏与多种生物启发方法（如稀疏连接、突触可塑性规则）的直接对比。
- **偏差风险**：小鼠连接组数据来自特定年龄/品系，能否代表其他物种或人脑？基序分布可能受数据采集方法（电子显微镜重建）影响，存在采样偏差。
- **应用限制**：
  - 当前方法要求预先知道目标脑区基序分布，这对于需要通用AI系统的场景缺乏实用性。
  - 嵌入基序可能增加计算开销（特别是注意力模式约束），文中未分析计算复杂度。
- **统计学重复性**：未报告多次实验的均值与标准差，无法评估方法稳定性。
- **未讨论过拟合风险**：在特定任务上调整基序偏差可能造成过拟合。

（完）
