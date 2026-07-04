---
title: Inverse reinforcement learning reveals action-oriented value signals in naturalistic decision making
title_zh: 逆强化学习揭示自然决策中的行动导向价值信号
authors: "Lee, S. H., Chung, C., Oh, M.-h., Ahn, W.-Y."
date: 2026-06-29
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.24.733779v1.full.pdf"
tags: ["query:comp-neuro"]
score: 6.0
evidence: 自然任务中的决策价值信号
tldr: 自然决策中价值信号的计算是认知神经科学难题，标准模型难以适用。本文采用逆向强化学习从行为反推逐时刻奖励，并检验其神经表征。结果发现IRL奖励轨迹与背侧纹状体等行动导向脑区活动最相关，且涉及认知控制与感觉运动区域。这表明IRL奖励可有效揭示自然决策中行动导向的分布式价值信号。
source: biorxiv
selection_source: fresh_fetch
motivation: 标准计算模型难以解释自然环境中目标导向行为的实时价值计算，需探索逆向强化学习的神经可解释性。
method: 在fMRI实时驾驶任务中，使用逆向强化学习从观察行为导出逐时刻奖励轨迹，并与脑活动进行关联分析。
result: IRL奖励轨迹与背侧纹状体、认知控制及感觉运动脑区活动显著相关，集中于奖励回路。
conclusion: IRL奖励为自然决策提供了行为基础、时间解析的行动导向价值代理，揭示估价与多过程的交互。
---

## 摘要
认知神经科学的一个主要挑战是解释目标导向行为的价值如何在复杂和自然环境中计算。标准的决策计算模型在受控的、基于试次的范式中非常成功，但通常不适用于自然范式中实时展开的行为。逆强化学习（IRL）提供了一种从自然环境中观察到的行为推断潜在评估状态的方法，但其神经可解释性仍然很大程度上未知。在这里，我们研究了在fMRI扫描期间执行实时驾驶任务时，从IRL导出的瞬时奖励轨迹是否映射到大脑中的价值信号。IRL导出的奖励轨迹与背侧纹状体的活动关联最为显著，该区域常与价值导向的动作选择相关。它们还显示出与支持额外过程（包括认知控制和感觉运动处理）的分布区域有关联。这种模式表明IRL奖励捕获了以奖励回路为中心的分布式神经活动，可能反映了价值评估如何与其他过程相互作用。总之，这些发现表明，IRL奖励为自然决策中的行动导向评估提供了基于行为的、时间解析的代理指标。

## Abstract
A major challenge for cognitive neuroscience is to explain how value of a goal-directed behavior is computed in complex and naturalistic environments. Standard computational models of decision making have been highly successful in controlled, trial-based paradigms, but they are often ill-suited to real-time behavior unfolding in naturalistic paradigms. Inverse reinforcement learning (IRL) offers a way to infer latent evaluative state from observed behavior in naturalistic environments, but its neural interpretability remains largely unknown. Here, we investigated whether moment-to-moment reward trajectories derived from IRL map onto value signals in the brain during a real-time driving task performed during fMRI scanning. IRL-derived reward trajectories were most robustly associated with activity in the dorsal striatum, a region often linked to value-guided action selection. They also showed associations with distributed regions supporting additional processes, including cognitive control and sensorimotor processing. This pattern suggests that IRL reward captures distributed neural activity centered on the reward circuitry, potentially reflecting how valuation interacts with other processes. Together, these findings suggest that IRL reward provides a behaviorally grounded, temporally resolved proxy for action-oriented valuation during naturalistic decision making.