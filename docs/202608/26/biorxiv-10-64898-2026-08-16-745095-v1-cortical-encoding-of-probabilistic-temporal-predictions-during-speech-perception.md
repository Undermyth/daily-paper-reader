---
title: Cortical encoding of probabilistic temporal predictions during speech perception
title_zh: 言语感知中概率时间预测的皮层编码
authors: "Deyna, L., Albouy, P., Trebuchon, A., Schon, D., Morillon, B., Guilleminot, P. H."
date: 2026-08-20
pdf: "https://www.biorxiv.org/content/10.64898/2026.08.16.745095v1.full.pdf"
tags: ["query:comp-neuro"]
score: 7.0
evidence: 语音感知中概率性时间预测的计算编码
tldr: 语音时间结构通常被简化为语言单元的平均发生率，但可能隐含上下文相关的概率预测。本文用递归神经网络（RNN）在大规模双语语料上学习预测音素/音节/词的起始时间，并以53名患者颅内记录验证。RNN显著优于平均率/危险率模型，其预测概率额外解释神经活动，且与内容编码分离，涉及颞叶至额叶网络。表明语音的时间预测是动态、上下文依赖的独立过程。
source: biorxiv
selection_source: fresh_fetch
motivation: 传统语音时间结构仅用平均发生率刻画，忽略了上下文依赖的概率性时间预测在听觉编码中的作用。
method: 在大型法语和英语语料上训练RNN预测语言单元起始，并用颅内电极记录53名患者听自然语音时的神经活动。
result: RNN预测优于平均率和危险率模型，其时间预测概率在声学和内容之外显著解释神经活动，并与内容编码分离，扩展至额叶/感觉运动网络。
conclusion: 语音中的时间预测是一个动态、上下文依赖的概率过程，可独立于语言内容进行神经编码。
---

## 摘要
言语的时间结构传统上以其典型语言单位（音素、音节、词）的节奏性为特征，每个单位都被概括为平均发生率。虽然这一观点有效，但它忽略了言语是否携带一种更精细的、依赖于上下文且具有概率性的时间结构，这种结构可能支持听觉过程中的时间预测编码。利用大型法语和英语语料库，我们训练了复杂度递增的模型来预测语言单位的起始时间。循环神经网络（RNN）优于平均率和危险率模型，表明这些率周围的变异性并非噪声，而是一种由局部上下文塑造的时间结构，在音素、音节和词之间具有统计可预测性。接下来，我们记录了53名神经外科患者聆听自然言语时的7,698个脑内电极信号，显示模型的输出——即将到来的起始事件的连续概率（何时）——能够解释超越声学和语言内容（什么）特征的神经活动，且RNN的效应显著强于平均率或危险率模型。这种关于起始事件何时发生的动态神经预测可与语言内容的编码分离，依赖于大致不同的通道群体。时间预测涉及一个分布式的皮层网络，从双侧颞叶皮层延伸至左额叶和感觉运动区域。总之，这些结果确立了言语中的时间预测本身就是一个动态的、依赖于上下文的概率过程。

## Abstract
The temporal structure of speech has traditionally been characterized by the rhythmicity of its canonical linguistic units (phonemes, syllables, words), each summarized by a mean occurrence rate. While valid, this view overlooks whether speech carries a finer, context-dependent and probabilistic temporal structure that could support temporal predictive coding during listening. Using large French and English speech corpora, we trained models of increasing complexity to predict the onsets of linguistic units. Recurrent neural networks (RNNs) outperform mean-rate and hazard-rate models, showing that the variability around these rates is not noise but a temporal structure shaped by local context, statistically predictable across phonemes, syllables and words. Recording from 7,698 intracerebral electrodes in 53 neurosurgical patients listening to natural speech, we next show that the models' output), the continuous probability of an upcoming onset (when), explains neural activity beyond acoustic and linguistic content (what) features, with markedly stronger effects for RNNs than for mean- or hazard-rate models. This dynamic neural prediction of when an onset will occur is dissociable from the encoding of linguistic content, relying on largely distinct channel populations. Temporal predictions engage a distributed cortical network extending from bilateral temporal cortex into left frontal and sensorimotor regions. Together, these results establish temporal prediction in speech as a dynamic, context-dependent and probabilistic process in its own right.