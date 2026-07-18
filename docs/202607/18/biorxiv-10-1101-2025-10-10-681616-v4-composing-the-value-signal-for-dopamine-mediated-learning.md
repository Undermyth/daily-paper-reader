---
title: Composing the value signal for dopamine-mediated learning
title_zh: 构建多巴胺介导学习的价值信号
authors: "Mahajan, P., Seymour, B."
date: 2026-07-17
pdf: "https://www.biorxiv.org/content/10.1101/2025.10.10.681616v4.full.pdf"
tags: ["query:comp-neuro"]
score: 7.0
evidence: 熵正则化强化学习框架用于多巴胺介导的学习
tldr: 传统多巴胺奖励预测误差理论面临多奖励学习困难、非平稳环境适应慢、纹状体反应异质性等问题。本文提出熵正则化强化学习框架，将多巴胺优化目标扩展为奖励价值函数与偏离默认策略惩罚的联合。该离策略方法能组合多个奖励值、避免优先级变化时的干扰和遗忘，在非平稳环境中更高效。框架统一解释了纹状体内部和之间的多巴胺异质性，并为厌恶性和动作预测误差共存提供了规范性解释。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-10-10-681616-v4/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1681, \"height\": 934, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-10-10-681616-v4/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1681, \"height\": 1217, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-10-10-681616-v4/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1663, \"height\": 861, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-10-10-681616-v4/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1643, \"height\": 1679, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-10-10-681616-v4/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1694, \"height\": 1429, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-10-10-681616-v4/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1623, \"height\": 1196, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-10-10-681616-v4/fig-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 1606, \"height\": 575, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-10-10-681616-v4/fig-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 1671, \"height\": 525, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-10-10-681616-v4/fig-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 1665, \"height\": 879, \"label\": \"Figure\"}]"
motivation: 解决传统多巴胺奖励预测误差理论在多奖励学习、非平稳适应和纹状体异质性方面的挑战。
method: 采用熵正则化强化学习框架，将多巴胺优化目标扩展为奖励价值函数与偏离默认策略惩罚的联合。
result: 离策略方法能组合多奖励值、避免优先级变化干扰，在非平稳环境中更高效适应，并统一解释纹状体多巴胺异质性。
conclusion: 多巴胺介导的学习更可能是可组合的熵正则化价值函数的预测误差，而非单一广播预测误差。
---

## 摘要
关于多巴胺的经典奖励预测误差理论虽取得巨大成功，但面临若干关键挑战。最显著的是难以同时学习多个奖励、在线学习效率低下，以及无法解释纹状体内部和跨纹状体靶区观察到的异质性反应。本文通过一个规范的熵正则化强化学习框架来解决这些问题。我们提出，多巴胺优化的不仅是累积奖励，而是一个由偏离默认行为策略的惩罚所增强的奖励价值函数。在模拟中，这种离策略公式为组合多个奖励值提供了原则性解决方案，避免了多目标在线方法在优先级变化时出现的干扰和意外遗忘，并在奖励非平稳的环境中比标准替代方案更高效地适应。更广泛地，该框架为纹状体内部和跨纹状体靶区的多巴胺异质性提供了统一解释，包括理解为什么厌恶和行动预测误差可能共存于纹状体尾部的规范性方式。综上所述，这些结果表明，多巴胺介导的学习可能更恰当地被可组合的、熵正则化价值函数中的预测误差所捕捉，而非单个广播预测误差，并为未来实验提供了可检验的预测。

## Abstract
The seminal reward prediction error account of dopamine has been highly successful, but faces several key challenges. Most notable are the difficulty of learning multiple rewards simultaneously, inefficient on-policy learning, and accounting for the heterogeneous striatal responses observed across and within striatal targets. Here we address these issues with a normative entropy-regularised reinforcement-learning framework. We propose that dopamine optimises not just cumulative rewards, but a reward value function augmented by a penalty for deviating from a default behavioural policy. In simulations, this off-policy formulation provides a principled solution to composing multiple reward values, avoids the interference and unintended unlearning seen in multi-objective on-policy methods when priorities change, and adapts more efficiently than standard alternatives in environments with non-stationary rewards. More broadly, the framework offers a unified account of dopamine heterogeneity between and within striatal targets, including a normative way to understand why aversive and action prediction errors may coexist in the tail of the striatum. Together, these results suggest that dopamine-mediated learning may be better captured by prediction errors in composable, entropy-regularised value functions than by a single broadcast prediction error, and offer testable predictions for future experiments.