---
title: "Sleep to forget: active control of consolidation and forgetting by slow-wave sleep dynamics"
title_zh: 睡眠以遗忘：慢波睡眠动态对巩固与遗忘的主动控制
authors: "Golden, R., Wei, M., Coury, S., Mizrahi-Kliger, A., Ganguly, K., Bazhenov, M."
date: 2026-06-19
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.15.732460v1.full.pdf"
tags: ["query:comp-neuro"]
score: 9.0
evidence: 利用STDP的生物物理模型研究睡眠中记忆巩固和遗忘的突触可塑性
tldr: 睡眠中记忆巩固与遗忘的灵活控制机制尚不明确。本研究构建丘脑皮层网络模型，通过操纵Ca2+动力学产生慢波和delta波两种Up状态。慢波因更长的Up状态提供自发重激活阶段，选择性保护记忆；而delta波因Up状态较短且导致突触稀疏化，促进遗忘。模型揭示慢波与delta波的比例可动态调控记忆巩固与遗忘的平衡。
source: biorxiv
selection_source: fresh_fetch
motivation: 探索慢波睡眠中不同Up状态如何通过突触可塑性机制分离记忆巩固与遗忘。
method: 构建含STDP可塑性的生物理丘脑皮层网络，操纵Ca2+动力学产生慢波和delta波Up状态，并模拟序列学习任务。
result: 慢波期间去除可塑性削弱记忆，delta波期间去除可塑性增强巩固；慢波Up状态更长，支持干扰后自发重激活，而delta波不能。
conclusion: 慢波与delta波的比例灵活调节记忆巩固与遗忘，为睡眠中记忆动态控制提供机制解释。
---

## 摘要
睡眠既支持新记忆的巩固，也支持其他记忆的遗忘，但皮层如何灵活控制这些结果仍知之甚少。近期研究表明，两种类型的Up状态在慢波睡眠（SWS）期间可能扮演不同且相互竞争的角色：慢波主动巩固记忆痕迹，而δ波则促进其弱化。本文采用一个配备脉冲时序依赖可塑性的生物物理丘脑皮层网络模型，研究这种分离背后的突触机制。通过操纵皮层锥体细胞的内在钙离子动力学，我们在单一网络中生成慢波和δ波Up状态。利用序列学习任务范式，我们重现了光遗传学分离：在慢波期间移除可塑性会降低记忆，而在δ波期间移除可塑性则增强巩固。机制上，模型揭示了较长的慢波Up状态提供了一个自发再激活阶段（发生在干扰输入之后），在此阶段训练的记忆被选择性再激活并保护，而截断的δ波Up状态无法支持这一阶段。我们进一步发现，δ波比慢波更稀疏化突触表征，并预测SWS期间慢波与δ波的比例可灵活调节巩固与遗忘之间的平衡。

## Abstract
Sleep supports both the consolidation of new memories and the forgetting of others, but how the cortex flexibly controls these outcomes remains poorly understood. Recent work has shown that two types of Up states may play distinct, competing roles during slow-wave sleep (SWS): slow waves actively consolidate memory traces, whereas delta waves promote their weakening. Here we use a biophysical thalamocortical network model equipped with spike-timing-dependent plasticity to investigate the synaptic mechanisms underlying this dissociation. By manipulating the intrinsic Ca2+ dynamics of cortical pyramidal cells, we generate both slow and delta wave Up states within a single network. Using a sequence-learning task paradigm we recapitulate the optogenetic dissociation: removing plasticity during slow waves degrades the memory, while removing it during delta waves enhances consolidation. Mechanistically, the model reveals the longer slow wave Up state affords a spontaneous reactivation phase, occurring after the interfering input, during which the trained memory is selectively reactivated and protected, a phase the truncated delta Up state cannot support. We further find that delta waves sparsen the synaptic representation more than slow waves and predict that the balance between consolidation and forgetting can be flexibly tuned by the ratio of slow to delta waves during SWS.

---

## 论文详细总结（自动生成）

# 论文详细中文总结

## 1. 论文的核心问题与整体含义（研究动机和背景）

- **研究动机**：睡眠同时支持新记忆的巩固和旧记忆的遗忘，但大脑皮层如何灵活控制这两种相反的结果，神经机制尚不明确。已有研究表明，慢波睡眠（SWS）中存在两种不同类型的Up状态——慢波（slow waves）和δ波（delta waves），它们可能扮演相互竞争的角色：慢波主动巩固记忆痕迹，而δ波促进记忆弱化（遗忘）。论文旨在揭示这种分离背后的突触机制。
- **整体含义**：该研究为理解睡眠中记忆的动态调节提供了计算层面的机制解释，有助于阐明睡眠障碍如何影响记忆，并为未来针对记忆增强或遗忘的干预策略提供理论基础。

## 2. 论文提出的方法论：核心思想、关键技术细节

- **核心思想**：通过构建一个配备脉冲时序依赖可塑性（STDP）的生物物理丘脑皮层网络模型，在同一网络中分别生成慢波和δ波的Up状态，研究不同Up状态下突触可塑性如何影响记忆巩固与遗忘。
- **关键技术细节**：
  - 模型操纵皮层锥体细胞的内在Ca²⁺动力学，从而在单一网络中产生两种不同时长的Up状态：较长的慢波Up状态和较短的δ波Up状态。
  - 利用序列学习任务范式模拟训练与干扰过程，量化记忆保留程度。
  - 通过“移除可塑性”操作（模拟光遗传学抑制可塑性）观察对记忆的影响：慢波期间移除可塑性降低记忆，δ波期间移除可塑性反而增强巩固，从而验证两种Up状态的功能分离。
  - 机制上，较长慢波Up状态在干扰输入后允许自发再激活阶段，选择性保护训练记忆；而δ波Up状态被截断，无法支持这一阶段，且δ波导致突触表征更稀疏化。

## 3. 实验设计：数据集/场景、benchmark、对比方法

- **数据集/场景**：采用序列学习任务范式的模拟场景，未使用真实神经数据或标准数据集。模型训练特定序列记忆，随后施加干扰输入，在不同Up状态条件下测试记忆保留。
- **Benchmark**：无明确外部基准，主要通过比较慢波与δ波条件下记忆保留程度，以及光遗传学分离实验（慢波/δ波期间移除可塑性）的复现结果作为验证。
- **对比方法**：论文没有对比其他模型或算法，属于自身构建模型的机制验证。通过控制变量（Ca²⁺动力学参数、可塑性开关）进行内部对比。

## 4. 资源与算力

- 论文元数据和摘要中**未明确说明**使用的GPU型号、数量、训练时长等计算资源信息。通常此类生物物理模拟可在单台高性能工作站或小型计算集群上完成，但具体细节未知。

## 5. 实验数量与充分性

- **实验数量**：根据摘要，主要进行了两类实验：
  1. 基础序列学习任务中，分别移除慢波或δ波期间的可塑性，观察记忆变化。
  2. 分析Up状态时长对自发再激活阶段的影响，以及δ波对突触表征稀疏化的作用。
- **充分性评价**：实验设计紧扣假设，分离变量清晰，复现了光遗传学的关键现象。但未提供完整的消融实验、参数敏感性分析或多任务验证。由于缺乏全文，难以评估是否进行了充分的统计测试和重复实验。总体而言，机制验证较为充分，但泛化性和统计稳健性尚需更多证据。

## 6. 论文的主要结论与发现

- **主要结论**：慢波睡眠中的慢波和δ波通过不同Up状态时长对突触可塑性进行差异调节，从而主动控制记忆巩固与遗忘的平衡。慢波Up状态较长，允许干扰后自发再激活并保护记忆；δ波Up状态较短，无法支持再激活，且导致突触表征稀疏化，促进遗忘。
- **具体发现**：
  - 慢波期间移除可塑性会降低记忆（说明慢波期间可塑性对巩固必不可少）。
  - δ波期间移除可塑性反而增强巩固（说明δ波期间可塑性通常导致遗忘，阻断后记忆保留更好）。
  - 模型预测慢波与δ波的比例可灵活调节巩固与遗忘之间的平衡。

## 7. 优点：方法或实验设计上的亮点

- **方法亮点**：使用生物物理细节的丘脑皮层网络模型，结合STDP可塑性，能够自发生成不同类型的Up状态，为抽象认知功能（记忆巩固/遗忘）提供了可解释的神经机制。
- **实验设计亮点**：
  - 巧妙利用“移除可塑性”操作模拟光遗传学抑制，直接验证因果作用。
  - 通过操纵单一参数（Ca²⁺动力学）在一个网络中产生两种Up状态，避免了跨网络比较的混淆。
  - 模型预测了慢波/δ波比例对记忆的影响，为未来实验提供了可检验的假说。

## 8. 不足与局限

- **实验覆盖不足**：
  - 仅使用单一序列学习范式，未测试其他类型记忆（如空间、语义）或更复杂的干扰模式。
  - 未与真实神经数据（如多电极记录、钙成像）进行定量比较，模型预测缺乏实验验证。
- **偏差风险**：模型参数和Ca²⁺动力学设定可能具有倾向性，需敏感性分析确认结论的稳健性。
- **应用限制**：模型基于单个丘脑皮层回路，未考虑海马-皮层交互、皮层-皮层长期重塑等更高层次网络的作用。睡眠阶段转换（如REM睡眠）的影响也未纳入。
- **资源与算力说明不充分**：未提供计算资源细节，难以评估模型的可复现性和计算代价。
- **统计测试缺失**：未报告重复次数、置信区间或显著性检验，结论的统计可靠性不明。

（完）
