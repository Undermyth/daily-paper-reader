---
title: "Hippocampal information topology breaks down in a mouse model of Alzheimer's disease"
title_zh: 阿尔茨海默病小鼠模型中，海马信息拓扑结构崩溃
authors: "Yu, J. J., Rajpal, H., Go, M. A., Schultz, S. R."
date: 2026-08-19
pdf: "https://www.biorxiv.org/content/10.64898/2026.08.14.744888v1.full.pdf"
tags: ["query:comp-neuro"]
score: 9.0
evidence: 将部分信息分解应用于海马CA1钙成像，揭示空间信息编码的拓扑结构，直接关联海马表征计算
tldr: 海马空间编码依赖神经元装配间的协调，但其信息拓扑组织及在疾病中的破坏机制未知。本文对CA1钙成像应用部分信息分解，发现健康小鼠中装配间的联合空间信息多于装配内，且以协同方式共享。在年老5xFAD小鼠中，该拓扑组织通过冗余失去拓扑依赖和协同失去情境敏感性两条途径瓦解，功能连接也出现模块性下降。研究揭示年龄与AD基因型的复合效应是破坏海马信息处理的关键驱动。
source: biorxiv
selection_source: fresh_fetch
motivation: 探索海马CA1网络拓扑如何组织空间信息处理，以及阿尔茨海默病如何破坏这种组织。
method: 对年轻/年老野生型和5xFAD小鼠的CA1钙成像数据应用部分信息分解，量化装配内外的冗余与协同信息。
result: 健康时装配间协同信息多于装配内；年老5xFAD中拓扑瓦解：冗余失去拓扑依赖、协同失去情境敏感性，功能连接模块性下降。
conclusion: 年龄与AD基因型的复合效应是海马信息处理与功能连接破坏的主要驱动，为理解AD神经机制提供新视角。
---

## 摘要
海马空间编码依赖于神经元集群之间的协调，然而网络拓扑如何组织这些集群间的信息处理，以及这一过程在疾病中如何被破坏，仍是未知的。我们应用部分信息分解对年轻和年老野生型及5xFAD小鼠的CA1钙成像数据进行分析，量化了集群内部和集群之间的冗余和协同信息共享。在健康的CA1区域，集群间配对比集群内配对携带更多的联合空间信息，且这种盈余是协同性的，从而确立了网络拓扑作为空间编码的组织原则。在老龄5xFAD小鼠的CA1中，这种拓扑组织通过两条不同的途径崩溃：随着模块化集群边界消解，冗余信息失去了其拓扑依赖性；在新异探索过程中，协同信息失去了情境敏感性，且当衰老与5xFAD基因型同时存在时，这种崩溃最为严重。这种功能衰退还伴随着功能连接中的拓扑效应，其中基因型与年龄的交互作用导致模块度、加权聚类系数和小世界性降低。社区层面的涌现揭示了衰老过程中向高阶整合的互补性跨尺度转变，而基因型-年龄的交互作用逆转了这一转变。我们分离出阿尔茨海默病中衰老的复合效应，将其视为小鼠海马神经元集群间信息处理和功能连接破坏的驱动因素。

## Abstract
Hippocampal spatial coding depends on coordination among neuronal assemblies, yet how network topology organises information processing across these assemblies, and how this is disrupted in disease, remain unknown. We apply Partial Information Decomposition to CA1 calcium imaging from young and aged wild-type and 5xFAD mice, quantifying redundant and synergistic information sharing within and between assemblies. In healthy CA1, between-assembly pairs carried more joint spatial information than within-assembly pairs, and this surplus was synergistic, establishing network topology as an organising principle of spatial coding. In aged 5xFAD CA1 this topological organisation broke down through two distinct routes: redundancy lost its topology dependence as modular assembly boundaries dissolved, and synergy lost context sensitivity during novel exploration, with the breakdown greatest where ageing and the 5xFAD genotype coincided. This functional decline was also accompanied by topological effects in the functional connectivity, where the genotype-age interaction resulted in reduced modularity, weighted clustering and small-worldness. Community-level emergence revealed a complementary cross-scale shift toward higher-order integration during ageing, which was reversed by the genotype-age interaction. We isolate the compounding effect of ageing in Alzheimer's disease as the driver of disruption in information processing and functional connectivity across neuronal assemblies in the mouse hippocampus.

---

## 论文详细总结（自动生成）

# 论文详细中文总结

## 1. 核心问题与整体含义（研究动机和背景）

- **研究背景**：海马体的空间编码依赖于神经元集群（assembly）之间的协调活动，但已有研究大多关注单个神经元或局部群体的编码特性，缺乏对“网络拓扑如何组织跨集群信息处理”的理解。
- **核心问题**：海马网络的信息拓扑组织原则是什么？在阿尔茨海默病（Alzheimer's disease, AD）中，这种组织如何被破坏？
- **整体含义**：论文将网络拓扑与信息论结合，提出“空间编码的拓扑组织原则”，并揭示衰老与AD基因型的复合效应是导致海马信息处理和功能连接破坏的关键驱动因素，为理解AD的神经机制提供了新视角。

## 2. 论文提出的方法论：核心思想、关键技术细节、公式或算法流程

- **核心思想**：利用部分信息分解（Partial Information Decomposition, PID）将两个神经元/集群的联合空间信息分解为冗余信息、协同信息、独特信息等成分，从而区分信息是来自单个集群内部还是跨集群协同。
- **关键技术步骤**：
  1. **数据来源**：使用年轻和年老野生型（WT）及 5xFAD 小鼠的 CA1 钙成像数据。
  2. **定义神经元装配（assembly）**：基于功能连接或空间调制特征识别神经元集群。
  3. **计算冗余与协同信息**：对装配内配对（within-assembly）和装配间配对（between-assembly）分别进行 PID，量化：
     - 冗余信息（redundant information）：两个源共同提供的相同信息；
     - 协同信息（synergistic information）：两个源联合提供而单独无法提供的信息。
  4. **拓扑依赖性分析**：比较装配内与装配间的信息成分差异，判断信息处理是否依赖网络拓扑结构。
  5. **功能连接分析**：计算模块度（modularity）、加权聚类系数（weighted clustering coefficient）、小世界性（small-worldness）以及社区层面的涌现（community-level emergence），评估网络拓扑的变化。
- **公式/算法说明**：摘要未给出具体 PID 公式，但其本质上是基于信息熵的分解方法：`I(S1,S2; T) = Red + Syn + Un1 + Un2`，其中 `Red` 为冗余，`Syn` 为协同，`Un` 为独特信息。论文通过比较不同条件下的 `Red` 与 `Syn` 成分来揭示组织原则。

## 3. 实验设计：使用了哪些数据集 / 场景，benchmark 是什么，对比了哪些方法

- **数据集**：来自小鼠海马 CA1 区的钙成像数据。
  - 基因型：野生型（WT）与 5xFAD（AD 模型）小鼠；
  - 年龄：年轻（young）与年老（aged）小鼠；
  - 因此共有 4 组：年轻 WT、年老 WT、年轻 5xFAD、年老 5xFAD。
- **任务场景**：涉及空间探索，特别提到“新异探索”（novel exploration）情境，用于检验情境敏感性。
- **Benchmark**：文献中没有明确的外部 benchmark，而是以健康状态（年轻 WT）下的组织模式作为基线。
- **对比方法**：
  - 主要对比装配内 vs 装配间的信息分解结果；
  - 对比不同基因型-年龄组合（WT vs 5xFAD; young vs aged）的差异；
  - 功能连接方面对比不同组间的网络指标（模块度、聚类系数、小世界性等）。

## 4. 资源与算力

- **论文未明确说明**所使用的计算资源（如 GPU 型号、数量、训练/推理时长等）。
- 由于是钙成像数据分析和信息论计算，不需要大规模深度学习训练，但具体硬件和运行时间未披露。
- 这一点反映出预印本在资源报告方面的不足，未来版本可补充。

## 5. 实验数量与充分性

- **实验组数**：至少 4 组（基因型 × 年龄），每组包含若干小鼠和成像 session（具体数量摘要未给出）。
- **分析维度**：
  - 信息分解（装配内 vs 装配间；冗余 vs 协同）；
  - 情境敏感性（新异探索）；
  - 功能连接指标（模块度、聚类系数、小世界性）；
  - 社区层面的跨尺度涌现。
- **充分性评估**：
  - 优点：实验设计覆盖了基因型和年龄的交互作用，且结合了信息拓扑与网络分析，角度较全面。
  - 不足：摘要未给出重复次数、样本量、统计检验的细节，无法判断效应量稳健性和统计功效；未提及消融实验或针对 PID 分解的置换检验；没有与其它信息分解方法（如基于编码模型的比较）做横向对比，因此结论的独特性仍需更多验证。

## 6. 论文的主要结论与发现

- **健康状态下的拓扑组织原则**：
  - 在健康 CA1 中，装配间配对比装配内配对携带更多的联合空间信息；
  - 这种装配间的信息盈余是**协同性**的，即跨集群的协同信息是空间编码的重要组织原则。
- **疾病状态下的崩溃机制（两条途径）**：
  1. **冗余信息失去拓扑依赖性**：模块化装配边界消解，导致冗余信息不再受装配内外关系约束；
  2. **协同信息失去情境敏感性**：在新异探索过程中，协同信息不再随情境变化而调节。
  - 这种崩溃在“年老 + 5xFAD”同时存在时最为严重。
- **功能连接层面的拓扑效应**：
  - 基因型-年龄交互作用导致模块度、加权聚类系数和小世界性显著降低；
  - 衰老本身引起向高阶整合的跨尺度转变（社区层面涌现），但基因型-年龄交互作用逆转了该转变。
- **核心结论**：衰老与 AD 基因型的复合效应是海马神经元集群间信息处理与功能连接破坏的主要驱动因素，揭示了 AD 中信息处理损伤的拓扑本质。

## 7. 优点

- **方法新颖**：首次将部分信息分解应用于海马 CA1 钙成像的装配内/间信息分析，将网络拓扑与信息论直接联系。
- **问题聚焦明确**：分离了“装配内”和“装配间”两个层次，并区分冗余与协同信息，能够揭示传统相关分析无法捕捉的协同编码机制。
- **多尺度分析**：同时覆盖微观（神经对）和介观（功能连接、社区结构）层面的拓扑变化，形成跨尺度视角。
- **实验设计合理**：使用 WT vs 5xFAD 和 young vs aged 双因素设计，能够识别基因型-年龄的交互效应，而非简单的叠加。
- **结论有临床启示**：指出“年龄 + 基因型”的复合效应比单一因素更能解释 AD 相关的功能破坏，有助于理解 AD 发病进程中衰老的贡献。

## 8. 不足与局限

- **信息省略**：作为预印本，摘要与元数据中未提供详细的样本量、数据采集参数、统计显著性阈值、效应量等信息，难以独立评估结果稳健性。
- **缺少方法对比**：未与其它信息度量（如互信息、传递熵）或其它 PID 实现进行系统性对比，无法判断该方法相对传统方法的优势。
- **无消融/控制实验**：未提及遮罩/置换检验、随机化对照或对 SNR 的鲁棒性分析，可能受钙信号噪声影响。
- **推广性有限**：结果仅基于小鼠 CA1 钙成像，未验证其它脑区或不同 AD 模型；人类 AD 的适用性尚不明确。
- **计算资源未披露**：无法评估可复现性与规模化分析的成本。
- **因果关系不足**：虽然识别了关联性，但“信息拓扑崩溃”与行为/认知障碍之间的因果联系未被直接验证，缺乏行为学数据支撑。

（完）
