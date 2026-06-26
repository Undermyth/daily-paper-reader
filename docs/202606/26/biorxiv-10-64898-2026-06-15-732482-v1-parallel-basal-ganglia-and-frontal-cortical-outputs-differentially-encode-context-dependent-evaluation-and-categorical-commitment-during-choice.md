---
title: Parallel basal ganglia and frontal cortical outputs differentially encode context-dependent evaluation and categorical commitment during choice
title_zh: 平行基底神经节和额叶皮层输出在抉择过程中差异编码情境依赖的评估与分类承诺
authors: "Yoshida, A., Krauzlis, R., Hikosaka, O."
date: 2026-06-18
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.15.732482v1.full.pdf"
tags: ["query:comp-neuro"]
score: 8.0
evidence: 选择过程中情境依赖评估和分类承诺的神经基础
tldr: 适应性选择需要将选项评估转化为具体行动承诺，其神经机制尚不清楚。本研究利用顺序提供选择任务，记录猴子黑质网状部（SNr）和额叶眼动区（FEF）神经元活动，部分分离序数排名与类别承诺。发现SNr活动主要由序数排名解释，而FEF活动由类别承诺解释，且两者在目标评估阶段表现出不同调制模式。这些结果揭示了基底节与额叶皮层在评估与决策承诺中的分工，为理解选择行为神经基础提供新见解。
source: biorxiv
selection_source: fresh_fetch
motivation: 探究选项评估向行动承诺转化的神经回路机制，特别是基底节与额叶皮层输出的不同功能角色。
method: 记录猴子执行顺序提供选择任务时SNr和FEF的神经元活动，通过行为模型分解分析活动与序数排名、类别承诺等变量的关系。
result: SNr活动主要由序数排名解释，FEF活动由类别承诺解释，两者在场景调制和目标评估时表现不同。
conclusion: 上下文依赖评估与类别承诺在平行基底节和额叶皮层输出通路中分工协作，指导自愿选择。
---

## 摘要
适应性抉择需要将可用选项的评估转化为对特定行动的承诺，但理解这种转化如何在神经回路中实现仍是一个核心挑战。在这里，我们在黑质网状部（SNr）和额叶眼动区（FEF）记录了良好分离的神经元，它们向视上丘发送平行投射以驱动眼动选择，同时让猴子执行一个序列式提议选择任务，该任务旨在部分解离情景定义的顺序等级与分类承诺。在目标出现之前，SNr显示出比FEF更强的场景相关调节。在目标评估期间，SNr的活动表现出以顺序等级主导的行为结果上的有序调节，而FEF的活动则将接受与拒绝明确分离，并强烈编码目标方向。行为模型分解揭示，仅顺序等级就能最好地解释SNr活动，优于奖励幅度甚至是一个包含等级、奖励、情境和等待成本的复合可接受性度量，而FEF活动则由分类承诺最好地解释。这种分离在多变量建模、单神经元响应模式和所有三只猴子中一致。总之，这些发现支持一种分工，其中情境依赖的评估和分类承诺分布在平行的基底神经节和额叶皮层输出通路中，以有效指导自愿选择。

## Abstract
Adaptive choice requires transforming the evaluation of available options into commitment to a specific action but understanding how this transformation is implemented across neural circuits remains a central challenge. Here we recorded well-isolated neurons in the substantia nigra pars reticulata (SNr) and frontal eye field (FEF), which send parallel projections to the superior colliculus for driving the eye movement choice, while monkeys performed a sequential-offer choice task designed to partially dissociate scene-defined ordinal rank from the categorical commitment. Before target onset, SNr displayed stronger scene-related modulation than FEF. During target evaluation, SNr activity showed ordered modulation across behavioral outcomes dominated by ordinal rank, whereas FEF activity categorically separated acceptance from rejection and strongly encoded target direction. Behavioral model decomposition revealed that ordinal rank alone best explained SNr activity, outperforming both reward magnitude and even a composite acceptability measure that incorporated rank together with reward, scene context, and waiting cost, whereas FEF activity was best explained by categorical commitment. This dissociation was consistent across multivariable modeling, single-neuron response patterns, and all three monkeys. Together, these findings support a division of labor in which context-dependent evaluation and categorical commitment are distributed across parallel basal ganglia and frontal cortical output pathways to efficiently guide voluntary choices.

---

## 论文详细总结（自动生成）

好的，以下是根据您提供的论文内容生成的结构化、深入、客观的中文总结。

---

### 1. 论文的核心问题与整体含义

-   **研究动机与背景**：适应性行为要求大脑将连续性的、对选项价值的评估（“这个选项多好？”）转化为离散的、对特定行动的承诺（“选这个！”）。这一转化的神经回路基础是系统神经科学的核心问题。
-   **核心问题**：大脑中负责评估和负责承诺的神经信号是存在于同一区域，还是由不同的大脑通路分而治之？具体来说，平行投射到视上丘的基底神经节输出（黑质网状部，SNr）和额叶皮层输出（额叶眼动区，FEF）在这一过程中分别扮演什么角色？
-   **整体含义**：本研究提供了关键证据，表明这种转化并非发生在一个单一脑区，而是通过基底神经节（SNr）和额叶皮层（FEF）的平行通路进行分工协作。SNr主要携带基于选项在情境中的相对重要性的、依赖情境的评估信号，而FEF则主要携带决定“做还是不做”以及“往哪里做”的类别承诺信号。两者在视上丘汇聚，共同指导最终的行动选择。

### 2. 论文提出的方法论

-   **核心思想**：设计一个能够部分分离“情境定义的序数排名（Ordinal Rank，即当前选项在场景中是相对较好还是较差）”和“类别性承诺（Categorical Commitment，即接受或拒绝该选项）”的行为任务。通过记录两个脑区的神经元活动，分析它们对不同变量的编码差异。
-   **关键技术细节**：
    1.  **任务设计**：猴子执行一个“顺序提供选择任务”（Sequential-offer choice task）。
        -   **场景（Scene）**：背景图像定义了当前可用的两个对象（如场景1：对象A vs. B，场景3：对象B vs. C）。
        -   **序数排名**：在每个场景内，奖励更高的对象定义为“好”（Good），奖励较低的定义为“坏”（Bad）。同一对象在不同场景中的排名可以不同（如对象B在场景1中是“坏”，在场景3中是“好”）。
        -   **做出选择**：猴子可以通过注视目标物体来接受（Accept）一个提议，也可以通过主动将目光移回注视点来拒绝（Reject）。后者定义了一种主动的运动行为，而非“无动作”状态。
    2.  **神经记录**：在三只猴子执行任务时，使用微电极记录其**SNr**（黑质网状部，基底神经节输出）和**FEF**（额叶眼动区，额叶皮层输出）的单个神经元活动。
    3.  **量化分析方法**：
        -   **线性混合效应模型 (LMM)**：用于量化场景信息、行为结果等变量对神经活动的影响大小。
        -   **多变量线性混合效应模型**：同时纳入“行动（Action，接受/拒绝）”、“排名（Rank，好/坏）”、“奖励量”、“目标方向”和“反应时”作为固定效应，剥离出每个变量的独立贡献。
        -   **行为模型分解**：构建逻辑回归模型（包含“奖励量”、“场景价值差”、“之前拒绝次数”、“序数排名”等变量）预测猴子的选择行为，并从中提取一个连续性的“可接受性评分（Margin）”变量。然后用这个Margin和离散的“行动”变量分别去解释神经活动。
-   **算法/模型流程（文字描述）**：
    1.  **提取行为变量**：对每个提议，记录其“场景ID”、“对象ID”、“实际行为（接受/拒绝）”、“序数排名（好/坏）”、“反应时”等。
    2.  **行为建模**：用逻辑回归模型拟合猴子的选择行为，找出最佳预测模型（M4），并从该模型中得到每个提议的“Margin”值。
    3.  **神经响应量化**：对每个神经元的放电率进行z-score标准化。
    4.  **回归分析（神经VS变量）**：使用LMM分析神经活动与“行动”、“排名”、“奖励量”、“目标方向”、“Margin”等变量之间的关系。
    5.  **模型比较**：通过AIC（赤池信息量准则）比较不同模型（如“排名”模型、“行动”模型、“Margin”模型）对神经活动的解释能力。

### 3. 实验设计

-   **数据集与场景**：
    -   **主体**：3只雄性恒河猴（Monkey Ch, Cr, Sp）。
    -   **任务场景**：10个视觉场景，分为2类：
        -   **选择场景 (Scenes 1-6)**：每个场景定义了两个可选对象（一好一坏），猴子可以根据情境自由选择接受哪一个。
        -   **强迫选择场景 (Scenes 7-10)**：每个场景只有一个对象可用，作为对照条件。
-   **Benchmark**：实验的内隐基准是“行动模型”（Action Model），即看任何其他模型（如“排名模型”、“可接受性模型”）是否比简单地用“接受/拒绝”这个二分变量能更好地解释神经活动。
-   **对比方法**：
    -   **区域间对比**：比较SNr和FEF在场景相关调制、目标评估时的活动模式上的差异。
    -   **变量间对比**：在同一脑区内，比较“排名（Rank）”、“行动（Action）”、“奖励量（Reward amount）”、“目标方向（Direction）”、“可接受性评分（Margin）”等变量对神经活动的解释力。
    -   **模型对比**：在行为层面比较不同逻辑回归模型（M0-M4）对行为的预测能力；在神经层面比较包含不同变量的LMM模型。

### 4. 资源与算力

-   论文中**没有明确提及**使用了何种型号的GPU、数量以及训练时长。分析主要依赖标准的数据处理库（如MATLAB, R, Python的statsmodels)在常规服务器或个人工作站上进行，未涉及大规模深度学习模型训练。

### 5. 实验数量与充分性

-   **记录神经元数量**：共记录了91个SNr神经元和99个FEF神经元。每个神经元对应一个完整的记录会话。
-   **实验组数量**：研究进行了多组核心分析：
    -   **场景-周期分析**：比较SNr和FEF在不同场景下的基线活动。
    -   **目标-周期分析**：比较两种脑区在“接受好选项”、“接受差选项”、“拒绝差选项”三种行为结果下的活动模式。
    -   **多变量模型分析**：量化“排名”、“行动”、“奖励量”、“方向”等变量的独立贡献。
    -   **行为模型分析及神经模型比较**：验证“排名”是解释SNr活动的最佳变量。
    -   **单神经元分类**：根据神经元对不同变量的编码强度进行分类。
-   **充分性与公平性评估**：
    -   **充分性**：实验非常充分。所有关键分析均在三个单猴数据和群体数据中复现，确保了结果的可重复性。使用了多种互补的分析方法（LMM, 单神经元分类, 行为模型分解），从不同角度印证了核心结论。
    -   **客观与公平**：实验设计精巧，通过“接受差选项”和“主动拒绝选项”的设计，巧妙地将“评估”与“行动准备”部分分离。通过多变量模型控制住了变量间的共线性问题。通过仿真分析（Simulation recovery）验证了使用AIC区分“连续性”和“类别性”神经信号的可靠性，增强了结论的说服力。

### 6. 论文的主要结论与发现

1.  **功能分离**：在目标评估阶段，SNr和FEF存在显著的功能分离。
    -   **SNr** 的活动是 **“分层的”** 或 **“有序的”**：从“接受好选项”（最低活动）到“接受差选项”（中等活动）再到“拒绝差选项”（最高活动），其活动水平呈现梯度变化。其中，序数排名（好与差）是驱动这种变化的主要因素。
    -   **FEF** 的活动是 **“分类的”** 或 **“二元的”**：其活动明确将“接受”（所有接受情况）和“拒绝”区分开，同时强烈编码目标方向。它几乎不区分所接受的是“好”还是“差”的选项。
2.  **预目标阶段**：在目标出现前，SNr就表现出比FEF更强的对当前场景信息的调制，表明基底神经节更早地编码了情境。
3.  **模型证据**：行为模型分解和神经模型比较发现，**“序数排名”**是解释SNr活动的主导变量，其解释力远超过“奖励量”甚至综合性的“可接受性评分”。**“行动类别”**则是解释FEF活动的最佳变量。
4.  **行为证据**：眼跳反应时（SRT）也支持这一结论：眼跳潜伏期与决策结果（接受/拒绝）相关性更强，而非具体的场景细节。
5.  **普适性**：以上结论在三只猴子中表现一致，表明其具有跨个体稳定性。

### 7. 优点

-   **创新的任务设计**：巧妙地将“序数排名”与“类别承诺”部分解耦，并设计了“主动拒绝”机制（主动返回），避免了传统任务中“拒绝”与“无动作”的混淆，这是分离评估与运动信号的关键创新。
-   **严谨的多层次分析方法**：结合了传统的t检验/方差分析、现代的线性混合效应模型、行为模型分解以及单神经元分类，形成了一个从宏观到微观的完整证据链，论证非常严密。
-   **高度的内部一致性**：所有分析（群体响应、多变量模型、单神经元分类）在不同猴子和脑区间的结果完全一致，结论非常稳健。
-   **理论贡献明确**：不仅发现了现象，还提出了一个清晰的回路模型——评价（SNr）与承诺（FEF）在平行通路中分工，并汇聚于视上丘。为理解认知-运动转化提供了新框架。
-   **方法验证**：通过仿真模拟验证了AIC模型比较方法区分不同信号类型（连续vs.分类）的能力，增加了结果的可靠性。

### 8. 不足与局限

-   **相关性而非因果性**：研究基于神经活动记录，属于相关性证据。作者在讨论中也明确指出，需要未来的因果性扰动实验（如光遗传、药物失活）来验证SNr和FEF在评估和承诺中的必要作用。
-   **未同时记录**：研究分别记录了SNr和FEF的神经元，没有在同一时间点对两个脑区及下游视上丘进行同步记录。这限制了直接观察两种信号如何在视上丘汇聚和整合的细节。
-   **场景周期分析的局限性**：对于场景前的活动，作者承认未能在实验设计中完全分离“场景视觉特征”和“情境定义”的影响，因此对该阶段的信号解读较为保守。
-   **神经元选择偏差**：纳入分析的神经元是基于其对目标刺激有反应筛选出来的，可能不代表整个SNr或FEF的完整神经元群体，尤其是在场景周期的活动中可能存在样本偏差。
-   **生态效度有限**：实验任务是人为设计的简单视觉-眼动任务，其结论是否能推广到更复杂的、涉及多感官和连续动作的自然决策环境，仍需进一步验证。

（完）
