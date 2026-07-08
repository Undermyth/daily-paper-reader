---
title: "Toward Optimizing Thalamic Deep Brain Stimulation for Cortical Modulation: A Surrogate Brain Approach"
title_zh: 面向皮层调制的丘脑深部脑刺激优化：一种代理大脑方法
authors: "Ahmed, R., Feng, Y., Roe, A. W., Chen, Z. S."
date: 2026-07-01
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.26.734900v1.full.pdf"
tags: ["query:comp-neuro"]
score: 6.0
evidence: 使用替代脑方法优化丘脑深部脑刺激的计算框架，属于计算神经科学主题
tldr: 丘脑深部脑刺激（DBS）可实现对多个皮层节点的调控，但需个体化的丘脑-皮层有效连接（EC）估计和刺激参数优化。本文提出基于神经网络扰动推断（NPI）的替代大脑方法，通过拟合静息态fMRI数据的非线性动力学模型估计EC，并引入tSNR加权损失和跨尺度一致性损失提升训练效果。进一步构建约束线性控制问题，识别稀疏丘脑刺激靶点以实现期望皮层激活。在猕猴和人脑数据上验证，预测结果与已知结构一致。
source: biorxiv
selection_source: fresh_fetch
motivation: 丘脑DBS能分布式调制皮层，但需要个体化有效连接图和优化刺激参数来达成预期皮层响应。
method: 基于NPI的替代大脑方法，扩展至高分辨率丘脑-皮层网络，使用tSNR加权损失和跨尺度一致性损失训练动力学模型，并求解约束线性控制问题。
result: 在合成数据和猕猴/人脑数据上，方法准确估计了位点特异性丘脑-皮层EC，预测与已知结构对齐，且优化目标可行。
conclusion: 为个体化优化丘脑DBS提供了计算基础，适用于灵长类模型，有望提升临床调控精度。
---

## 摘要
丘脑是与广泛皮层和皮层下节点交互的中枢枢纽。丘脑深部脑刺激（DBS）为分布式皮层调制提供了一种策略：由于不同的丘脑核团投射到空间分离的皮层区域，单个丘脑部位的刺激可以影响多个皮层节点。实现这一潜力需要对定向丘脑皮层有效连接（EC）进行准确的个体特异性估计，并构建一个计算框架来优化刺激参数，以产生期望的皮层反应。在这里，我们利用神经扰动推断（NPI）来应对这两个挑战，这是一种代理大脑方法，通过对拟合静息态fMRI数据的非线性动力学模型施加虚拟扰动来估计EC。我们将NPI扩展到高分辨率丘脑皮层网络，包括360个皮层区域和覆盖12个核团的442个丘脑体素。我们在训练中引入了两项创新：(i) 考虑信号异质性的时间信噪比（tSNR）加权损失，以及(ii) 多分辨率、跨尺度一致性损失，用于正则化模型复杂度。这些策略在不同的tSNR条件下在合成基准测试中提升了性能。利用推断出的个体特异性EC，我们进一步构建了一个约束线性控制问题，以识别稀疏的丘脑刺激目标，实现期望的皮层激活模式。我们在两个独立数据集上验证了推断的EC结构：包含两只接受内侧枕核红外神经刺激的猕猴的MacStim数据集，以及包含12名人类受试者的HumanTC静息态fMRI数据集。我们的结果揭示了位点特异性的丘脑皮层EC轮廓，产生了与已知真实结构一致的可解释预测。总之，这项工作为人类和非人类灵长类动物丘脑DBS的个性化优化建立了一条计算基础途径。

## Abstract
The thalamus is a central hub that interfaces with widespread cortical and subcortical nodes. Thalamic deep brain stimulation (DBS) offers a principled strategy for distributed cortical modulation: since distinct thalamic nuclei project to spatially segregated cortical territories, stimulation at a single thalamic site can influence multiple cortical nodes. Realizing this potential requires accurate subject-specific estimates of directed thalamocortical effective connectivity (EC) and a computational framework for optimizing stimulation parameters that achieve desired cortical responses. Here, we address both challenges using Neural Perturbational Inference (NPI), a surrogate-brain approach that estimates EC by applying virtual perturbations to a nonlinear dynamical model fitted to resting-state fMRI data. We extend NPI to a high-resolution thalamocortical network comprising 360 cortical regions and 442 thalamic voxels spanning 12 nuclei. We introduce two innovations in training: (i) a temporal signal-to-noise ratio (tSNR)-weighted loss accounting for signal heterogeneity, and (ii) a multi-resolution, cross-scale consistency loss that regularizes model complexity. These strategies yield improved performance in synthetic benchmarks across varying tSNR regimes. Leveraging the inferred subject-specific EC, we further formulate a constrained linear control problem to identify sparse thalamic stimulation targets that achieve desired cortical activation patterns. We validate the inferred EC structure on two independent datasets: the MacStim dataset comprising two macaque monkeys with infrared neural stimulation on medial pulvinar, and the HumanTC resting-state fMRI dataset comprising twelve human subjects. Our results reveal site-specific thalamocortical EC profiles, producing interpretable predictions that align with known ground-truth structures. Together, this work establishes a computationally grounded pathway toward personalized optimization of thalamic DBS in both human and nonhuman primates.