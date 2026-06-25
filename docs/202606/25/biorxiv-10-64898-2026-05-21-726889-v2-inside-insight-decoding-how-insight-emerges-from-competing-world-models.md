---
title: "Inside insight: decoding how insight emerges from competing world models"
title_zh: 内在洞察：解码洞见如何从竞争的世界模型中涌现
authors: "Inutsuka, K., Nishioka, T., Macpherson, T., Fujiwara, M., Hikida, T., Naoki, H."
date: 2026-06-23
pdf: "https://www.biorxiv.org/content/10.64898/2026.05.21.726889v2.full.pdf"
tags: ["query:comp-neuro"]
score: 7.0
evidence: 将洞察建模为世界模型重构，并从行为数据推断转换
tldr: 顿悟被概念化为世界模型重组带来的突然领悟，但其潜在动态难以直接观测。本文提出IID机器学习框架，从行为数据中推断小鼠在间接和直接规则任务中世界模型转换的时机与机制。分析发现间接任务适用门控学习，直接任务适用并行学习。IID为仅从行为量化顿悟动态开辟了新途径。
source: biorxiv
selection_source: fresh_fetch
motivation: 理解顿悟如何从竞争的世界模型重组中涌现，需解析难以观测的潜在动态。
method: 提出IID框架，基于行为数据估计世界模型转换时机，比较门控学习与并行学习机制。
result: 间接规则任务由门控学习最佳解释，直接规则任务由并行学习最佳解释。
conclusion: IID能从行为中量化顿悟动态，揭示不同任务下的世界模型学习机制。
---

## 摘要
洞见何时以及如何涌现？我们将洞见概念化为一种源自重构世界模型的突然领悟：一个将行动与结果联系起来的内部解释。然而，这些潜在的动态过程即使通过行为和口头报告也难以触及。在此，我们发展了内在洞察动态（IID）这一机器学习框架，能从行为数据中估计潜在的世界模型动态。利用IID，我们分析了间接规则和直接规则任务中的小鼠行为，这两项任务都需要从初始世界模型转向符合规则的表示。IID通过估计竞争世界模型之间转换的时间点来推断类似洞见的转变“何时”发生，并通过比较其背后的不同学习过程来探讨“如何”发生。这一分析揭示了世界模型学习的不同机制：间接规则任务和直接规则任务分别由门控学习和并行学习更好地解释。因此，IID开辟了一条仅通过可观察行为来量化潜在洞见动态的路径。

## Abstract
When and how does insight emerge? We conceptualize insight as a sudden realization arising from restructuring a world model: an internal interpretation linking actions to outcomes. Yet these latent dynamics remain difficult to access, even with behavior and verbal report. Here we developed inside insight dynamics (IID), a machine-learning framework that estimates latent world-model dynamics from behavioral data. Using IID, we analyzed mouse behavior in indirect- and direct-rule tasks, each requiring a shift from an initial world model to a rule-consistent representation. IID inferred the "when" of insight-like shifts by estimating the timing of transitions between competing world models, and examined the "how" by comparing alternative learning processes underlying them. This analysis revealed distinct mechanisms of world-model learning: the indirect- and direct-rule tasks were better explained by gated learning and parallel learning, respectively. Thus, IID opens a route to quantifying latent insight dynamics from observable behavior alone.