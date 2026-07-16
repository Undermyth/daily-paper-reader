---
title: Low-latency neuromorphic closed-loop control of hippocampal ripples in vivo
title_zh: 海马体涟漪的低延迟神经形态闭环控制活体研究
authors: "Alves, P., Jurado-Parras, M.-T., Freitas, J., Ventura, J., de la Prida, L. M., Aguiar, P."
date: 2026-07-15
pdf: "https://www.biorxiv.org/content/10.64898/2026.07.09.737518v1.full.pdf"
tags: ["query:comp-neuro"]
score: 7.0
evidence: 利用低延迟事件驱动计算实现海马 ripple 的神经形态闭环控制
tldr: "针对实时闭环神经调控对低延迟、高能效处理的需求，提出基于脉冲神经网络的神经形态框架，用于检测和调控海马尖波涟漪。通过41神经元和530参数的紧凑网络，在SpiNNaker上实现与深度学习相当的性能，能耗低200倍。集成Open Ephys平台达到约50ms延迟，在小鼠实验中实现80%的涟漪内光遗传抑制，有效改变涟漪动力学。该工作为快速脑动态的低延迟闭环控制提供了实用方案。"
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-09-737518-v1/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1654, \"height\": 1106, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-09-737518-v1/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1534, \"height\": 1842, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-09-737518-v1/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1644, \"height\": 1236, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-09-737518-v1/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1653, \"height\": 707, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-09-737518-v1/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1395, \"height\": 1351, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-09-737518-v1/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1646, \"height\": 1000, \"label\": \"Figure\"}]"
motivation: 传统计算架构难以满足闭环神经调控对低延迟、高能效处理高频振荡信号的需求。
method: 训练紧凑脉冲神经网络（41神经元，530参数），部署于SpiNNaker神经形态硬件，集成Open Ephys平台。
result: "检测性能媲美深度学习，能耗低200倍，闭环延迟约50ms，实现80%涟漪内光遗传刺激。"
conclusion: 首次在体内验证神经形态闭环框架对快速脑动态的有效控制，为神经疾病治疗和神经科学研究提供新工具。
---

## 摘要
实时闭环神经调控，其中刺激精确地与持续的脑动力学同步，对于治疗神经系统疾病和探索神经回路功能具有变革性潜力。然而，它需要低延迟、高能效地处理高带宽神经信号，而传统计算架构难以满足这一需求。神经形态计算模拟了生物神经回路的事件驱动和大规模并行操作，提供了一种引人注目的替代方案。然而，其在活体验证的快速、瞬时振荡闭环框架中的集成尚未得到证明。在这里，我们展示了一个完全集成的神经形态框架，用于实时检测和操控海马体涟漪：短暂（30-100毫秒）、高频（100-250赫兹）的振荡，这些振荡对于记忆巩固至关重要，并与神经系统疾病相关。我们使用代理梯度反向传播训练了由41个神经元和530个参数组成的紧凑型脉冲神经网络，在23个记录会话中实现了与深度学习模型相媲美的检测性能，同时在部署到SpiNNaker神经形态硬件上时能耗降低高达200倍。与开源Open Ephys平台的集成实现了约50毫秒的总闭环延迟，使得高达80%的涟漪可实现事件内刺激。通过在清醒、头部固定的小鼠中验证完整的感知-处理-刺激流程，我们证明神经形态触发的光遗传学抑制显著改变了涟漪动力学并降低了振荡能量。这项工作为快速脑动力学的低延迟闭环控制建立了一个实用且易于获取的神经形态框架。

## Abstract
Real-time closed-loop neuromodulation, in which stimulation is precisely timed to ongoing brain dynamics, holds transformative potential for treating neurological disorders and probing neural circuit function. However, it requires low-latency, energy-efficient processing of high-bandwidth neural signals that conventional computing architectures struggle to deliver. Neuromorphic computing, which emulates the event-driven and massively parallel operation of biological neural circuits, offers a compelling alternative. Yet, its integration into closed-loop frameworks validated in vivo for fast, transient oscillations has not been demonstrated. Here, we present a fully integrated neuromorphic framework for real-time detection and manipulation of hippocampal ripples: brief (30-100 ms), high-frequency (100-250 Hz) oscillations that are critical for memory consolidation and implicated in neurological disorders. We train compact spiking neural networks comprising 41 neurons and 530 parameters using surrogate-gradient backpropagation, achieving detection performance competitive with deep learning models across 23 recording sessions while consuming up to 200-fold less energy when deployed on SpiNNaker neuromorphic hardware. Integration with the open-source Open Ephys platform yields total closed-loop latencies of approximately 50 ms, enabling intra-event stimulation in up to 80% of ripples. Validating the complete sensing-processing-stimulation pipeline in awake, head-fixed mice, we demonstrate that neuromorphic-triggered optogenetic inhibition significantly alters ripple dynamics and reduces oscillatory energy. This work establishes a practical and accessible neuromorphic framework for low-latency closed-loop control of fast brain dynamics in vivo.