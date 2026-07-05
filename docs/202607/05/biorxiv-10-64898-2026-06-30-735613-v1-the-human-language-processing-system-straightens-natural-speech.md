---
title: The human language processing system straightens natural speech
title_zh: 人类语言处理系统使自然语音变得平直
authors: "Xu, J., Nguyen, T. D., Tang, J., Huth, A. G., Goris, R. L. T."
date: 2026-07-02
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.30.735613v1.full.pdf"
tags: ["query:comp-neuro"]
score: 7.0
evidence: 语音表征拉直的计算神经科学研究
tldr: 大型语言模型通过预测学习语言，但大脑如何利用预测进行语音处理尚不清楚。本研究假设预测驱动神经表示轨迹沿层级变直，开发了基于fMRI测量曲率的方法，并借助语音模型wavLM验证。结果显示，从初级听皮层到高级区域，轨迹曲率递减，且仅在自然语言统计结构下出现层级变直。这建立了时间预测目标、表示几何与皮层时间尺度层次之间的直接联系。
source: biorxiv
selection_source: fresh_fetch
motivation: 时间预测对语言处理至关重要，但其如何影响大脑中语音表示的结构仍未知。
method: 利用fMRI测量神经群体轨迹曲率，结合单细胞时间尺度与曲率的联系，并对比wavLM模型反应。
result: 轨迹曲率沿听觉-皮层层次递减，层次变直效应仅对自然语言刺激显著。
conclusion: 时间预测驱动语音表示沿皮层层次变直，连接了预测目标、表示几何与皮层时间尺度。
---

## 摘要
基于下一个词预测训练的大型语言模型具有令人印象深刻的语言能力。这表明时间预测的目标对语言处理至关重要，但这一目标如何影响人脑中语音表征的结构仍不清楚。在此，我们检验了一个假设，即预测通过沿语音处理层次结构的表征轨迹的时间平直化得到促进。我们开发了一种使用功能磁共振成像测量这些轨迹曲率的方法。我们的方法利用了单神经元响应时间尺度与群体轨迹曲率之间先前未知的联系。我们检查了聆听自然语音的受试者的大脑响应。响应轨迹在低级听觉区域曲率最大，并沿着皮层层次结构逐渐平直化。我们将相同的语音刺激及其扰动版本呈现给wavLM——一个与人脑响应高度对齐的语音表征模型——发现对于统计结构类似于自然语音的刺激，层次平直化效应最为强烈。总之，我们的结果建立了时间预测目标、神经语音表征几何以及表征时间尺度的皮层层次结构之间的直接联系。

## Abstract
Large language models trained on next-word prediction have impressive linguistic capabilities. This suggests that the goal of temporal prediction is essential to language processing, but how this goal impacts the structure of speech representations in the human brain remains unknown. Here, we test the hypothesis that prediction is facilitated by the temporal straightening of representational trajectories along the speech processing hierarchy. We developed a methodology for measuring the curvature of these trajectories using fMRI. Our method exploits a previously unknown connection between the timescale of single-unit responses and the curvature of population trajectories. We examined brain responses of subjects listening to natural speech. Response trajectories were most curved in lower-level auditory areas and progressively straightened along the cortical hierarchy. We presented the same speech stimuli and perturbed versions thereof to wavLM--a speech representation model that is well aligned with human brain responses--and found that hierarchical straightening effects are strongest for stimuli whose statistical structure resembles natural speech. Together, our results establish a direct connection between the goal of temporal prediction, the geometry of neural speech representations, and the cortical hierarchy of representational timescales.