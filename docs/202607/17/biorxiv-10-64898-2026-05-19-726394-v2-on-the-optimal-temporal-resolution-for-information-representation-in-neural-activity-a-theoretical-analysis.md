---
title: "On the Optimal Temporal Resolution for Information Representation in Neural Activity: A Theoretical Analysis"
title_zh: 论神经活动中信息表示的最优时间分辨率：一项理论分析
authors: "Ahmed, H. F., Samiei, T., Nozari, E."
date: 2026-07-14
pdf: "https://www.biorxiv.org/content/10.64898/2026.05.19.726394v2.full.pdf"
tags: ["query:comp-neuro"]
score: 6.0
evidence: 神经信息表示最优时间分辨率的理论分析
tldr: 神经活动的时间尺度对信息表示有重要影响，但最优尺度的理论尚缺。本文构建多尺度模型，推导不同时间分辨率下的敏感度指数，发现信号与噪声自相关是决定因素。当两者都衰减时，时间积分产生权衡，中等尺度成为最优。该框架解释了预处理操作对解码能力的影响，提供了可验证预测。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-05-19-726394-v2/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1619, \"height\": 1434, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-05-19-726394-v2/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1640, \"height\": 1726, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-05-19-726394-v2/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1269, \"height\": 1954, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-05-19-726394-v2/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1267, \"height\": 1925, \"label\": \"Figure\"}]"
motivation: 神经活动跨多时间尺度组织，但最优信息表示尺度的理论机制不明，尤其缺乏解释中尺度最优性的理论。
method: 建立多尺度模型，将神经群体活动表示为不同时间分辨率的试次向量，并引入信号与噪声自相关参数化，通过解析计算敏感度指数评估可解码性。
result: 信号与噪声自相关都衰减时，时间积分在抑制噪声与保持信号间产生权衡，导致中尺度表示最优；否则最优处于极端尺度。
conclusion: 该理论框架将时间积分作为连接多尺度动力学与信息表示的机制，解释了最优时间尺度的出现条件及预处理的影响。
---

## 摘要
引言：尽管神经活动在多个时间和空间尺度上组织，但决定跨尺度信息表示的原理仍不清楚。特别是，虽然最近的实证结果报道了神经解码中的介观尺度最优性，但尚无理论解释能够说明这种中间尺度何时以及为何成为最优。本文开发了一个分析框架，用于确定神经信息表示的最优时间尺度及其对信号和噪声动态的依赖性。材料与方法：我们制定了一个多尺度模型，其中神经群体活动由微尺度、粗介观尺度、细介观尺度和宏观尺度分辨率下的时间编码试验向量表示。神经响应被建模为受时间相关噪声破坏的刺激依赖性平均激活，信号和噪声自相关衰减率作为参数变化。表示质量使用敏感性指数（d-prime）量化，衡量最优解码器区分刺激条件的能力。结果：我们推导了每个时间尺度下敏感性指数的封闭形式表达式，并确定了信号和噪声自相关作为可解码性的关键决定因素。然后，我们针对合成神经数据的经验可解码性估计验证了我们的理论预测。在时间上比较这些表达式在各种信号和噪声自相关组合下的结果，揭示了两个主要机制。首先，当信号和噪声相关性不存在或随时间持续时，最优分辨率落在两个极端之一：如果信号自相关显著强于（或弱于）噪声自相关，则为宏观尺度（或微尺度）。当信号和噪声自相关都衰减时，时间积分产生了一种权衡：适度积分通过抑制噪声同时保留相干信号来提高可解码性，而过度积分则降低了信号和可解码性。因此，仅在后者机制下，介观尺度表示在广泛的生物学合理参数范围内成为最优机制。讨论：这项工作提供了关于最优时间尺度如何依赖于信号和噪声自相关相互作用的理论解释。该框架将时间积分确立为连接多尺度神经动态与信息表示的原理性机制，解释了何时预处理操作（如分箱和平滑）增强或降低可解码性，并提供了跨记录模态和神经系统的可检验预测。

## Abstract
IntroductionAlthough neural activity is organized across multiple temporal and spatial scales, the principles determining information representation across scales remain unclear. In particular, while recent empirical results have reported mesoscale optimality in neural decoding, no theoretical accounts exist that can explain when and why such intermediate scales emerge as optimal. Here, we develop an analytical framework to determine optimal temporal scales of neural information representation and their dependence on signal and noise dynamics.

Materials and MethodsWe formulate a multiscale model where neural population activity is represented by temporally encoded trial vectors at micro-, coarse meso-, fine meso- and macroscale resolutions. Neural responses are modeled as stimulus-dependent mean activations corrupted by temporally correlated noise, with signal and noise autocorrelation decay rates varied parametrically. Representational quality is quantified using the sensitivity index (d-prime), measuring the ability of an optimal decoder to distinguish stimulus conditions.

ResultsWe derive closed-form expressions for the sensitivity index at each temporal scale and identify signal and noise autocorrelations as key determinants of decodability. We then validate our theoretical predictions against empirical decodability estimates from synthetic neural data. Comparing these expressions under various combinations of signal and noise autocorrelations across time reveals two main regimes. First, when signal and noise correlations are absent or persistent over time, the optimal resolution falls at one of the two extremes: macroscale (resp. microscale) if signal autocorrelations are significantly stronger (resp. weaker) than noise autocorrelations. When both signal and noise autocorrelations decay, temporal integration creates a trade-off: moderate integration improves decodability by suppressing noise while preserving coherent signal, whereas excessive integration degrades signal and decodability. Therefore, only in the latter regime, mesoscale representations emerge as the optimal regime across a broad range of biologically plausible parameters.

DiscussionThis work provides a theoretical explanation for how optimal temporal scales depend on the interplay between signal and noise autocorrelations. The framework establishes temporal integration as a principled mechanism linking multiscale neural dynamics to information representation, explains when preprocessing operations such as binning and smoothing enhance or degrade decodability, and provides testable predictions across recording modalities and neural systems.