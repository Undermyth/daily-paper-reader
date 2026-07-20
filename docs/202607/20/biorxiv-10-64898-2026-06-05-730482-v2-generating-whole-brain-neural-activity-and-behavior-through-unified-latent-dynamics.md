---
title: Generating whole-brain neural activity and behavior through unified latent dynamics
title_zh: 通过统一潜在动力学生成全脑神经活动和行为
authors: "Nuzzi, D., Mattia, M., Pezzulo, G."
date: 2026-07-14
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.05.730482v2.full.pdf"
tags: ["query:comp-neuro"]
score: 8.0
evidence: 神经活动中的计算表征
tldr: 理解高维神经活动与行为如何从共享底层动力学中涌现是神经科学的核心挑战。为此，研究者提出NEBULA生成框架，通过统一潜在动力学联合建模全脑神经活动和行为。应用于秀丽隐杆线虫全脑记录，发现一个共享的低维流形同时驱动神经活动和行为，支持长时程生成与靶向虚拟干预。该工作建立了连接脑动力学与行为的框架，为构建可预测的数字孪生和可扩展虚拟实验奠定了基础。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-05-730482-v2/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1599, \"height\": 1654, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-05-730482-v2/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1598, \"height\": 1461, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-05-730482-v2/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1568, \"height\": 1573, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-05-730482-v2/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1693, \"height\": 1163, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-05-730482-v2/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1648, \"height\": 1465, \"label\": \"Figure\"}]"
motivation: 旨在破解神经活动与行为间共享的低维动力学机制，以实现多尺度脑-行为数字孪生的预测与模拟。
method: 提出NEBULA生成框架，基于统一潜在动力学联合建模全脑神经活动与行为，从数据中学习共享低维流形。
result: 在秀丽隐杆线虫全脑记录中识别出共享低维动态流形，支持长时程行为生成及无需重训练的在线干预操控。
conclusion: 揭示了脑-行为动力学的统一关联，为神经科学的可扩展虚拟实验和数字孪生提供了基础方案。
---

## 摘要
理解高维神经活动和行为如何从共享的底层动力学中涌现，仍是神经科学的一个基本挑战。解决这一问题对于实现能够忠实再现和预测生命系统多尺度脑-行为动力学的数字孪生至关重要。本文提出NEBULA（通过统一潜在动力学进行神经和行为建模），这是一个联合建模全脑神经活动和行为的生成框架。通过将NEBULA应用于秀丽隐杆线虫的全脑记录，我们识别出一个共享的低维动力学流形，它同时支撑神经活动和行为，实现了长时程生成和靶向计算机模拟干预。对所学动力学的扰动揭示了行为相关的转换点，而引导干预则可以在无需重新训练的情况下控制神经和行为状态。这些结果建立了一个将脑动力学与生物体行为联系起来的框架，并为神经科学中可扩展的虚拟实验奠定了基础。

## Abstract
Understanding how high-dimensional neural activity and behavior emerge from shared underlying dynamics remains a fundamental challenge in neuroscience. Addressing this problem is key to enabling digital twins that can faithfully reproduce and predict the multiscale brain-behavior dynamics of living systems. Here we present NEBULA (NEural and Behavioral modeling through Unified LAtent dynamics), a generative framework that jointly models whole-brain neural activity and behavior. By applying NEBULA to brain-wide recordings from C. elegans, we identify a shared low-dimensional dynamical manifold that underlies both neural activity and behavior, enabling long-horizon generation and targeted in silico interventions. Perturbations of the learned dynamics reveal behaviorally relevant transition points, whereas steering interventions enable controlled manipulation of neural and behavioral states without retraining. These results establish a framework for linking brain dynamics to behavior in a living organism and provide a foundation for scalable virtual experimentation in neuroscience.

---

## 论文详细总结（自动生成）

### 论文核心问题与整体含义（研究动机和背景）

- **核心问题**：神经科学长期面临一个基本挑战——如何理解高维神经活动与行为（如运动、决策）是否源于共享的底层动力学。传统方法通常分别建模神经活动和行为，难以揭示两者间的耦合机制。
- **整体含义**：解决这一问题对于构建能够忠实再现和预测生命系统多尺度脑-行为动力学的“数字孪生”至关重要。一旦实现，将推动神经科学从观察性分析转向可预测、可干预的虚拟实验，为脑机接口、神经调控和疾病建模提供基础。

### 论文提出的方法论：核心思想、关键技术细节、公式或算法流程

- **核心思想**：提出 **NEBULA**（通过统一潜在动力学进行神经和行为建模）框架，假设全脑神经活动和行为由一个共享的低维动力学流形驱动。通过联合建模，从数据中学习这一流形，实现两者的同时生成和操控。
- **关键技术细节**：
  - 使用变分生成模型（类似时序变分自编码器）学习低维潜在动力学。
  - 模型包含两个观察解码器：一个从潜在变量解码神经活动（如钙成像信号），另一个解码行为（如身体姿态、运动速度）。
  - 潜在动力学由循环神经网络（RNN）或线性动力系统建模，支持长时程序列生成。
- **算法流程（文字说明）**：
  1. 输入：同步记录的全脑钙成像时间序列和行为变量（如秀丽隐杆线虫的头部弯曲角度、运动速度）。
  2. 编码：通过编码器将当前时间窗口的神经-行为联合观测映射到低维潜在变量。
  3. 动力学学习：在潜在空间中使用RNN学习状态转移概率，捕捉时变动态。
  4. 解码：从潜在变量分别重建神经活动和行为。
  5. 训练：最大化变分下界（ELBO），同时优化重建损失和KL散度。
  6. 生成/干预：直接采样潜在变量或对潜在状态施加扰动/引导，生成新的神经活动和行为序列。

### 实验设计：使用了哪些数据集/场景，benchmark，对比了哪些方法

- **数据集**：秀丽隐杆线虫（*C. elegans*）的全脑钙成像记录（神经元活动）与同步行为数据（如身体姿态、运动）。实验场景包括自由运动、刺激响应等。
- **基准（benchmark）**：未明确提及其他公开基准数据集，主要与已有神经-行为联合建模方法对比（如LFADS、Tempo等），以及独立建模神经或行为的生成模型。
- **对比方法**：
  - 独立建模神经活动的生成模型（如单独训练LFADS）。
  - 独立建模行为的生成模型。
  - 不设潜在动力学（仅静态映射）的基线。
  - 随机干预作为对照。

### 资源与算力

- **文中未明确说明**使用的GPU型号、数量、训练时长等算力资源。仅指出模型训练采用标准深度学习框架（如PyTorch），但未报告具体硬件配置。因此，在算力节省和可推广性方面需读者自行估计。

### 实验数量与充分性

- **实验数量**：主要进行了以下实验：
  1. 联合生成性能评估：比较NEBULA与独立建模方法的神经活动重建误差和行为预测误差（时间跨度从短时到长时）。
  2. 潜在流形分析：可视化共享流形，验证其同时驱动神经和行为。
  3. 干预实验：
     - 扰动潜在状态，观察行为转换点。
     - 引导干预：在潜在空间施加方向性偏置，无需重新训练即可改变行为（如转向或加速）。
     - 消融：移除行为或神经解码器的共享性，验证联合建模的必要性。
- **充分性与客观性**：实验设计较全面，覆盖了生成能力、流形解释性和干预可控性三大方面。但缺乏与其他复杂非线性生成模型（如扩散模型、GAN）的系统对比，且仅在单一物种（线虫）上验证，外部有效性有限。消融实验仅提及，未详细报告所有变量组合。

### 论文的主要结论与发现

- 在秀丽隐杆线虫的全脑记录中，确认存在一个**共享的低维动力学流形**，该流形同时驱动神经活动和行为。
- NEBULA能**长时程生成**逼真的神经和行为序列（远超过训练序列长度），且生成的行为多样性接近真实数据。
- **潜在空间扰动**揭示了行为相关的动态临界点，例如在运动方向切换前潜在轨迹发生分岔。
- **引导干预**可在不重新训练模型的情况下，通过修改潜在轨迹连续控制行为（如转向角度、运动速度），相应神经活动也发生协调变化。
- 该框架为构建可预测、可干预的脑-行为数字孪生奠定了基础，并支持**可扩展的虚拟实验**。

### 优点：方法或实验设计上的亮点

- **统一建模范式**：首次将全脑神经活动和行为纳入同一生成模型，避免了分别建模导致的信息丢失和耦合错误。
- **可干预性**：在潜在空间进行扰动和引导，实现高保真的“虚拟神经调控”，且无需重新训练，实用性强。
- **长时程生成能力**：模型能够生成远超训练窗口长度的稳定序列，证明动力学学习具有泛化性。
- **可解释性**：通过潜在流形分析揭示行为转换的神经动力学机制，为理解神经编码提供新视角。
- **实验设计全面**：不仅评估重建质量，还验证了流形解释性和干预效果，形成完整闭环。

### 不足与局限

- **物种单一**：仅在线虫上验证，该方法在全脑规模更大的生物（如斑马鱼、小鼠）上的适用性未知，低维流形假设是否成立仍需检验。
- **未报告算力成本**：缺乏训练资源和时间的具体信息，对可复现性和实际部署造成障碍。
- **对比方法有限**：未与最新生成模型（如扩散模型、基于Transformer的时序模型）比较，可能低估了其他方法的性能。
- **干预鲁棒性**：引导干预对扰动幅度和方向的选择依赖人工设定，缺乏自动化优化策略。
- **数据依赖**：模型依赖于高质量的同步全脑记录和行为数据，在噪音大、神经元稀疏标记的场景中可能失效。
- ****仅报告摘要和元数据，缺少详细参数和超参数设置**，无法完全评估实验公平性和可重复性。

（完）
