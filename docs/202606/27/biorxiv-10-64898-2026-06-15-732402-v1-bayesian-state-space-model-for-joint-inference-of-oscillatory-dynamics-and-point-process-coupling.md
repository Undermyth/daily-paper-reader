---
title: BAYESIAN STATE-SPACE MODEL FOR JOINT INFERENCE OF OSCILLATORY DYNAMICS AND POINT-PROCESS COUPLING
title_zh: 贝叶斯状态空间模型：振荡动态与点过程耦合的联合推断
authors: "Zheng, B., Brincat, S., Donoghue, J., Miller, E., Brown, E."
date: 2026-06-19
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.15.732402v1.full.pdf"
tags: ["query:comp-neuro"]
score: 6.0
evidence: 用于神经振荡与尖峰-场耦合联合推断的贝叶斯状态空间模型
tldr: 传统尖峰-场耦合度量（如SFC和PLV）独立估计频谱，忽略了尖峰时序信息。本文提出Joint SSMT，一种贝叶斯状态空间模型，联合推断LFP振荡谱和点过程耦合，将窄带LFP建模为连续时间潜过程，通过伯努利-逻辑斯蒂模型将尖峰序列与复频谱状态关联。模拟和真实数据表明，该方法能准确恢复耦合强度，利用尖峰时间解析精细时间结构，在麻醉和认知任务中识别频率特异性耦合，优于经典方法并提供不确定量化。
source: biorxiv
selection_source: fresh_fetch
motivation: 现有度量独立估计LFP频谱与尖峰耦合，无法充分利用尖峰时间信息进行联合推断。
method: 构建贝叶斯状态空间模型，将窄带LFP视为连续时间潜变量，通过伯努利-逻辑斯蒂函数将尖峰序列与复频谱状态耦合。
result: 在模拟和麻醉数据中精确恢复耦合强度，在联想学习任务中揭示海马和前额叶皮层的频率特异性耦合。
conclusion: 相比经典SFC和PLV，Joint SSMT提供更频率特异的耦合估计和原则性的不确定量化。
---

## 摘要
在多种行为和生理条件下，尖峰时间与局部场电位振荡在特定频段内表现出相位耦合。经典的测量方法如尖峰-场相干性（SFC）和相位锁定值（PLV）虽能量化这种耦合，但独立于尖峰时间估计LFP频谱。我们引入了Joint SSMT，一种贝叶斯状态空间框架，可联合推断LFP频谱图和尖峰-场耦合强度。该模型将窄带LFP活动视为在连续时间中演化的潜在过程，并通过伯努利-逻辑斯蒂模型将尖峰序列与复频谱状态相关联。在模拟中，Joint SSMT能准确恢复耦合强度、去噪频谱图，并利用尖峰时间解析LFP中的精细时间结构。应用于丙泊酚麻醉数据时，该模型在SFC和PLV仅报告宽泛低频耦合的特定慢振荡频率下识别出耦合。我们将Joint SSMT扩展到试验结构实验，并在联想学习任务中的灵长类记录中应用，揭示了海马体和前额叶皮层的频率特异性耦合。我们还推导了SFC和PLV作为生成模型参数函数的闭式表达式。在模拟和两个灵长类数据集中，Joint SSMT比经典PLV和SFC提供了更具频率特异性的耦合估计，并具有合理的量化不确定性。

## Abstract
Under a range of behavioral and physiological conditions, spike times and local field potential (LFP) oscillations exhibit phase coupling within specific frequency bands. Classical measures such as spike-field coherence (SFC) and the phase-locking value (PLV) quantify this coupling but estimate the LFP spectrum independently of spike timing. We introduce Joint SSMT, a Bayesian state-space framework that jointly infers LFP spectrograms and spike-field coupling strength. The model treats narrowband LFP activity as a latent process evolving in continuous time, with spike trains linked to the complex spectral state through a Bernoulli-logistic model. In simulations, Joint SSMT accurately recovers coupling strength, denoises the spectrogram, and uses spike timing to resolve fine temporal structure in the LFP. Applied to propofol anesthesia data, the model identifies coupling at a specific slow-oscillation frequency where SFC and PLV report only broad low-frequency coupling. We extend Joint SSMT to trial-structured experiments and apply it to primate recordings during an associative learning task, revealing frequency-specific coupling in hippocampus and prefrontal cortex. We also derive closed-form expressions for SFC and PLV as functions of the generative model parameters. Across simulations and two primate datasets, Joint SSMT provides more frequency-specific coupling estimates with principled uncertainty quantification than classical PLV and SFC.