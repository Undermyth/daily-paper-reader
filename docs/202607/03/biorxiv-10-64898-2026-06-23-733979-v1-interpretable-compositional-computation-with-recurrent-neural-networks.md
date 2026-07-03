---
title: Interpretable compositional computation with recurrent neural networks
title_zh: 基于循环神经网络的可解释组合计算
authors: "Pezon, L., Van Meegen, A."
date: 2026-06-29
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.23.733979v1.full.pdf"
tags: ["query:comp-neuro"]
score: 7.0
evidence: RNN的可解释组合计算，共享动态结构，任务依赖重配置
tldr: 循环神经网络中组合计算依赖跨任务共享的动态结构，但其本质及任务依赖使用方式尚不清楚。本文针对低秩循环神经网络，发展基于低维潜空间共享结构的可解释组合计算理论，证明共享组件不直接显现于神经活动但兼容任务依赖响应，并识别连接统计和表征中的标志。该理论揭示了任务依赖进入计算的不同位点，提供了组合计算的机制性理解和实验可测试预测。
source: biorxiv
selection_source: fresh_fetch
motivation: 循环神经网络中组合计算依赖共享动态组件，但其本质及任务依赖使用方式尚不清楚。
method: 利用低秩循环神经网络，分析其低维潜空间中共享动态结构，构建可解释组合计算理论。
result: 发现共享潜组件不直接显现于神经活动但兼容任务依赖响应，识别连接统计和神经表征中的标志。
conclusion: 为组合计算提供了机制性理解和实验可测试标志，加深对灵活认知神经基础的认识。
---

## 摘要
灵活认知利用可复用组件实现对不同情境或任务的快速行为适应。对多任务训练的人工神经网络分析表明，这种组合性得到跨任务共享和复用的动力学结构支持。然而，这些共享组件的本质及其任务依赖的使用方式尚不清楚。本文基于低秩循环神经网络低维潜空间中的共享动力学结构，提出一种可解释组合计算理论。我们证明这些共享潜成分在神经活动中并非直接可见，因此与任务依赖的活动兼容。我们在连接统计和神经表征中识别出共享潜成分的特征。这些特征为网络对特定扰动实验的响应提供了可检验的预测。最后，我们确定了任务依赖性进入计算的不同位置，从而能够表征组合任务的定性不同解。总之，我们的理论通过低秩网络中的共享组件，为组合计算提供了机制性理解和可检验特征。

## Abstract
Flexible cognition utilizes reusable components to enable rapid adaptation of behavior to different contexts or tasks. Analysis of artificial neural networks trained on multiple tasks suggested that this compositionality is supported by dynamical structures which are shared and re-used across tasks. However, the nature of these shared components, and how they can be used in a task-dependent manner, remained unclear. Here, we develop a theory of interpretable compositional computation based on shared dynamical structures in the low-dimensional latent space of low-rank recurrent neural networks. We show that these shared latent components are not immediately visible in the neural activity, and are thus compatible with task-dependent activity. We identify hallmarks of shared latent components both in the connectivity statistics and the neural representations. These hallmarks yield testable predictions for the networks response to specific perturbation experiments. Finally, we identify distinct loci where task-dependence can enter the computation, allowing us to characterize qualitatively different solutions to compositional tasks. In summary, our theory provides a mechanistic understanding and testable hallmarks of compositional computation via shared components in low-rank networks.