---
title: Uncovering dynamic human brain phase coherence networks
title_zh: 揭示动态人脑相位相干网络
authors: "Olsen, A. S., Brammer, A., Fisher, P. M., Moerup, M."
date: 2026-06-26
pdf: "https://www.biorxiv.org/content/10.1101/2024.11.15.623830v5.full.pdf"
tags: ["query:comp-neuro"]
score: 6.0
evidence: 大脑相位相干性动态网络；计算神经科学方法
tldr: 传统脑功能连接分析多依赖信号幅度相关性，易受噪声和伪影干扰。本文提出复角高斯混合模型，直接对fMRI信号相位进行建模，以捕捉全脑动态同步模式。模型可重复识别出不同认知任务下的同步活动状态，并泛化至未见过的个体，无需任务标签。该方法为研究大规模神经协调提供了稳健且可解释的新视角。
source: biorxiv
selection_source: fresh_fetch
motivation: 传统基于信号幅度的功能连接对噪声敏感，难以有效捕捉脑区间的动态同步模式。
method: 提出复角高斯混合模型，对fMRI信号相位进行无监督聚类，直接分析全脑相位一致性网络的状态。
result: 模型识别出可区分认知任务的重复同步状态，且无需训练标签即可泛化至新个体。
conclusion: 相位建模提供了干净、信息丰富的脑同步动态视图，为研究大规模神经协调开辟了新途径。
---

## 摘要
复杂的认知功能依赖于分布式脑区之间的协调通信，但捕捉这些随时间演变的相互作用仍然具有挑战性。传统的功能脑连接分析主要依赖于信号幅度的相关性，但这些相关性对噪声和头部运动等伪迹敏感。在这里，我们引入了一种混合建模方法，该方法聚焦于脑信号的相位，从而能够直接且完整地研究大规模脑相位相干网络中的动态同步模式。我们为相位建模奠定了数学和概念基础，并引入了复角中心高斯混合模型，为分析全脑基于相位的相互作用提供了一种规范方法。将该模型应用于fMRI数据，它识别出反复出现的全脑同步活动状态，这些状态能够可靠地区分认知任务，并在未见过的个体中泛化，而训练过程中无需任何任务标签。这些结果表明，对信号相位进行建模能够提供关于脑同步动态的清晰且信息丰富的视角，为研究大规模神经协调开辟了新途径。

意义声明：理解人脑如何协调跨远距离区域的活动是解释认知和行为的核心。大多数现有方法通过追踪信号强度的变化来研究这些相互作用，而这可能受到非神经伪迹的强烈影响。在这里，我们转而关注脑信号之间的相位关系：脑区域如何同步其振荡，形成动态的相位相干网络。我们引入了一个灵活且规范的混合建模框架来直接捕捉这些模式，并揭示出个体间一致反复出现的全脑同步活动状态。该方法能够揭示不同认知任务之间的有意义差异，而训练过程中无需任务标签。通过强调信号相位而非幅度，我们的方法为研究动态脑同步模式提供了一种互补的、鲁棒且可解释的途径。

## Abstract
Complex cognitive functions rely on coordinated communication between distributed brain regions, yet capturing these interactions as they evolve over time remains challenging. Traditional analyses of functional brain connectivity largely rely on correlations in signal amplitude, which are sensitive to noise and artifacts such as head motion. Here, we introduce a mixture modeling approach that focuses on the phase of brain signals, allowing dynamic patterns of large-scale synchronization in brain phase coherence networks to be studied directly and in their entirety. We lay the mathematical and conceptual groundwork for phase modeling and introduce the complex angular central Gaussian mixture model, providing a principled way to analyze phase-based interactions across the brain. Applied to fMRI data, the model identifies recurring states of brain-wide synchronized activity that reliably distinguish cognitive tasks and generalize across previously unseen individuals, without requiring any task labels during training. These results show that modeling signal phase offers a clean and informative view of brain synchronization dynamics, opening new avenues for studying large-scale neural coordination.

Significance statementUnderstanding how the human brain coordinates activity across distant regions is central to explaining cognition and behavior. Most existing approaches study these interactions by tracking changes in signal strength, which can be strongly affected by non-neural artifacts. Here, we focus instead on the phase relationships between brain signals: How brain regions synchronize their oscillations forming dynamic phase coherence networks. We introduce a flexible and principled mixture modeling framework to capture these patterns directly and reveal recurring states of brain-wide synchronized activity consistent across individuals. This approach uncovers meaningful differences between diverse cognitive tasks, without requiring task labels during training. By emphasizing signal phase rather than amplitude, our method offers a complementary robust and interpretable way to study dynamic brain synchronization patterns.