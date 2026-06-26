---
title: Modeling Dynamical Vision with Biologically Plausible Recurrent Convolutional Networks
title_zh: 具有生物合理性的递归卷积网络建模动态视觉
authors: "Gutzen, R., Lindsay, G. W."
date: 2026-06-26
pdf: "https://www.biorxiv.org/content/10.1101/2025.08.11.669756v2.full.pdf"
tags: ["query:comp-neuro"]
score: 7.0
evidence: 生物合理的循环网络建模视觉皮层动力学
tldr: "标准前馈CNN缺乏视觉皮层中普遍存在的循环连接，难以模拟适应、延迟归一化等时空动态。本文提出DynVision开源工具箱，基于ODE求解器和异质延迟实现五种循环类型，通过配置驱动设计分离建模决策与实现细节。实验表明该方法在参数探索中加速52%，并发现循环集成位置和时间窗口敏感；连续时间循环可自然产生皮层时间现象，特定配置达到类人噪声鲁棒性。该框架为系统比较不同循环架构提供了可扩展平台，推动生物视觉建模发展。"
source: biorxiv
selection_source: fresh_fetch
motivation: 传统前馈CNN无法模拟视觉皮层的循环动力学，现有工具难以系统比较不同循环架构对动态和行为的塑造。
method: 开发模块化开源工具箱DynVision，实现ODE数值求解器、异质延迟及五种侧向循环类型，采用配置驱动设计分离建模与实现。
result: "训练加速52%；循环集成位置和损失时间窗口显著影响动态特性；连续时间循环自然产生皮层现象，特定配置达到人类水平噪声鲁棒性。"
conclusion: 不同循环配置具有功能差异，强调需要综合建模框架以应对创建完全真实模型的挑战。
---

## 摘要
用于图像识别的卷积神经网络（CNN）已显示出与灵长类腹侧视觉通路显著的概念相似性，但其标准前馈架构缺乏视觉皮层中普遍存在的递归连接。这种递归被认为支撑了诸如适应、延迟归一化和对噪声输入的鲁棒性等时空现象。然而，将功能上有益的递归纳入能够捕捉生物视觉时空现象的CNN仍然具有挑战性。尽管最近的进展已经融入了神经生物学约束，但该领域缺乏可用的工具来系统地比较不同的架构选择（如递归类型、时间延迟和连接模式）如何塑造神经动力学和行为。在此，我们介绍DynVision，一个模块化的开源工具箱，用于构建和评估具有生物合理性的递归卷积神经网络（RCNN）。DynVision实现了具有异质性延迟的数值ODE求解器，支持从简单自连接到皮层组织的局部递归的五种侧向递归类型，并通过配置驱动的设计将科学建模决策与实现细节分离。训练计算效率高，相比参考实现实现了52%的加速。我们通过系统探索参数空间来演示该框架，揭示出时间动态的定性差异对经常隐含的建模选择（如递归整合的目标位置和用于损失计算的时间窗口）高度敏感。关键的是，我们发现连续时间递归动态可以自然地产生皮层时间现象，而无需显式的除法归一化，而另一种递归配置产生的噪声鲁棒性接近人类水平的表现。这些发现暗示了功能上不同的递归配置，并突出了创建完全真实模型的挑战，从而强调了需要一个全面且连贯的建模框架来辅助探索。代码和文档可在https://github.com/Lindsay-Lab/DynVision/获取。

## Abstract
Convolutional Neural Networks (CNNs) trained for image recognition have demonstrated remarkable conceptual similarities to the primate ventral visual pathway, but their standard feedforward architectures lack the recurrent connections that are ubiquitous in visual cortex. Such recurrence is thought to underlie spatiotemporal phenomena including adaptation, delayed normalization, and robustness to noisy input.However, incorporating functionally beneficial recurrence into CNNs that captures spatiotemporal phenomena of biological vision remains challenging. Although recent advances have incorporated neurobiological constraints, the field lacks accessible tools for systematically comparing how different architectural choices, such as recurrence type, temporal delays, and connectivity patterns, shape neural dynamics and behavior. Here, we introduce DynVision, a modular open-source toolbox for constructing and evaluating biologically plausible recurrent convolutional neural networks (RCNNs). DynVision implements numerical ODE solvers with heterogeneous delays, supports five types of lateral recurrence ranging from simple self-connections to cortically-organized local recurrence, and separates scientific modeling decisions from implementation details through a configuration-driven design. Training is computationally efficient, achieving a 52% speedup over reference implementations.We demonstrate the framework through systematic exploration of the parameter space, revealing that qualitative differences in temporal dynamics are highly sensitive to often-implicit modeling choices such as the target location of recurrent integration and the temporal window used for loss computation. Critically, we find that continuous-time recurrent dynamics can naturally give rise to cortical temporal phenomena without requiring explicit divisive normalization, while a different recurrent configuration produces noise robustness approaching human-level performance. These findings suggest functionally distinct configurations of recurrence and highlight the challenge of creating fully realistic models, thus emphasizing the need for a comprehensive and cohesive modeling framework to aid exploration. Code and documentation are available at https://github.com/Lindsay-Lab/DynVision/.