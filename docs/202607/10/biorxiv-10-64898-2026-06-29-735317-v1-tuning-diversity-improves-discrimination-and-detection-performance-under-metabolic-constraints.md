---
title: Tuning Diversity Improves Discrimination and Detection Performance under Metabolic Constraints
title_zh: 调节多样性改善代谢约束下的判别与检测性能
authors: "Ringach, D."
date: 2026-07-03
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.29.735317v1.full.pdf"
tags: ["query:comp-neuro"]
score: 6.0
evidence: 调谐多样性通过计算模型改善群体编码
tldr: 皮层神经元调谐曲线呈现广泛多样性，其功能意义尚存争议。本研究构建异质调谐曲线家族模型，在相同代谢成本下，发现异质群体比均质群体具有更优的辨别和检测性能。这表明均质调谐不稳定，调谐多样性可能是代谢约束下优化编码的进化结果。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-29-735317-v1/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1623, \"height\": 373, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-29-735317-v1/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1257, \"height\": 592, \"label\": \"Figure\"}]"
motivation: 探究皮层调谐多样性的功能意义，是否源于代谢约束下的编码优化。
method: 构建异质调谐曲线家族，以等间距优选角度复制，与均质均值调谐曲线群体对比。
result: 异质群体在相同代谢成本下辨别和检测性能均优于均质群体。
conclusion: 均质调谐不稳定，多样性是代谢约束下优化编码的进化结果。
---

## 摘要
皮层群体表现出广泛的调谐特性，这引发了这样的疑问：这种变异性是皮层功能的特征还是缺陷？先前的研究表明，调谐多样性可以通过减轻相关噪声的影响并提高几何表征的判别和识别能力来改善群体编码。受这些发现的启发，我们研究了一个模型，在该模型中，编码圆形变量的异质性调谐曲线族以等间距的偏好角度复制。我们证明，与从该族平均调谐曲线的平移副本构建的同等大小的同质性群体相比，这种异质性群体在使用相同脉冲预算的情况下实现了更好的判别和检测。因此，在保持平均调谐曲线的扰动下，同质性调谐是不稳定的，因为这种扰动在保持代谢成本不变的同时提高了编码性能。我们提出，这种不稳定性产生了朝向调谐异质性的进化压力，使其普遍性成为代谢约束下优化编码性能过程的结果。

意义声明：皮层神经元的调谐曲线差异很大，这引发了这种多样性是否具有功能意义或仅仅反映生物噪声的问题。我们证明，在保持平均调谐曲线的同时扰动初始同质性群体，会产生一个异质性群体，在相同的代谢成本下具有更好的判别和检测性能。因此，调谐多样性可能作为代谢约束下选择高效编码的自然结果而出现。

## Abstract
Cortical populations exhibit a wide range of tuning properties, raising the question of whether such variability is a feature or a bug of cortical function. Prior work has shown that tuning diversity can improve population codes by mitigating the effects of correlated noise and increasing the discrimination and identification capacity of geometric representations. Motivated by these findings, we study a model in which a heterogeneous family of tuning curves, coding for a circular variable, is replicated at equally spaced preferred angles. We show that this heterogeneous population achieves better discrimination and detection than an equally sized homogeneous population constructed from shifted copies of the familys mean tuning curve, while using the same spike budget. Thus, homogeneous tuning is unstable under perturbations that preserve the mean tuning curve, because such perturbations leave metabolic cost unchanged while improving coding performance. We propose that such instability creates evolutionary pressure toward heterogeneity of tuning, making its prevalence a consequence of a process that optimizes coding performance under metabolic constraints.

Significance StatementThe tuning curves of cortical neurons vary substantially, raising the question of whether this diversity has functional significance or merely reflects biological noise. We show that perturbing an initially homogeneous population while preserving its mean tuning curve produces a heterogeneous population with better discrimination and detection performance at the same metabolic cost. Thus, tuning diversity may emerge as a natural consequence of selection for efficient coding under metabolic constraints.