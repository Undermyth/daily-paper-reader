---
title: Time space signatures of hybrid search resolution using EEG and eye movements concurrent recordings
title_zh: 混合搜索分辨率的时空特征：基于脑电图和眼动同步记录
authors: "Care, D., Gonzalez, J. E., Ison, M. J., Kamienkowski, J. E."
date: 2026-06-28
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.22.733836v1.full.pdf"
tags: ["query:comp-neuro"]
score: 6.0
evidence: 使用EEG和眼动追踪研究混合视觉和记忆搜索
tldr: 传统事件相关方法难以解析自然场景中时间重叠的神经信号。本研究采用去卷积时间响应函数分析联合记录的EEG和眼动数据，成功分离出视觉处理和靶检测成分（如P300），并发现漏检引发类似但更弱的反应。该方法在增加模型复杂度时保持估计稳定，揭示了注意与记忆的动态交互，为生态效度下的认知研究提供了新途径。
source: biorxiv
selection_source: fresh_fetch
motivation: 传统事件相关方法无法分离自然视觉搜索中时间重叠的神经信号，阻碍了对注意与记忆协同机制的生态效度研究。
method: 采用去卷积方法对联合记录的EEG和眼动数据进行时间响应函数（TRF）分析，包括假设驱动和数据驱动模型，并用方差膨胀因子控制模型复杂度。
result: 成功复制了P300等靶检测成分，发现漏检引发类似但更弱的反应；TRF估计随模型复杂度增加保持稳定，模型性能（皮尔逊相关系数）提升。
conclusion: 去卷积TRF方法能稳健分离自由观看中重叠的神经信号，揭示注意与记忆的动态交互，为高生态效度认知研究提供了有效工具。
---

## 摘要
理解大脑如何在自然环境中支持视觉搜索——其中注意力和记忆必须协同工作以在干扰物中找到目标——需要分析神经信号，这些信号在时间上存在重叠响应，且多个环境变量同时相互作用。传统的事件相关方法无法分离这些重叠信号，这成为在生态有效情境下研究认知的根本瓶颈。本文旨在隔离自然场景中混合视觉和记忆搜索任务期间的激活模式。我们证明，基于反卷积的方法应用于共配准的脑电图和眼动追踪数据可以解决这一问题，捕获主效应及其交互作用的时间响应函数中的精细激活模式。从假设驱动模型出发，我们在无限制眼动的混合搜索任务中复制了视觉处理和目标检测的已知成分。此外，将我们的方法扩展到分层更大的数据驱动模型，使我们能够探索之前分别研究的效应之间的相互作用。我们表明，随着模型复杂性的增加，时间响应函数估计保持稳定，这得益于模型性能的提高（皮尔逊相关系数）和方差膨胀因子的控制。我们识别出与目标检测的P300成分一致的晚期激活，并揭示漏检引发了类似但较弱的响应，表明其作用比简单检测更微妙。这些发现展示了反卷积方法，辅以支持其在特征空间扩展的稳健模型性能度量，如何揭示自由观看行为背后注意和记忆过程的动态交互。

## Abstract
Understanding how the brain supports visual search in naturalistic environments--where attention and memory must work together to find targets among distractors--requires analysing neural signals where responses overlap in time and multiple environmental variables simultaneously interact. Conventional event-related methods cannot disentangle these overlapping signals, creating a fundamental bottleneck for studying cognition in ecologically valid settings. Here, we seek to isolate activation patterns during a hybrid visual and memory search task in naturalistic scenarios. We show that our deconvolution-based approach applied to coregistered EEG and eye-tracking data resolves this problem, capturing fine-grained activation patterns in the temporal response functions (TRFs) for main effects and their interactions. Starting from hypothesis-driven models, we replicated established components for visual processing and target detection in a Hybrid Search task with unrestricted eye movements. Moreover, extending our approach to hierarchically larger data-driven models enabled us to explore interactions between the effects that have otherwise been studied separately. We showed that the TRF estimates remained stable with increasing model complexity, supported by improved model performance (Pearsons correlation coefficient) and controlled by the variance inflation factor (VIF). We identified a late activation consistent with the P300 component for target detection, and revealed that missed detections elicited similar but weaker responses, suggesting a more nuanced role than simple detection. These findings demonstrate how deconvolution methods, complemented with robust measures of model performance that support its expansion in features space, can uncover the dynamic interplay of attention and memory processes underlying free-viewing behavior.