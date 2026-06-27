---
title: A Tripartite Map of the Ventromedial Prefrontal Cortex
title_zh: 腹内侧前额叶皮层的三分区图谱
authors: "Chen, G., Song, D., Fu, M., Li, S., Zhang, M., Cui, Z., Xia, M., Sun, L., He, Y., Xu, T., Yu, X., Zang, Y., Zhou, J., Zhang, K., Qin, S., Popal, H., Saygin, Z. M., Osher, D. E., Olson, I. R., Rushworth, M. F. S., Wang, Y."
date: 2026-06-19
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.18.732791v1.full.pdf"
tags: ["query:comp-neuro"]
score: 8.0
evidence: 使用元分析和神经网络编码模型揭示VMPFC功能架构
tldr: 腹内侧前额叶皮层（VMPFC）参与情感、评估与社会认知，但其内部功能组织长期未明。本研究通过整合大规模元分析、个体任务fMRI、人工神经网络编码模型及多模态连接分析，揭示了沿前后轴的三部分组织：后部情感、中部评估、前部社会功能基序。每个基序嵌入不同大规模脑网络，该组织在个体水平可重复，推广至自然刺激，并跨发育与物种存在。研究为理解VMPFC功能提供了生物学基础框架。
source: biorxiv
selection_source: fresh_fetch
motivation: 揭示VMPFC情感、评估与社会认知功能如何在同一脑区内部组织。
method: 融合元分析、个体fMRI、神经网络编码模型与多模态连接分析。
result: 发现沿前后轴的三部分组织：后部情感、中部评估、前部社会功能基序。
conclusion: 建立VMPFC功能分区的生物学框架，解决长期组织问题。
---

## 摘要
腹内侧前额叶皮层（VMPFC）反复被证实参与情感、估价和社会认知，但这些多样功能如何在同一皮质区域内组织尚不清楚。本文整合大规模元分析、个体水平任务fMRI、人工神经网络编码模型和多模态连接分析，揭示了人类VMPFC的内部功能架构。通过四项互补研究，我们沿前后轴识别出一个稳健的三分区组织，包括后部情感、中部估价和前部社会功能主题。连接指纹分析表明，每个主题优先嵌入不同的大规模脑网络，为VMPFC功能特化提供了机制性解释。该组织在个体受试者水平可重复，泛化至自然刺激，贯穿发育过程，并与非人灵长类动物及多种神经生物学标志物表现出跨物种对应。这些发现共同解决了一个长期存在的组织问题，并建立了用于解释VMPFC功能的生物学基础框架。

## Abstract
The ventromedial prefrontal cortex (VMPFC) has been repeatedly implicated in affect, valuation, and social cognition, yet how these diverse functions are organized within a single cortical territory has remained unresolved. Here, we integrate large-scale meta-analysis, individual-level task fMRI, artificial neural-network encoding models, and multimodal connectivity analyses to reveal the internal functional architecture of the human VMPFC. Across four complementary studies, we identify a robust tripartite organization along the anterior-posterior axis, comprising posterior affective, middle valuation, and anterior social functional motifs. Connectivity fingerprinting demonstrates that each motif is preferentially embedded within distinct large-scale brain networks, providing a mechanistic account of VMPFC functional specialization. This organization is reproducible at the level of individual subjects, generalizes to naturalistic stimuli, extends across development, and shows cross-species correspondence with non-human primates and multiple neurobiological markers. Together, these findings resolve a long-standing organizational question and establish a biologically grounded framework for interpreting VMPFC function.

---

## 论文详细总结（自动生成）

### 1. 论文的核心问题与整体含义（研究动机和背景）

- **核心问题**：腹内侧前额叶皮层（VMPFC）被反复证实参与情感、估价和社会认知等多种功能，但这些不同功能如何在同一皮质区域内组织，长期以来缺乏统一解释。
- **研究动机**：现有研究多孤立地考察VMPFC的某个功能（如决策、情感或社会认知），而未系统地揭示其内部功能架构。术语“VMPFC”涵盖多个细胞构筑分区，边界存在争议；个体间沟形态变异大；fMRI易受磁敏感伪影影响。这些因素导致文献碎片化。
- **整体含义**：本研究旨在通过多模态、数据驱动方法，揭示VMPFC是否存在稳定的、可重复的内部功能组织原则，并测试其能否在个体、自然刺激、发育和跨物种层面泛化。

### 2. 论文提出的方法论：核心思想、关键技术细节

- **核心思想**：VMPFC的功能异质性源于沿前后轴排列的三个功能主题（motif）——后部情感、中部估价、前部社会。每个主题通过偏好连接不同的大规模脑网络而实现特化，并非严格模块化，而是连续整合架构中的主导模式。
- **关键技术细节**：
  - **Meta分析**（Study 1）：使用Neurosynth数据库（14,371项研究）进行反向推断和共激活建模（MACM）。对VMPFC内每个体素计算全脑共激活模式，经PCA降维后执行K-means聚类（K=2–6），通过Silhouette系数和Davies–Bouldin指数选择最优K=3。随后对每个簇进行功能解码（反向推断概率）。
  - **个体任务fMRI验证**（Study 2）：使用HCP青年数据集（n=667）的三个任务范式（情感处理、价值决策、社会认知）。提取个体峰值激活坐标，采用k近邻（KNN）分类器（k=3000）进行五折交叉验证，评估三分区在个体水平的可区分性。还使用支持向量分类和逻辑回归验证鲁棒性。
  - **ANN编码模型**（Study 2）：基于Natural Scenes Dataset（NSD，7T fMRI，每受试者22,000–30,000刺激-响应对）训练特征加权感受野（fwRF）模型，以AlexNet分层特征预测后、中、前VMPFC子区的平均响应。训练好的模型泛化至约30,000张自然图像（来自情感、价值、社会图片数据库），比较各子区预测响应。
  - **连接指纹预测活动**（Study 3）：使用自采优化数据集（n=42，改进EPI序列减少VMPFC信号丢失），对每个VMPFC体素计算结构连接（扩散纤维追踪）和功能连接（静息态fMRI）指纹。使用最小二乘线性回归，以留一被试交叉验证预测任务激活。通过标准化β权重识别各主题贡献最大的网络节点。
  - **跨生命期和跨物种验证**（Study 4）：利用HCP生命周期数据集（BCP、HCP-D、HCP-YA、HCP-Aging，n=2,293）及恒河猴数据（n=19），进行无任务连接性分区。还使用多模态特征（灰质体积、髓鞘指数、BOLD熵、神经递质受体密度）进行分区，比较K=2–6的一致性。
- **算法流程**：MACM：体素共激活向量 → PCA降维 → K-means聚类 → 选择K=3。连接预测：连接指纹作为特征 → 线性回归预测体素激活 → 留一交叉验证。被广泛应用于脑分区和连接-功能映射。

### 3. 实验设计：数据集、基准、对比方法

- **数据集**：
  - **Neurosynth**（14,371项fMRI研究）：用于MACM和反向推断。
  - **BrainMap**（4,341项研究）：独立验证MACM。
  - **HCP青年数据集**（n=667）：任务fMRI（情感-面貌匹配、赌博-奖励、社会-心理理论）。
  - **NSD数据集**（8名受试者）：7T fMRI自然场景，用于训练ANN编码模型。
  - **自采优化数据集**（n=42）：改进EPI序列，包含社交、价值、情感再评估任务及静息态/扩散成像。
  - **HCP生命期数据集**：BCP（0–5岁）、HCP-D（5–21岁）、HCP-YA（21–35岁）、HCP-Aging（36–100岁），共2,293人。
  - **PRIME-DE恒河猴数据**（n=19）。
  - 多模态特征数据：HCP结构MRI、PET受体图谱等。
- **基准**：无明确标准基准，但通过噪声上限（任务重测信度）和置换检验评估预测性能。
- **对比方法**：
  - 不同K值（2–6）的聚类方案对比。
  - 不同聚类算法（K-means、谱聚类、凝聚聚类）的鲁棒性检验。
  - 不同分类器（KNN、SVC、逻辑回归）的个体分类比较。
  - 不同连接模态（结构vs功能）预测效果对比。
  - 跨数据集泛化（自采模型泛化至HCP）。
  - 跨语言模型和神经空间聚类验证功能术语分类（Qwen3、Gemini 3 Pro）。

### 4. 资源与算力

- **文中未明确说明**。论文未提及使用的GPU型号、数量、训练时长等算力信息。仅描述了使用AlexNet作为特征提取器（预训练模型）和fwRF模型训练，但未给出计算资源细节。可能使用了标准CPU/GPU集群，具体不可知。需要指出这一点。

### 5. 实验数量与充分性

- **实验数量**：共四项研究（Study 1–4），涵盖：
  - 多数据库（Neurosynth、BrainMap）重复分析。
  - 三组不同阈值（≥100/150/200）和三种聚类算法鲁棒性检验。
  - 三种分类器个体验证。
  - 跨模态（结构/功能连接、灰质、髓鞘、熵、受体）分区比较（K=2–6）。
  - 跨生命周期和跨物种内部验证（5个人类队列+1个猴队列）。
  - 临床探索性映射（MDD、SUD、ASD、CD）。
  - ANN组合选择性测试（双/三属性混合刺激）。
  - 连接预测的跨数据集泛化（自采→HCP）。
- **充分性**：实验设计系统且全面，从群体级到个体级，从任务到自然刺激，从发育到进化，从多种神经模态综合验证。每个分析均包含统计检验（置换检验、交叉验证等）。整体客观、公平，方法透明（代码开源）。不足之处在于某些子分析（如临床映射）比较初步，样本量有限（自采42人、NSD 8人）。

### 6. 论文的主要结论与发现

- VMPFC沿前后轴存在稳健的三分区组织：**后部情感主题**（pVMPFC，与杏仁核、脑岛、dACC共激活，偏好恐惧、唤醒等情感词）、**中部估价主题**（mVMPFC，与腹侧纹状体、外侧眶额皮层连接，偏好价值、金钱、选择等词）、**前部社会主题**（aVMPFC，与DMPFC、TPJ、前颞叶、precuneus连接，偏好心理理论、自传体等词）。
- 这种组织在个体水平可通过KNN等分类器可靠区分（左半球0.688，右半球0.716，显著高于随机）。
- ANN编码模型证明该组织泛化至自然刺激：情感图片最大激活pVMPFC，价值图片激活mVMPFC，社会图片激活aVMPFC；组合刺激（如社会×价值）引起相应子区联合激活。
- 连接指纹可预测体素级任务激活，其中：aVMPFC由社交网络连接预测，mVMPFC由奖赏系统连接预测，pVMPFC由情感环路连接预测。
- 该三分区在人类全生命周期（0–100岁）和恒河猴中均可复现，且可通过灰质体积、髓鞘、熵、神经递质受体等多模态特征捕获，K=3是跨模态一致性最优解。
- 为VMPFC多样功能（情感、决策、社会认知）提供了统一的组织框架，支持神经认知的整合视角。

### 7. 优点

- **多模态、多尺度交叉验证**：整合元分析、个体fMRI、计算模型（ANN）、连接指纹、生命期和跨物种数据，结论稳健。
- **方法论严谨**：使用数据驱动而非先验定义边界；避免循环分析（如聚类功能术语时排除VMPFC内体素）；使用置换检验、交叉验证、噪声上限等控制。
- **实践导向**：提供开源代码和数据，提升可重复性；优化fMRI采集方法减少VMPFC信号丢失，利于未来研究。
- **可解释性强**：连接预测采用线性回归，保留了β权重解释性，明确了各主题的网络来源。
- **理论贡献**：将碎片化的VMPFC功能归因于连续组织原则，而非严格模块，兼容经典理论（如躯体标记假说、默认模式网络）。

### 8. 不足与局限

- **计算资源未报告**：缺少GPU模型、训练时长等，影响可复现性细节。
- **临床试验探索性**：临床映射仅基于有限研究，未进行系统Meta分析或因果检验，结论应视为假设。
- **样本量局限**：自采数据集n=42，ANN编码模型仅3/8名NSD受试者达到严格预测阈值（r>0.05），虽用宽松阈值复现，但泛化性需更大样本验证。
- **任务范式覆盖有限**：仅使用HCP三种任务，估价任务（赌博）个体重测信度较低，可能影响个体差异分析。
- **功能标签模糊**：“情感”“估价”“社会”是宽泛描述，而非精确计算变量。未来应使用模型驱动变量（如预期误差、自我-他人推理）替代。
- **反向推断受文献偏差影响**：某些VMPFC功能（如自主神经控制）在现有数据库中可能被低估。
- **边界变异未充分建模**：个体间边界位置存在差异，文中虽提及但未采用梯度或概率方法系统刻画。未来可发展连续梯度模型。

（完）
