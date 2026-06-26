---
title: Next-Generation Neural Mass Models Reproduce Features of Speech Processing
title_zh: 下一代神经群体模型再现语音处理特征
authors: "Shannon, A. J., Barton, D. A. W., Homer, M., Houghton, C. J."
date: 2026-06-22
pdf: "https://www.biorxiv.org/content/10.1101/2025.10.20.683434v2.full.pdf"
tags: ["query:comp-neuro"]
score: 6.0
evidence: 语音处理的神经群模型
tldr: 语音处理中音节分割依赖神经活动与韵律结构对齐，但皮层机制不明。本文采用下一代神经群体模型，对比相位重置与诱发响应假设，通过四项测试验证。模型通过阈值相位重置响应语音包络锐利起始，产生跨频率嵌套振荡，复现实验双峰特征。该工作为从皮层振荡到语音跟踪计算提供了生物物理桥梁。
source: biorxiv
selection_source: fresh_fetch
motivation: 探索神经语音跟踪背后皮层电路的具体机制，弥补现象学模型在生物物理细节上的缺失。
method: 采用下一代神经群体模型，以现象学模型为基线，设计四项测试验证其复现语音跟踪特征的能力。
result: 模型再现锐度调谐的语音跟踪，机制为阈值相位重置与跨频率嵌套振荡，匹配实验双峰特征。
conclusion: 神经群体模型桥接了皮层振荡动态与语音跟踪的认知计算，提供了生物物理层面的解释。
---

## 摘要
将语音分解为音节是神经语音处理的关键步骤，它依赖于神经活动与语音节律结构的对齐。两种竞争性假说——相位重置和诱发反应——解释这种神经语音跟踪。虽然这些假说的现象学建模已取得成功，但我们仍缺乏对底层皮层回路的理解。为了探究这些机制，我们评估了一个生物物理的下一代神经群体模型能否再现神经语音跟踪的若干特征，并以竞争假说的现象学模型作为算法基线。我们通过四项测试研究模型动力学：在计算机中重现一项识别出跟踪强度与音素锐度之间相关性的EEG实验；计算相位集中度量；测试不同音节速率的影响；以及评估跨音素起始的事件间相位一致性。在我们研究的所有模型中，虽然都能再现锐度调谐的节律语音跟踪，但诱发反应模型需要预先处理的声学边缘脉冲刺激。我们证明，神经群体模型执行的是由连续语音包络中尖锐起始触发的阈值化相位重置，这会产生跨频率嵌套振荡，在事件间相位一致性中定性地匹配实验观察到的双峰特征。我们的结果表明，生物物理的神经群体模型在皮层群体的通用振荡动力学与语音跟踪的认知计算之间提供了机制性桥梁。实际上，神经群体模型的非线性动力学解释了听觉皮层活动中的峰值速率事件表征如何响应连续声学输入而产生。

意义声明：音节分解至关重要但充满挑战，因为自然语音缺乏清晰边界，而人类却能毫不费力地完成这一计算。语音使神经活动与音节节律对齐，预测音节定时，但潜在的皮层机制尚不清楚。将这种宏观行为与神经生物学联系起来是困难的；然而，下一代神经群体模型有望解决这一问题。我们证明这些模型能够再现锐度调谐的跟踪和声学边缘提取。动力学分析表明，这是通过阈值化相位重置到音素起始，触发跨频率嵌套振荡而实现的。我们的结果既推进了对音节分解的生物学理解，也验证了该模型模拟宏观神经活动的能力。这些模型为听觉皮层神经生物学与语音处理动力学之间架起了一座桥梁，这是现象学模型无法提供的。

## Abstract
Segregation of speech into syllables is a key step in neural speech processing. It relies on the alignment of neural activity with the rhythmic structure of speech. Two competing hypotheses explain this  neural speech tracking, phase-resetting and evoked responses. While phenomenological modelling of these hypotheses has been successful, we still lack understanding of the underlying cortical circuits. To investigate these mechanisms, we evaluate whether a biophysical next-generation neural mass model can reproduce several features of neural speech tracking, using phenomenological models of the competing hypotheses as algorithmic baselines. We investigate the models dynamics with four tests: recreating in-silico an EEG experiment that identified a correlation between tracking strength and phoneme sharpness, computing the Phase Concentration Metric, testing the effect of varying syllabic rates, and evaluating the Inter Event Phase Coherence across phoneme onsets. While all of the models that we study reproduce the sharpness-tuned rhythmic speech tracking, the evoked model requires a pre-processed acoustic edge impulse stimulus. We demonstrate that the neural mass model is performing thresholded phase-resetting triggered by sharp onsets in the continuous speech envelope. This produces cross-frequency nested oscillations that qualitatively match an experimentally-observed dual-peak signature in the Inter Event Phase Coherence. Our results indicate that the biophysical neural mass model provides a mechanistic bridge between generic oscillatory dynamics in cortical populations and the cognitive computations of speech tracking. Indeed, the non-linear dynamics of the neural mass model offer an explanation for how peak-rate event representations in auditory cortex activity arise in response to continuous acoustic input.

Significance StatementSyllable segregation is crucial but challenging as natural speech lacks clear boundaries, yet humans perform this computation effortlessly. Speech aligns neural activity to syllabic rhythms, predicting syllable timing, but the underlying cortical mechanisms remain unknown. Relating this macroscopic behaviour to neurobiology is challenging; however, next-generation neural mass models promise to resolve this. We demonstrate that these models reproduce sharpness-tuned tracking and acoustic edge extraction. Dynamical analyses indicate this occurs through thresholded phase-resetting to phoneme onsets, triggering cross-frequency nested oscillations. Our results both advance biophysical understanding of syllable segregation and validate the models capacity for simulating macroscopic neural activity. These models offer a bridge between the neurobiology of the auditory cortex and speech processing dynamics that phenomenological models cannot provide.