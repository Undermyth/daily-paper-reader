---
title: Cortical encoding of probabilistic temporal predictions during speech perception
title_zh: 言语感知中概率性时间预测的皮层编码
authors: "Deyna, L., Albouy, P., Trebuchon, A., Schon, D., Morillon, B., Guilleminot, P. H."
date: 2026-08-20
pdf: "https://www.biorxiv.org/content/10.64898/2026.08.16.745095v1.full.pdf"
tags: ["query:comp-neuro"]
score: 7.0
evidence: 关于皮层预测编码与循环网络模型的计算神经科学研究
tldr: 语音时间结构传统上仅以语言单位的平均速率描述，忽略了上下文依赖的概率性时序。为探究时序预测，本研究利用法/英语料训练均值、风险率与RNN模型预测音素/音节/词起始，并在53名患者的7698个颅内电极自然语音记录中检验。结果RNN优于简单模型，其“何时”概率显著解释超出声学-语言内容（“什么”）的神经活动，且编码通道群体不同，涉及双侧颞叶到左额叶及感觉运动区。这证明语音时序预测是动态概率过程，独立于内容编码。
source: biorxiv
selection_source: fresh_fetch
motivation: 传统语音时间结构仅用平均速率刻画，忽略上下文相关的概率性时序，难以支持预测编码。
method: 基于大规模语料训练均值、风险率和RNN预测语音单位起始，并用颅内电极记录比较模型解释力。
result: RNN预测最优，其“何时”概率在内容特征外显著解释神经活动，且与内容编码分离，涉及广泛感觉运动网络。
conclusion: 语音时间预测是动态、上下文依赖的概率过程，是独立于语言内容编码的神经机制。
---

## 摘要
言语的时间结构传统上以其典型语言单位（音素、音节、词）的节奏性为特征，每个单位都以平均发生频率来概括。虽然这一观点有效，但它忽略了言语是否具有更精细的、依赖于情境的且概率性的时间结构，这种结构可能在聆听过程中支持时间预测编码。利用大型法语和英语语料库，我们训练了复杂度递增的模型来预测语言单位的起始点。循环神经网络（RNNs）优于平均频率模型和危险率模型，表明这些频率周围的变异性并非噪声，而是一种由局部情境塑造的时间结构，在音素、音节和词之间具有统计可预测性。随后，我们记录了53名神经外科患者听自然言语时的7,698个脑内电极信号，显示模型的输出——即将到来的起始点的连续概率（何时），能够解释超越声学和语言内容（什么）特征的神经活动，且RNNs的效应明显强于平均频率或危险率模型。这种关于起始点何时发生的动态神经预测与语言内容的编码是可分离的，依赖于大体不同的通道群体。时间预测涉及一个分布广泛的皮层网络，从双侧颞叶皮层延伸至左侧额叶和感觉运动区域。总之，这些结果确立了言语中的时间预测本身就是一个动态的、依赖于情境的且概率性的过程。

## Abstract
The temporal structure of speech has traditionally been characterized by the rhythmicity of its canonical linguistic units (phonemes, syllables, words), each summarized by a mean occurrence rate. While valid, this view overlooks whether speech carries a finer, context-dependent and probabilistic temporal structure that could support temporal predictive coding during listening. Using large French and English speech corpora, we trained models of increasing complexity to predict the onsets of linguistic units. Recurrent neural networks (RNNs) outperform mean-rate and hazard-rate models, showing that the variability around these rates is not noise but a temporal structure shaped by local context, statistically predictable across phonemes, syllables and words. Recording from 7,698 intracerebral electrodes in 53 neurosurgical patients listening to natural speech, we next show that the models' output), the continuous probability of an upcoming onset (when), explains neural activity beyond acoustic and linguistic content (what) features, with markedly stronger effects for RNNs than for mean- or hazard-rate models. This dynamic neural prediction of when an onset will occur is dissociable from the encoding of linguistic content, relying on largely distinct channel populations. Temporal predictions engage a distributed cortical network extending from bilateral temporal cortex into left frontal and sensorimotor regions. Together, these results establish temporal prediction in speech as a dynamic, context-dependent and probabilistic process in its own right.