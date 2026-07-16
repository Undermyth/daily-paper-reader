---
title: "Data-driven oscillatory network modeling with condition-dependent coupling laws: Identifying directed neural interactions in working memory attention dynamics"
title_zh: 数据驱动的具有条件依赖性耦合律的振荡网络建模：识别工作记忆注意动态中的定向神经交互
authors: "Ohkawa, M., Zhou, Y. J., Haegens, S., Jafarian, M."
date: 2026-07-10
pdf: "https://www.biorxiv.org/content/10.64898/2026.07.06.736523v1.full.pdf"
tags: ["query:comp-neuro"]
score: 7.0
evidence: 提出数据驱动振荡网络建模框架，推断工作记忆注意力动态中的条件依赖神经连接
tldr: 大脑在干扰下适应新信息的能力与注意力和工作记忆的动态交互有关。本文提出数据驱动的振荡网络建模框架，从神经记录学习条件依赖的耦合定律。应用通用微分方程和符号回归分析MEG数据，识别出干扰条件下从背外侧前额叶皮层到初级视觉皮层的定向路径。该方法无需强先验假设即可发现适应性变化中的候选定向通路。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-06-736523-v1/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1467, \"height\": 528}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-06-736523-v1/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1359, \"height\": 452}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-06-736523-v1/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1012, \"height\": 473}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-06-736523-v1/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1368, \"height\": 500}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-06-736523-v1/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1367, \"height\": 1003}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-06-736523-v1/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 909, \"height\": 1265}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-06-736523-v1/fig-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 1492, \"height\": 401}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-06-736523-v1/fig-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 1056, \"height\": 704}]"
tables_json: "[{\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-07-06-736523-v1/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1350, \"height\": 206}, {\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-07-06-736523-v1/table-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 892, \"height\": 199}]"
motivation: 现有方法难以从神经数据中识别条件依赖的耦合变化，需要不依赖强先验的框架来揭示注意力与工作记忆的动态交互机制。
method: 构建线性振荡网络模型，用通用微分方程捕捉干扰引起的耦合变化，通过符号回归获得可解释的非线性函数，并识别新兴非线性项对应的定向路径。
result: 四个被试的MEG数据均显示干扰条件下从dlPFC到V1的定向通路出现，与认知控制中dlPFC的已知作用一致。
conclusion: 结合线性模型、通用微分方程和可解释性方法能有效识别条件依赖的耦合定律及定向通路，为研究动态脑网络提供新途径。
---

## 摘要
在有干扰物和变化条件的情况下学习新信息需要适应能力。在大脑中，这种适应能力与注意和工作记忆之间的动态交互有关，这些交互能够选择性地过滤无关输入，同时保留与行为相关的信息。特定的神经振荡被认为参与了这个过程。

在这里，我们引入了一个现象学数据驱动的振荡网络建模框架，该框架直接从神经记录中学习条件依赖性耦合律，并能够推断条件依赖的定向通路。我们将该方法应用于参与者执行有或没有干扰物的工作记忆任务时收集的脑磁图数据。首先使用线性振荡网络对无干扰条件下的回忆动态进行建模，其中每个感兴趣区域由两个α波段谐波振荡器表示。我们使用通用微分方程（UDF，神经微分方程的扩展）来捕捉干扰物引起的耦合律变化。然后使用符号回归将UDF识别出的修改解释为非线性函数，并提出额外的方法来从新出现的非线性项中识别出感兴趣脑区动力学的定向通路。

尽管存在个体间差异，但所有四名参与者在有干扰条件下检查的工作记忆回忆数据显示，出现了从背外侧前额叶皮层到初级视觉皮层的通路。这一发现与背外侧前额叶皮层在认知控制中的既定作用一致，并表明干扰物处理招募了从前额叶到视觉区域的定向交互。更广泛地说，我们的结果表明，将数据学习参数的线性模型与通用微分方程（通过可解释性方法增强）相结合，能够识别条件依赖的耦合律，将其表示为可解释的数学函数，并发现振荡网络中适应性变化背后的候选定向通路，而无需对潜在机制做出强先验假设。

## Abstract
Learning new information in the presence of distracters and changing conditions requires the ability to adapt. In the brain, this adaptive capability has been linked to dynamic interactions between attention and working memory, which enable the selective filtering of irrelevant input while preserving behaviorally relevant information. Specific neural oscillations have been implicated in this process.

Here, we introduce a phenomenological data-driven framework for oscillatory network modeling that learns condition-dependent coupling laws directly from neural recordings and enables inference of condition-dependent directed pathways. We apply our approach to magnetoen-cephalography (MEG) data collected while participants performed a working-memory task with and without distracters. Recall dynamics in the non-distracter condition are first modeled using a linear oscillatory network in which each region of interest is represented by two alpha-band harmonic oscillators. We use universal differential equations (UDE), an extension of neural differential equations, to capture distracter-induced changes in coupling laws. Symbolic regression is then used to interpret the modifications identified by UDE as nonlinear functions, and an additional method is proposed to identify the directed pathway from the newly emerging nonlinear terms in the dynamics of brain regions of interest.

Despite inter-subject variability, working memory recall data from all four participants examined under distraction showed the emergence of a pathway from the dorsolateral prefrontal cortex (dlPFC) to the primary visual cortex (V1). This finding is consistent with the established role of the dlPFC in cognitive control and suggests that distracter processing recruits a directed interaction from prefrontal to visual regions. More broadly, our results illustrate that combining linear models whose parameters are learned from the data with universal differential equations augmented by interpretability methods enables the identification of condition-dependent coupling laws, their representation as interpretable mathematical functions, and the discovery of candidate directed pathways underlying adaptive changes in oscillatory networks without requiring strong prior assumptions about the underlying mechanisms.