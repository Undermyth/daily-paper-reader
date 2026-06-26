---
title: Looking beyond stereotyped neuron structures reveals links between beading and morphological rearrangements in aging phenotypes.
title_zh: 超越刻板神经元结构揭示了串珠与衰老表型中形态重排之间的联系
authors: "Gomez, K., Nguyen, K., Lagergren, J., Flores, K., San Miguel, A."
date: 2026-06-18
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.15.732273v1.full.pdf"
tags: ["query:comp-neuro"]
score: 6.0
evidence: CNN引导的树突追踪用于衰老表型分析
tldr: 理解衰老和急性应激下神经元形态变化对神经退行性疾病至关重要，但复杂树突结构分析困难。本研究采用CNN引导区域生长框架自动追踪树突，结合拓扑算法按分支度分类，实现了高精度（中位Dice 0.82）和十倍加速。发现衰老树突珠饰由分支历史决定，而非低阶脆弱；冷休克则引发全局扩散。表明慢性衰老与急性应激激活不同退行性通路，强调可靠分析变化形态的必要性。
source: biorxiv
selection_source: fresh_fetch
motivation: 探究衰老和急性应激下树突珠饰与形态重排的机制差异，传统范式忽略分支历史导致错误归因。
method: 采用CNN引导区域生长框架自动追踪树突，结合拓扑算法按分支度分类，分析分支历史对珠饰的影响。
result: 算法中位Dice 0.82，分析时间缩短10倍；发现衰老珠饰由分支历史决定，冷休克则全局扩散且严重程度依赖。
conclusion: 慢性衰老和急性应激通过不同通路（区室特异性谱系脆弱 vs 全局架构崩溃）影响树突形态，需新范式分析变化形态。
---

## 摘要
理解神经元形态在衰老和急性应激过程中的变化对于阐明神经退行性机制至关重要。秀丽隐杆线虫的高度分支的PVD神经元为研究树突重塑和与退化相关的表型（如树突串珠）提供了强大的模型。然而，这种树突结构的复杂性给自动分割和定量分析带来了重大挑战。在本研究中，我们采用了一种卷积神经网络（CNN）引导的区域生长框架进行自动树突追踪，并结合两种基于拓扑的算法，按分支程度对树突段进行分类。与手动追踪相比，该分割算法达到了高精度，中位Dice系数为0.82，同时将分析时间减少约十倍。自动树突分类在各分支阶次上与手动注释表现出高度一致性，然而基于位置的映射性能因渐进性形态扭曲而随年龄增长而下降。利用这一平台，我们研究了在衰老和冷休克过程中观察到的树突串珠模式的机制差异。与先前研究一致，衰老与串珠间距减小相关，而冷休克则随应激严重程度增加导致串珠分散程度增加。结构分析表明，这些趋势并非由树突修剪或树突复杂性降低驱动。相反，传统的解剖学上不灵活的范式错误地将低阶树突视为高度脆弱，而我们的分支感知框架揭示了年龄依赖性串珠从根本上由节段连续分支事件的历史决定。相反，急性冷休克触发了系统性串珠，以严重性依赖的方式扩展到所有树突阶次。总之，这些发现表明慢性衰老和急性应激涉及不同的退行性通路（区室特异性谱系脆弱性与整体结构崩溃），而非整体形态丧失，并强调了需要能够可靠分析形态变化的范式。

## Abstract
1Understanding how neuronal morphology changes during aging and acute stress is essential for elucidating mechanisms of neurodegeneration. The highly branched PVD neuron of Caenorhabditis elegans provides a powerful model for studying dendritic remodeling and degeneration-associated phenotypes such as dendritic beading. However, the complexity of this arbor presents substantial challenges for automated segmentation and quantitative analysis. In this study, we adapted a convolutional neural network (CNN)-guided region growing framework for automated dendrite tracing, coupled with two topology-based algorithms for categorizing dendritic segments by branching degree. The segmentation algorithm achieved high accuracy relative to manual tracing, with a median Dice coefficient of 0.82, while reducing analysis time by approximately tenfold. Automated dendrite categorization demonstrated strong agreement with manual annotations across branching orders, though position-based mapping performance declined with age due to progressive morphological distortion. Leveraging this platform, we investigated mechanistic differences in dendritic beading patterns observed during aging and cold shock. Consistent with prior work, aging was associated with decreased inter-bead spacing, whereas cold shock produced increased bead dispersion with stress severity. Structural analysis revealed that these trends were not driven by dendritic pruning or reduced arbor complexity. Instead, while a traditional anatomically unflexible paradigm falsely implicated lower-degree dendrites as highly vulnerable, our branching-informed framework revealed that age-dependent beading is fundamentally dictated by a segments history of successive branching events. Conversely, acute cold shock triggered systemic beading that expanded across all dendritic orders in a severity-dependent manner. Together, these findings demonstrate that chronic aging and acute stress engage distinct degenerative pathways (compartment-specific lineage vulnerability versus global architectural collapse) rather than gross morphological loss, as well as highlighting the need for paradigms that enable reliable analysis of changing morphologies.