---
title: Bayesian Nonparametric Identification of Frequency-Selective Neural Oscillatory States
title_zh: 频率选择性神经振荡状态的贝叶斯非参数识别
authors: "Yamada, S., Nagel, S. E., Kobeleva, X., Schmidt, R."
date: 2026-06-25
pdf: "https://www.biorxiv.org/content/10.64898/2025.12.20.695571v3.full.pdf"
tags: ["query:comp-neuro"]
score: 6.0
evidence: 贝叶斯非参数识别神经振荡状态
tldr: 神经振荡识别对理解认知过程至关重要，但现有方法需预设频段或状态数，易导致检测偏差。本文提出结合时间延迟嵌入与狄利克雷过程高斯混合模型的贝叶斯非参数方法，自动从数据中推断振荡状态数量。在含1/f噪声的合成数据中，该方法可靠恢复多个频率成分；在真实MEG数据中，识别出多个短暂频率选择性状态及不同频谱的周期状态，揭示了显著的个体差异。该框架无需预定义频段或状态数，实现了对频率选择性振荡状态的无监督发现。
source: biorxiv
selection_source: fresh_fetch
motivation: 现有神经振荡识别方法需预设频段或状态数，结果敏感且易欠/过拟合，亟需自适应的无监督方案。
method: 将时间延迟嵌入（TDE）与狄利克雷过程高斯混合模型（DP-GMM）结合，通过TDE捕捉局部自协方差结构，DP先验自适应调整模型复杂度。
result: 合成数据中可靠恢复多个频率成分；MEG数据发现多个短暂频率选择性振荡状态及不同频谱的周期状态，个体间峰值频率、发生率和功率差异显著。
conclusion: 提出一种无需预定义频段或状态数的无监督框架，能直接从数据中发现频率选择性神经振荡状态。
---

## 摘要
识别神经振荡对于将快速的大脑动态与潜在的认知过程联系起来至关重要。然而，这具有挑战性，因为振荡事件可能是短暂的，嵌入在类似1/f的背景活动中，并且可能包含未知数量的频谱不同状态。传统方法通常将窄带带通滤波器应用于一个或几个预定义的频带，然后使用幅度阈值来识别振荡事件，但检测结果可能对这些选择高度敏感。尽管最近基于隐马尔可夫模型（HMM）的无监督替代方案解决了这些局限性，但它们仍然需要预先指定状态数量，并且当这个数量被错误指定时，可能导致欠拟合或过拟合。我们提出了一种贝叶斯非参数方法，该方法在识别不同振荡状态的同时，直接从数据中推断出适当的状态数量。该方法结合了时延嵌入（TDE）和狄利克雷过程高斯混合模型（DP-GMM）。TDE用时间平移副本增强信号，使DP-GMM能够捕获特定频率的局部自协方差结构，而狄利克雷过程先验通过修剪非活动成分来调整模型复杂度。我们使用设计用于模拟神经时间序列（例如EEG、MEG和局部场电位）的单通道合成数据，其中多个频率成分被类似1/f的噪声掩盖，将该方法与基于滤波器的阈值方法以及时延嵌入HMM进行了基准测试。在这种设置下，所提出的模型在噪声条件下可靠地恢复了多个不同频率成分，同时还推断出了振荡状态的数量。应用于静息态运动皮层MEG数据集时，该模型识别出了多个频率选择性、短暂的振荡状态以及具有不同频谱分布的独特非周期状态。这些状态在峰值频率、发生率和功率方面表现出显著的个体间异质性。总的来说，这提供了一种无监督框架，用于发现频率选择性的振荡状态，无需预定义频带或固定状态数量。

## Abstract
Identifying neural oscillations is essential for linking fast brain dynamics to underlying cognitive processes. However, this is challenging because oscillatory events can be brief, embedded in 1/f-like background activity, and may comprise an unknown number of spectrally distinct states. Conventional approaches often apply narrowband band-pass filters to one or a few predefined frequency bands and then use amplitude thresholding to identify oscillatory events, but detection outcomes can be highly sensitive to these choices. Although recent unsupervised alternatives based on hidden Markov models (HMMs) address these limitations, they still require the number of states to be specified in advance and can underfit or overfit when this number is misspecified. We propose a Bayesian nonparametric method that identifies distinct oscillatory states while inferring an appropriate number of states directly from the data. This method combines time-delay embedding (TDE) with the Dirichlet-process Gaussian mixture model (DP-GMM). TDE augments the signal with time-shifted copies, enabling the DP-GMM to capture frequency-specific local autocovariance structures, while the Dirichlet-process prior adapts model complexity by pruning inactive components. We benchmarked the approach against a filter-based thresholding method and the time-delay embedded HMM using single-channel synthetic data designed to mimic neural time series (e.g., EEG, MEG, and local field potentials), with multiple frequency components masked by 1/f-like noise. In this setting, the proposed model reliably recovered multiple distinct frequency components under noisy conditions while also inferring the number of oscillatory states. Applied to a resting-state motor-cortex MEG dataset, the model identified multiple frequency-selective, short-lived oscillatory states alongside distinct aperiodic states with different spectral profiles. These states exhibited substantial inter-individual heterogeneity in peak frequency, occurrence rate, and power. Overall, this provides an unsupervised framework for discovering frequency-selective oscillatory states without predefining frequency bands or fixing the number of states.