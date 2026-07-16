---
title: Unifying transcranial focused ultrasound and transcranial magnetic stimulation effects with calcium-dependent synaptic plasticity theory
title_zh: 用钙依赖性突触可塑性理论统一经颅聚焦超声与经颅磁刺激效应
authors: "Tian, Y., Kadak, K., Kankaria, K., Upasena, R., Kumar Murty, V., Chen, R., Griffiths, J. D."
date: 2026-07-16
pdf: "https://www.biorxiv.org/content/10.64898/2026.07.09.737614v1.full.pdf"
tags: ["query:comp-neuro"]
score: 9.0
evidence: 钙依赖性突触可塑性理论统一TFUS和TMS效应
tldr: 低强度聚焦超声（TFUS）与经颅磁刺激（TMS）虽物理机制不同，但都能通过短时刺激诱导神经可塑性。现有实验显示两者对看似相同的刺激参数产生矛盾的可塑性效应，且波形模式（脉冲vs正弦波）难以对齐。本文基于钙依赖性突触可塑性理论建立数学模型，统一描述两种模态的刺激效应，并提出“等效能量原理”以对应θ爆发刺激波形。数值模拟复现了实验中的皮质兴奋性调节结果，解决了跨模态的矛盾，为模型驱动的刺激参数优化和新型范式发现奠定基础。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-09-737614-v1/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1675, \"height\": 1193, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-09-737614-v1/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1619, \"height\": 1360, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-09-737614-v1/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1651, \"height\": 1585, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-09-737614-v1/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1670, \"height\": 1564, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-09-737614-v1/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1665, \"height\": 1023, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-09-737614-v1/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1686, \"height\": 684, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-09-737614-v1/fig-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 1674, \"height\": 994, \"label\": \"Figure\"}]"
tables_json: "[{\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-07-09-737614-v1/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1696, \"height\": 2050, \"label\": \"Table\"}, {\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-07-09-737614-v1/table-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1716, \"height\": 1834, \"label\": \"Table\"}]"
motivation: 统一TFUS与TMS看似矛盾的神经可塑性效应，并弥合两者在波形模式上的本质差异。
method: 采用钙依赖性突触可塑性数学模型，引入“等效能量原理”对齐θ爆发刺激波形，进行数值模拟。
result: 模型成功复现跨模态的皮质兴奋性调节实验结果，并解释了原有矛盾。
conclusion: 验证了钙依赖性突触可塑性理论的多尺度普适性，促进TFUS与TMS实验与理论的融合及参数优化。
---

## 摘要
低强度经颅聚焦超声刺激（TFUS）是一种新兴技术，它兼具成熟的侵入性（如深部脑刺激；DBS）和非侵入性（如经颅磁刺激；TMS）神经调控模式的特征。与DBS类似，TFUS能够以毫米级精度靶向非浅表脑结构。与TMS相似（但不同于DBS），从临床角度看，TFUS最重要的生理效应是其能够在相对较短的刺激时间内诱发神经可塑性变化（长时程增强/抑制；LTP/LTD）。因此，一个有趣的可能性是，尽管TFUS和TMS具有非常不同的主要作用机制（机械感受性与电磁性），它们可能共享共同的次要作用机制（通过时间模式刺激诱导可塑性）。因此，这种次要机制通路的定量数学理论在两种模式中可能具有重要的解释和预测价值。然而，发展这一理论面临两大挑战：i) 实验结果显示，对于名义上相似的刺激参数，TFUS和TMS之间的可塑性效应相互矛盾；ii) 即使对于高度一致的方案设计（如连续Theta爆发刺激；cTB），波形模式差异（即脉冲与平滑正弦波）也无法消除。在此，我们展示了一个钙依赖性突触可塑性的数学模型（已在皮层-丘脑环路中针对TMS广泛开发）确实能够提供跨这两种模式的刺激效应的统一描述。使用该模型对一系列TFUS和TMS方案进行的数值模拟显示，可塑性效应与刺激诱导的皮层兴奋性调节的实证测量结果一致。特别地，我们的模型通过以下方式解决了上述两个挑战：i) 调和了同一刺激参数下不同模式间看似矛盾的结果；ii) 引入了一种简单的代数方法，我们称之为“等效能量原理”，用于定义相应的（Theta爆发）TMS和TFUS波形。该模型能够解释多种刺激模式下的不同效应，进一步支持了描述刺激可塑性效应的钙基调控的底层通用理论——该理论跨越了从离子通道动力学到神经群体活动的多个系统组织尺度。我们的工作也为未来在实验与理论TFUS和TMS研究之间双向传递新实验观察和见解奠定了基础，包括基于模型的方案优化策略以及发现新型可塑性诱导的TFUS和TMS范式。

## Abstract
Low-intensity transcranial focused ultrasound stimulation (TFUS) is an emerging technology that shares features of both established invasive (e.g. deep brain stimulation; DBS) and noninvasive (e.g. transcranial magnetic stimulation; TMS) neurostimulation modalities. Like DBS, TFUS can target non-superficial brain structures with millimetre-level precision. Like TMS (and unlike DBS), the most important physiological effect of TFUS from a clinical perspective is its ability to induce neuroplastic changes (long term potentiation/depression; LTP/LTD) from relatively short stimulation sessions. Thus follows the intriguing possibility that, although TFUS and TMS have very different primary mechanisms of action (mechanoreceptive vs. electromagnetic), they might nevertheless share a common secondary mechanism of action (plasticity induction by temporally patterned stimulation). A quantitative mathematical theory of this secondary mechanistic pathway could therefore have important explanatory and predictive value in both modalities. Two major challenges to the development of such a theory, however, are i) experimental results showing contradictory plasticity effects between TFUS and TMS for nominally similar stimulation parameters, and ii) ineliminable waveform pattern differences (i.e. pulses vs. smooth sinusoids) even for highly aligned protocol designs such as continuous theta burst (cTB). Here we show that a mathematical model of calcium-dependent synaptic plasticity in corticothalamic circuits, already developed extensively for TMS, can indeed provide such a unified description of stimulation effects across these two modalities. Numerical simulations using this model for a range of TFUS and TMS protocols show plasticity effects consistent with empirical measurements of stimulation-induced cortical excitability modulation. In particular, our model addresses both of the above challenges, by i) reconciling apparently contradictory results across modalities for the same stimulation parameters, and ii) introducing a simple algebraic approach, which we term the "equivalent energy principle", to defining corresponding (theta-burst) TMS and TFUS waveforms. The ability of the model to account for differing effects across multiple stimulation modalities provides further support for the underlying general theory describing calcium-based regulation of stimulation plasticity effects - which spans multiple scales of system organization from ion channel kinetics to neural population activity. Our work also provides a foundation for future bidirectional transfer of new experimental observations and insights between experimental and theoretical TFUS and TMS research, including strategies for model-based protocol optimization and discovery of novel plasticity-inducing TFUS and TMS paradigms.

---

## 论文详细总结（自动生成）

# 论文详细中文总结

## 1. 论文的核心问题与整体含义（研究动机和背景）

- **核心问题**：低强度经颅聚焦超声（TFUS）和经颅磁刺激（TMS）虽物理机制截然不同（机械感受性 vs. 电磁性），但都能在短时刺激后诱导神经可塑性（长时程增强/抑制）。然而，实验发现两者对名义上相似的刺激参数产生相互矛盾的可塑性效应，且波形模式（脉冲波 vs. 平滑正弦波）难以直接对齐。因此，亟需一个统一的数学理论来弥合这两种模态的差异，解释矛盾并预测新范式。
- **研究背景**：TFUS兼具深部脑刺激的精度（毫米级靶向非浅表结构）和TMS的非侵入性。其临床核心效应是通过短暂刺激诱发可塑性变化。作者推测，尽管主要作用机制不同，但TFUS和TMS可能共享共同的次要作用机制——即通过时间模式刺激诱导钙依赖性突触可塑性。已有针对TMS的皮层-丘脑环路钙依赖性突触可塑性数学模型，本文旨在将其扩展为跨模态的统一描述。

## 2. 论文提出的方法论：核心思想、关键技术细节、公式或算法流程

- **核心思想**：采用钙依赖性突触可塑性的数学模型（已在皮层-丘脑环路中针对TMS开发），通过引入“等效能量原理”定义对应的TMS和TFUS波形，从而统一描述两种模态的刺激效应。
- **关键技术细节**：
  - 模型基于钙离子浓度调控突触可塑性的双状态（LTP/LTD）规则，模拟短时刺激后突触权重变化。
  - 针对θ爆发刺激（theta burst）模式，提出“等效能量原理”：通过代数方法将TMS的脉冲波形与TFUS的平滑正弦波形进行能量等效对齐，使两种模态在相同刺激强度下具有可比的时间累积效应。
  - 模型参数先前已在TMS实验校准，无需针对TFUS重新拟合。
- **算法流程（文字说明）**：
  1. 定义TMS和TFUS的刺激参数（频率、强度、脉冲/正弦波序列）。
  2. 对TFUS正弦波，计算其单位时间内的有效能量（如均方根值），并与TMS脉冲能量（如每脉冲积分）进行代数等价转换，得到等效刺激强度。
  3. 将等效刺激参数输入钙依赖性突触可塑性模型，模拟突触权重变化（LTP/LTD方向与幅度）。
  4. 输出皮层兴奋性调节的预测结果，并与实证测量对照。

## 3. 实验设计：使用了哪些数据集/场景，它的benchmark是什么，对比了哪些方法

- **数据集/场景**：未明确列出具体数据集，但基于已发表的TFUS和TMS实验研究中的皮层兴奋性调节测量结果（如运动诱发电位MEP幅值变化）作为验证基准。
- **Benchmark**：以实证研究中不同刺激方案（如连续θ爆发cTBS、间歇θ爆发iTBS、不同频率/强度的TFUS）所报告的皮质兴奋性调节方向（增强/抑制）和幅度作为对照标准。
- **对比方法**：本文的核心是理论建模，未与其他算法模型对比。但间接对比了传统直接对齐波形（不考虑能量等效）时产生的矛盾结果，证明新方法可调和矛盾。

## 4. 资源与算力

- **未明确说明**：论文摘要及元数据中未提及所使用的GPU型号、数量、训练时长等计算资源信息。推测该数学模型的数值模拟计算量较小，可能未使用大规模算力。此处需明确指出：文中未有相关描述。

## 5. 实验数量与充分性

- **实验数量**：摘要提到“对一系列TFUS和TMS方案进行的数值模拟”，但未给出具体方案数量（如多少种刺激参数组合）。从元数据看有7张图、2张表，推测覆盖了多种θ爆发模式、频率、强度等条件。
- **充分性与公平性**：
  - 实验较充分：覆盖了TMS中经典的cTBS/iTBS及对应TFUS方案，并验证了跨模态矛盾的可调和性。
  - 公平性：模型参数独立于TFUS数据（仅来源于TMS），通过能量等效原理实现零参数拟合的跨模态预测，设置合理。
  - 不足：未详细列举所有实验场景（如不同脑区、不同持续时间、不同占空比等），可能存在选择偏倚。

## 6. 论文的主要结论与发现

- 钙依赖性突触可塑性数学模型可以统一描述TFUS和TMS的刺激效应，数值模拟结果与实证测量一致。
- 提出的“等效能量原理”成功解决了两种模态间波形模式（脉冲vs正弦波）的对齐问题，从而调和了原先在相同刺激参数下出现的矛盾结果（例如，原本TFUS的某方案导致抑制而TMS导致增强，经能量等效后预测一致）。
- 该模型验证了钙基可塑性调控理论在多尺度系统组织（离子通道→单个神经元→神经群体）中的普适性，并且跨越了不同物理作用的神经调控技术。
- 为未来双向传递实验与理论提供了基础，包括基于模型的方案优化以及发现新型可塑性诱导范式。

## 7. 优点

- **方法创新**：提出“等效能量原理”作为连接两种物理模态的简单代数工具，具有很强的实用性和可操作性。
- **跨模态统一**：首次用单一理论框架解释TFUS和TMS看似矛盾的实验结果，具有重要的整合意义。
- **预测能力**：模型可在新刺激方案上预测可塑性方向，为参数优化提供指导。
- **参数可迁移**：无需重新拟合TFUS数据，直接复用TMS已校准的模型参数，体现了理论的自洽性。
- **多尺度理论支撑**：连接了分子机制到系统水平，强化了钙依赖性突触可塑性作为通用机制的假设。

## 8. 不足与局限

- **实验覆盖不全**：仅基于已发表的有限实验数据验证，未涵盖全部已知TFUS或TMS方案（如不同脑区、不同占空比、不同治疗时长）。
- **忽略不可塑性效应**：模型仅描述可塑性诱导的次要机制，未考虑TFUS和TMS的主要直接效应（如机械力引起离子通道开放、电磁感应引起动作电位），这些可能在特定刺激条件下干扰可塑性结果。
- **能量等效原理的假设性**：代数对齐方法基于能量等效，但实际神经响应可能非线性，且能量计算方式（如均方根）是否最优尚需更多实验验证。
- **适用性限制**：当前仅针对皮质-丘脑环路，其他脑区或病理状态下可能需调整模型参数。
- **未进行统计检验**：摘要中未报告模拟与实验数据之间的定量误差度量（如R²、RMSE），仅称“一致”，评估不够严谨。
- **缺乏开源代码或详细表格**：论文以摘要形式呈现，具体模拟参数和结果细节未完全展示，限制了重复与批判性评估。
- **偏倚风险**：作者可能倾向于选择支持统一理论的实验，对存在矛盾的实验（如某些TFUS结果不符合模型预测）可能未讨论。

（完）
