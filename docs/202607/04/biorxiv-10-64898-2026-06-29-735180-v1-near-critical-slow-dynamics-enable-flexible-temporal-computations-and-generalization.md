---
title: Near-critical slow dynamics enable flexible temporal computations and generalization
title_zh: 近临界慢动力学实现灵活的时间计算与泛化
authors: "Ramesan, G., Nandan, A., Koch, D., Koseska, A."
date: 2026-07-02
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.29.735180v1.full.pdf"
tags: ["query:comp-neuro"]
score: 7.0
evidence: RNN中时间计算的动态机制
tldr: 研究通过循环神经网络训练时间间隔任务，发现网络在接近临界动力学处自组织形成由近零特征值梯度谱表征的慢点鬼集。这些慢集构成动态支架，约束瞬态演化，输入重构向量场后慢集主导后续动力学，实现时间计算。慢集范围预测泛化能力，缺乏此类组织的网络无法外推。构建的具有类似慢集几何的最小动力学系统无需学习即可再现时间间隔，证明慢瞬变是时间计算的关键机制。
source: biorxiv
selection_source: fresh_fetch
motivation: 揭示低维流形背后产生、约束和稳定神经计算的动力学机制。
method: 使用循环神经网络训练时间间隔任务，分析状态空间结构和动力学特征。
result: 网络在临界点附近形成慢点鬼集，慢集程度预测泛化能力，缺乏者无法外推。
conclusion: 结构化慢瞬变是时间计算的关键机制，计算能力源于瞬态流组织而非吸引子状态。
---

## 摘要
尽管神经活动通常沿低维流形演化，但这类描述并未解释生成、约束和稳定计算的动力学机制。识别这些机制对于预测对扰动的响应、理解对未训练信号的泛化，以及解释不同电路实现如何产生相似计算至关重要。本文以训练于间隔计时任务的循环神经网络作为模型系统，揭示神经计算的动力学机制。我们发现，尽管训练后的网络收敛到高度多样的吸引子架构，但它们共享一种保守的瞬态动力学。在学习过程中，网络在动力学分岔附近自组织，形成由近零特征值的分级谱所表征的慢点结构化幻影集。这些慢集构成了约束轨迹演化的动力学支架。输入会瞬态地重构向量场并在此支架内重新定位活动，而底层慢集则支配后续动力学。因此，时间计算是通过结构化瞬态演化而非收敛到不动点或持续活动状态来实现的。慢集的程度预测了对未见时间间隔的泛化能力，而缺乏这种组织的网络无法可靠地外推。为测试充分性，我们构建了一个具有类似慢集几何结构的极小动力学系统，无需学习即可复现间隔计时，为识别时间计算的基本动力学要素提供了基准。综上，这些结果将结构化慢瞬态确定为时间计算的一种候选动力学机制，为慢低维流形作为底层状态空间结构的涌现结果提供了机制性解释，并表明近临界系统的计算能力源于瞬态流的组织而非单纯的吸引子状态。

## Abstract
Although neural activity often evolves along low-dimensional manifolds, such descriptions do not explain the dynamical mechanisms that generate, constrain, and stabilize computation. Identifying these mechanisms is essential for predicting responses to perturbations, understanding generalization to untrained signals, and explaining how similar computations arise from distinct circuit implementations. Here we use recurrent neural networks trained on an interval timing task as a model system to uncover the dynamical mechanisms of neural computation. We show that, despite converging to highly diverse attractor architectures, trained networks share a conserved transient dynamics. During learning, networks self-organize near dynamical bifurcations, forming structured ghost sets of slow points characterized by graded spectra of near-zero eigenvalues. These slow sets form a dynamical scaffold that constrains trajectory evolution. Inputs transiently reconfigure the vector field and reposition activity within this scaffold, while the underlying slow set governs subsequent dynamics. As a result, temporal computation is implemented through structured transient evolution rather than convergence to fixed points or persistent activity states. The extent of the slow sets predicts generalization to unseen temporal intervals, and networks lacking such organization fail to extrapolate reliably. To test sufficiency, we construct a minimal dynamical system endowed with analogous slow set geometry that reproduces interval timing without learning, providing a benchmark for identifying the essential dynamical ingredients of temporal computation. Together, these results identify structured slow transients as a candidate dynamical mechanism for temporal computation, provide a mechanistic interpretation of slow low-dimensional manifolds as emergent consequences of underlying state-space structure, and suggest that computational capacity in near-critical systems arises from the organization of transient flow rather than attractor states alone.