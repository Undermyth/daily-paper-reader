---
title: Intrinsic representational drift from predictive excitatory-inhibitory plasticity
title_zh: 来自预测性兴奋-抑制可塑性的内在表征漂移
authors: "Asabuki, T., Clopath, C."
date: 2026-06-23
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.17.733055v1.full.pdf"
tags: ["query:comp-neuro"]
score: 9.0
evidence: 预测性兴奋-抑制可塑性驱动表示漂移
tldr: 神经表征在稳定环境中也会逐渐漂移，但其突触机制尚不清楚。本文通过预测性兴奋-抑制（E/I）可塑性在尖峰网络中建模，发现重复暴露不变输入时，单个神经元偏好逐渐变化而群体编码稳定，且偏好变化前净E/I驱动相对减弱。扩展到海马CA1位置编码，重现了经验依赖的调谐曲线漂移。结果表明，表征漂移可源于维持平衡选择性群体编码的预测性E/I可塑性的内在结果。
source: biorxiv
selection_source: fresh_fetch
motivation: 探究稳定环境下神经表征逐渐漂移的突触机制。
method: 利用预测性E/I可塑性在兴奋-抑制尖峰网络中进行建模与仿真。
result: 重复输入导致单个神经元偏好漂移而群体编码稳定，漂移前净E/I驱动相对减弱可预测变化。
conclusion: 表征漂移是维持平衡群体编码的预测性E/I可塑性的内在结果。
---

## 摘要
即使在稳定的环境条件下，神经表征也会随时间逐渐漂移，但驱动这种漂移的突触机制尚不清楚。这里我们证明，在脉冲兴奋-抑制网络中，表征漂移可以内在地源于预测性突触可塑性。在反复暴露于不变的输入模式期间，单个神经元逐渐改变其偏好模式，而群体水平的编码保持稳定。这些偏好的变化发生在支持当前偏好的净兴奋-抑制驱动相对于竞争模式减弱之前，并且这种相对驱动预测了后续试验中的变化。将该模型扩展到海马位置编码，再现了CA1中经验依赖的调谐曲线漂移，包括经过时间和中间暴露之间的分离。在群体水平上，漂移表现为神经状态空间的协调旋转和平移。因此，表征漂移可以作为维持平衡、选择性群体编码的预测性E/I可塑性的内在结果而出现。

## Abstract
Neural representations drift gradually over time even under stable environmental conditions, but the synaptic mechanisms driving this drift remain unclear. Here we show that representational drift can arise intrinsically from predictive synaptic plasticity in spiking excitatory-inhibitory networks. During repeated exposure to unchanged input patterns, individual neurons gradually changed their preferred pattern while ensemble-level coding remained stable. These changes in preference were preceded by a weakening of the net excitatory-inhibitory drive supporting the current preference relative to competing patterns, and this relative drive predicted changes on the following trial. Extending the model to hippocampal place coding reproduced experience-dependent tuning-curve drift in CA1, including the dissociation between elapsed time and intervening exposure. At the population level, drift was expressed as coordinated rotation and translation of neural state space. Thus, representational drift can emerge as an intrinsic consequence of predictive E/I plasticity that maintains balanced, selective population codes.

---

## 论文详细总结（自动生成）

# 论文详细总结

## 1. 论文的核心问题与整体含义（研究动机和背景）

- **核心问题**：即使在稳定环境下，神经表征（如海马位置细胞的空间调谐）会随时间逐渐漂移，但驱动这种漂移的突触机制尚不清楚。现有模型多将漂移归因于外部噪声或随机扰动，缺乏内在的突触可塑性解释。
- **研究动机**：探索系统内在的预测性兴奋-抑制（E/I）可塑性是否能够自然产生表征漂移，同时维持群体水平编码的稳定性。
- **整体含义**：表征漂移并非记忆衰退的随机降解，而是维持平衡群体编码的预测性可塑性的内在结果——同一局部学习规则在不断平衡兴奋与抑制的过程中，逐渐重新分配单个神经元的表征角色。

## 2. 论文提出的方法论：核心思想、关键技术细节、算法流程

### 核心思想
- 使用**预测性E/I可塑性规则**训练脉冲兴奋-抑制递归网络。兴奋性突触（前馈和递归）学习预测突触后活动，抑制性突触追踪兴奋性驱动以维持预测性平衡。局部误差信号驱动权重更新，使得网络在重复暴露于相同输入时不断重调E/I平衡，从而自然引发单神经元偏好变化。

### 关键技术细节
- **网络模型**：400个泊松神经元，全连接。膜电位由前馈输入、递归兴奋和递归抑制贡献，激活函数为sigmoid，最大瞬时发放率50 Hz。
- **突触可塑性规则**：
  - 兴奋性权重更新：\(\Delta W_{ij} = \epsilon [f_i - \varphi(v_i^F)] x_j\)（前馈），\(\Delta M_{ij} = \epsilon [f_i - \varphi(v_i^R)] y_j\)（递归），其中\(f_i\)是实际发放率，\(\varphi(v_i)\)是预测值。
  - 抑制性权重更新：\(\Delta G_{ij} = \epsilon [v_i^F + v_i^R - v_i^I] y_j\)，旨在平衡总兴奋驱动与抑制驱动。
- **学习率**：模式输入实验\(\epsilon=10^{-4}\)，空间导航实验\(\epsilon=3\times10^{-4}\)。
- **算法流程**：
  1. 初始化权重（高斯）。
  2. 在每个时间步，计算膜电位、发放率，按规则更新所有可塑突触。
  3. 训练后测试冻结权重下的调谐曲线。
- **分析手段**：滑动窗口平均跟踪每个神经元的偏好模式；计算净E/I驱动、权重更新、选择性指标；用PCA分解群体状态空间的旋转、平移、缩放。

## 3. 实验设计：数据集/场景、基准、对比方法

### 数据集/场景
- **场景一（图2-3）**：三种离散输入模式（各500 ms），每种激活不重叠的100个输入神经元，以30 Hz发放。重复呈现这些模式，模拟长期学习。
- **场景二（图4-5）**：模拟Geva et al. (2023)的海马CA1纵向成像实验。涉及两个线性轨道环境（Env A和Env B），Gaussian调谐的输入神经元覆盖400个位置。暴露计划：Env A每2天访问，Env B每4天访问，持续21天。

### 基准与对比
- **无外部基准方法**：本文未与其他模型直接对比，而是将模拟结果与已知实验现象进行定性/定量匹配：
  - 与Geva et al. (2023)的CA1记录对比（时间与经验对ensemble rate correlation和tuning curve correlation的不同影响）。
  - 与Sylte et al. (2025)的群体几何分析对比（旋转、平移、缩放贡献）。
- **自身对照**：比较不同排序方式（同一天排序 vs. 固定第一天排序）对群体结构的影响；比较选择性高低与变化概率的关系。

## 4. 资源与算力

- **文中未明确说明使用的GPU型号、数量、训练时长**。所有模拟使用自定义Python3代码（numpy, scipy），欧拉积分时间步1 ms。作者未提供硬件信息。
- **推断**：模型规模较小（400神经元），每个模拟运行时间可能在数分钟至数小时（基于个人经验），但论文未提及具体算力需求。

## 5. 实验数量与充分性

- **主要实验**：
  - 模式输入实验（图2-3）：至少展示了10天的漂移过程，20次偏好变化事件用于触发平均分析（图3B-D）。进行了5次独立仿真（图5C-D）。
  - 空间导航实验（图4-5）：21天模拟，两种环境，每种环境多次测量。使用多种指标（ERC, TCC, 位置场的位移分布，PCA分析）。补充材料包含解码准确性、排序图等。
- **充分性评价**：
  - 实验覆盖了主要实验现象（单神经元漂移、群体稳定、时间/经验分离、群体几何变换），且定量结果（ERC/TCC随天数和会话数的趋势）与实验报道一致。
  - 缺乏与不同可塑性规则（如STDP、单纯Hebbian）的系统对比，也未进行超参数敏感性分析（如学习率、网络规模的影响）。未进行真实数据拟合。
  - 总体而言，对于一篇理论建模论文，实验设计较充分，但可进一步扩展以增强鲁棒性和通用性。

## 6. 论文的主要结论与发现

1. **局部预测性可塑性就足以产生表征漂移**：重复暴露相同输入，单个神经元逐渐改变其模式偏好，但群体编码保持结构化。
2. **偏好变化由E/I再平衡驱动**：变化前，净E/I驱动减弱（抑制增强→兴奋学习信号反转），导致当前偏好的突触支持削弱，增加切换到其他模式的可能性。
3. **选择性预测后续变化**：响应选择性越高，变化概率越低；兴奋性驱动选择性同样有效，抑制性驱动选择性预测力弱。
4. **复现海马CA1时间/经验解离**：ensemble rate correlation随经过时间衰减，tuning curve correlation随会话次数衰减——与Geva et al. (2023)一致。
5. **群体漂移表现为协调的旋转和平移**：PCA子空间旋转和质心位移随时间增加，而均匀缩放稳定；旋转是群体向量漂移的主要预测因子，与Sylte et al. (2025)观察一致。
6. **漂移是维持平衡群体编码的必然结果**，而非记忆衰退。

## 7. 优点：方法或实验设计上的亮点

- **机制清晰**：突触可塑性规则完全局部、生物合理（预测编码框架），无需外部噪声或全局信号即可产生漂移。
- **复现多个实验现象**：不仅定性匹配，还定量复现了ERC/TCC的解离以及群体几何变换的贡献排序。
- **因果分析**：通过transition-triggered average和选择性-变化概率曲线，揭示了E/I驱动变化与偏好改变的直接因果关系。
- **可验证预测**：提出三个可实验检验的预测（弱选择性→高变化概率、抑制可塑性抑制→漂移减慢、结构突变可增强长时程漂移）。
- **跨区域泛化**：从离散模式推广到连续空间导航，证明了框架的通用性。

## 8. 不足与局限

- **缺乏与替代可塑性模型的系统比较**：没有对比STDP、单纯Hebbian或基于噪声的模型在相同设置下的表现，无法证明预测性可塑性的唯一必要性。
- **超参数敏感性未分析**：学习率、网络规模、时间常数等可能影响漂移速率，但未做系统扫描。
- **生物精确性局限**：泊松神经元简化了尖峰发放的真实动力学；未考虑突触结构周转、内在兴奋性波动、神经调质等已知影响漂移的因素。
- **实验范围有限**：仅模拟两个环境（模式输入和线性轨道），未涉及更复杂的环境（如开放场、多感官线索）或跨天行为变化。
- **群体几何分析仅使用PCA**：假设线性流形，可能掩盖非线性变换；且未与真实数据中更精细的等距对齐方法比较。
- **论文为预印本，未经同行评审**，部分结论需进一步验证。

（完）
