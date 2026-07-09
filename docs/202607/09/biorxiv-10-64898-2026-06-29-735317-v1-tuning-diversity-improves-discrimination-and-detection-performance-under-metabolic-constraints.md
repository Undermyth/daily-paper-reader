---
title: Tuning Diversity Improves Discrimination and Detection Performance under Metabolic Constraints
title_zh: 调节多样性可改善代谢约束下的辨别与检测性能
authors: "Ringach, D."
date: 2026-07-03
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.29.735317v1.full.pdf"
tags: ["query:comp-neuro"]
score: 6.0
evidence: 调谐多样性在代谢约束下改善神经群体编码
tldr: 皮层神经元调谐曲线呈现广泛多样性，其功能意义存疑。本研究在保持平均调谐曲线不变的条件下，构建由复制等间隔偏好角度的异质调谐曲线族组成的群体，并与同质群体比较，发现异质群体在相同代谢成本下实现更优的辨别和检测性能。这一发现表明调谐多样性是代谢约束下编码优化的进化产物，为皮层多样性提供了合理解释。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-29-735317-v1/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1623, \"height\": 373, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-29-735317-v1/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1257, \"height\": 592, \"label\": \"Figure\"}]"
motivation: 基于调谐多样性可改善群体编码的发现，研究其是否源于代谢约束下的编码优化。
method: 构建复制等间隔偏好角度的异质调谐曲线族，与同质群体在相同平均调谐曲线和尖峰预算下对比。
result: 异质群体在辨别和检测性能上显著优于同质群体，且代谢成本相同。
conclusion: 调谐多样性是代谢约束下优化编码性能的自然结果，同质调谐在该条件下不稳定。
---

## 摘要
皮层群体表现出广泛的调谐特性，这引发了关于这种变异性是皮层功能的一个特征还是一个缺陷的问题。先前的研究表明，调谐多样性可以通过减轻相关噪声的影响并提高几何表征的辨别和识别能力来改善群体编码。受这些发现的启发，我们研究了一个模型，其中针对一个循环变量编码的异质性调谐曲线族，以等间距的偏好角度进行复制。我们表明，与从该族平均调谐曲线的平移副本构建的同等大小的同质群体相比，这种异质性群体在相同的脉冲预算下实现了更好的辨别和检测。因此，在保持平均调谐曲线的扰动下，同质调谐是不稳定的，因为这种扰动在改善编码性能的同时不改变代谢成本。我们提出，这种不稳定性产生了朝向调谐异质性的进化压力，使其普遍存在成为在代谢约束下优化编码性能过程的结果。

意义声明 皮层神经元的调谐曲线差异很大，这引发了关于这种多样性是否具有功能意义或仅仅反映生物噪声的问题。我们表明，扰动一个初始同质的群体同时保持其平均调谐曲线，会产生一个具有更好辨别和检测性能且代谢成本相同的异质性群体。因此，调谐多样性可能是代谢约束下高效编码选择的自然结果。

## Abstract
Cortical populations exhibit a wide range of tuning properties, raising the question of whether such variability is a feature or a bug of cortical function. Prior work has shown that tuning diversity can improve population codes by mitigating the effects of correlated noise and increasing the discrimination and identification capacity of geometric representations. Motivated by these findings, we study a model in which a heterogeneous family of tuning curves, coding for a circular variable, is replicated at equally spaced preferred angles. We show that this heterogeneous population achieves better discrimination and detection than an equally sized homogeneous population constructed from shifted copies of the familys mean tuning curve, while using the same spike budget. Thus, homogeneous tuning is unstable under perturbations that preserve the mean tuning curve, because such perturbations leave metabolic cost unchanged while improving coding performance. We propose that such instability creates evolutionary pressure toward heterogeneity of tuning, making its prevalence a consequence of a process that optimizes coding performance under metabolic constraints.

Significance StatementThe tuning curves of cortical neurons vary substantially, raising the question of whether this diversity has functional significance or merely reflects biological noise. We show that perturbing an initially homogeneous population while preserving its mean tuning curve produces a heterogeneous population with better discrimination and detection performance at the same metabolic cost. Thus, tuning diversity may emerge as a natural consequence of selection for efficient coding under metabolic constraints.