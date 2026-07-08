---
title: Changes in perceptual sampling contribute to representational drift
title_zh: 知觉采样的变化导致表征漂移
authors: "Yuan, Y., Aoi, M. C., Serences, J."
date: 2026-06-30
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.24.734121v1.full.pdf"
tags: ["query:comp-neuro"]
score: 7.0
evidence: 表征漂移归因于突触可塑性和注意力变化
tldr: 神经表征漂移通常被认为源于内在神经动态，但本研究提出行为变化也可能导致漂移。通过纵向眼动追踪实验，14名被试在2-4周内多次自由观看自然图像，注视模式随实验间隔增加呈现系统性漂移。将注视掩码图像输入CORnet-S模型后，各层表征距离也随间隔增加而显著增大。这表明注视模式的系统性变化足以驱动视觉皮层的表征漂移，无需内在重构。
source: biorxiv
selection_source: fresh_fetch
motivation: 检验行为变化（如注视模式）是否足以引起视觉皮层的表征漂移。
method: 纵向眼动追踪实验记录14名被试多次观看自然图像的注视模式，并用CORnet-S模型计算表征距离。
result: 注视模式随间隔增加而漂移，模型各层表征距离也显著增大。
conclusion: 行为中微小的系统性变化足以导致视觉表征漂移，提示行为因素在神经漂移中的重要作用。
---

## 摘要
随着时间的推移，同一刺激的神经反应模式逐渐发生变化，这种现象被称为表征漂移，已在多个皮层区域被广泛观察到。漂移通常归因于由突触可塑性或周转驱动的内在神经动力学。在这里，我们测试了一个互补的假设：漂移是由于行为上的系统性变化（如注意力或注视转移）引起的。我们进行了一项纵向眼动追踪实验，14名成年人在2-4周内的6个实验环节中自由观看自然图像，其中一部分图像在环节内和环节间重复出现。对于每位参与者，我们使用Wasserstein距离量化了环节对之间的注视密度图相似性。随着环节之间时间间隔的增大，注视模式变得越来越不相似，表明注视行为存在系统性和方向性的漂移。为了评估这些行为变化是否可能合理地诱导神经表征的变化，我们将注视掩蔽图像输入CORnet-S，这是一个灵长类动物腹侧视觉通路的层次化深度神经网络模型。以配对激活差异的Frobenius范数量化的表征距离，随着分离注视图的环节数量增加而增大，在所有四个模型层（V1、V2、V4、IT）中均如此。基于核的最大均值差异检验进一步证实，表征距离的经验分布与打乱的控制组有显著差异。这些发现表明，随时间推移对视觉场景的采样的微小但系统性的变化足以引起视觉皮层中的表征漂移。更一般地，这些结果表明，即使在简单任务中，随时间推移的行为微妙变化是不可避免的，并且这些变化可能足以在没有神经编码内在重组的情况下驱动表征漂移。

作者总结在视觉皮层表征漂移的研究中，重复刺激呈现过程中注意力和注视的变化可以产生类似漂移的神经模式。虽然当前的重点是视觉采样的变化对漂移的贡献，但这些结果提出了可能性：其他行为上的微妙变化（许多难以量化）可能驱动其他领域的漂移。

## Abstract
Gradual changes in neural response patterns to the same stimulus over time, termed representational drift, have been widely observed across cortical areas. Drift is typically attributed to intrinsic neural dynamics driven by synaptic plasticity or turnover. Here we test a complementary hypothesis that drift arises due to systematic changes in behavior such as shifts in attention or gaze. We conducted a longitudinal eye-tracking experiment in which fourteen adults freely viewed naturalistic images across 6 experimental sessions spanning 2-4 weeks, with a subset of images repeated within and across sessions. For each participant, we quantified the similarity of fixation density maps between session pairs using the Wasserstein distance. Fixation patterns became increasingly dissimilar with greater temporal separation between sessions, indicating systematic and directional drift in gaze behavior. To assess whether these behavioral changes could plausibly induce changes in neural representations, we passed fixation-masked images through CORnet-S, a hierarchical deep neural network model of the primate ventral visual stream. Representational distances, quantified as the Frobenius norm of pairwise activation differences, increased with the number of sessions that separated the fixation maps across all four model layers (V1, V2, V4, IT). A kernel-based maximum mean discrepancy test further confirmed that the empirical distribution of representational distances differed significantly from shuffled controls. These findings suggest that small but systematic shifts in the sampling of a visual scene over time are sufficient to cause representational drift in visual cortex. More generally, these results suggest that subtle changes in behavior over time are inevitable, even in simple tasks, and that these changes may be sufficient to drive representational drift in the absence of intrinsic reconfigurations of neural codes.

Author summaryIn studies of representational drift in visual cortex, shifts in attention and gaze across repeated stimulus exposures can produce drift-like neural patterns. While the current focus is on contributions of changes in visual sampling to drift, the results raise the possibility that other subtle changes in behavior, many that are hard to quantify, could drive drift in other domains.