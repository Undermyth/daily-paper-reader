---
title: A two-stage algorithm underlies the transformation from vision to familiarity in the primate brain
title_zh: 灵长类大脑中视觉到熟悉性转化的两阶段算法
authors: "Bohn, S., Hacker, C. M., Jannuzi, B. G. L., Meyer, T., Hay, M., Rust, N. C."
date: 2026-07-03
pdf: "https://www.biorxiv.org/content/10.1101/2025.06.13.659490v3.full.pdf"
tags: ["query:comp-neuro"]
score: 9.0
evidence: 研究从视觉到熟悉度的两阶段转换，涉及ITC和海马体
tldr: 视觉图像如何转变为熟悉性记忆是认知神经科学的核心问题。通过利用图像记忆性差异，记录猕猴执行单次视觉熟悉任务时下颞叶皮层（ITC）和海马（HC）的神经活动，发现两阶段算法：首先ITC编码混合了记忆性和重复抑制的熟悉性信号，随后内侧颞叶从中提取出纯净的熟悉性表征。该发现揭示了视觉到熟悉性转换的机制，并首次描述内侧颞叶的新型计算功能。
source: biorxiv
selection_source: fresh_fetch
motivation: 探究视觉输入如何被转化为熟悉性记忆的神经算法。
method: 分析不同记忆性图像在猕猴ITC和HC的神经反应，对比记忆性与熟悉性信号。
result: ITC呈现记忆性驱动的熟悉性信号混合，而HC选择性提取纯净熟悉性表征。
conclusion: 发现视觉到熟悉性转换的两阶段算法，揭示内侧颞叶新计算角色。
---

## 摘要
看到图像的行为如何转化为对该图像已被见过的记忆？为了探究这一问题，我们利用某些图像比另一些图像更易被记住的系统性差异（即图像可记忆性），比较了猕猴在执行单次暴露视觉熟悉性任务时，下颞叶皮层（ITC）和海马体（HC）的神经反应。我们发现从视觉表征到熟悉性存在一个两阶段算法转换的证据，其中包括一个此前未描述的颞叶内侧熟悉性计算转换。在第一阶段，更易记住的图像激发了更强烈的ITC放电率反应和更强的ITC熟悉性信号（表现为重复抑制）。这导致ITC中熟悉性和可记忆性信号出现反直觉的混合，但形成了一个可通过线性解码器读取的表征。在下一阶段，颞叶内侧选择性提取ITC熟悉性信号，产生一个更孤立的熟悉性表征，其可记忆性调制最小化，并反映在下游的HC中。这些结果揭示了看到如何转化为熟悉性，并证实了此前未描述的颞叶内侧计算的存在。

## Abstract
How is the act of seeing an image transformed into the memory that it has been seen? To investigate, we leveraged the systematic variation with which some images are better remembered than others, image memorability, to compare neural responses in inferotemporal cortex (ITC) and the hippocampus (HC) as macaque monkeys performed a single-exposure visual familiarity task. We found evidence for a two-stage algorithmic transformation from visual representations to familiarity, including a previously undescribed computational transformation of familiarity in the medial temporal lobe. At the first stage, more memorable images elicited more vigorous ITC firing-rate responses and stronger ITC familiarity signals (reflected as repetition suppression). This led to a counterintuitive intermingling of familiarity and memorability signals in ITC, but a representation that could be read out by a linear decoder. At the next stage, the medial temporal lobe selectively extracted ITC familiarity signals to produce a more isolated familiarity representation with minimal memorability modulation, reflected downstream in HC. These results shed light on how seeing is transformed into familiarity, and they establish the existence of a previously undescribed medial temporal lobe computation.

---

## 论文详细总结（自动生成）

# 论文详细中文总结

## 1. 论文的核心问题与整体含义（研究动机和背景）

- **核心问题**：视觉系统如何将“看到图像”这一过程转化为“该图像已被见过”的熟悉性记忆？具体而言，大脑如何区分由图像可记忆性（memorability）和熟悉性（familiarity）引起的神经放电率变化，因为两者都会影响下颞叶皮层（ITC）的群体放电活力。
- **背景**：已知图像可记忆性是稳定的行为特征，在一些图像上更容易被记住。ITC中的重复抑制（repetition suppression）被认为是熟悉性的神经相关物，但可记忆性也会增强ITC的放电率，导致两种信号相互干扰。之前的理论（如基于放电活力的解码）无法解释行为上可记忆性越高熟悉性识别正确率越高的现象，因为高可记忆性图像在重复时仍有较高放电率，可能被误判为新颖。本研究旨在揭示从视觉表征到熟悉性行为之间的完整算法转换，并找出内侧颞叶（MTL）在其中扮演的新角色。

## 2. 论文提出的方法论：核心思想、关键技术细节、公式或算法流程

- **核心思想**：提出一个两阶段算法。第一阶段：在ITC中，视觉输入产生一个混合了可记忆性与熟悉性的表征，但可通过特定的线性解码轴（行为对齐轴）提取纯净的熟悉性信号。第二阶段：内侧颞叶（特别是海马体HC）接收ITC输入，并通过类似于该线性解码的计算，输出一个几乎不受可记忆性调制的熟悉性表征。
- **关键技术细节**：
  - **任务与记录**：两只猕猴执行单次暴露视觉熟悉性任务（每张图像仅出现一次新颖、一次重复），记录ITC和HC的神经活动（24通道U-probe）。
  - **伪群体与伪图像构建**：将不同会话的神经单元合并为伪群体，并将具有相近可记忆性得分的图像对齐为伪图像，以增加统计效力。
  - **解码器设计**：
    - **活力解码器（Vigor decoder, VG）**：将每个神经元等权重相加，用总放电率判断新颖/重复。
    - **可记忆性解码器（Memorability decoder, MB）**：训练区分高/低可记忆性图像的线性解码器。
    - **行为对齐解码器（Behaviorally aligned decoder, BA）**：在由VG和MB轴张成的平面上旋转，寻找与真实行为（识别正确率随可记忆性变化）斜率最匹配的轴，并通过交叉验证确保公平。
  - **预测质量（Prediction Quality, PQ）**：通过计算神经预测斜率与行为斜率之间的角度，量化解码器与行为的一致程度（0~1）。
  - **统计检验**：使用bootstrap检验PQ差异、置换检验比较ITC与HC的斜率差异。
- **公式流程**（文字描述）：
  - 步骤1：利用训练数据计算MB解码器权重（高记忆性与低记忆性平均响应差）。
  - 步骤2：在VG-MB平面内搜索使PQ最大化的旋转角θ，确定BA轴。
  - 步骤3：用完全独立的测试数据评估BA轴上的解码性能，得到神经预测，并与实际行为比较。

## 3. 实验设计：数据集/场景、基准、对比方法

- **数据集**：使用大量自然图像（来自互联网，涵盖多种物体和场景），通过MemNet（一个预测人类记忆性的卷积神经网络）为每张图像赋予0-1的可记忆性得分。实验中共使用10816个新颖-重复图像对。
- **场景**：单次暴露视觉熟悉性任务，图像在500ms内呈现，猴子通过眼动报告新颖或重复。n-back间隔从1到192个试次不等。
- **基准方法**：
  - 活力解码器（VG）作为基线，预测结果与行为严重不匹配（PQ约0.4）。
  - Fisher线性判别解码器（FLD）作为另一种基准，同样表现差。
  - 行为对齐解码器（BA）作为提出的方法，显著优于VG。
- **对比方法**：
  - 比较ITC和HC的表示：ITC中记忆性-活力相关性很高，HC中几乎消失。
  - 检验简单阈值化（sparsification）假说：模拟将ITC神经元调谐曲线截断一定百分比，发现要匹配HC的记忆性衰减需要截断93%的调谐曲线，但会破坏几乎所有熟悉性信息，从而排除该简单机制。

## 4. 资源与算力

- **未明确说明**：论文未提及使用的GPU型号、数量或训练时长。所有神经记录为湿实验（macrophysiology），离线分析在MATLAB中完成，未涉及大规模深度学习训练。因此资源与算力信息缺失。

## 5. 实验数量与充分性

- **主体实验数量**：两只猴子（M1、M2），每只猴子记录ITC和HC的多个会话（M1 ITC: 20 sessions, 保留7个; M1 HC: 36 sessions, 保留16个; M2 ITC: 9 sessions, 保留8个; M2 HC: 30 sessions, 保留21个）。每个会话包含至少200个新颖-重复图像对。最终ITC伪群体包含623个单元，HC包含815个单元。
- **解码器实验**：使用1000次交叉验证，每次60%训练MB、20%选择BA、20%测试。重复1000次取平均和标准误。
- **消融与控制实验**：
  - 检验BA轴的角度分布与随机打乱标签的null模型对比，证明角度稳定。
  - 去除重复增强单元进行排序分析，确认熟悉性信息主要来自重复抑制单元。
  - 对HC进行同样的解码器分析，验证三个预测（重复抑制保留、记忆性相关减弱、BA轴更接近VG轴）。
  - 阈值化模拟（图6）对比了不同截断比例对记忆性相关和熟悉性解码性能的影响。
- **统计检验**：使用bootstrap、置换检验、t检验、逻辑回归等，显著性水平明确，多重比较校正。
- **充分性**：实验设计全面，使用了不同的解码器、跨区域比较、模拟验证，统计严谨，个体水平和群体水平分析一致。唯一不足是动物数量仅2只，但重复性较好。

## 6. 论文的主要结论与发现

- **结论1**：ITC中重复抑制与可记忆性共同调制群体放电活力，且两者存在部分重叠（角度约51.6°），导致直接使用活力解码无法解释可记忆性行为。
- **结论2**：在ITC内，存在一个线性解码轴（行为对齐轴，约46.7°偏离VG轴）能有效提取熟悉性信号，同时丢弃可记忆性调制，并与实际行为一致（PQ从约0.4提高到约0.75）。
- **结论3**：内侧颞叶（以HC为代表）实现了该选择性提取：HC中记忆性-活力相关性显著减弱，而重复抑制仍保留；HC的BA轴更接近VG轴（角度仅13°），说明HC已经完成了ITC中所需的计算。
- **结论4**：简单的阈值化（稀疏化）无法解释从ITC到HC的转变，因为要达到记忆性衰减会破坏熟悉性信息。
- **整体意义**：首次描述了一个从视觉到熟悉性的两阶段算法，并揭示了内侧颞叶中此前未知的熟悉性提取计算。

## 7. 优点

- **方法创新**：利用可记忆性这一自然变异系统，将行为与神经表示紧密联系，提出“行为对齐轴”的概念并验证。
- **算法层面分析**：遵循Marr的计算层次，不纠缠实现细节，提供普适性解释。
- **严格的交叉验证**：双重交叉验证（MB训练、BA选择、测试分层），防止过拟合，并通过null模型证明亚稳定。
- **跨区域对比**：同时记录ITC和HC，直接检验了下游表示是否反映上游解码预测，增强了因果性推断。
- **模拟排除替代假说**：阈值化模拟清晰排除了简单稀疏化机制，增加结论可靠性。
- **统计充分性**：使用bootstrap、置换检验、个体分析等多种统计方法，结果稳健。

## 8. 不足与局限

- **动物数量少**：仅2只猕猴，虽然个体分析结果一致，但样本量限制了泛化能力。
- **伪群体方法**：将不同会话的神经元合并会忽略潜在的动态变化和单神经元精确定位，可能引入偏差。
- **因果关系不明确**：记录结果是相关性而非因果性，不能完全确认内侧颞叶确实执行了所描述的计算，需要未来进行损伤或失活实验。
- **范围有限**：仅研究了单次暴露熟悉性（图像仅出现两次），不适用于多次暴露或长期熟悉化任务（如经典文献中的重复增强）。
- **解剖范围**：记录仅覆盖ITC和HC，未直接记录内侧颞叶内的其他结构（如内嗅皮层、旁海马皮层），无法定位具体计算节点。
- **解码器假设**：假设熟悉性读取是线性的，且所有单元参与解码，但真实生物系统可能采用更复杂（如非线性、子集选择）的策略。
- **计算资源描述缺失**：未提供硬件信息，不利于复现性评估。

（完）
