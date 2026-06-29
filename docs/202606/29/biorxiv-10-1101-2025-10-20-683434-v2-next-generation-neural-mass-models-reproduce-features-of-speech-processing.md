---
title: Next-Generation Neural Mass Models Reproduce Features of Speech Processing
title_zh: 下一代神经群体模型重现语音处理特征
authors: "Shannon, A. J., Barton, D. A. W., Homer, M., Houghton, C. J."
date: 2026-06-22
pdf: "https://www.biorxiv.org/content/10.1101/2025.10.20.683434v2.full.pdf"
tags: ["query:comp-neuro"]
score: 6.0
evidence: 使用神经质量模型计算建模神经语音处理
tldr: 语音分割依赖神经活动与音节节奏对齐，但底层皮层机制尚不清楚。本研究使用生物物理的下一代神经群体模型，模拟语音跟踪过程，并与现象学模型对比。模型通过阈值化相位重置机制，对连续语音包络中的清晰起始进行响应，成功再现了清晰度调谐的节奏跟踪和交叉频率嵌套振荡。这一结果架起了皮层群体振荡动态与语音跟踪认知计算之间的机制桥梁，深化了对音节分割生物物理基础的理解。
source: biorxiv
selection_source: fresh_fetch
motivation: 缺乏对神经语音跟踪底层皮层电路机制的理解。
method: 采用下一代神经群体模型，结合相位重置和诱发反应等假设进行模拟与分析。
result: 模型通过阈值化相位重置重现清晰度调谐跟踪，并产生交叉频率嵌套振荡，匹配实验双峰特征。
conclusion: 模型提供了皮层振荡与语音跟踪认知之间的机制桥梁，推进了生物物理理解。
---

## 摘要
将语音分割成音节是神经语音处理的关键步骤，它依赖于神经活动与语音节奏结构的对齐。两种相互竞争的假说解释了这种神经语音跟踪：相位重置和诱发电位。虽然这些假说的现象学建模已取得成功，但我们仍缺乏对底层皮层环路机制的理解。为探究这些机制，我们评估了生物物理的下一代神经群体模型能否重现神经语音跟踪的多个特征，并以竞争假说的现象学模型作为算法基线。我们通过四项测试研究模型动态：在计算机中重现一项识别跟踪强度与音素锐度之间相关性的EEG实验；计算相位集中度指标；检验不同音节速率的影响；以及评估音素起始处的事件间相位一致性。尽管我们研究的所有模型都重现了锐度调制的节奏性语音跟踪，但诱发电位模型需要预处理的声学边缘脉冲刺激。我们证明神经群体模型执行的是由连续语音包络中的锐利起始触发的阈值化相位重置，这产生了交叉频率嵌套振荡，并在定性上匹配实验观察到的事件间相位一致性的双峰特征。我们的结果表明，生物物理神经群体模型为皮层群体的一般振荡动力学与语音跟踪的认知计算之间提供了机制桥梁。事实上，神经群体模型的非线性动力学解释了听觉皮层活动中的峰值率事件表征是如何响应连续声学输入而产生的。

意义声明：音节分割至关重要但具有挑战性，因为自然语音缺乏清晰边界，而人类却能毫不费力地完成这一计算。语音将神经活动与音节节奏对齐以预测音节时序，但背后的皮层机制尚不清楚。将这种宏观行为与神经生物学相联系是困难的；然而，下一代神经群体模型有望解决这一问题。我们证明这些模型能够重现锐度调制的跟踪和声学边缘提取。动力学分析表明，这是通过对音素起始进行阈值化相位重置，触发交叉频率嵌套振荡而实现的。我们的结果既推进了对音节分割的神经生物学理解，也验证了该模型模拟宏观神经活动的能力。这些模型提供了听觉皮层神经生物学与语音处理动态之间的桥梁，而这是现象学模型无法提供的。

## Abstract
Segregation of speech into syllables is a key step in neural speech processing. It relies on the alignment of neural activity with the rhythmic structure of speech. Two competing hypotheses explain this  neural speech tracking, phase-resetting and evoked responses. While phenomenological modelling of these hypotheses has been successful, we still lack understanding of the underlying cortical circuits. To investigate these mechanisms, we evaluate whether a biophysical next-generation neural mass model can reproduce several features of neural speech tracking, using phenomenological models of the competing hypotheses as algorithmic baselines. We investigate the models dynamics with four tests: recreating in-silico an EEG experiment that identified a correlation between tracking strength and phoneme sharpness, computing the Phase Concentration Metric, testing the effect of varying syllabic rates, and evaluating the Inter Event Phase Coherence across phoneme onsets. While all of the models that we study reproduce the sharpness-tuned rhythmic speech tracking, the evoked model requires a pre-processed acoustic edge impulse stimulus. We demonstrate that the neural mass model is performing thresholded phase-resetting triggered by sharp onsets in the continuous speech envelope. This produces cross-frequency nested oscillations that qualitatively match an experimentally-observed dual-peak signature in the Inter Event Phase Coherence. Our results indicate that the biophysical neural mass model provides a mechanistic bridge between generic oscillatory dynamics in cortical populations and the cognitive computations of speech tracking. Indeed, the non-linear dynamics of the neural mass model offer an explanation for how peak-rate event representations in auditory cortex activity arise in response to continuous acoustic input.

Significance StatementSyllable segregation is crucial but challenging as natural speech lacks clear boundaries, yet humans perform this computation effortlessly. Speech aligns neural activity to syllabic rhythms, predicting syllable timing, but the underlying cortical mechanisms remain unknown. Relating this macroscopic behaviour to neurobiology is challenging; however, next-generation neural mass models promise to resolve this. We demonstrate that these models reproduce sharpness-tuned tracking and acoustic edge extraction. Dynamical analyses indicate this occurs through thresholded phase-resetting to phoneme onsets, triggering cross-frequency nested oscillations. Our results both advance biophysical understanding of syllable segregation and validate the models capacity for simulating macroscopic neural activity. These models offer a bridge between the neurobiology of the auditory cortex and speech processing dynamics that phenomenological models cannot provide.