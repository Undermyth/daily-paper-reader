---
title: Interpretable compositional computation with recurrent neural networks
title_zh: 基于循环神经网络的可解释组合计算
authors: "Pezon, L., Van Meegen, A."
date: 2026-06-29
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.23.733979v1.full.pdf"
tags: ["query:comp-neuro"]
score: 7.0
evidence: 循环神经网络的组合动力学
tldr: 灵活认知依赖可重用组件，但神经网络中共享动态结构的性质尚不清楚。本文基于低秩循环神经网络，发展了一套可解释的组合计算理论，揭示低维潜在空间中存在共享潜在成分，它们虽不在神经活动中显式出现，但可通过连接统计和神经表征的标志识别。该理论提供了组合计算的可测试预测，并区分了任务依赖性进入计算的不同方式。
source: biorxiv
selection_source: fresh_fetch
motivation: 理解神经网络如何通过共享动态结构实现可重用组件的组合计算，并揭示其机制。
method: 通过分析低秩循环神经网络的低维潜在空间，识别共享潜在成分及其在连接和表征中的标志。
result: 共享潜在成分在神经活动中不显式出现，但可通过统计学标志识别，且与任务依赖性活动兼容。
conclusion: 提供了组合计算的可解释机制与可测试预测，为灵活认知的神经基础提供了新的理解。
---

## 摘要
灵活认知利用可重用组件，使行为能够快速适应不同情境或任务。对多任务训练的人工神经网络分析表明，这种组合性由跨任务共享和重用的动力学结构支持。然而，这些共享组件的本质以及它们如何以任务依赖的方式被使用仍不清楚。在此，我们基于低秩循环神经网络低维潜在空间中的共享动力学结构，发展了一种可解释组合计算的理论。我们表明，这些“共享潜在组件”在神经活动中并不直接可见，因此与任务依赖的活动兼容。我们在连接统计和神经表征中识别出共享潜在组件的标志。这些标志为网络对特定扰动实验的反应提供了可检验的预测。最后，我们识别出任务依赖性可以进入计算的不同位点，使我们能够表征组合任务的定性不同解决方案。总之，我们的理论提供了通过低秩网络中的共享组件实现组合计算的机制性理解和可检验标志。

## Abstract
Flexible cognition utilizes reusable components to enable rapid adaptation of behavior to different contexts or tasks. Analysis of artificial neural networks trained on multiple tasks suggested that this compositionality is supported by dynamical structures which are shared and re-used across tasks. However, the nature of these shared components, and how they can be used in a task-dependent manner, remained unclear. Here, we develop a theory of interpretable compositional computation based on shared dynamical structures in the low-dimensional latent space of low-rank recurrent neural networks. We show that these "shared latent components" are not immediately visible in the neural activity, and are thus compatible with task-dependent activity. We identify hallmarks of shared latent components both in the connectivity statistics and the neural representations. These hallmarks yield testable predictions for the network's response to specific perturbation experiments. Finally, we identify distinct loci where task-dependence can enter the computation, allowing us to characterize qualitatively different solutions to compositional tasks. In summary, our theory provides a mechanistic understanding and testable hallmarks of compositional computation via shared components in low-rank networks.