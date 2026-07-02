---
title: Perceptual glimpses are locally accumulated and globally maintained at distinct processing levels
title_zh: 知觉一瞥在局部累积并在不同处理层级全局维持
authors: "Pares-Pujolras, E., Geuzebroek, A. C., O'Connell, R. G., Kelly, S. P."
date: 2026-07-02
pdf: "https://www.biorxiv.org/content/10.1101/2025.04.30.651428v4.full.pdf"
tags: ["query:comp-neuro"]
score: 8.0
evidence: 知觉推理中的神经证据积累机制
tldr: 决策常需整合多片段信息，但间歇性视觉 glimpses 下的神经机制尚不明确。本研究通过两个EEG实验，让被试判断间歇出现的运动脉冲方向。发现运动β偏侧化累积并维持证据，而CPP瞬态表征每次脉冲的更新；第二脉冲信息仅在未达决策边界时被整合。揭示了证据累积在不同神经层级的分工：局部瞬态整合与全局维持，为理解间歇信息决策提供模型。
source: biorxiv
selection_source: fresh_fetch
motivation: 探索间歇性视觉 glimpses 下证据累积的神经机制及其层级分工。
method: 采用两个EEG实验，要求被试判断方向不同的两脉冲运动，并模拟神经层级模型。
result: 行为上参与者低估第二脉冲，准确率不受间隔影响；运动β偏侧化累积证据，CPP瞬态响应脉冲更新。
conclusion: 证据在CPP层局部瞬态整合，在运动层全局维持，第二脉冲仅在未达阈值时才被整合。
---

## 摘要
做出决策通常需要整合多个信息片段。大量研究探讨了在信息持续呈现的知觉任务中，支持证据积累的神经架构，但对于这种神经架构如何仅在间歇性瞥见证据来源的情况下运作，我们知之甚少。在两个脑电图（EEG）实验中，参与者判断了多达两个运动证据脉冲的方向，脉冲之间间隔不同时长。我们的行为分析发现，参与者使用了两个脉冲，但对第二个脉冲利用不足，并且随着间隔时长增加，准确率没有系统性下降。在神经层面，运动β频段侧化追踪了跨脉冲的累积证据，通过间隔期维持决策变量的持续表征，直至反应。相比之下，中央顶叶正波（CPP）——先前被描述为证据积累的特征信号——短暂地建立到一个峰值，该峰值与每个脉冲对决策变量的贡献（即其产生的绝对信念更新）成比例，并在脉冲之间回落到基线。这些模式在一个模型中得到了重现：在CPP水平短暂整合的脉冲信息被输入并维持在有限制的运动水平。在该模型中，第二个脉冲中的证据仅在第一个脉冲的证据未达到界限的程度上被整合，如果已经达到界限，则根本不整合。

## Abstract
Making decisions often requires the integration of multiple pieces of information. An extensive body of research has investigated the neural architecture underpinning evidence accumulation in perceptual tasks where information is continuously present, but less is known about how this neural architecture operates in situations affording only intermittent glimpses of an evidence source. In two electroencephalography (EEG) experiments, participants judged the direction of up to two pulses of motion evidence separated by gaps of varying duration. Our behavioural analysis found that participants used both pulses but underutilised the second, and showed no systematic decrease in accuracy as a function of gap duration. At the neural level, motor beta lateralisation tracked cumulative evidence across pulses, maintaining a sustained representation of the decision variable through the gap and until response. In contrast, the centroparietal positivity (CPP), a previously-characterised signature of evidence accumulation, built up transiently to a peak that scaled with each pulse's contribution to the decision variable (i.e. the absolute belief update it produced), falling back to baseline in between pulses. These patterns were recapitulated in a model where pulse-information transiently integrated at the CPP level is fed to and maintained at a bounded motor level. In this model, the evidence in the second pulse is only integrated to the extent that the evidence in the first pulse falls short of the bound, or not integrated at all if a bound has already been hit.

---

## 论文详细总结（自动生成）

# 论文详细中文总结

## 1. 核心问题与整体含义（研究动机和背景）

**研究动机**：现实世界中的许多决策（如观察被间歇遮挡的移动物体）依赖于对**间歇性、不连续的信息“瞥见”** 进行整合。然而，现有大规模研究主要关注信息持续呈现（如连续随机点运动）下的证据积累机制，对**间歇性证据场景**下神经架构如何运作知之甚少。尤其是，已知的两个重要神经信号——**中央顶叶正波（CPP）** 和**运动β频段侧化（MBL）**——在连续任务中分别扮演“证据累积”和“运动准备”角色，但在任务中它们是否及如何分工处理间歇性证据尚不清楚。

**整体含义**：本研究通过人类EEG实验和计算建模，揭示了**知觉决策系统在层级上实现功能分工**：上游的CPP负责对每个证据脉冲进行**局部、瞬态**的累积（反映每次更新量|ΔDV|），下游的MBL则负责**全局、持续**地维持整个决策变量（DV）直至反应。第二脉冲仅在DV未触及决策边界时才被进一步整合，这解释了行为中“首因效应”及信息利用不足的成因。

## 2. 方法论

### 核心思想
将决策过程建模为**两级层级架构**：
- **中间累积器（对应CPP）**：仅在证据呈现期间（黄色圆点运动脉冲内）进行有噪累积，累积量取绝对值（|ΔDV|），证据暂停（蓝色不相关运动）时快速回零；
- **下游运动级（对应MBL）**：接收CPP的输出，维持一个**有界**的决策变量（DV）——当CPP逐脉冲提供的增量被累加到此级时，DV持续保持不变；一旦DV达到±Bound，后续脉冲的证据便不再被整合。

### 关键技术细节
- **任务**：改编自Kiani et al. (2013)的“间隔任务”（gaps task），使用随机点动图（RDK）。每个试次最多含两个200 ms的运动证据脉冲（黄色点），其间为可变间隔（蓝色不相关运动点），最后延迟后按键报告运动方向。脉冲方向始终一致，但相干度（高/低两种，经楼梯法个体化调整）可不同。
- **EEG记录与预处理**：128通道BioSemi系统，512 Hz采样；带通滤波0.1-40 Hz；使用CSD变换减少空间弥散；时间-频率分解采用7周期Morlet小波。
- **神经信号提取**：
  - **MBL**：对侧/同侧运动区β频段（13-30 Hz）功率差；
  - **CPP**：一组中央顶叶电极的平均电位；
  - **枕区α功率**（8-12 Hz）作为注意力指标。
- **行为分析**：逻辑混合效应模型，检验相干度、间隔时长对正确率的影响，以及顺序效应（HL vs. LH）。
- **计算模型**：有界扩散模型（3个自由参数：边界B、低/高相干漂移率d_low/d_high）。模拟时：MBL取DV的带符号值；CPP取每个脉冲内累积量的绝对值（|ΔDV|），并在脉冲结束后以200ms线性衰减至0。通过最小化G²拟合总体正确率。

### 公式/算法流程（文字说明）
1. 在每个脉冲内，DV按扩散过程更新：  
   `DV[t] = DV[t-1] + drift_rate + Gaussian_noise`
2. 间隔期间DV保持稳定（无漏、无噪声）。
3. 若DV达到±Bound，累积终止，DV保持在Bound值直至反应。
4. 模拟CPP：提取每个脉冲内的|ΔDV|，若Bound在脉冲内被击中，该部分后立即下降（线性至0）；若未击中，则在脉冲结束后立即下降。
5. 模拟MBL：直接取DV数值（正值代表正确侧，负值代表错误侧）。

## 3. 实验设计

- **数据集/场景**：两个独立的EEG实验，使用相同的RDK任务，仅在间隔时长的分布上不同。
  - **实验1**：N=22，间隔均匀分布：0, 0.5, 1.0秒。
  - **实验2**：N=21，间隔偏向短时：0, 0.12, 0.36, 1.08秒。
- **任务细节**：共700（Exp1）/933（Exp2）试次，85.7%双脉冲，14.3%单脉冲；相干度经楼梯法（2-down-1-up）个体化校准，目标单脉冲准确率70%；高低相干分别设为±25%相对于楼梯估计值，块间动态调整以防地板/天花板。
- **Benchmark**：行为上比较了真实正确率与“完美累积器”预测的正确率；神经上比较了CPP和MBL在不同相干组合下的动态；模型比较了有界累积器与多种可替代模型（如无界+权重衰减、有界+权重衰减等），基于BIC选择最优。

## 4. 资源与算力

文中**未明确说明**所使用的GPU型号、数量或训练时长。模型拟合使用Matlab的Global Optimization Toolbox的particleswarm函数，在普通CPU上即可完成。EEG预处理和统计在Matlab中完成，不涉及大规模深度学习训练。

## 5. 实验数量与充分性

- **行为实验**：两个实验共43名参与者。每个实验包含多个条件：4种相干组合（LL, LH, HL, HH）× 多种间隔时长（Exp1: 3种，Exp2: 4种）× 双脉冲与单脉冲。统计采用混合效应模型，涵盖主效应和交互项，并控制了随机效应。
- **EEG分析**：报告了CPP和MBL的组平均时间-波形，基于集群置换检验（p<0.05，双尾）进行显著性判断。进行了多个单试次回归分析（如CPP-P1幅度与决策权重的关联）。
- **模型比较**：除了主模型（有界累积），还比较了5种其他模型（无界+均匀衰减、无界+P1反向衰减、有界+均匀衰减、有界+P1反向衰减等），使用BIC进行客观模型选择。此外，还模拟了不同衰减时间假设下的CPP动态。
- **充分性评价**：实验设计较为全面，覆盖了关键变量（相干度、间隔时长、顺序）。两个实验的结果一致，增加了可重复性。模型能够同时拟合行为和两个神经信号的模式。不足之处在于：未对间隔时长与相干度的某些交互效应（仅Exp2中显著）提供先验假设或充分解释；统计功效可能不足以检测某些细小的差异（如高低正确率条件下的CPP-P2交互）。

## 6. 主要结论与发现

1. **行为**：参与者同时利用两个脉冲，但对**第一脉冲的权重更高**（首因效应），准确率顺序 HL > LH；准确率不随间隔时长系统下降（排除信息泄露）；双脉冲准确率低于完美累积器预测。
2. **神经信号**：
   - **MBL**：从第一脉冲开始逐渐侧化，并**持续维持**通过整个间隔直至反应，反映了全局DV的状态（有界）。
   - **CPP**：每个脉冲引发**瞬态**的构建-峰值-衰减过程，脉冲间歇期返回基线；CPP-P1幅度随首脉冲相干度增加而增大；CPP-P2幅度受两种因素调制：①与P2相干度正比；②与P1相干度**反比**（P1低相干时CPP-P2更大）。
3. **模型解释**：有界累积器模型可以同时解释上述行为与神经模式。早期终止（首脉冲强时更易达到界限）导致第二脉冲证据被部分或完全浪费；CPP-P2幅度反映P1低相干→更多未达边界→第二脉冲需要更长的累积路径。对比无界+权重衰减模型，有界模型在BIC上更优。
4. **注意力动态**：枕区α功率在脉冲期间去同步化，间隔期间超同步化；α水平在长间隔时高于基线，可能反映注意力暂时脱离。两个实验的α动态差异提示与时间预期有关。

## 7. 优点

- **任务创新**：巧妙地利用“间隔任务”将连续知觉决策与不连续证据呈现结合，揭示了CPP在间歇性输入下的功能新特性（局部瞬态累积而非全局追踪），拓展了对决策神经架构的理解。
- **多层级神经测量**：同时记录CPP（决策级）和MBL（运动级）以及枕区α（注意级），实现了多层级、多维度的对应分析。
- **模型驱动的严谨分析**：不仅拟合行为数据，还从同一模型生成了两个神经信号的模拟，并进行多种衰减假设检验，加强了因果推断的强度。
- **实验可重复性**：两组独立实验，且间隔分布不同，但主要模式一致（首因效应、CPP双峰、MBL持续），增加了结论的可泛化性。
- **模型比较详尽**：考虑了多种替代机制（如均匀衰减、P1依赖性衰减、有界+衰减混合），使用BIC选择最简洁模型，避免了过度拟合。

## 8. 不足与局限

- **间隔时长效应的解释不足**：在Exp2中观察到了P2相干度×间隔的交互效应，但作者未作深入解释，仅将其归为“意外且不一致”而搁置。这一效应可能反映时间预期对整合策略的调制，但缺乏严格操控实验。
- **缺乏反应时数据**：由于任务采用延迟反应（延迟至线索出现后按键），没有记录决策时间点，导致无法直接验证“早期终止”假说的实时性；模型也无法拟合反应时分布。
- **CPP衰减动力学的假设粗放**：模拟中假设CPP在脉冲结束后线性衰减至0（200ms），但实际衰减速度可能取决于是否达到边界，且不同条件（长短间隔）下的衰减曲线形状差异未被充分建模。
- **个体差异的统计分析有限**：虽然进行了个体层级的模型拟合（图S13-14），但主要依赖群体平均拟合。个体策略差异（如某些人更倾向有界、某些人更倾向无界加权）未被量化讨论。
- **注意力机制的因果证据不足**：虽观察到α功率与P2权重在Exp2中的关联（单试次回归），但相关性分析不能确立因果关系。未来可通过直接操纵注意（如提示或干扰）进一步检验。
- **通用性限制**：任务中证据方向始终一致（无冲突），且具有明确颜色提示区分信息期与非信息期。在更自然的间歇性环境中（如无外部提示、方向可能反转）CPP的功能是否相同尚不清楚。

（完）
