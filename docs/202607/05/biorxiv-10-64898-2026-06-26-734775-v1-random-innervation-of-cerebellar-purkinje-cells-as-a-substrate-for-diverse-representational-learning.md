---
title: Random innervation of cerebellar Purkinje cells as a substrate for diverse representational learning
title_zh: 小脑浦肯野细胞的随机神经支配作为多样性表征学习的基础
authors: "Holtrup, A. A., Khajeh, R., Lee, W.-C. A."
date: 2026-06-28
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.26.734775v1.full.pdf"
tags: ["query:comp-neuro"]
score: 7.0
evidence: 小脑回路建模与表征学习的计算神经科学研究
tldr: 小脑微环路中，平行纤维与浦肯野细胞的连接并非传统认为的全连接，而是一种部分随机支配。基于电子显微镜重建，我们发现这种连接符合伯努利随机模型，且平行纤维的上升分支与水平段连接无预测关系。在计算模型中，随机部分连接的浦肯野细胞群体性能优于全连接，表明部分连接作为固定随机掩码，能够促进神经元多样性，是小脑学习多样性的重要基质。
source: biorxiv
selection_source: fresh_fetch
motivation: 小脑浦肯野细胞仅接收部分平行纤维输入，其功能意义和机制尚不明确。
method: 基于电镜重建数据验证连接分布是否符合伯努利随机模型，并建立计算模型比较部分与全连接的性能。
result: 连接符合随机独立分布，且随机部分连接的浦肯野细胞群体在任务中表现优于全连接。
conclusion: 随机部分连接是小脑学习多样性的基质，为类小脑系统提供理论框架。
---

## 摘要
尽管小脑微回路是研究神经计算最完善的系统之一，但最近的连接组学分析突显了与经典模型的偏差，引发了关于该系统连接性、功能和学习的根本性问题。该回路的一个关键特征是大量平行纤维（PFs）汇聚到浦肯野细胞（PCs）上。主流的小脑计算模型假设在这个交叉点存在全对全连接，即单个PC从所有PFs中“采样”。然而，实验证据表明，每个PC只被一部分可接触的PFs所支配。这种部分采样产生了差异化的连接性，可能反映了小脑学习的组织原则，但其意义尚不清楚。

基于电子显微镜（EM）重建，我们显示PCs的PF支配在很大程度上与伯努利模型一致，其中连接在解剖约束内随机且独立分布。为了进一步支持随机模型，我们观察到颗粒细胞上升分支的连接不能预测其PFs的连接，并且PF与同一PC的多次空间接触之间的连接也不相关。在小脑回路模型中，我们探讨了部分连接性可能是学习基础的可能性，即一个固定的随机掩码，强制PCs之间的多样性。我们发现，当考虑PCs的“集合”时，随机部分连接性确实可以胜过全对全连接。我们的结果为理解小脑PFs和PCs之间部分连接性的作用提供了一个理论框架，并可能对小脑样系统及其他领域有启示意义。

## Abstract
Although the cerebellar microcircuit is among the most well-characterized systems for studying neural computation, recent connectomic analyses highlight deviations from canonical models, raising fundamental questions about connectivity, function, and learning in the system. A key feature of the circuit is the convergence of a vast number of parallel fibers (PFs) onto Purkinje cells (PCs). Prevailing models of cerebellar computation assume all-to-all connectivity at this intersection, whereby a single PC "samples" from all PFs. However, experimental evidence suggests that each PC is innervated by only a subset of accessible PFs. This partial sampling creates differential connectivity that may reflect an organizational principle of cerebellar learning, but its implications are poorly understood.

Based on electron microscopy (EM) reconstructions, we show that PF innervation of PCs is largely consistent with a Bernoulli model where connections are randomly and independently distributed within anatomical constraints. In further support of a random model, we observe that connections of the ascending branches of granule cells are not predictive of connections of their PFs, nor is connectivity correlated across separate spatial encounters of a PF with the same PC. In a model of the cerebellar circuit, we then address the possibility that partial connectivity is a substrate of learning, i.e., a fixed, random mask that enforces diversity between PCs. We find that when considering "ensembles" of PCs, random partial connectivity can indeed outperform all-to-all connectivity. Our results provide a theoretical framework for understanding the role of partial connectivity between cerebellar PFs and PCs and may have implications for cerebellum-like systems and beyond.