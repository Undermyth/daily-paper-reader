---
title: "BraiNN: A Modern Simulator for Clinically Feasible Personalized Whole-Brain Network Modeling"
title_zh: BraiNN：用于临床可行个性化全脑网络建模的现代模拟器
authors: "Fasse, A., Billi, C., Garvalov, V., Morvan, M., Newton, T., Kuster, N., Neufeld, E."
date: 2026-07-13
pdf: "https://www.biorxiv.org/content/10.64898/2026.07.08.737156v1.full.pdf"
tags: ["query:comp-neuro"]
score: 7.0
evidence: 基于JAX的全脑网络模拟器，支持计算神经科学研究
tldr: 个性化全脑网络建模需模拟大脑动力学以辅助治疗规划，但基于神经质量模型的全脑网络计算开销巨大。BraiNN框架利用JAX和GPU/TPU加速，将区域级Jansen-Rit模型与皮质表面网格耦合，实现高效仿真。通过贝叶斯优化与梯度精化结合的混合个性化流程，EEG谱拟合耗时从数天缩短至2-3小时。这使得高细节全脑表面模型个性化在消费级硬件上成为可能，为临床数字孪生奠定基础。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-08-737156-v1/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 891, \"height\": 571}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-08-737156-v1/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1664, \"height\": 907}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-08-737156-v1/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 894, \"height\": 534}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-08-737156-v1/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 904, \"height\": 517}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-08-737156-v1/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 901, \"height\": 518}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-08-737156-v1/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 901, \"height\": 518}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-08-737156-v1/fig-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 896, \"height\": 518}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-08-737156-v1/fig-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 1842, \"height\": 915}]"
tables_json: "[{\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-07-08-737156-v1/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 867, \"height\": 556}, {\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-07-08-737156-v1/table-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 898, \"height\": 297}]"
motivation: 现有个性化全脑建模框架计算耗时过长，难以满足临床时间要求。
method: 采用JAX实现GPU/TPU加速的Jansen-Rit网络，结合皮质表面网格与可微计算图，实现混合贝叶斯-梯度优化。
result: 在单消费级GPU上2-3小时完成EEG驱动谱拟合，速度提升2-3个数量级。
conclusion: 将高细节全脑模型个性化时间从天级降至小时级，推动临床可行应用。
---

## 摘要
个性化全脑建模旨在通过实现患者特异性脑网络动力学模拟来改变神经系统疾病的治疗规划。神经质量模型（NMM）在生物物理细节和计算成本之间提供了可处理的折衷，并且可以直接与宏观观测指标（如脑电图）相关联。然而，将NMM扩展到具有真实连接性、传导延迟和皮层表面分辨率的全脑网络，并将其拟合到个体患者数据中，对计算提出了现有框架在临床相关时间尺度上无法满足的要求。在此，我们介绍BraiNN，一个基于JAX的Python框架，用于大规模神经质量建模，通过利用GPU/TPU加速和XLA编译的数组计算，比现有工具实现了高达两到三个数量级的加速。BraiNN将区域级Jansen-Rit网络与耦合神经质量模型的个体特异性皮层表面网格以及基于互易性的导联场的生物物理合理EEG正向建模相结合。其全微分计算图实现了一种混合个性化流水线，将贝叶斯优化用于全局参数探索，并结合基于梯度的精化，在单个消费级GPU上大约2-3小时内完成EEG驱动的八维参数空间谱拟合——而传统神经质量建模软件则需要数天时间。对已建立基准的数值验证确认，BraiNN忠实地再现了Jansen-Rit网络的经典同步和分岔动力学。通过将高细节全脑表面模型的个性化时间从数天减少到消费级硬件上的数小时，BraiNN使个性化脑网络建模更接近临床实际应用。我们预期BraiNN将成为患者特异性数字孪生和EEG引导神经调控规划的基础。

## Abstract
Personalized whole-brain modeling aims to transform treatment planning for neurological disorders by enabling patient-specific simulations of brain network dynamics. Neural mass models (NMMs) offer a tractable compromise between biophysical detail and computational cost and can be directly linked to macroscopic observables such as EEG. However, scaling NMMs to whole-brain networks with realistic connectivity, conduction delays, and cortical surface resolution--and fitting them to individual patient data--imposes computational demands that existing frameworks cannot meet at clinically relevant timescales. Here we introduce BraiNN, a JAX-based Python framework for large-scale neural mass modeling that achieves speedups of up to two to three orders of magnitude over existing tools by leveraging GPU/TPU-accelerated, XLA-compiled array computation. BraiNN combines a region-level Jansen-Rit network with a subject-specific cortical surface mesh of coupled neural mass models and biophysically grounded EEG forward modeling via reciprocity-based lead fields. Its fully differentiable computational graph enables a hybrid personalization pipeline that pairs Bayesian optimization for global parameter exploration with gradient-based refinement, completing EEG-driven spectral fitting of an eight-dimensional parameter space in approximately 2-3 hours on a single consumer GPU--compared to multiple days with conventional neural mass modeling software. Numerical verification against established benchmarks confirms that BraiNN faithfully reproduces canonical synchronization and bifurcation dynamics of Jansen-Rit networks.

By reducing the time requirements for personalizing a high-detail whole-brain surface model from days to a few hours on consumer-grade hardware, BraiNN brings personalized brain network modeling closer to practical use in clinical contexts. We anticipate that BraiNN will serve as a foundation for patient-specific digital twins and EEG-guided neuromodulation planning.