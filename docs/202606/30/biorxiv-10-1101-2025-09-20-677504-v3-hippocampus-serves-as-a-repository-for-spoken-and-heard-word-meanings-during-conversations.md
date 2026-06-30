---
title: Hippocampus serves as a repository for spoken and heard word meanings during conversations
title_zh: 海马体在对话中充当口语和听到词语意义的存储库
authors: "Chavez, A. G., Franch, M., Mickiewicz, E., Baltazar, W., Belanger, J., Devara, D., Etta, M., Hamre, T., Ismail, T., Joiner, B., Kim, Y., Kona, A., Mansourian, K., Nangia, A., Pluenneke, M., Soubra, S., Venkateswaran, T., Venkudusamy, K., Chericoni, A., Kabotyanski, K., Katlowitz, K. A., Mathura, R., Paulo, D., Yan, X., Zhu, H., Bartoli, E., Provenza, N., Watrous, A., Josic, K., Sheth, S., Hayden, B. Y."
date: 2026-06-29
pdf: "https://www.biorxiv.org/content/10.1101/2025.09.20.677504v3.full.pdf"
tags: ["query:comp-neuro"]
score: 8.0
evidence: 海马对对话中词语意义的表征
tldr: 在对话中，海马体神经元同时编码口语和听到单词的意义，通过共享几何嵌入实现抽象跨人语义表示，并通过部分子空间对齐将说话者身份与意义绑定，子空间旋转程度随语义类别变化。该发现揭示了海马体如何平衡抽象意义与身份绑定的神经机制。
source: biorxiv
selection_source: fresh_fetch
motivation: 探究海马体如何同时支持抽象、模态无关的单词意义表示以及说话者身份绑定。
method: 分析对话中的单神经元记录，检验海马体是否使用共享几何嵌入编码听到和说出的单词意义。
result: 海马体神经元以共同几何嵌入编码口语和听到单词，并通过部分子空间对齐实现说话者-意义绑定。
conclusion: 海马体通过几何原则实现抽象跨人意义表示，同时保留与说话者身份的绑定。
---

## 摘要
我们利用内部意义表征有两个目的：理解我们听到的词语和生成我们自己的话语。这种双重需求要求抽象、模态无关的表征。基于将其识别为关系映射枢纽的研究，我们假设海马体支持抽象的、跨个体的表征，并通过共享语义几何来实现这一点。我们通过检查来自对话语音的显著单神经元数据集中的海马体活动来验证这一假设。神经元稳健地编码了口语和听到词语的意义，并对两者使用共同的几何嵌入，从而产生抽象的意义表现。说话者身份通过部分子空间对齐与意义对齐，这通过按说话者划分意义同时保持跨说话者泛化来实现说话者-意义绑定。子空间旋转的程度在单个词语水平上变化，并系统地取决于语义类别。综合起来，这些发现表明几何原则如何允许抽象的跨个体意义，同时保留与说话者身份的绑定。

## Abstract
We utilize internal representations of meaning for two purposes: to understand the words we hear and to generate our own speech. This dual requirement necessitates abstract, modality-agnostic representations. Building on work identifying it as a hub for relational mapping, we hypothesized that the hippocampus supports abstract, cross-person representations, and uses shared semantic geometries to do so. We tested this hypothesis by examining hippocampal activity in a remarkable single-neuron dataset derived from conversational speech. Neurons robustly encoded meanings of both spoken and heard words, and used common geometric embeddings for both, leading to abstract meaning performance. Speaker identity was aligned with meaning via partial subspace alignment, which affords speaker-meaning binding by partitioning meaning by speaker while maintaining cross-speaker generalization. Degrees of subspace rotation varied on a single word level and depended systematically on semantic category. Together, these findings indicate how geometric principles allow for abstract cross-personal meanings while preserving binding to speaker identity.