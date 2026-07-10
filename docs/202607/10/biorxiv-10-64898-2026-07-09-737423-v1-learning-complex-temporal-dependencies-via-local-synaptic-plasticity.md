---
title: Learning complex temporal dependencies via local synaptic plasticity
title_zh: 通过局部突触可塑性学习复杂的时间依赖性
authors: "Ng-Kee-Kwong, J., Tang, M., Akam, T., Bogacz, R."
date: 2026-07-10
pdf: "https://www.biorxiv.org/content/10.64898/2026.07.09.737423v1.full.pdf"
tags: ["query:comp-neuro"]
score: 8.0
evidence: 局部突触可塑性学习时间依赖关系
tldr: 人类大脑能提取时间结构，但用于训练循环神经网络的反向传播通过时间（BPTT）缺乏生物合理性。本文研究时间预测编码（tPC），一种基于局部可塑性学习时间依赖的框架。发现tPC等价于单步BPTT，能利用储备池动力学编码短期上下文，并通过层次结构增强对复杂依赖和干扰的鲁棒性。引入资格痕迹后，tPC可解决长时延任务。结果表明局部可塑性足以在复杂场景中学习时间结构。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-09-737423-v1/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1040, \"height\": 667, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-09-737423-v1/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1236, \"height\": 1229, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-09-737423-v1/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1209, \"height\": 1491, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-09-737423-v1/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1253, \"height\": 1071, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-09-737423-v1/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1221, \"height\": 876, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-09-737423-v1/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1214, \"height\": 1420, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-09-737423-v1/fig-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 1212, \"height\": 723, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-09-737423-v1/fig-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 1283, \"height\": 923, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-09-737423-v1/fig-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 567, \"height\": 616, \"label\": \"Figure\"}]"
tables_json: "[{\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-07-09-737423-v1/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 741, \"height\": 404, \"label\": \"Table\"}, {\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-07-09-737423-v1/table-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1389, \"height\": 397, \"label\": \"Table\"}, {\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-07-09-737423-v1/table-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 930, \"height\": 441, \"label\": \"Table\"}]"
motivation: 探索生物合理的局部突触可塑性如何学习复杂时间依赖关系。
method: 扩展时间预测编码（tPC）框架，分析其与BPTT、储备池计算、e-prop等模型的关系。
result: tPC与单步BPTT功能等价；利用储备池动力学编码短期上下文；层次结构提升复杂依赖学习与抗干扰能力；资格痕迹扩展至长时任务。
conclusion: 局部可塑性驱动的简单递归网络能有效学习复杂时间结构，具有生物合理性。
---

## 摘要
跨不同任务提取和利用时间结构的能力是人类认知的核心。神经科学家通常在建模决策和运动控制等神经和行为过程时，依赖通过时间反向传播（BPTT）训练的循环神经网络（RNN）。然而，该算法的生物学合理性有限，因此时间依赖性高效学习的计算原理仍未解决。在这里，我们研究了时间预测编码（tPC），这是一个最近提出的框架，它将预测编码扩展到时间域，同时保留局部赫布更新规则。我们分析并扩展了tPC，以建立其与几种有影响力的RNN学习计算模型（包括BPTT、储层计算和资格传播（e-prop））的关系。我们首先证明了tPC与tBPTT1（BPTT的一种变体，其中梯度仅向过去传播一个时间步）之间的功能等价性。然后我们展示了tPC可以利用储层动力学来编码短程时间上下文，同时塑造状态空间中的神经轨迹以支持下游读出。我们进一步证明了层次循环动力学可以促进更复杂时间依赖性的学习，同时赋予对强干扰物的鲁棒性。最后，我们展示了tPC网络可以通过生物学启发的资格迹进行增强，以解决时间上扩展的上下文相关任务。综合这些结果，揭示了由局部可塑性支配的相对简单的循环网络可以支持比以前认为的更复杂设置下的时间学习。

## Abstract
The ability to extract and exploit temporal structure across diverse tasks is central to human cognition. Neuroscientists have typically relied on recurrent neural networks (RNNs) trained with backpropagation through time (BPTT) when modelling neural and behavioural processes such as decision-making and motor control. However, this algorithm has limited biological plausibility, hence the computational principles underlying efficient learning of temporal dependencies remain unresolved. Here, we investigate temporal predictive coding (tPC), a recently proposed framework that extends predictive coding to the temporal domain while preserving local Hebbian update rules. We analyse and extend tPC to establish its relationship with several influential computational models of learning in RNNs, including BPTT, reservoir computing, and eligibility propagation (e-prop). We first demonstrate a functional equivalence between tPC and tBPTT1, a variant of BPTT in which gradients are propagated only one time step into the past. We then show that tPC can leverage reservoir dynamics to encode short-range temporal context, and simultaneously sculpt neural trajectories in state space to support downstream readout. We further demonstrate that hierarchical recurrent dynamics can facilitate learning of more complex temporal dependencies, while additionally conferring robustness to strong distractors. Finally, we show that tPC networks can be augmented with biologically inspired eligibility traces to solve temporally extended context-dependent tasks. Together, these results reveal that relatively simple recurrent networks governed by local plasticity can support temporal learning in more complex settings than previously appreciated.

---

## 论文详细总结（自动生成）

好的，请查收以下基于您提供的论文内容生成的结构化、深入、客观的中文总结。

---

### 1. 论文的核心问题与整体含义（研究动机和背景）

- **核心问题**：人类大脑能够高效地学习并利用复杂的时序依赖信息（如语言理解、运动控制）。计算神经科学通常使用通过时间反向传播（BPTT）训练的循环神经网络（RNN）来模拟这一过程。然而，BPTT算法在生物学上是不合理的，因为它要求精确存储过去的状态并将误差信号反向传播，这在生物神经元中难以实现。因此，论文旨在探索一种基于局部突触可塑性的、更符合生物合理性的学习框架，来解决复杂时序依赖的学习问题。
- **整体含义**：论文研究并扩展了“时间预测编码（tPC）”框架。该框架继承了预测编码理论，同时在时间域上进行扩展，并仅依赖局部的赫布（Hebbian）更新规则。通过一系列实验，论文证明这种相对简单的生物合理性网络能够学习比以前认为的更复杂的时序结构和任务，为理解大脑如何实现时序学习提供了新的计算视角。

### 2. 论文提出的方法论：核心思想、关键技术细节

- **核心思想**：将预测编码框架扩展到时间域，构建一个生成式模型。该模型假设世界由一个隐藏状态序列驱动，观察结果由这些隐藏状态生成。学习过程通过最小化一个由“时序预测误差”和“感官预测误差”组成的自由能F_t来实现。
- **关键技术细节**：
    1.  **模型架构**：tPC网络包含“价值神经元”（编码隐藏状态和观测估计）和“误差神经元”（编码预测误差）。
    2.  **自由能目标**：
        F_t = 1/2 || z_t - f(Az_{t-1} + Bx_t) ||^2 + 1/2 || y_t - Cz_t ||^2
        - 第一项：时序预测误差（当前推断状态z_t与基于过去状态和输入预测的状态的差异）。
        - 第二项：感官预测误差（当前观测y_t与基于推断状态预测的观测的差异）。
    3.  **学习与推理的交替**：
        - **推理**：通过梯度下降优化自由能，更新隐藏状态z_t（公式4）。
        - **学习**：通过梯度下降优化自由能，更新权重矩阵A、B、C（公式5-7）。
        - **关键特性**：这些权重更新规则（公式5-7）完全是**局部的**，只依赖于突触前后神经元的可用信息，符合生物合理性。
    4.  **算法等价性**：论文从理论上证明了tPC的权重更新规则在形式上等价于单步截断的BPTT（tBPTT1），即梯度只向过去传播一个时间步。
    5.  **关键区别**：与标准RNN不同，tPC的推理过程（状态更新）允许观测信息直接流入隐藏状态（见公式17），这为其带来了信息优势。
    6.  **架构扩展**：
        - **层次化tPC (tPC-H)**：引入多层递归动力学，高层的隐藏状态依赖于低层的当前和过去状态，从而在多个时间尺度上整合信息。
        - **资格痕迹tPC (tPC-E)**：引入泄漏积分和指数衰减的资格轨迹（e_t），代替瞬时活动，使得长时间之前的活动能与当前的误差信号耦合，实现长期信用分配。

### 3. 实验设计：数据集/场景、基准测试、对比方法

- **任务场景（数据集）**：
    1.  **位置估计任务**：根据速度输入预测粒子位置。用于证明tPC与标准RNN在状态更新上的差异。
    2.  **交替二态任务**：预测一个由0和1构成的交替序列（块长为2或4）。用于测试学习**非马尔可夫序列**的能力。
    3.  **延迟奇偶校验任务**：计算输入序列中“1”个数的奇偶性（3-bit和4-bit）。用于测试学习**复杂跨时间交互**的能力。
    4.  **干扰任务**：模型接收线索-干扰-提示符，要求在线索后重现最初线索。用于测试模型对**强干扰**的鲁棒性。
    5.  **延迟响应任务**：模型接收初始线索，经过一段可变延迟后，要求重现该线索。用于测试**长时延任务**的学习能力。
- **基准测试与对比方法**：
    - **BPTT / tBPTT**：标准通过时间反向传播及其变体tBPTT1、tBPTT3等，作为性能上界和主要比较对象。
    - **储层计算（Reservoir Computing）**：一个RNN作为固定随机储层，只训练读出层。
    - **资格传播（e-prop）**：基于资格轨迹的生物合理性RNN学习算法。
    - **RFLO (Random Feedback Local Online)**：一个具有生物合理性的局部在线学习算法。
    - **RNN-P**：将前一步的观测作为显式输入的标准RNN。
    - **tPC** 和 **tPC-P**：时间预测编码及其接收前一步观测信息的变体。

### 4. 资源与算力

- **未明确说明**：论文中并未明确提及所使用的GPU型号、数量和训练时长。仅提到使用了牛津大学的Advanced Research Computing (ARC) 设施。

### 5. 实验数量与充分性

- **实验数量**：论文在**五大类任务场景**上进行了实验，涵盖了从简单动力学模拟到复杂的奇偶校验、抗干扰和长时延任务。每个实验通常使用了**至少5个随机种子**，有的达到20个，并计算了均值和标准误差，保证了统计可靠性。
- **充分性**：实验设计**非常充分且公平**。
    - **对比全面**：在每个任务上都与相关的基线方法（如BPTT、e-prop、RFLO）进行了比较，清晰地展示了tPC及其变体的性能位置和特点。
    - **消融分析**：通过tPC-H与单层tPC的比较，验证了层次结构的作用；通过tPC-E与标准tPC的比较，验证了资格痕迹的作用。此外，“重置隐藏状态”的控制实验也证明了记忆的必要性。
    - **参数控制**：在可比较的实验中（如Fig4和Fig5），模型参数数量被匹配，以进行公平对比。
- **客观性**：实验结果表明tPC在某些任务上（如位置估计、抗干扰）表现优异，但在某些方面（如长时延任务相比e-prop，复杂奇偶任务相比长截断BPTT）存在差距，作者对此进行了客观的描述和讨论。

### 6. 论文的主要结论与发现

1.  **功能等价性**：tPC的权重更新规则在形式上等同于tBPTT1（单步截断BPTT）。关键区别在于tPC的推理过程引入了从观测到隐藏状态的直接信息流，使其在信息利用上更具优势。
2.  **储层效应与状态塑造**：tPC可以利用其递归结构作为储层来编码短期时间上下文。同时，通过局部可塑性训练权重，tPC能够重塑其在状态空间中的神经轨迹，使其更好地支持下游读出，性能优于固定储层。
3.  **层次结构优势**：层次化tPC（tPC-H）通过在不同时间尺度的隐层间进行交互，能够更有效地学习复杂的跨时间依赖（如延迟奇偶校验），并对强干扰具有更强的鲁棒性。
4.  **资格痕迹的价值**：通过引入生物启发的资格痕迹，tPC-E可以成功学习需要长时间延迟的任务（如延迟响应），而标准tPC则无法胜任。
5.  **整体结论**：该研究揭示了，仅依赖于局部突触可塑性的相对简单的递归网络，能够在比以往认为的更复杂的环境中支持时间学习。这为理解生物大脑如何高效进行时序信用分配提供了有力的计算模型基础。

### 7. 优点：方法或实验设计上的亮点

1.  **生物合理性**：整个方法（tPC、tPC-H、tPC-E）的核心都坚持使用局部的、赫布式的学习规则，极大地增强了模型的生物学可解释性。
2.  **理论清晰与实证结合**：论文不仅从理论上推导了tPC与tBPTT1的等价性（结果1），还通过一系列精心设计的实验来验证和揭示tPC的特性（储层效应、层次优势、资格痕迹作用），理论与实证相互印证。
3.  **系统性的框架扩展**：论文不是在真空中分析tPC，而是将其与储层计算、BPTT、e-prop等主流框架系统地联系起来，并在此基础上提出了层次化和资格痕迹这两种有效的扩展方案，构成了一个完整的算法谱系。
4.  **问题驱动**：实验设计很有针对性，每个任务都是为了回答一个特定问题（能否学非马尔可夫序列？层级结构是否有用？干扰如何？长时延怎么解决？），这使得结论非常清晰有力。

### 8. 不足与局限

1.  **离散时间近似**：论文承认，其对层次化tPC（tPC-H）的实现采用了离散时间，未能完全满足预测编码理论中对连续时间延迟的精确处理要求。
2.  **参数设置的简化**：在tPC-E中使用了固定的泄漏参数（α=0.5），而生物系统中时间常数是高度异质的。
3.  **任务规模**：所有实验都基于相对简单、低维的玩具任务。论文本身也指出了将方法扩展到更高维度输入和更丰富行为场景的必要性。
4.  **与SOTA算法的差距**：在延迟奇偶校验任务上，tPC-H需要多层才能赶上tBPTT3的性能。在长时延任务上，tPC-E的收敛速度慢于e-prop，而RFLO无法处理更长延迟。这表明tPC在复杂任务上还有性能提升空间。
5.  **性能偏差风险**：在训练tPC时，使用了额外的推理循环，这虽然提供了更多信息，但也可能增加计算开销，实验中没有详细比较与BPTT在计算时间上的差异。

---

（完）
