---
title: Estimation of neuronal tuning for word meaning from passively recorded naturalistic speech
title_zh: 从被动记录的自然言语中估计词语意义的神经调谐
authors: "Ismail, T., Chavez, A. G., Yan, X., Zhu, H., Franch, M., Belanger, J., Chamarthi, S., Kabotyanski, K., Katlowitz, K., Chericoni, A., Mickiewicz, E., Merk, T., Zhou, Y., Shivakumar, N., Steffan, P., Hingorani, R., Ogg, M., Yi, H., Fraczek, T., Bartoli, E., Hennig, J. A., Sheth, S. A., Provenza, N., Hayden, B. Y."
date: 2026-06-28
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.23.733980v1.full.pdf"
tags: ["query:comp-neuro"]
score: 7.0
evidence: 神经元语言调谐与编码模型
tldr: 针对神经编码模型受限于输入数据规模和生态效度的问题，提出一种从被动记录的自然语音中估计单词意义神经调谐的pipeline。该pipeline包括转录、分割、视频辅助说话人标注、神经数据对齐和尖峰检测。在21名患者、800小时和5百万词数据集上，通过基准测试验证了编码和解码模型的有效性。结果表明日常自然语音足以用于估计神经级嵌入。
source: biorxiv
selection_source: fresh_fetch
motivation: 现有神经编码模型受限于输入数据的规模和生态效度，需从日常自然语音中推断神经编码。
method: 构建处理自发自然语音的pipeline，包含转录、分割、视频辅助说话人标注、神经数据对齐和尖峰检测。
result: 在21名患者、800小时和5百万词数据集上，编码和解码模型表现出色，验证了自然语音的可用性。
conclusion: 从被动记录的自然语音中可以估计出单词意义的神经调谐，具有科学和临床潜力。
---

## 摘要
构建神经层面语言编码模型的能力具有巨大的科学和临床潜力。当前方法受限于输入数据的规模和生态效度；需要大规模、罕见或自然样本的应用尤其能从从日常言语中推断神经编码的能力中获益。本文提出了一种新颖的处理流程，旨在利用自发和偶然的自然言语。该流程执行转录、分割、视频辅助的说话人识别，以及神经数据的对齐和尖峰检测。我们将此流程应用于来自21名患者的数据集（每人6天以上，总计超过800小时和500万词）。我们针对由人工整理的词级时间对齐和手动分类的尖峰组成的大量且罕见的地面实况控制数据集，对编码和解码模型进行了基准测试。我们进一步通过量化表征漂移、数据集大小的影响以及六个脑区之间的差异来验证我们的方法。这些发现共同表明，偶然的自然言语在大脑中得到了充分处理，从而能够估计神经层面的嵌入。

## Abstract
The ability to derive neural-level language coding models holds great scientific and clinical potential. Current approaches are limited by the scale and ethological validity of input data; applications requiring large, rare, or naturalistic samples in particular would benefit from the ability to infer neural coding from incidental everyday speech. Here we present a novel pipeline designed to leverage spontaneous and incidental naturalistic speech. This pipeline performs transcription, segmentation, and video-assisted diarization, as well as alignment and spike detection of neural data. We apply this pipeline to a dataset derived from 21 patients (6+ days each, over 800 hours and 5 million words total). We benchmark both encoding and decoding models against extensive and rare ground-truth control datasets consisting of human-curated word-level temporal alignment and manually sorted spikes. We further validate our approach by quantifying representational drift, effect of dataset size, and differences between six brain areas. Together, these findings demonstrate that incidental natural speech is sufficiently processed in the brain to enable the estimation neural-level embeddings.