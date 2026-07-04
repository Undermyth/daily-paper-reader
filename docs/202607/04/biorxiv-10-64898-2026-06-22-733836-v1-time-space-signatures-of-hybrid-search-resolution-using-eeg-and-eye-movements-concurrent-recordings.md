---
title: Time space signatures of hybrid search resolution using EEG and eye movements concurrent recordings
title_zh: 基于脑电图和眼动同步记录的混合搜索解析的时间空间特征
authors: "Care, D., Gonzalez, J. E., Ison, M. J., Kamienkowski, J. E."
date: 2026-06-28
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.22.733836v1.full.pdf"
tags: ["query:comp-neuro"]
score: 6.0
evidence: 混合视觉与记忆搜索的EEG和眼动研究
tldr: 自然场景中的视觉搜索涉及注意与记忆协同，但传统事件相关方法难以分离重叠的神经信号。本研究采用反卷积方法分析联合记录的EEG和眼动数据，在混合搜索任务中成功提取出视觉处理和靶标检测的精细时间响应函数（TRF），并扩展到数据驱动模型探索多维交互。结果表明漏检诱发的P300反应虽弱但类似，揭示了注意力与记忆的动态交互。该方法为生态效度下的认知研究提供了新工具。
source: biorxiv
selection_source: fresh_fetch
motivation: 传统事件相关方法无法分离自然场景中重叠的神经信号，限制了对注意与记忆协同机制的探究。
method: 采用反卷积方法分析联合记录的EEG和眼动数据，构建从假设驱动到数据驱动的层次化模型提取TRF。
result: 成功分离视觉处理和靶标检测的TRF，发现漏检与检测诱发的P300反应类似但较弱，模型性能稳定。
conclusion: 反卷积方法能有效揭示自然自由观看中注意与记忆的动态交互，为生态效度认知研究提供新范式。
---

## 摘要
理解大脑如何在自然环境中支持视觉搜索——其中注意力和记忆必须协同工作以在干扰物中寻找目标——需要分析神经信号，这些信号在时间上响应重叠，且多个环境变量同时相互作用。传统的事件相关方法无法分离这些重叠信号，这成为在生态有效环境中研究认知的基本瓶颈。在此，我们试图在自然场景下的混合视觉和记忆搜索任务中分离激活模式。我们证明，基于反卷积的方法应用于配准的脑电图和眼动追踪数据可解决这一问题，捕获时间响应函数中主效应及其交互作用的精细激活模式。从假设驱动模型出发，我们在无限制眼动的混合搜索任务中复制了视觉处理和目标检测的已有成分。此外，将我们的方法扩展到层次更大的数据驱动模型，使我们能够探索原本被分开研究的效应之间的交互作用。我们表明，随着模型复杂度的增加，时间响应函数估计保持稳定，模型性能（皮尔逊相关系数）提高，并由方差膨胀因子控制。我们识别出与目标检测的P300成分一致的晚期激活，并揭示漏检引发了相似但较弱的响应，这表明其作用比简单检测更为微妙。这些发现证明了反卷积方法辅以支持特征空间扩展的稳健模型性能测量，能够揭示自由观看行为背后注意力和记忆过程的动态交互。

## Abstract
Understanding how the brain supports visual search in naturalistic environments--where attention and memory must work together to find targets among distractors--requires analysing neural signals where responses overlap in time and multiple environmental variables simultaneously interact. Conventional event-related methods cannot disentangle these overlapping signals, creating a fundamental bottleneck for studying cognition in ecologically valid settings. Here, we seek to isolate activation patterns during a hybrid visual and memory search task in naturalistic scenarios. We show that our deconvolution-based approach applied to coregistered EEG and eye-tracking data resolves this problem, capturing fine-grained activation patterns in the temporal response functions (TRFs) for main effects and their interactions. Starting from hypothesis-driven models, we replicated established components for visual processing and target detection in a Hybrid Search task with unrestricted eye movements. Moreover, extending our approach to hierarchically larger data-driven models enabled us to explore interactions between the effects that have otherwise been studied separately. We showed that the TRF estimates remained stable with increasing model complexity, supported by improved model performance (Pearsons correlation coefficient) and controlled by the variance inflation factor (VIF). We identified a late activation consistent with the P300 component for target detection, and revealed that missed detections elicited similar but weaker responses, suggesting a more nuanced role than simple detection. These findings demonstrate how deconvolution methods, complemented with robust measures of model performance that support its expansion in features space, can uncover the dynamic interplay of attention and memory processes underlying free-viewing behavior.