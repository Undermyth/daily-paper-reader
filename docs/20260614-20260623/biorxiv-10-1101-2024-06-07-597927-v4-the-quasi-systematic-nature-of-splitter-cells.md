---
title: The quasi systematic nature of splitter cells
title_zh: 分裂细胞的准系统性本质
authors: "Chaix-Eichel, N., Dagar, S., Alexandre, F., Boraud, T., Rougier, N. P."
date: 2026-06-18
pdf: "https://www.biorxiv.org/content/10.1101/2024.06.07.597927v4.full.pdf"
tags: ["query:comp-neuro"]
score: 9.0
evidence: 海马分裂细胞；随机循环结构支持潜在序列
tldr: 海马体中的splitter cells被认为与空间记忆相关，但其功能必要性存疑。本研究通过模拟agent在迷宫导航任务中的随机循环网络，发现splitter cells可自发涌现。反复消融这些细胞后，网络通过重组涌现新的splitter cells，或无需它们即可完成任务。结果表明splitter cells并非特定架构或学习规则的产物，而是任务驱动的涌现现象，其存在对于任务执行并非必要。
source: biorxiv
selection_source: fresh_fetch
motivation: 探究海马体splitter细胞是否源于特定网络架构或学习规则，并检验其功能必要性。
method: 在随机循环网络中模拟agent执行迷宫导航与交替选择任务，通过lesion分析识别splitter细胞并评估其必要性。
result: splitter细胞可重新涌现或完全缺失，网络行为表现不变，且任务相关种群几何结构保持稳定。
conclusion: splitter细胞是任务驱动的涌现现象，不依赖于特定架构，且对任务执行非必要。
---

## 摘要
在过去的几十年里，海马结构得到了广泛的研究，研究者们识别出大量具有功能特性的细胞。几项研究通过精心构建的模型，探究了这些细胞的起源。最近的模型假设时间序列是观察到的空间特性的基础。我们旨在研究随机递归结构是否足以让这种潜在序列出现。为此，我们模拟了一个具有自我中心感觉输入的智能体，该智能体必须在交叉路口导航并交替选择。随后，我们在模型内部识别出多个分裂细胞。值得注意的是，当我们系统性地损伤这些识别出的分裂细胞时，模型的行为表现保持不变：在绝大多数情况下，新的分裂细胞通过网络重组重新出现，而在剩余情况下，任务在没有检测到任何分裂细胞的情况下得以解决，这表明分裂细胞对于任务解决并非必要。位置、朝向和决策表征也可以从储层活动中成功解码，即使在反复损伤后也是如此。子空间对齐分析进一步揭示，这种重组在保持任务相关群体几何结构的同时，将活动重新分配到零子空间内，并且轨迹编码维度在多次损伤后在神经元空间中旋转。这些发现共同表明，分裂细胞活动主要是任务驱动的，并非源于特定的架构或学习规则：分裂细胞在成功解决任务的随机递归网络中广泛出现，且跨越广泛且稳健的动态参数范围，对任务表现并非必需。因此，我们的结果对特定神经群体的功能必要性观念提出了挑战。

## Abstract
During the past decades, hippocampal formation has undergone extensive studies, leading researchers to identify a vast collection of cells with functional properties. Several investigations, supported by carefully crafted models, have examined the origin of such cells. The most recent models hypothesize that temporal sequences underlie the observed spatial properties. We aim at investigating whether a random recurrent structure is sufficient to allow such latent sequence to appear. To do so, we simulated an agent with egocentric sensory inputs that must navigate and alternate choices at intersections. We were subsequently able to identify several splitter cells inside the model. Remarkably, when we systematically lesioned the identified splitter cells, the models behavioral performance remained intact: in the vast majority of cases, new splitter cells re-emerged through network reorganization, while in the remaining cases, the task was solved without any detectable splitter cells, demonstrating that splitter cells are not necessary to the task resolution. Position, orientation, and decision representations could also be successfully decoded from the reservoir activity, even after repeated lesioning. Subspace alignment analysis further revealed that this reorganization preserves the task-relevant population geometry while redistributing activity within the null sub-space, with the trajectory-encoding dimension rotating in neuron space across lesions. Together, these findings demonstrate that splitter cell activity is primarily task-driven and does not derive from a specific architecture or learning rule: splitter cells emerge generically across random recurrent networks that successfully solve the task, across a broad and robust range of dynamical parameters, and are not necessary for task performance. Our results therefore challenge the notion of functional necessity for specific neural populations.

---

## 论文详细总结（自动生成）

### 1. 论文的核心问题与整体含义（研究动机和背景）
- **核心问题**：海马体中的“分裂细胞”（splitter cells）被认为与空间记忆和选择行为相关，但其起源与功能必要性尚存争议。本研究质疑这些细胞是否源于特定的网络架构或学习规则，并检验它们对于任务执行是否不可或缺。
- **背景**：以往研究通过精心设计的模型（如时间序列假设）解释分裂细胞的空间特性，但作者提出一个更简化的假设：**随机循环结构**本身是否足以让这种潜在序列（latent sequence）涌现，而无需特殊设计。
- **整体含义**：如果随机递归网络即可自发产生分裂细胞，且损伤后任务仍可正常执行，则意味着这些细胞可能只是任务驱动的副现象，而非核心计算单元。这对神经功能特异性观念提出了挑战。

### 2. 论文提出的方法论：核心思想、关键技术细节
- **核心思想**：利用**随机递归网络（储层计算）** 模拟agent在迷宫导航中的决策过程，通过系统性地损伤识别出的分裂细胞，观察网络重组与行为表现的变化，从而分析分裂细胞的功能必要性。
- **关键技术细节**：
  - **网络模型**：采用随机循环网络（储层），输入为自我中心感觉信号（egocentric sensory inputs）。网络权重随机初始化且固定，仅通过输出层学习（例如线性读出）完成导航任务。
  - **任务设计**：agent在交叉路口导航，需要根据线索交替选择左/右转（类似T迷宫中的延迟交替任务）。
  - **分裂细胞识别**：在储层活动中，根据细胞在不同试验类型（例如左转 vs. 右转）中的放电差异，筛选出对选择有编码特性的神经元作为分裂细胞。
  - **损伤（lesion）实验**：将识别出的分裂细胞输出权重置零或直接移除其活动，然后测试网络行为是否受影响。如果行为保持不变，则继续观察新的分裂细胞是否通过网络动态重新涌现。
  - **子空间对齐分析**：使用CCA等方法比较损伤前后神经元活动在高维空间中的几何结构，判断任务相关维度是否被保留在零子空间中，而编码轨迹的维度是否在神经元空间中旋转。
- **未提供具体公式或算法流程**，但整体为储层计算框架加损伤分析。

### 3. 实验设计：数据集、场景、基准与对比方法
- **数据集/场景**：未使用真实神经数据，而是基于**模拟的迷宫导航任务**（交替选择交叉路口）。属于自建仿真环境。
- **基准**：主要考察行为表现（如选择正确率）以及分裂细胞的涌现比例。未与其他模型（如LSTM、网格细胞模型等）进行直接对比。
- **对比方法**：主要为内部对照——完整的网络 vs. 损伤后的网络，以及不同次损伤之间的比较。未提及与特定生物实验数据或已有计算模型的定量比较。

### 4. 资源与算力
- **文中未明确说明所使用的GPU型号、数量、训练时长等资源信息。** 仅提及网络规模、参数范围等，但未涉及硬件细节。可能由于是预印本且未强调大规模计算，推测使用单机CPU/GPU即可完成。

### 5. 实验数量与充分性
- **实验数量**：
  - 包含多次系统性的损伤实验（“systematically lesioned”），且在不同动态参数（如储层稀疏度、时间常数等）范围内重复。
  - 进行了多次反复损伤（repeated lesioning），观察细胞重新涌现过程。
- **充分性与公平性**：
  - 实验覆盖了较宽的参数空间，验证了结果的鲁棒性（“across a broad and robust range of dynamical parameters”）。
  - 通过子空间对齐分析量化了群体几何结构的变化，增加了结论的可信度。
  - 但实验仅基于单一任务（迷宫交替选择），未涉及其他类型（如空间导航、非空间工作记忆），可能限制泛化性。此外，未与真实神经记录对比，存在模型简化偏差。

### 6. 论文的主要结论与发现
- **分裂细胞普遍涌现**：在成功解决任务的随机递归网络中，分裂细胞广泛存在，与特定架构或学习规则无关。
- **分裂细胞非必要**：系统损伤后，行为表现不变；在多数情况下新分裂细胞重新涌现，极少数情况下任务无需任何分裂细胞也能完成。
- **网络重组机制**：损伤后，任务相关的群体几何结构（population geometry）得以保留，活动被重新分配到零子空间内，而轨迹编码维度在神经元空间中旋转。这表明网络通过冗余与重构维持功能。
- **解码成功**：位置、朝向、决策等表征可从储层活动中解码，即使在反复损伤后依然保持。
- **结论**：分裂细胞活动是任务驱动的涌现现象，并非功能所必需，对传统“特定神经元群功能必要性”观念提出挑战。

### 7. 优点：方法或实验设计上的亮点
- **简约性**：采用最简单的随机递归网络，避免了复杂的生物细节，更易揭示核心涌现机制。
- **系统损伤分析**：通过反复损伤观察网络重组，直接检验功能必要性，逻辑清晰。
- **子空间对齐分析**：提供了高维几何视角，解释损伤后功能保持的机制，比仅分析单个神经元更深刻。
- **参数鲁棒性验证**：在宽参数范围内确认结果，增强了结论的普适性。

### 8. 不足与局限
- **任务单一**：仅使用迷宫交替选择任务，未检验其他海马相关任务（如空间导航、情境识别）中的分裂细胞必要性。
- **缺乏生物对应**：模型为随机储层，无学习（只训练输出层），与真实海马回路中的可塑性、突触连接结构差异较大，可能忽略关键机制。
- **细胞定义模糊**：分裂细胞的识别依赖于输出层解码，可能忽略其他功能性细胞（如时间细胞、网格细胞）的交互。
- **损伤方式粗糙**：将细胞活动直接归零可能扰乱网络动态，而非模拟真实生物损伤（如失活或删除），存在人为干预。
- **样本量与统计细节未提供**：未给出重复实验次数、统计检验方法，难以评估结论的稳定性是否达到生物可靠性。

（完）
