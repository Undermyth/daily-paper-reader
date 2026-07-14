---
title: Changes in perceptual sampling contribute to representational drift
title_zh: 感知采样变化导致表征漂移
authors: "Yuan, Y., Serences, J., Aoi, M. C."
date: 2026-07-06
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.24.734121v3.full.pdf"
tags: ["query:comp-neuro"]
score: 7.0
evidence: 表征漂移与感知采样变化相关，涉及突触可塑性
tldr: 神经表征漂移通常归因于突触可塑性等内在神经动力学，但本文提出系统性行为变化（如注意力或注视点转移）也是潜在原因。通过纵向眼动追踪实验，让14名被试在2-4周内6次自由观看自然图像，发现注视模式的Wasserstein距离随时间增大，表明注视行为存在系统性方向性漂移。将注视掩膜图像输入腹侧视觉流层次模型CORnet-S后，各层表征距离随会话间隔增加而增大，且显著不同于随机对照。结果表明视觉采样的小但系统性变化足以引发视觉皮层的表征漂移，暗示行为细微变化可能是漂移的普遍驱动力。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-24-734121-v3/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1395, \"height\": 1257, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-24-734121-v3/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1352, \"height\": 1844, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-24-734121-v3/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1400, \"height\": 1592, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-24-734121-v3/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1361, \"height\": 1406, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-24-734121-v3/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1403, \"height\": 1443, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-24-734121-v3/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1325, \"height\": 1599, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-24-734121-v3/fig-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 1384, \"height\": 1588, \"label\": \"Figure\"}]"
motivation: 探究系统性的行为变化（如注视点转移）是否足以引发视觉皮层中的表征漂移，而不仅仅是内在神经回路重组。
method: 14名被试在6次跨2-4周的实验中自由观看自然图像，用Wasserstein距离量化注视模式相似性，并将注视掩膜图像输入CORnet-S模型计算表征距离。
result: 注视模式随时间呈系统性方向性漂移；模型各层表征距离随会话间隔增加而增大，且显著偏离随机分布。
conclusion: 视觉采样的小但系统性变化可独立于神经内在重构驱动表征漂移，提示行为细微变化可能是漂移的普遍原因。
---

## 摘要
随着时间的推移，同一刺激的神经反应模式逐渐发生变化，这种现象被称为表征漂移，在皮层区域中已被广泛观察到。漂移通常归因于突触可塑性或更新驱动的内在神经动力学。在这里，我们检验了一个补充假说，即漂移源于行为上的系统性变化，如注意力或注视点的转移。我们进行了一项纵向眼动追踪实验，14名成年人在跨越2-4周的6个实验阶段中自由观看自然图像，其中一部分图像在阶段内和阶段间重复。对于每个参与者，我们使用Wasserstein距离量化了阶段对之间注视密度图的相似性。随着阶段间时间间隔的增加，注视模式变得越来越不相似，表明注视行为存在系统性和方向性的漂移。为了评估这些行为变化是否可能合理地诱导神经表征变化，我们将注视掩蔽图像输入CORnet-S，这是一个灵长类腹侧视觉流的分层深度神经网络模型。表征距离（量化为成对激活差异的Frobenius范数）随着分离注视图的阶段数量在所有四个模型层（V1、V2、V4、IT）中增加。基于核的最大均值差异检验进一步证实，表征距离的经验分布与随机对照显著不同。这些发现表明，随着时间的推移，视觉场景采样的微小但系统性的变化足以引起视觉皮层中的表征漂移。更一般地，这些结果表明，即使在简单任务中，行为随时间的微妙变化也是不可避免的，并且这些变化可能足以在缺乏神经编码的内在重构的情况下驱动表征漂移。

作者总结：在视觉皮层表征漂移的研究中，重复刺激呈现时注意力和注视点的转移可以产生类似漂移的神经模式。虽然当前焦点是视觉采样变化对漂移的贡献，但结果提示，其他行为中的微妙变化（其中许多难以量化）可能驱动其他领域的漂移。

## Abstract
Gradual changes in neural response patterns to the same stimulus over time, termed representational drift, have been widely observed across cortical areas. Drift is typically attributed to intrinsic neural dynamics driven by synaptic plasticity or turnover. Here we test a complementary hypothesis that drift arises due to systematic changes in behavior such as shifts in attention or gaze. We conducted a longitudinal eye-tracking experiment in which fourteen adults freely viewed naturalistic images across 6 experimental sessions spanning 2-4 weeks, with a subset of images repeated within and across sessions. For each participant, we quantified the similarity of fixation density maps between session pairs using the Wasserstein distance. Fixation patterns became increasingly dissimilar with greater temporal separation between sessions, indicating systematic and directional drift in gaze behavior. To assess whether these behavioral changes could plausibly induce changes in neural representations, we passed fixation-masked images through CORnet-S, a hierarchical deep neural network model of the primate ventral visual stream. Representational distances, quantified as the Frobenius norm of pairwise activation differences, increased with the number of sessions that separated the fixation maps across all four model layers (V1, V2, V4, IT). A kernel-based maximum mean discrepancy test further confirmed that the empirical distribution of representational distances differed significantly from shuffled controls. These findings suggest that small but systematic shifts in the sampling of a visual scene over time are sufficient to cause representational drift in visual cortex. More generally, these results suggest that subtle changes in behavior over time are inevitable, even in simple tasks, and that these changes may be sufficient to drive representational drift in the absence of intrinsic reconfigurations of neural codes.

Author summaryIn studies of representational drift in visual cortex, shifts in attention and gaze across repeated stimulus exposures can produce drift-like neural patterns. While the current focus is on contributions of changes in visual sampling to drift, the results raise the possibility that other subtle changes in behavior, many that are hard to quantify, could drive drift in other domains.