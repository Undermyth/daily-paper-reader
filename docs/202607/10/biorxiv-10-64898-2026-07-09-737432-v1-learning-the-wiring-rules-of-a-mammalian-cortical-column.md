---
title: Learning the wiring rules of a mammalian cortical column
title_zh: 学习哺乳动物皮层柱的连接规则
authors: "Richter, O., Schneidman, E."
date: 2026-07-10
pdf: "https://www.biorxiv.org/content/10.64898/2026.07.09.737432v1.full.pdf"
tags: ["query:comp-neuro"]
score: 8.0
evidence: 使用表示学习学习皮层柱的连接规则
tldr: 针对神经回路建模依赖先验假设的局限，提出基于表征学习的方法，联合学习神经元低维嵌入与预测突触连接的布线规则。该方法仅用少量维度准确预测突触、连接度和网络模体，优于传统细胞类型分类模型。学习到的表示可解释，再现皮层深度、细胞类型和形态，揭示皮层连接遵循简洁逻辑。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-09-737432-v1/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1362, \"height\": 1500, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-09-737432-v1/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1825, \"height\": 1446, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-09-737432-v1/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1819, \"height\": 883, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-09-737432-v1/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1809, \"height\": 1164, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-09-737432-v1/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1838, \"height\": 1206, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-09-737432-v1/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1824, \"height\": 1631, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-09-737432-v1/fig-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 1069, \"height\": 1194, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-09-737432-v1/fig-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 1192, \"height\": 688, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-09-737432-v1/fig-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 1786, \"height\": 879, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-09-737432-v1/fig-010.webp\", \"caption\": \"\", \"page\": 0, \"index\": 10, \"width\": 1821, \"height\": 1106, \"label\": \"Figure\"}]"
motivation: 现有神经回路生成模型受限于测量和先验假设，需更通用方法。
method: 使用表征学习框架，联合学习神经元低维嵌入与突触预测的布线规则。
result: 嵌入模型在预测突触、连接度和模体统计上优于传统细胞类型分类模型。
conclusion: 皮层连接逻辑简洁，该框架可推广学习连接组简约生成模型。
---

## 摘要
神经回路结构的表征通常依赖于可测量的神经元特征，如形态、分子特性和空间位置。虽然利用这些特征的生成模型已被证明是准确的，但它们仍然受到现有测量和我们关于潜在特征的假设的限制。在这里，我们提出了一种使用表征学习的替代方法，并将其用于模拟小鼠初级视觉皮层一个柱的回路。我们的框架在抽象特征空间中联合学习神经元的低维嵌入，以及预测突触连接的连接规则。这些基于嵌入的模型能够准确预测单个突触、连接度和网络基序统计——仅使用少数几个嵌入维度和连接规则，就优于依赖于详细细胞类型分类的标准生成模型。关键的是，学习到的表示被证明是可解释的，能够重现皮层深度、细胞类型和树突形态。最终的连接蓝图既简单又具有生物学意义，表明皮层连接遵循了令人惊讶的简约逻辑。该框架为学习连接组的极小生成模型提供了一个通用且可移植的工具。

## Abstract
Characterization of neural circuits' architecture typically relies on measurable neuronal features such as morphology, molecular identity, and spatial location. While generative models leveraging these properties have proven accurate, they remain constrained by available measurements and our assumptions regarding the prospective features. Here, we present an alternative approach using representational learning and use it to model the circuitry of a column of the mouse primary visual cortex. Our framework learns jointly low-dimensional embeddings of neurons in an abstract feature space alongside wiring rules that predict synaptic connectivity. These embedding-based models accurately predict individual synapses, connectivity degrees, and network motif statistics -- outperforming standard generative models that depend on detailed cell-type classifications -- using only a handful of embedding dimensions and wiring rules. Crucially, the learned representations prove interpretable, recapitulating cortical depth, cell type, and dendritic morphology. The resulting wiring blueprint is both simple and biologically meaningful, suggesting that cortical connectivity follows surprisingly parsimonious logic. This framework offers a general and exportable tool for learning minimal generative models of connectomes.

---

## 论文详细总结（自动生成）

## 1. 核心问题与整体含义（研究动机和背景）

- **传统生成模型的局限**：现有神经回路生成模型依赖于手动设计的神经元特征（如细胞类型、形态、空间位置）和统计公式（如随机块模型 SBM、指数随机图模型 ERGM）。这些模型受限于**已知可测量的特征**和**设计者的先验假设**，可能遗漏尚未被识别或测量的关键生物物理特性。
- **本文目标**：提出一种**无偏的表示学习方法**，仅从连接数据中自动学习神经元的抽象特征（嵌入）和对应连接规则，以构建更准确、简洁且可解释的皮层连接模型。

## 2. 方法论

- **核心思想**：同时学习两个部分：
  1. **低维嵌入**：每个神经元被表示为 D 维向量（D=5），通过一个线性嵌入层从 one-hot 编码获得。
  2. **连接预测器（Connector）**：一个单隐层 MLP，隐层单元数为 R（R=6），每个隐层单元代表一条“布线规则”。
- **技术细节**：
  - 输入：前后神经元嵌入的拼接（2D 维）。
  - 隐层：ReLU 激活，输出：\( h_r = \text{ReLU}(\vec{w}_r^{pre}·\vec{e}_i + \vec{w}_r^{post}·\vec{e}_j) \)。
  - 输出：sigmoid 函数给出连接概率，\( P(G_{ij}=1) = \sigma(\sum_{r=1}^R w_r^{out} h_r) \)。
  - 训练：最大化训练数据似然，使用 Adam 优化器（batch size 64，200 epochs），Xavier 初始化。
- **数据划分策略**（解决嵌入学习与泛化验证的冲突）：
  - 训练神经元对（80%用于训练嵌入和Connector，20%验证）。
  - 固定 Connector，用跨训练-测试神经元对（80%）学习测试神经元嵌入。
  - 最终用纯测试神经元对（完全未见过）评估模型性能。

## 3. 实验设计

- **数据集**：小鼠初级视觉皮层（V1）单个皮层柱的 1351 个神经元连接组（MICrONS 联盟，数据版本 1507）。包含 75251 个二元连接（忽略自连接）。附带细胞类型（22 种形态类型）、皮层深度、兴奋/抑制身份、树突长度等生物标注。
- **基准对比方法**：
  - **SBM**（随机块模型）：基于 22 种形态类型的连接计数。
  - **ERGM**（指数随机图模型）：在 SBM 基础上增加连接神经元之间的物理距离约束。
- **评估场景**：
  1. **标准交叉验证**：随机分割神经元为训练/测试（各半），对比预测精度、层间密度、度分布、三元组模体分布。
  2. **泛化到未见细胞类型**：将三种形态类型全部置入测试集，训练集不包含这些类型的数据。对比无类型的基线模型（仅含连接数和距离特征的 ERGM）。

## 4. 资源与算力

- **文中未明确说明**使用的 GPU 型号、数量或训练时长。
- 仅提及：超参数网格搜索包含 172800 个配置（10 种子 × 10 嵌入维度 × 9 隐层大小 × 4 学习率 × 4 正则系数 × 3 数据分割）。
- 最终模型训练使用 100 个交叉验证分割，每个分割 10 个初始化，选最优。

## 5. 实验数量与充分性

- **数量充分**：超参数覆盖广泛；最终模型在 100 个分割上重复；泛化实验覆盖全部 1540 个可能的三元组类型（每种类型 15 个数据分割）；消融分析包括对嵌入生物特征的可解码性、混合模型性能、最近邻类型精度等。
- **公平性**：对比的 SBM 和 ERGM 是给定特征下的最大熵模型，属于理论最优基线；无类型基线模型合理。
- **局限**：仅在单一皮层柱数据上验证，未跨脑区或物种验证；未比较更复杂的深度学习方法（如图神经网络）。

## 6. 主要结论与发现

- **高精度与简洁性**：仅需 5 维嵌入 + 6 条规则即可达到饱和性能，在预测单个突触（AUROC 0.863）、层间密度（CCC 0.96）、度分布、三元组模体分布上均优于 SBM 和 ERGM。
- **可解释性**：嵌入空间自然地反映了皮层深度、兴奋/抑制身份和基底树突长度；最近邻在嵌入空间几乎总是同形态类型。
- **泛化能力**：对未见细胞类型，嵌入模型能恢复全模型绝大部分预测能力（泛化指数中位数 0.72）。
- **混合模型揭示生物学规则**：固定深度和 E/I 作为部分嵌入，剩余 3 维抽象，模型性能不变。通过分析权重可提取出清晰规则：不同深度神经元倾向不连接；抑制性神经元倾向连接更表层的兴奋性神经元；兴奋性神经元倾向连接更深层的兴奋性神经元。

## 7. 优点

- **方法创新**：端到端学习神经元表示和连接规则，避免特征工程偏差。
- **模型简约**：仅 5+6 参数极少的架构即达高性能。
- **可解释性强**：自动发现皮层深度、E/I 等已知关键特征，且剩余维度仍含未知生物信息。
- **泛化验证严谨**：特殊的数据划分策略确保嵌入和规则都能泛化到未见神经元。
- **对比合理**：使用信息论最优模型作为基线。

## 8. 不足与局限

- **数据来源单一**：仅使用小鼠 V1 一个皮层柱，结论的通用性存疑；需更多脑区、物种验证。
- **未完全解释的嵌入维度**：5 维中仍有 3 维无法用现有生物特征对应，虽表明存在未知因素，但缺乏实验手段进一步验证。
- **资源信息缺失**：未报告计算资源消耗，影响可复现性。
- **忽略功能信息**：仅基于结构连接，未结合神经活动数据，无法直接推断功能回路。
- **简化假设**：连接矩阵二值化（忽略突触数量），可能丢失弱连接信息。
- **无发育/学习过程建模**：仅描述静态连接模式，不涉及连接的形成机制。

（完）
