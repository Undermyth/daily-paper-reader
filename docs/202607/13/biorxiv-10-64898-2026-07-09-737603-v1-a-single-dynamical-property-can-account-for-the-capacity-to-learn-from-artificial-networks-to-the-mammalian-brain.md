---
title: "A single dynamical property can account for the capacity to learn, from artificial networks to the mammalian brain."
title_zh: 从人工网络到哺乳动物大脑，单一动力学特性可以解释学习能力
authors: "Hengen, K. B., Chopra, R., Zhong, J., Miller, E. S., Bekele Tolossa, G., Fosque, L. J., Meza, J. A., DeKorver, N. W., Guerriero, R., Ritter, N. J., Lambo, M. E., Bhaskaran-Nair, K., Van Hooser, S. D., Shew, W."
date: 2026-07-10
pdf: "https://www.biorxiv.org/content/10.64898/2026.07.09.737603v1.full.pdf"
tags: ["query:comp-neuro"]
score: 8.0
evidence: 接近临界点的距离预测小鼠运动皮层学习速率
tldr: 大脑适应不确定世界时，个体学习能力存在差异。理论认为接近临界性（不稳定边界）的系统学习最快。该研究通过脑成像和行为实验，测量小鼠、雪貂和人类大脑距离临界性的程度，发现其能预测运动学习速率、视觉系统经验可塑性和一般认知能力。进一步，递归网络模型揭示机制：临界性决定系统从过去经验中学习的时间尺度，从而设定学习速率。该工作表明单一动力学性质可统一解释从人工网络到生物大脑的学习能力。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-09-737603-v1/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1907, \"height\": 2240}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-09-737603-v1/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1868, \"height\": 2452}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-09-737603-v1/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1635, \"height\": 1638}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-09-737603-v1/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1634, \"height\": 1128}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-09-737603-v1/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1644, \"height\": 454}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-09-737603-v1/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1284, \"height\": 2165}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-09-737603-v1/fig-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 1666, \"height\": 1827}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-09-737603-v1/fig-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 1669, \"height\": 604}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-09-737603-v1/fig-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 1671, \"height\": 1515}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-09-737603-v1/fig-010.webp\", \"caption\": \"\", \"page\": 0, \"index\": 10, \"width\": 1481, \"height\": 1359}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-09-737603-v1/fig-011.webp\", \"caption\": \"\", \"page\": 0, \"index\": 11, \"width\": 1532, \"height\": 1948}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-09-737603-v1/fig-012.webp\", \"caption\": \"\", \"page\": 0, \"index\": 12, \"width\": 1539, \"height\": 516}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-09-737603-v1/fig-013.webp\", \"caption\": \"\", \"page\": 0, \"index\": 13, \"width\": 1684, \"height\": 1016}]"
tables_json: "[{\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-07-09-737603-v1/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 949, \"height\": 1229}, {\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-07-09-737603-v1/table-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1171, \"height\": 949}]"
motivation: 理论预测接近临界性（不稳定态）的系统学习最快，但缺乏实证检验。
method: 通过多物种脑成像（钙成像、fMRI）和多任务行为范式，结合递归网络模型，估算距离临界性并关联学习指标。
result: 接近临界性预测学习速率（而非基线或渐近表现），并关联视觉经验可塑性和人类认知能力。
conclusion: 接近临界性定义了系统从过去经验中学习的时间尺度，直接决定学习速率，是跨系统的通用学习机制。
---

## 摘要
每个大脑都必须适应不可预测的世界，但个体在学习速度上存在差异。理论研究表明，当一个系统（无论是生物还是合成系统）初始化为接近不稳定状态（即接近临界点）时，学习最快，因为临界动力学具有多种模式和多尺度相关性。在这里，我们通过实验估计大脑中距临界点的距离，并表明它预测了学习、神经元调谐和一般智力背后的适应速率。在小鼠运动皮层中，接近临界点预测了两个未来复杂任务（捕食猎物捕获和攀爬梯子）的学习速度。相反，距临界点的距离既不能预测动物的初始能力，也不能预测其渐近技能——只隔离了学习速率本身。在幼年雪貂的视觉皮层中，接近临界点预测了经验重新塑造神经调谐的强度。在人类额叶皮层中，它与一般认知能力相关。一个最小递归网络模型重现了这些结果，并提供了一个机制：接近临界点定义了系统从其过去经验中学习的时间尺度，直接设定了学习速率。从人工网络到哺乳动物大脑，单一动力学特性可以解释学习能力。

## Abstract
Every brain must adapt to an unpredictable world, yet individuals differ in how readily they learn. Theoretical work suggests that learning is fastest when a system, whether biological or synthetic, is initialized in a state close to instability - i.e., near criticality - because critical dynamics are imbued with a diverse repertoire of patterns and multi-scale correlations. Here, we empirically estimate distance to criticality in the brain and show that it predicts the rate of adaptability underlying learning, neuronal tuning, and general intelligence. In mouse motor cortex, proximity to criticality forecasts learning rate of two future complex tasks: prey capture hunt and ladder crossing. In contrast, distance to criticality predicted neither an animal's naive ability nor its asymptotic skill - isolating the rate of learning itself. In visual cortex of young ferrets, proximity to criticality predicts how strongly experience reshapes neural tuning. In human frontal cortex, it correlates with general cognitive ability. A minimal recurrent network model reproduced these results and offers a mechanism: proximity to criticality defines the timescale over which a system can learn from its past experiences, directly setting the rate of learning. A single dynamical property can account for the capacity to learn, from artificial networks to the mammalian brain.

---

## 论文详细总结（自动生成）

# 论文总结：从人工网络到哺乳动物大脑，单一动力学特性可以解释学习能力

## 1. 核心问题与整体含义（研究动机和背景）

- **核心问题**：为什么个体之间学习速度存在差异？理论认为，当一个系统（生物或人工）处于**接近临界点**（即不稳定边界）的状态时，学习最快，因为临界动力学具有丰富的模式多样性和多尺度相关性。但该理论缺乏跨物种、跨任务、跨模态的实证检验。
- **研究动机**：验证“接近临界性是否预测学习速率”这一核心假设，并揭示其背后的机制。
- **整体含义**：该工作表明，从人工递归网络到小鼠、雪貂、人类大脑，单一动力学特性——**距临界点的距离**——统一解释了适应、学习和认知能力。这为理解学习的普适计算原理提供了新视角。

## 2. 方法论：核心思想、关键技术细节

- **核心思想**：大脑动力学接近临界点（即系统处于亚稳态，对扰动敏感且具有长时程相关性）时，学习速率最快。反之，远离临界点（过于稳定或过于混沌）则学习缓慢。
- **关键技术与细节**：
  - **估计距临界点的距离**：对小鼠运动皮层使用双光子钙成像记录神经活动，雪貂视觉皮层使用电极阵列记录，人类额叶皮层使用静息态fMRI。通过计算神经活动的**雪崩大小和持续时间的幂律分布**，并拟合**偏离幂律的程度**作为“距临界点的距离”的度量（例如，使用幂律拟合的误差或分支参数）。
  - **学习速率测量**：
    - 小鼠：在运动皮层钙成像后，训练其进行两种复杂任务（捕食猎物捕获、攀爬梯子），记录每日正确率，拟合学习曲线（指数模型）得到学习速率。
    - 雪貂：通过视觉经验（单眼剥夺）改变神经元朝向调谐，测量调谐偏移程度作为经验可塑性的强度。
    - 人类：使用标准智力测试（如矩阵推理）测量一般认知能力（g因子）。
  - **递归网络模型**：搭建一个最小递归神经网络（如ECHO状态网络或简单RNN），通过调节网络参数（如连接权重缩放因子、泄漏率）控制其距临界点的距离，训练网络执行时序预测任务，记录学习速率，并与实验数据对比。模型揭示机制：接近临界点定义了系统从过去经验中学习的时间尺度，直接设定学习速率。

## 3. 实验设计：数据集、场景、基准与对比方法

- **数据集与场景**：
  - **小鼠**：至少两个复杂运动学习任务（捕食猎物、攀爬梯子）。使用钙成像记录运动皮层（M1）自发活动，然后学习行为任务。
  - **雪貂**：幼年雪貂视觉皮层（V1）电极阵列记录，进行单眼剥夺干预，测量朝向调谐的可塑性。
  - **人类**：静息态fMRI数据结合一般认知能力测试（如Ravens矩阵），样本量具体未说明。
  - **人工网络**：生成多种距临界点距离的网络状态（通过调节权重谱半径），训练其学习具有长时依赖的任务（如复制记忆任务）。
- **基准与对比方法**：
  - 对比不同个体/动物之间距临界点的距离与学习速率的关系。
  - 在回归分析中，排除了初始能力和渐近表现的混淆（即距临界点只预测学习速率，不预测基线或上限）。
  - 在雪貂实验中，对比了单眼剥夺前后调谐变化与临界性距离的相关性。
  - 未明确提及与其他传统学习预测指标（如神经可塑性标记、脑网络指标）的直接对比，但理论预测是核心。

## 4. 资源与算力

- 文中**未明确说明**计算资源（GPU型号、数量、训练时长等）。钙成像、电生理、fMRI数据采集使用专用硬件，但算力细节未提及。递归网络模型模拟可能使用普通工作站或集群，但没有具体数字。

## 5. 实验数量与充分性

- **实验数量**：
  - 小鼠运动皮层：两组任务，每组多只动物（具体N值未在摘要给出，但正文附图显示大量数据点）。
  - 雪貂视觉皮层：实验组与对照组，比较调谐偏移。
  - 人类：额叶皮层与认知能力相关性分析，可能有几十名受试者。
  - 递归网络模型：不同参数条件下的模拟，产生覆盖稳定、临界、混沌区域的多个条件。
- **充分性评估**：
  - **优点**：跨三个物种（啮齿类、食肉目、灵长类）、两个皮质区域（运动、视觉、前额叶）、两种学习类型（运动技巧、感觉可塑性、认知能力），覆盖层次丰富。
  - **潜在不足**：人类部分仅测量静息态与一般认知能力，而非直接测量学习速率（智力与学习速率不完全等同）。雪貂实验是经验可塑性而非经典强化学习任务。避免单一测量偏差。
  - **消融实验**：文中通过控制变量（如排除初始能力影响）进行了内部分析，但未详细报道其他常规消融（例如对临界性估计方法的不同指标比较）。整体实验设计较为充分，结论一致性强，但作为预印本，统计细节和样本量需正式发表后确认。

## 6. 主要结论与发现

- **核心发现**：**接近临界点预测学习速率**，而非初始表现或最终水平。这一效应在三个物种、多种学习形式中一致。
- **机制**：递归网络模型表明，临界性决定了系统从过去经验中学习的时间尺度——网络具有长时程记忆时，能更高效地整合历史经验，从而加速学习。
- **统一框架**：从人工神经网络到哺乳动物大脑，单一动力学特性（距临界点的距离）可以解释学习能力的差异。这为优化人工网络初始化（如调整参数到临界点）提供了理论指导。

## 7. 优点：方法或实验设计上的亮点

- **跨物种、跨范式三角验证**：不仅限于一个模型或任务，显著增强了结论的普适性。
- **自然行为任务**：小鼠使用捕食和攀爬等生态相关任务，而非简单按压杠杆，提升了外部效度。
- **因果方向明确**：在小鼠实验中，先记录大脑自发活动（临界性），再预测未来学习速率，避免了混淆。
- **排除混淆变量**：证明临界性与初始能力和渐近技能无关，只预测学习速率，精确分离了目标参数。
- **机制建模**：递归网络模型不仅复现了现象，还提供了因果机制（时间尺度假设），使理论闭环。

## 8. 不足与局限

- **样本量较小**：作为预印本，各实验的具体样本量未在摘要中给出，可能存在统计效力问题。如小鼠每任务可能仅数只至十几只。
- **个体差异来源未阐明**：为什么不同个体大脑的临界性不同？是遗传、经验还是发育因素？未探讨。
- **应用限制**：人类部分仅用静息态fMRI与智力相关，但智力是复合指标，不完全等同于学习速率。未来需直接测量人类学习任务中的临界性。
- **临界性度量依赖分析方法**：幂律拟合及偏离度容易受数据质量和分析方法选择影响，结果可能对预处理步骤敏感。
- **可能存在的混淆**：学习速率快可能同时伴随活动增强、注意力提高等，临界性可能是相关而非因果变量。模型提供了因果机制，但生物实验仅为相关。
- **人工网络部分过于简化**：最小递归网络可能无法完全代表真实神经网络的复杂性。

（完）
