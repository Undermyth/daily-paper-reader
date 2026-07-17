---
title: "Data-driven oscillatory network modeling with condition-dependent coupling laws: Identifying directed neural interactions in working memory attention dynamics"
title_zh: 基于数据驱动的条件依赖耦合定律振荡网络建模：识别工作记忆注意动态中的定向神经交互
authors: "Ohkawa, M., Zhou, Y. J., Haegens, S., Jafarian, M."
date: 2026-07-10
pdf: "https://www.biorxiv.org/content/10.64898/2026.07.06.736523v1.full.pdf"
tags: ["query:comp-neuro"]
score: 8.0
evidence: 工作记忆注意动态的数据驱动振荡网络建模
tldr: 在学习新信息时，大脑需动态协调注意与工作记忆以应对干扰。本文提出数据驱动的振荡网络建模框架，利用通用微分方程学习条件依赖的耦合定律，并结合符号回归进行解释。在分心条件下，所有被试的MEG数据均显示从背外侧前额叶皮层（dlPFC）到初级视觉皮层（V1）的有向通路。该方法无需强先验假设即可识别条件依赖的耦合及有向通路，为理解认知控制的神经机制提供新视角。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-06-736523-v1/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1467, \"height\": 528}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-06-736523-v1/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1359, \"height\": 452}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-06-736523-v1/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1012, \"height\": 473}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-06-736523-v1/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1368, \"height\": 500}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-06-736523-v1/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1367, \"height\": 1003}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-06-736523-v1/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 909, \"height\": 1265}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-06-736523-v1/fig-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 1492, \"height\": 401}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-06-736523-v1/fig-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 1056, \"height\": 704}]"
tables_json: "[{\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-07-06-736523-v1/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1350, \"height\": 206}, {\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-07-06-736523-v1/table-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 892, \"height\": 199}]"
motivation: 学习时存在干扰需适应性调控注意与工作记忆，但条件依赖的耦合定律及有向通路难以直接识别。
method: 用通用微分方程扩展线性振荡网络，学习分心条件引起的耦合变化，再通过符号回归得到可解释函数。
result: 分心条件下，所有被试均出现从dlPFC到V1的有向通路，表明前额叶对视觉皮层的定向调控。
conclusion: 结合线性模型与通用微分方程及可解释性方法，可识别条件依赖耦合与有向通路，揭示适应性神经机制。
---

## 摘要
在面对干扰和条件变化时学习新信息需要适应的能力。在大脑中，这种适应能力与注意力和工作记忆之间的动态交互有关，这些交互使得能够选择性地过滤无关输入，同时保留行为相关信息。特定的神经振荡已被认为与此过程相关。

本文引入了一种基于现象学的数据驱动框架，用于振荡网络建模，该框架直接从神经记录中学习条件依赖的耦合定律，并能够推断条件依赖的定向路径。我们将该方法应用于参与者在执行有干扰和无干扰的工作记忆任务时收集的脑磁图（MEG）数据。首先使用线性振荡网络对无干扰条件下的回忆动态进行建模，其中每个感兴趣区域由两个α频带谐波振荡器表示。我们使用通用微分方程（UDE），一种神经微分方程的扩展，来捕捉干扰引起的耦合定律变化。然后使用符号回归将UDE识别出的修改解释为非线性函数，并提出了另一种方法来识别新出现的非线性项在大脑感兴趣区域动态中的定向路径。

尽管存在个体间差异，但在干扰条件下检查的所有四名参与者的工作记忆回忆数据均显示出从背外侧前额叶皮层（dlPFC）到初级视觉皮层（V1）的通路出现。这一发现与dlPFC在认知控制中的既定作用一致，并表明干扰处理招募了从前额叶到视觉区域的定向交互。更广泛地说，我们的结果表明，将数据学习参数的线性模型与通过可解释性方法增强的通用微分方程相结合，能够识别条件依赖的耦合定律，将其表示为可解释的数学函数，并发现振荡网络中适应性变化的候选定向路径，而无需对潜在机制做出强先验假设。

## Abstract
Learning new information in the presence of distracters and changing conditions requires the ability to adapt. In the brain, this adaptive capability has been linked to dynamic interactions between attention and working memory, which enable the selective filtering of irrelevant input while preserving behaviorally relevant information. Specific neural oscillations have been implicated in this process.

Here, we introduce a phenomenological data-driven framework for oscillatory network modeling that learns condition-dependent coupling laws directly from neural recordings and enables inference of condition-dependent directed pathways. We apply our approach to magnetoen-cephalography (MEG) data collected while participants performed a working-memory task with and without distracters. Recall dynamics in the non-distracter condition are first modeled using a linear oscillatory network in which each region of interest is represented by two alpha-band harmonic oscillators. We use universal differential equations (UDE), an extension of neural differential equations, to capture distracter-induced changes in coupling laws. Symbolic regression is then used to interpret the modifications identified by UDE as nonlinear functions, and an additional method is proposed to identify the directed pathway from the newly emerging nonlinear terms in the dynamics of brain regions of interest.

Despite inter-subject variability, working memory recall data from all four participants examined under distraction showed the emergence of a pathway from the dorsolateral prefrontal cortex (dlPFC) to the primary visual cortex (V1). This finding is consistent with the established role of the dlPFC in cognitive control and suggests that distracter processing recruits a directed interaction from prefrontal to visual regions. More broadly, our results illustrate that combining linear models whose parameters are learned from the data with universal differential equations augmented by interpretability methods enables the identification of condition-dependent coupling laws, their representation as interpretable mathematical functions, and the discovery of candidate directed pathways underlying adaptive changes in oscillatory networks without requiring strong prior assumptions about the underlying mechanisms.

---

## 论文详细总结（自动生成）

好的，作为一名资深学术论文分析助手，现根据您提供的论文内容，对其进行详细、结构化、客观的中文总结。

### **论文分析总结**

**标题**: 基于数据驱动的条件依赖耦合定律振荡网络建模：识别工作记忆注意动态中的定向神经交互

#### **1. 论文的核心问题与整体含义（研究动机和背景）**
*   **核心问题**: 当存在外部干扰时，大脑如何动态地协调注意力与工作记忆，以选择性过滤无关信息并保护行为相关的内容？具体而言，涉及注意与工作记忆交互的脑区之间如何进行动态的、有向的（定向）信息传递？
*   **研究动机**: 现有理论（如**偏向竞争理论**）和神经影像证据（如**α频段神经振荡**的调制）已暗示了相关机制，但潜在的生物物理机制尚不完全清楚。现有的“白盒”模型（如生物物理神经元网络、神经质量模型）通常是假设驱动的，参数多、拟合数据困难，且难以进行数据驱动的探索和解释。条件变化（如有无干扰）下的脑区间耦合变化通常仅用标量值表示，难以提供机制层面的洞见。
*   **整体含义**: 本文旨在开发一种**现象学的、数据驱动的振荡网络建模框架**，能够直接从神经记录（MEG）中学习**条件依赖的耦合定律**，并推断出在不同条件下（例如有/无干扰）新出现的**定向神经通路**，从而无需强先验假设就能揭示适应性变化的神经机制。

#### **2. 论文提出的方法论：核心思想、关键技术细节**
*   **核心思想**: 结合**线性模型**（捕捉已知的基线动力学）与**通用微分方程（UDE）**（捕捉未知的条件特异性变化），并通过**符号回归**将UDE学习到的非线性变化转化为可解释的数学函数，最后通过分析函数形式推断有向通路的候选者。
*   **关键技术细节与流程**:
    1.  **基线模型构建（无干扰条件）**:
        *   构建一个**双谐波振荡器网络**作为基线模型 `l(s)`。每个感兴趣区域（ROI）包含两个分别代表低频和高频的线性谐波振荡器。
        *   网络拓扑：四个ROI（V1, L-IPS, R-dlPFC, L-dlPFC）内的两个振荡器形成两个全连接网络，并在高低频网络之间存在交叉耦合。
        *   参数识别：使用多级单链接算法和Adam优化器等策略，拟合无干扰条件下的功率谱数据。
    2.  **注意力模型识别（有干扰条件）**:
        *   模型结构：`ds/dt = l(s) + g(s)`，其中`g(s)`代表干扰引起的动力学变化。
        *   使用**通用微分方程（UDE）** 建模`g(s)`：将`g(s)`用一个**神经网络** `N(s)` 来表示，其参数与基线模型参数`l(s)` 一起进行联合优化。
        *   通过**高斯伴随灵敏度方法**高效求解梯度，使用Adam优化器。
    3.  **数学解释与有向通路识别**:
        *   **符号回归（SINDy）**: 使用稀疏识别非线性动力学方法，将训练好的神经网络`N(s)`简化为驱动项的非线性函数，如`SR(p, s)`。
        *   **通路识别方法**: 通过分析符号回归得到的非线性函数`SR(p, s)`，识别哪些新的项（如`p*z41`, `p*z31`等）出现在了哪个ROI的动态方程中。这些项表示了其他ROI状态对当前ROI动力学的影响。通过可视化这些项在动力学轨迹上的贡献大小，定位“受影响”和“影响者”脑区，从而推断出条件依赖的定向通路。

#### **3. 实验设计**
*   **数据集**: 来自一项已发表的人类**MEG研究**的数据。
    *   **实验范式**: 工作记忆任务，包含**有干扰**和**无干扰**两个条件。任务分为编码、维持和回忆三阶段，本研究聚焦于**回忆阶段**。
    *   **数据获取**: 275通道MEG系统，1,200 Hz采样。
    *   **预处理**: 包括降采样、线噪声滤除、ICA伪迹去除、使用LCMV波束形成器进行源重建等。
*   **评估指标 & 方法对比**:
    *   **基线模型选择**: 比较了三种候选模型：
        1.  **Duffing-Van der Pol振荡器网络**
        2.  **Wilson-Cowan振荡器网络**
        3.  **双谐波振荡器网络**（本文提出的）
        *   **评价标准**: 最小化模型输出功率谱与无干扰条件下数据中位数功率谱之间的**均方误差（MSE）**。
*   **被试**: 4名参与者的数据。

#### **4. 资源与算力**
*   **文中未明确说明**使用了何种GPU型号、数量以及具体的训练时长。但文中提到使用了Julia编程语言、SciML框架。理论上，UDE训练涉及到对包含5000个参数的神经网络进行梯度计算，可能使用了GPU加速，但作者并未提供详细信息。

#### **5. 实验数量与充分性**
*   **基线模型对比实验**: 进行了3种模型（Duffing-Van der Pol, Wilson-Cowan, 双谐波振荡器）在4名被试数据上的性能对比。实验设计相对客观，对比了不同复杂度和生物可解释性的模型。
*   **最终模型验证**: 在4名被试数据上验证了完整的UDE模型和符号回归简化模型。实验结果显示模型能较好拟合个体数据。
*   **充分性评估**:
    *   **优点**: 方法在个体水平上进行了验证。
    *   **不足**:
        1.  **样本量极小**：仅有4名被试，结果的统计显著性和泛化能力受到极大限制。
        2.  **缺乏跨验证（Cross-validation）**: 模型可能仅拟合了单个被试的特定数据，存在过拟合风险。作者也承认“个体间差异未被显式处理”。
        3.  **缺乏消融实验**: 没有系统性地分析UDE、符号回归、或基线模型不同组件对最终结果的影响。
        4.  **基准对比单一**: 仅对比了不同基线模型，但未与如**动态因果模型（DCM）** 等主流方法进行对比。作者指出DCM需要大的模型库且更适合假设检验。

#### **6. 论文的主要结论与发现**
*   **方法可行性**: 提出的数据驱动框架（线性基线模型 + UDE + 符号回归）有效。
*   **关键生物学发现**: 在4名被试中，存在分心条件时，一致地出现了从**背外侧前额叶皮层（dlPFC）** 到**初级视觉皮层（V1）** 的定向通路（通过 `R-dlPFC -> V1` 或 `L-dlPFC -> R-dlPFC -> V1` 的形式体现）。
*   **意义**: 该发现与dlPFC（尤其是右侧）在认知控制中的经典角色一致，表明在预期有干扰时，前额叶会通过定向的神经交互来调控视觉皮层的回忆过程，且这种调控无法通过简单的比较有/无干扰条件下的耦合权重来发现。

#### **7. 优点：方法或实验设计上的亮点**
*   **新颖的方法论框架**: 首次将**通用微分方程（UDE）** 结合符号回归应用于神经振荡网络建模，为探索未知的、条件依赖的动态耦合提供了一种强大的数据驱动方法。
*   **增强解释性**: 通过符号回归将“黑箱”的神经网络转化为可解释的数学函数，并提出了**基于非线性项分析来推断有向通路**的新思路，这是关键创新点。
*   **灵活性**: 结合了物理先验知识（线性基线模型）与机器学习灵活性的优点，模型结构允许在无强假设下发现新机制。
*   **客观性**: 在模型选择上进行了量化比较，论证了所选模型（高维线性振荡器）的优越性，而非仅依赖主观判断。
*   **结果的可解释性**: 识别出的dlPFC到V1的通路与认知神经科学的现有知识一致，为方法学的可靠性提供了间接的生物学验证。

#### **8. 不足与局限**
*   **实验覆盖不足**:
    *   **样本量太小**（N=4），结论的统计可靠性和普适性存疑。
    *   **缺乏跨被试建模**: 仅对每个被试分别建模，未利用群体信息，增加了模型复杂度和过拟合风险。
*   **偏差风险**:
    *   **ROI及频率选择**: 手工选择的四个ROI和α频段可能有主观性，可能忽略其他重要脑区和频段（虽然文中提出了基于知识的理由）。
    *   **符号回归库设计**: 库函数的设计（如多项式的阶数、是否包含特定耦合项）对结果有直接影响，存在潜在的设计偏差。
*   **应用限制**:
    *   **仅关注静态频域特征**: 模型目前仅拟合功率谱，忽略了时域动态特征（如瞬态耦合），可能丢失重要信息。
    *   **未整合行为数据**: 没有将MEG数据与行为表现（如反应时、准确率）结合建模，减少了对认知过程理解的深度。
    *   **功能而非生物结构**: 模型是现象学的，识别出的“通路”是功能性的信息流方向，并不等同于解剖学上的突触连接。
    *   **计算复杂性**: 尽管有方法简化，但训练包含神经网络的UDE过程仍可能计算代价高昂，并依赖特定计算环境。

（完）
