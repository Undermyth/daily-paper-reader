---
title: Diffusion Latent Representations for Neural Decoding
title_zh: 用于神经解码的扩散潜在表示
authors: "Wong, B., Laschowski, B."
date: 2026-07-13
pdf: "https://www.biorxiv.org/content/10.64898/2026.07.08.737343v1.full.pdf"
tags: ["query:comp-neuro"]
score: 8.0
evidence: 扩散潜在表示用于神经解码
tldr: "神经解码可视为表示学习问题，中间表示的选择对下游性能至关重要。本文提出一个系统研究框架，以扩散模型不同时间步的潜变量作为中间表示进行神经语音解码。实验发现，不同时间步对应的重建性能差异显著，教师强制词错误率从44.7%降至3.5%。该框架证明扩散潜变量的有效性依赖于时间步选择，为研究中间表示的影响提供了基础。"
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-08-737343-v1/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1864, \"height\": 1043, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-08-737343-v1/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1837, \"height\": 1094, \"label\": \"Figure\"}]"
tables_json: "[{\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-07-08-737343-v1/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 931, \"height\": 193, \"label\": \"Table\"}, {\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-07-08-737343-v1/table-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 929, \"height\": 159, \"label\": \"Table\"}]"
motivation: 神经解码中中间表示的选择对下游学习和重建性能有重要影响，但缺乏系统比较的方法。
method: 提出框架，利用扩散模型不同时间步的潜变量作为中间表示，在神经语音解码任务中评估其效果。
result: "不同扩散时间步的潜变量导致词错误率显著不同，最优时间步达到3.5%的错误率，远优于其他时间步。"
conclusion: 扩散潜变量可作为有效的中间表示，但其性能强烈依赖于时间步选择；该框架为系统研究表示选择提供基础。
---

## 摘要
神经解码可被视为一个表示学习问题，其中神经活动在下游重建之前被映射到中间表示。中间表示的选择影响性能和学习的难度。这里我们开发了一个新框架，用于研究中间表示选择如何影响下游学习和重建。作为概念验证，我们使用从不同扩散时间步提取的扩散潜在表示进行神经语音解码，实例化了我们的框架。逐分量评估显示，不同扩散时间步的重建性能差异显著，不同潜在模型的教师强制词错误率分别为44.7%、7.5%和3.5%。这些结果表明，扩散潜在表示可以作为从神经活动中学习的有效中间表示，但其有效性强烈依赖于所选扩散时间步。更广泛地说，我们的框架为系统研究中间表示选择如何影响下游学习和重建提供了基础。

## Abstract
Neural decoding can be viewed as a representation learning problem in which neural activity is mapped into an intermediate representation before downstream reconstruction. The choice of intermediate representation influences both performance and learning difficulty. Here we developed a novel framework for studying how intermediate representation choice influences downstream learning and reconstruction. As a proof-of-concept, we instantiated our framework using diffusion latent representations extracted from different diffusion timesteps for neural speech decoding. Component-wise evaluation showed that reconstruction performance differed substantially across diffusion timesteps, with teacher-forced Word Error Rates of 44.7%, 7.5%, and 3.5% for different latent models. These results demonstrate that diffusion latent representations can serve as effective intermediate representations for learning from neural activity, but that their effectiveness depends strongly on the selected diffusion timestep. More broadly, our framework provides a basis for systematically studying how intermediate representation choice influences downstream learning and reconstruction.

---

## 论文详细总结（自动生成）

# 详细中文总结

## 1. 论文的核心问题与整体含义（研究动机和背景）

神经解码可以视为表示学习问题：神经信号被映射为中间表示，再由下游解码器重建目标信号。中间表示的选择直接影响重建性能和学习难度。然而，现有研究多聚焦于单一表示，缺乏系统比较不同中间表示影响的方法。本文旨在提出一个通用框架，以研究中间表示选择如何影响下游学习和重建，并以扩散潜在表示在神经语音解码中的表现为概念验证案例。

## 2. 论文提出的方法论：核心思想、关键技术细节、公式或算法流程

### 核心思想
将神经解码分解为三个步骤：(1) 从目标信号中生成中间表示（扩散潜在变量及条件因子）；(2) 从神经活动预测这些中间表示；(3) 使用冻结的扩散模型重建目标信号。

### 关键技术细节
- **扩散模型**：使用DiffWave（T=6时间步），条件因子为Mel频谱图。
- **潜在变量提取与分词化**：对每个扩散时间步 i 的潜在变量 z_i，使用EnCodec（J=4个RVQ码本，每码本1024项）进行残差向量量化（RVQ），得到分词化序列 V_i。
- **编码器**：两个Transformer编码器-解码器模型：
  - **潜在模型**：自回归预测所有J个RVQ码本索引，使用交叉熵损失。
  - **条件因子模型**：用线性投影层回归连续Mel频谱图，使用MSE损失；包含终止概率头。
- **解码器**：将预测的分词化潜在变量解码回连续变量 z'_i，再与预测的条件因子 M' 一起输入冻结的DiffWave进行逆向扩散（公式1），迭代去噪重建信号。

### 训练流程
- 冻结扩散模型，仅优化编码器。
- 分别训练条件因子模型和三个潜在模型（对应i=1,2,3），每个潜在模型学习特定时间步的表示。
- 超参数：隐藏层128，4层Transformer，2头注意力，Adam优化器，学习率5e-4，batch size 128，100 epoch，无学习率调度或dropout。

## 3. 实验设计：数据集、基准、对比方法

- **数据集**：采用脑机语音解码竞赛数据集（Brain-to-Text '25），包含一位植入256电极微阵列的参与者的皮层内记录。神经活动以20ms非重叠窗口分箱，提取阈值交叉和频谱带功率特征，每时间步512维。训练/验证分割7849/1409个句子对。
- **基准**：与先前研究（Card et al., 2024，发表于NEJM）的脑机语音神经假体结果对比（该研究使用自回归生成，WER 6.3%）。
- **对比方法**：论文自身设计了三种不同扩散时间步的潜在模型（1/2/3）以及条件因子模型，进行分量评估和端到端评估。

## 4. 资源与算力

论文明确注明：所有模型使用PyTorch实现，通过DistributedDataParallel在四块NVIDIA H100 GPU上训练。

## 5. 实验数量与充分性

- **实验组**：共训练4个模型（1个条件因子模型 + 3个潜在模型），在验证集上进行了：
  - 分量评估：分别对每个模型进行教师强制（teacher-forced）测试。
  - 端到端评估：结合条件因子模型和最佳潜在模型（模型3），在教师强制和完全自回归两种模式下测试。
- **消融实验**：通过比较不同扩散时间步的潜在表现，本质上是一种消融实验。
- **充分性**：实验设计较为清晰，但仅使用了单一数据集、单一扩散模型（DiffWave）和单一任务（神经语音解码）。未进行多任务、多模态或多模型对比，也未深入分析表示统计/几何性质。公平性：与Card et al. (2024)的结果对比，但后者使用了不同脑机接口设备和训练数据，直接比较需谨慎。

**总体评价**：实验数量有限，但作为概念验证论文，基本覆盖了研究目标。不过，缺乏对表示可学习性背后的数学/统计特性的深入探讨。

## 6. 论文的主要结论与发现

- **表示选择强烈影响重建性能**：教师强制WER在潜在模型1/2/3中分别为44.7%、7.5%、3.5%，条件因子模型为3.5%。后期扩散时间步（i=3）优于早期时间步。
- **扩散潜在表示可作为有效中间表示**：最佳潜在模型（模型3）与条件因子模型性能持平。
- **端到端自回归生成存在严重误差累积**：完全自回归生成WER达125.3%，而教师强制仅4.6%，说明序列预测是主要瓶颈。
- **训练损失收敛不等于表示有效性**：尽管所有模型损失稳定收敛，但不同时间步的WER差异显著，表明低损失不代表下游重建性能好。

## 7. 优点

- **创新性**：首次系统比较不同扩散时间步潜在表示对神经解码的影响，提出通用研究框架。
- **可扩展性**：框架适用于不同条件扩散架构和多种神经解码任务（不限于语音）。
- **技术整合**：巧妙结合扩散模型、RVQ分词、Transformer编码器，实现从神经活动到潜在变量的预测。
- **实验设计**：通过分量评估和端到端评估分离表示贡献，清晰展示表示选择与误差来源。

## 8. 不足与局限

- **实验规模小**：仅使用单个参与者数据集，样本数量有限（约1.4k验证句），泛化性存疑。
- **任务单一**：仅测试了神经语音解码，未推广到图像解码或其他模态。
- **表示缺乏理论分析**：未深入解释为何后期时间步效果更好（仅推测“更多随机性允许扩散模型纠正误差”）。
- **自回归误差问题未解决**：端到端自回归WER极高，表明当前框架在实际部署中不可行。
- **对比基线弱**：仅与一篇先前研究比较，且该研究使用不同方法（直接解码词汇而非中间表示），公平性有待验证。
- **计算成本高**：需要为每个扩散时间步单独训练潜在模型，扩展性受限于时间步数量。
- **未评估不同扩散模型**：仅使用DiffWave，结论对更大/更新的扩散模型（如Stable Audio）可能不成立。

（完）
