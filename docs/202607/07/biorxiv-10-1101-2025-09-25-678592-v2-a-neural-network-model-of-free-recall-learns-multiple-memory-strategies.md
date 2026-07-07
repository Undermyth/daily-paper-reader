---
title: A neural network model of free recall learns multiple memory strategies
title_zh: 自由回忆的神经网络模型学习多种记忆策略
authors: "Li, M., Jensen, K. T., Zhang, Q., Lu, Q., Mattar, M. G."
date: 2026-07-06
pdf: "https://www.biorxiv.org/content/10.1101/2025.09.25.678592v2.full.pdf"
tags: ["query:la"]
score: 7.0
evidence: 自由回忆神经网络模型学习多种记忆策略
tldr: 人类自由回忆表现出结构化模式，但单一机制难以解释所有策略。本文让神经网络优化自由回忆任务，发现模型可发展出多种检索策略，其中最佳模型采用了一种刺激无关的索引编码，优先关注项目在列表中的位置而非时间情境，类似于记忆宫殿技术。该策略在鼓励回忆所有项目且避免近因效应时更易出现，揭示了专家级记忆表现的计算基础。
source: biorxiv
selection_source: fresh_fetch
motivation: 现有时间情境模型无法完全解释人类记忆策略多样性，尤其是专家采用的记忆宫殿技术。
method: 训练神经网络在自由回忆任务上优化，分析其发展出的不同检索策略，特别是索引编码的使用。
result: 最佳模型学会使用刺激无关的索引编码（项目位置）进行顺序回忆，优于依赖时间情境的策略。
conclusion: 人类记忆策略可由多种计算机制产生，基于索引的序列检索是专家级回忆的优化策略。
---

## 摘要
人类表现出有结构的记忆回忆模式，包括倾向于回忆更新的信息以及按照经历顺序回忆事件。经典的计算模型通过假设记忆融入了由刺激历史平滑整合形成的持续“时间情境”来解释这些模式。然而，单一机制能否解释人类记忆策略的全部 repertoire 尚不清楚，因为最优方法可能依赖于任务。例如，人类记忆专家广泛使用“记忆宫殿”策略，该策略在经验上更优，但未被时间情境模型捕捉。在这里，我们展示了为自由回忆优化的神经网络发展了多样化的检索策略，其中只有部分类似于时间情境模型。表现最佳的模型发现了一种刺激不变的索引码，它强调每个列表项目的研究位置，而不是其时间情境。这为类似于记忆宫殿技术的前向回忆创建了稳定的支架。当网络（i）被鼓励回忆所有研究过的项目而不是优先考虑少数项目，以及（ii）被阻止依赖近因效应时，这种索引码更可能出现，这与人类数据相符。我们的发现表明，类人回忆模式可以由多种不同的计算机制产生，并且使用项目索引的顺序检索是解释专家级回忆表现的最优策略。

## Abstract
Humans exhibit structured patterns of memory recall, including a tendency to recall more recent information and to recall events in the same order they were experienced. Classic computational models explain these patterns by positing that memories incorporate the ongoing ''temporal context'', formed by smoothly integrating the stimulus history. However, it is unclear whether a single mechanism can account for the full repertoire of human memory strategies, as the optimal approach may be task-dependent. For example, human memory experts widely apply the ''memory palace'' strategy, which is empirically better but not captured by temporal context models. Here we show that neural networks optimized for free recall develop diverse retrieval strategies, with only some of them resembling temporal context models.The best-performing models discovered a stimulus-invariant index code that emphasizes the studied position of each list item, instead of its temporal context. This creates a stable scaffold for forward recall akin to the memory palace technique. This index code was more likely to emerge when networks were i) encouraged to recall all studied items rather than prioritizing a few items, and ii) prevented from relying on recency, resonating with human data. Our findings demonstrate that human-like recall patterns can arise from multiple distinct computational mechanisms, and that sequential retrieval using item index is an optimal strategy that explains expert-level recall performance.