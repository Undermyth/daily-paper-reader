---
title: Brain-Language Alignment During Naturalistic Reading and Its Disruption by Mind-Wandering
title_zh: 自然阅读期间的大脑-语言对齐及其被走神干扰
authors: "Sun, H., Jangraw, D. C."
date: 2026-08-19
pdf: "https://www.biorxiv.org/content/10.64898/2026.08.14.744875v1.full.pdf"
tags: ["query:comp-neuro"]
score: 8.0
evidence: 自然阅读中大脑-语言对齐的计算编码模型
tldr: 自然阅读中的脑-语言对齐及其受走神影响尚不清楚。本研究利用ROAMM数据（44人EEG+眼动），用五种词嵌入训练岭回归模型预测注视对齐的谱功率与FRP，发现可靠对齐：上下文嵌入优于静态，谱对齐在顶叶alpha/低beta频段，FRP在200-300ms；走神时对齐减弱，振荡特征更甚。这证明自然阅读EEG可反映语言模型表征，注意力波动是编码研究的重要变异来源。
source: biorxiv
selection_source: fresh_fetch
motivation: 多数EEG脑-语言对齐证据来自逐词范式，自然阅读下的对齐性及走神的影响尚不清楚，构成关键研究空白。
method: 采用ROAMM数据集（44人EEG与眼动），用五种词嵌入训练岭回归编码模型，预测注视对齐的谱功率与FRP，经排列检验校正。
result: 上下文嵌入优于静态；谱对齐最强在顶叶alpha/低beta频段，FRP对齐在200-300ms；走神时对齐下降，PSD特征受影响更大。
conclusion: 自然阅读中语言模型表征可在EEG中可靠解码，注意力波动是编码研究不可忽视的变异来源。
---

## 摘要
编码模型为将语言的计算表征与神经活动联系起来提供了一个原则性框架，但大多数关于大脑-语言对齐的脑电图（EEG）证据来自严格控制、逐词阅读的范式。在自然阅读过程中是否能检测到这种对齐，以及它如何受到注意力下降的影响，仍不清楚。我们使用ROAMM解决了这些问题，这是一个多模态数据集，包含44名参与者阅读自然文本时的同步EEG和眼动记录，以及时间分辨的走神（MW）注释。我们训练岭回归编码模型，从五种词嵌入模型（GloVe、word2vec、BERT、GPT-2和Llama 3）预测注视对齐的EEG频谱功率和注视相关电位（FRP）。使用错误发现率校正的置换检验，我们发现了两种特征类型中统计上可靠的大脑-语言对齐，且上下文嵌入优于静态嵌入。频谱对齐在顶叶电极上的alpha和低beta频段最强，而基于FRP的对齐在注视开始后200-300毫秒在中央和顶枕区达到峰值。利用ROAMM的跨度级MW注释，我们进一步表明，大脑-语言对齐在走神期间系统性降低，且这种效应在振荡（PSD）特征中显著大于事件相关（FRP）特征。这些发现表明，尽管模态存在固有噪声，现代语言模型表征仍能在自然阅读期间的EEG活动中得到反映，而注意力波动构成了大脑-语言编码研究中未被充分重视的变异性来源。

## Abstract
Encoding models offer a principled framework for linking computational representations of language to neural activity, but most electroencephalography (EEG) evidence for brain--language alignment comes from tightly controlled, word-by-word reading paradigms. Whether such alignment is detectable during naturalistic reading, and how it is affected by lapses in attention, remains unclear. We addressed these questions using ROAMM, a multimodal dataset containing simultaneous EEG and eye-tracking recordings with time-resolved mind-wandering (MW) annotations from 44 participants reading naturalistic texts. Ridge regression encoding models were trained to predict fixation-aligned EEG spectral power and fixation-related potentials (FRPs) from five word-embedding models (GloVe, word2vec, BERT, GPT-2, and Llama 3). Using permutation testing with false discovery rate correction, we found statistically reliable brain--language alignment across both feature types, with contextual embeddings outperforming static embeddings. Spectral alignment was strongest in the alpha and low-beta bands over parietal electrodes, while FRP-based alignment peaked 200--300 ms after fixation onset over central and parietal-occipital regions. Leveraging ROAMM's span-level MW annotations, we further show that brain--language alignment is systematically reduced during MW, an effect that was substantially larger for oscillatory (PSD) than for event-related (FRP) features. These findings demonstrate that modern language-model representations are reflected in EEG activity during naturalistic reading despite the modality's inherent noise, and that fluctuations in attention constitute an underappreciated source of variability in brain--language encoding studies.

---

## 论文详细总结（自动生成）

### 1. 核心问题与整体含义（研究动机与背景）

- **研究空白**：编码模型（encoding model）是将语言的计算表征与神经活动联系起来的原则性框架。然而，现有脑电图（EEG）证据大多来自严格控制、逐词（word-by-word）呈现的实验室范式，在**自然阅读**（naturalistic reading）情境下是否仍能检测到大脑-语言对齐，以及**走神/心智游移**（mind-wandering, MW）会如何影响这一对齐，此前尚不清楚。
- **研究动机**：自然阅读是语言理解的生态效度更高的场景，但伴随着眼球运动、注视时间变异和注意力波动等额外噪声。作者希望回答两个核心问题：(1) 在自然阅读的 EEG 信号中，语言模型表征是否仍可被可靠解码？(2) 走神这种常见的注意流失状态是否系统性削弱大脑与语言表征之间的对齐？
- **整体含义**：该研究将脑-语言编码模型的验证从严格实验范式推进到自然场景，同时揭示**注意力波动是编码研究中不可忽视的变异来源**。这对未来自然主义神经语言学研究和脑机接口应用具有方法论意义。

### 2. 方法论：核心思想与技术细节

- **核心思想**：采用**岭回归编码模型**，从词嵌入（word embedding）特征预测注视对齐（fixation-aligned）的 EEG 信号，从而量化语言刺激表征与神经活动之间的映射关系。
- **特征构建**：
  - 语言特征：使用五类词嵌入模型提取每个注视点对应单词的向量表征。
  - 神经特征：两类 EEG 特征——(a) **频谱功率**（PSD，注视对齐的谱功率）；(b) **注视相关电位**（FRP，fixation-related potential）。
- **模型训练与评估**：
  - 以词嵌入为输入、EEG 特征为输出，训练岭回归模型（通过 L2 正则化控制过拟合）。
  - 通过比较模型预测与真实 EEG 信号的匹配程度来评估对齐强度。
- **统计推断**：
  - 采用**置换检验**（permutation testing）评估对齐是否显著高于偶然水平。
  - 多重比较校正使用**错误发现率（FDR）**控制。
- **走神分析**：利用 ROAMM 数据集中的跨度级（span-level）走神标注，将数据划分为走神状态与非走神状态，分别计算并比较大脑-语言对齐强度，以检验注意力波动的影响。

### 3. 实验设计

- **数据集**：使用 **ROAMM**（一个多模态自然阅读数据集），包含：
  - 44 名参与者；
  - 同步记录的 EEG 与眼动数据；
  - 参与者阅读自然文本（非逐词呈现）；
  - 带有时间分辨的走神（MW）标注。
- **Benchmark / 对比基线**：
  - **词嵌入模型对比**：静态嵌入（GloVe、word2vec） vs. 上下文嵌入（BERT、GPT-2、Llama 3），用于考察嵌入类型对预测效力的影响。
  - **统计基线**：通过置换检验构造的机会水平（chance level）作为对齐是否显著存在的零假设基准。
- **特征维度对比**：两类 EEG 特征（PSD 与 FRP）互为对照，考察不同神经信号成分对语言表征的敏感度差异。
- **状态对比**：走神状态 vs. 非走神状态，考察注意力波动对对齐的调节作用。

### 4. 资源与算力

- 论文摘要与元数据中**未明确说明**所使用的 GPU 型号、数量、训练时长等算力信息。
- 考虑到任务仅为 44 人的 EEG 回归预测（非大规模深度学习训练），计算负载应属中等水平，但这一点**无法从提供的信息中确认**，需要查阅全文或补充材料才能获知具体硬件配置。

### 5. 实验数量与充分性

- **实验数量**：
  - 两种神经特征类型（PSD、FRP）× 五种词嵌入模型，构成系统的交叉验证；
  - 每种条件下进行置换检验统计推断；
  - 走神 vs. 非走神的对比分析。
- **充分性评估**：
  - **优点**：实验设计覆盖了嵌入类型（静态 vs. 上下文）、神经特征（振荡 vs. 事件相关）、注意力状态（走神 vs. 非走神）三个关键维度，结构对称、对比清晰，统计检验规范。
  - **局限**：摘要中未报告交叉验证的具体折数、置换检验次数、超参数选择（如岭回归正则化强度）等细节；未提及是否存在按参与者/文本的泛化测试或留出验证；也未见对模型深度、层数或嵌入维度等变量进行消融分析。因此，虽然核心结论成立，但**实验完备性仍有待全文确认**。

### 6. 主要结论与发现

- **对齐可检测**：在自然阅读的 EEG 中，两种特征类型（频谱功率和 FRP）均表现出统计上可靠的大脑-语言对齐。
- **上下文嵌入优于静态嵌入**：BERT、GPT-2、Llama 3 等上下文嵌入的预测效力显著高于 GloVe 和 word2vec 等静态嵌入，说明语境化语义表征与神经活动的对应关系更强。
- **时空-频率特异性**：
  - 频谱对齐在**顶叶（parietal）电极**的 **alpha 和低 beta 频段**最强；
  - FRP 对齐在**注视开始后 200-300 ms** 于**中央和顶枕区（central and parietal-occipital）**达到峰值。
- **走神系统性降低对齐**：走神期间大脑-语言对齐显著下降，且这种下降对**振荡（PSD）特征的影响远大于事件相关（FRP）特征**，提示走神主要干扰持续的神经振荡跟踪而非瞬态的事件相关响应。
- **总体含义**：尽管 EEG 模态固有噪声较大，现代语言模型表征仍能在自然阅读中被可靠解码；注意力波动是脑-语言编码研究中不可忽视的变异来源。

### 7. 优点

- **生态效度高**：采用自然文本阅读而非逐词呈现，结论更贴近真实语言加工情境。
- **多模态同步数据**：EEG 与眼动同步记录，并以注视点而非刺激呈现时刻为对齐基准，更符合自然阅读的认知节奏。
- **模型谱系覆盖全面**：从静态嵌入（GloVe、word2vec）到不同规模的上下文模型（BERT、GPT-2、Llama 3），可系统比较表征类型的影响。
- **双特征通道验证**：同时分析频谱功率（振荡层面）和 FRP（事件相关层面），相互印证，增强结论稳健性。
- **引入注意力状态维度**：利用自然出现的走神标注，考察内部认知状态对神经编码的影响，拓展了编码模型的分析范围。
- **统计严谨**：使用置换检验 + FDR 校正，控制多重比较误差。

### 8. 不足与局限

- **模态噪声限制效应量**：EEG 信噪比低，自然阅读中眼球运动和肌电伪迹较多，可能导致对齐效应被低估或某些真实效应未被检测到。
- **走神标注粒度**：ROAMM 采用跨度级（span-level）MW 标注，而非逐词或逐注视点粒度，可能模糊走神状态转换瞬间的精细动态。
- **个体差异未充分讨论**：摘要未报告个体层面的变异性分析，不同参与者的走神倾向、阅读习惯可能对结果产生混杂影响。
- **模型可解释性有限**：岭回归 + 深度嵌入的组合虽能预测神经活动，但难以揭示具体是哪些语言特征（句法、语义、情感等）驱动了对齐。
- **计算细节缺失**：未报告超参数选择、交叉验证方案、置换次数等，影响结果的可复现性和与其他研究的直接比较。
- **样本量中等**：44 人对于基于 EEG 的个体差异研究而言属于中等规模，统计功效有限，需更大样本验证。
- **泛化性未知**：仅基于单一数据集（ROAMM）和英语自然文本，结论向其他语言、其他模态或临床人群推广时需谨慎。
- **对比公平性**：未提及是否对各嵌入模型的维度进行了统一或是否控制了参数量差异，不同模型之间的比较可能受维度、训练语料和架构差异的干扰。

（完）
