---
title: Neuromodulation enhances the capability and efficiency of spiking neural networks
title_zh: 神经调控增强脉冲神经网络的能力与效率
authors: "AlKilany, A., Goodman, D. F. M."
date: 2026-07-13
pdf: "https://www.biorxiv.org/content/10.1101/2025.07.25.666748v2.full.pdf"
tags: ["query:comp-neuro"]
score: 6.0
evidence: 神经调制提升脉冲神经网络效率和能力
tldr: 脉冲神经网络（SNN）受生物神经元启发，具有高能效潜力，但在实际感知任务中性能有限。本文引入生物神经调节机制，使网络能根据上下文动态调整自身参数，显著提升了多种任务（包括噪声语音识别）的性能。该方法仅需极少的额外神经元、能量和参数，实现了神经元数量减少一个数量级，并大幅降低脉冲发放频率，从而提升能效。该工作揭示了神经调节在生物计算中的重要作用，为神经形态硬件的高效实现提供了理想方案。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-07-25-666748-v2/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1542, \"height\": 1246, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-07-25-666748-v2/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1488, \"height\": 1254, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-07-25-666748-v2/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1552, \"height\": 1264, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-07-25-666748-v2/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1538, \"height\": 1316, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-07-25-666748-v2/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1550, \"height\": 1021, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-07-25-666748-v2/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1556, \"height\": 1393, \"label\": \"Figure\"}]"
tables_json: "[{\"url\": \"assets/tables/biorxiv/biorxiv-10-1101-2025-07-25-666748-v2/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1546, \"height\": 1007, \"label\": \"Table\"}]"
motivation: 脉冲神经网络虽能效高，但实际任务性能不足，需增强其能力。
method: 引入生物神经调节机制，使网络动态上下文调整参数。
result: 多个感知任务性能显著提升，神经元减至十分之一，脉冲稀疏度提高，能耗极低。
conclusion: 神经调节同时提升SNN性能与效率，对神经形态计算和生物计算有重要意义。
---

## 摘要
脉冲神经元是大脑极高能效的基础，因此在神经形态计算中具有巨大潜力，尽管在实践中实现这种效率已被证明具有挑战性。我们利用神经调控——一种让网络动态且根据上下文修改自身参数的生物机制——发现它能在极少增加额外资源（神经元、能量、参数）的情况下，显著提升一系列感觉处理任务的性能，包括我们引入的一项具有挑战性的新型噪声环境语音数据集。神经调控网络在空间和能量上高效，这得益于两种与神经形态计算和生物学直接相关的机制：首先，它们使得所需神经元数量减少一个数量级；其次，它们能实现极稀疏的发放，通过使用数量级更少的脉冲获得更好的结果。这些特性共同可能揭示神经调控在生物体中的计算作用，并使神经调控成为提升神经形态设备性能和效率的理想机制。

## Abstract
Spiking neurons underlie the brain's extreme energy efficiency, and therefore have great potential in neuromorphic computing, although realising this efficiency in practice has proven challenging. We use neuromodulation, a biological mechanism that lets the network dynamically and contextually modify its own parameters. We find it substantially increases performance across a range of sensory processing tasks, including a challenging new speech-in-noise dataset we introduce, with very few additional resources (neurons, energy, parameters). Neuromodulatory networks are space and energy efficient thanks to two mechanisms that are directly relevant to neuromorphic computing and biology: firstly, they allow for an order-of-magnitude reduction in the number of neurons required; and secondly, they enable very sparse firing, achieving better results using orders of magnitude fewer spikes. Together, these properties may throw light on the computational role of neuromodulation in biology, and make neuromodulation an ideal mechanism to improve performance and efficiency for neuromorphic devices.