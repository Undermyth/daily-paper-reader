---
title: Closed-loop control of in vitro neuronal activity using reinforcement learning after in silico pre-training
title_zh: 使用强化学习在计算机预训练后对体外神经元活动进行闭环控制
authors: "Carvalho, E., Mateus, J. C., Pinto, R., Aroso, M., Aguiar, P."
date: 2026-07-20
pdf: "https://www.biorxiv.org/content/10.64898/2026.07.13.738298v1.full.pdf"
tags: ["query:comp-neuro"]
score: 7.0
evidence: 强化学习用于体外神经元闭环控制
tldr: 神经调控需要控制神经元活动，但生物网络复杂且非平稳。本研究采用强化学习在仿真中预训练控制策略，再迁移至体外培养神经元，实现了高效的网络爆发现状控制。迁移策略优于启发式控制，且刺激使用受限。钙成像揭示了策略通过时空优化利用局部拓扑和生理动态。该工作表明可从数字孪生直接迁移有效控制策略至活体网络。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-13-738298-v1/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1913, \"height\": 964, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-13-738298-v1/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1876, \"height\": 1619, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-13-738298-v1/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1915, \"height\": 1068, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-13-738298-v1/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1892, \"height\": 1844, \"label\": \"Figure\"}]"
motivation: 强化学习用于神经调控需大量探索，但活体组织有生理限制，需高效策略转移。
method: 在生物物理校准的数字孪生中预训练强化学习控制策略，再迁移至体外培养神经元网络。
result: 迁移策略优于启发式控制，同时约束刺激使用；钙成像揭示其利用局部网络拓扑和生理时间动态。
conclusion: 体外脑芯片可作为强化学习神经调控的可行阶梯，数字孪生策略可直接迁移至活体网络。
---

## 摘要
通过电刺激控制特定的神经元动力学对于治疗性神经调控至关重要，但由于生物神经元网络的复杂性和非平稳性，推导最优控制策略仍然具有挑战性。虽然强化学习（RL）提供了强大的闭环控制框架，但其对长时间刺激驱动的探索的依赖难以与活体组织的生理限制相协调。在这里，我们展示了一种从计算机到体外的迁移策略，该策略实现了对培养神经元中网络爆发的有效状态依赖控制。迁移后的策略优于启发式控制，同时保持了受限的刺激使用。同步钙成像揭示了所学策略的机制基础：智能体在空间和时间上优化刺激，利用局部网络拓扑和内在的生理时间动力学。这些结果将体外脑芯片培养确立为基于强化学习的神经调控的一个易于处理的垫脚石，并证明可以在生物物理校准的数字孪生中推导出有效的控制策略，并直接迁移到活体网络中。

## Abstract
Controlling specific neuronal dynamics with electrical stimulation is critical for therapeutic neuromodulation, yet deriving optimal control policies remains challenging due to the complex and non-stationary nature of biological neuronal networks. While reinforcement learning (RL) offers a powerful closed-loop control framework, its reliance on prolonged stimulus-driven exploration is difficult to reconcile with the physiological limits of living tissue. Here, we demonstrate an in silico-to-in vitro transfer strategy that achieves efficient state-dependent control of network bursting in cultured neurons. The transferred policy outperforms heuristic controls, while maintaining constrained stimulation usage. Concurrent calcium imaging reveals the mechanistic basis of the learned policy: the agent optimizes stimulation spatially and temporally, exploiting local network topology and intrinsic physiological temporal dynamics. These results establish in vitro brain-on-chip cultures as a tractable stepping stone for RL-based neuromodulation and demonstrate that effective control policies can be derived in biophysically calibrated digital twins and transferred directly to living networks.