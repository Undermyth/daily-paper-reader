---
title: Efficient Learning of Predictive Maps for Flexible Planning
title_zh: 高效学习预测地图以实现灵活规划
authors: "Bazarjani, A., Piray, P."
date: 2026-06-22
pdf: "https://www.biorxiv.org/content/10.64898/2026.02.11.705395v2.full.pdf"
tags: ["query:comp-neuro"]
score: 9.0
evidence: 使用重要性采样的后继表示，获得策略无关的预测地图
tldr: 认知地图使灵活行为成为可能，但现有继代表征因策略依赖限制了规划能力。本文提出SR-IS模型，结合时序差分学习与重要性采样，构建策略无关的预测地图，能高效更新环境变化。实验表明SR-IS在规划任务中优于现有模型，并解释了人类重规划中的分级偏差。该工作桥接了预测地图理论与灵活决策行为。
source: biorxiv
selection_source: fresh_fetch
motivation: 现有预测地图模型策略依赖性强，难以实现灵活规划与快速适应环境变化。
method: 结合时序差分学习与重要性采样，构建策略无关的继代表征模型SR-IS。
result: SR-IS在规划任务中优于现有模型，并解释了人类重规划中以往模型无法解释的分级偏差。
conclusion: 本研究桥接了预测地图理论与规划行为，为理解大脑灵活决策机制提供了新视角。
---

## 摘要
认知地图通过提供可重复使用的任务结构内部表征来实现灵活行为。继任表征作为一种预测地图，编码了预期的未来状态占用，已被提出是大脑中计算此类地图的一种方式，但其策略依赖性严重限制了灵活规划。我们引入了一个新模型——带重要性采样的继任表征（SR-IS），它将时序差分学习与重要性采样相结合，以构建策略无关的预测地图。SR-IS学习环境的结构而不受智能体当前决策策略的约束。当环境发生变化时，这些表征能够高效更新，从而实现快速的行为适应。我们表明，SR-IS在规划任务中优于现有模型，并更好地解释了先前模型无法解释的人类重新规划中的分级偏差。这项工作将预测地图理论与观察到的规划行为联系起来，为大脑中的灵活决策提供了新的见解。

## Abstract
Cognitive maps enable flexible behavior by providing reusable internal representations of task structure. The successor representation, a predictive map that encodes expected future state occupancy, has been proposed as one way such maps might be computed in the brain, but its policy dependence severely limits flexible planning. We introduce a new model, the successor representation with importance sampling (SR-IS), which combines temporal-difference learning with importance sampling to construct policy-independent predictive maps. SR-IS learns the structure of the environment without being constrained by the agents current decision policy. These representations can be efficiently updated when the environment changes, enabling rapid behavioral adaptation. We show that SR-IS outperforms existing models in planning tasks and provides a better account of the graded biases in human replanning that previous models could not explain. This work bridges theories of predictive maps with observed planning behavior and offers new insights into flexible decision-making in the brain.

---

## 论文详细总结（自动生成）

### 1. 论文的核心问题与整体含义（研究动机和背景）

- **核心问题**：如何构建**策略无关**的预测地图，使其既能通过经验高效学习，又能在目标和环境变化时保持灵活性。现有后继表征（SR）依赖具体决策策略，灵活规划能力差；而线性 RL 中的默认表示（DR）虽灵活但缺乏高效的在线学习算法。
- **整体含义**：提出一种结合时序差分（TD）学习与重要性采样的新模型 SR-IS，能够从带有策略偏差的体验中学习到策略无关的表示，从而同时实现**高效的缓存式规划**和**灵活的任务适应**，并为人类重规划中的分级偏差提供统一的规范性解释。

### 2. 论文提出的方法论

- **核心思想**：利用重要性采样纠正 SR 学习中的策略偏差，使 TD 更新目标转向默认策略下的预测地图。
- **关键技术细节**：
  - 定义默认策略 π_d（通常为均匀分布）和目标策略 π（当前决策策略）。
  - 在状态转移后，使用重要性权重 w(s,s′) = π_d(s′|s) / π(s′|s) 加权 TD 更新：
    ```
    M(s,:) ← (1-α) M(s,:) + α [1_s^T + γ M(s′,:)] w(s,s′)
    ```
  - 学习得到的矩阵 M 收敛于默认表示（DR），即默认策略下的后继矩阵。
  - 结合线性 RL 框架的低秩更新公式（Woodbury 引理），可在环境变化（如新增障碍或目标）时高效更新 M，仅需对局部变化状态进行矩阵运算。
- **算法流程**：
  1. 智能体与马尔可夫决策过程（MDP）环境交互，依据当前策略 π 选择动作。
  2. 经历状态转移 s → s′ 并获得奖励。
  3. 计算重要性权重 w = π_d(s′|s)/π(s′|s)。
  4. 执行带权重的 TD 更新（上式）。
  5. 利用学习到的 M 和线性 RL 公式计算状态值，并通过 softmax 策略选择动作。
  6. 环境变化时，使用 Woodbury 引理对 M 进行低秩更新。

### 3. 实验设计

- **实验场景**：
  - **四房间迷宫**：验证 SR-IS 的收敛性（与完全矩阵求逆计算的 DR 对比）及跨房间重规划能力。
  - **复杂迷宫**：测试首次训练后对新目标（非初始终止状态）的重规划性能。
  - **策略重评价任务**（Russek et al. 2017）：检验 SR-IS 能否在奖励变化后切换偏好。
  - **人类重规划实验**（Momennejad et al. 2017）：包含奖励重评价、策略重评价、转移重评价三种条件，考察行为灵活性的不对称性。
  - **两步决策任务**（Kahn & Daw 2024）：区分模型基础和 SR 签名的行为分析。
  - **大鼠与人类导航轨迹**（de Cothi et al. 2022）：Tartarus 迷宫，跨物种比较。
  - **随机转移环境**：演示 SR-IS 在随机性下的失败案例。
- **基准与对比方法**：
  - 标准 SR（无重要性采样）
  - 完全 DR（通过矩阵求逆，作为最优参考）
  - 模型基础（MB）RL
  - 模型自由（MF）RL
  - 混合 SR+MB 模型
  - 线性 RL 完全模型（部分实验中作为“Complete”）

### 4. 资源与算力

- **文中未明确提及**使用的 GPU 型号、数量或训练时长。仅说明代码使用 Python、MATLAB、Julia 编写，模型比较通过贝叶斯选择实现。推测使用常规 CPU 或单 GPU 即可完成模拟，未涉及大规模分布式训练。

### 5. 实验数量与充分性

- **实验数量**：论文包含约**7组主要实验**（收敛性、跨房间重规划、复杂迷宫重规划、策略重评价、人类重规划不对称性、两步决策任务、导航轨迹拟合），每个实验均在不同随机种子下重复（10-800次）。
- **充分性**：
  - 实验覆盖了多种经典和新型任务场景，对比了多种基线模型。
  - 对人类数据进行了正式的模型比较（受保护超越概率），在两步任务和导航数据中均表现最优。
  - 消融实验有限（如未单独分析重要性权重的作用或不同默认策略的影响），但核心对比—有无重要性采样—已在收敛和重规划实验中展示。
- **公平性**：所有模型均在尽量一致的超参数下运行（γ、α、β、λ 等，文中固定值或合理范围），并通过拟合和贝叶斯选择比较，方法相对客观。

### 6. 论文的主要结论与发现

- SR-IS 通过重要性加权的 TD 更新，可以收敛到策略无关的默认表示（DR），且在线学习。
- 在重规划任务中，SR-IS 显著优于标准 SR，尤其在跨区域规划时保持高效，接近完全 DR 的性能。
- SR-IS 能够解释人类重规划中的**分级不对称性**（奖励重评价更容易，策略/转移重评价更困难），而纯 MB 或纯 SR 均无法解释；其解释不需要混合两个系统，仅源于重要性采样的方差特性。
- 在大鼠和人类导航轨迹的最大似然分析和模型比较中，SR-IS 均获得最高支持率（受保护超越概率 72%-89%）。
- SR-IS 继承了线性 RL 的低秩更新优势，可高效适应环境变化。
- 在随机转移环境中，SR-IS 因假设完全可控而出现乐观偏差，可作为未来实证检验的**区分性预测**。

### 7. 优点

- **方法简洁高效**：仅需在标准 SR 的 TD 更新中引入重要性权重，不增加算法复杂度，保留了在线学习的实用性。
- **统一解释性**：用单一机制（重要性采样的方差）解释了原本需要混合双系统（SR+MB）才能拟合的行为模式，提供了规范性理论。
- **灵活性与效率兼得**：既能利用缓存规划加速决策（如 SR），又能像 MB 一样适应目标和结构变化。
- **与线性 RL 框架无缝衔接**：继承了其低秩更新和最优值近似等优点。
- **跨物种验证**：在人、大鼠、模拟环境中均表现良好，增强了模型的生物学合理性。
- **代码公开**：提供完整仓库，便于复现和扩展。

### 8. 不足与局限

- **策略非零覆盖假设**：要求决策策略对所有可能动作赋予非零概率，贪婪策略无法工作，限制了在极端偏好场景下的应用。
- **确定性转移假设**：在随机环境中（如两步随机任务）会产生乐观偏差，无法应对真正的随机性。
- **方差问题**：当默认策略下的常见状态被决策策略很少访问时，重要性采样方差大，学习不稳定，导致性能下降（如策略重评价中的轻微偏差）。
- **控制成本参数固定**：未考虑动态调整控制成本以适应任务需求（如从探索转向利用），限制了模型对个体内变异的解释。
- **规模限制**：实验主要在小型迷宫和有限状态空间中进行，未测试大规模连续控制或高维状态任务（如 Atari）。
- **神经生物学验证不足**：虽然引用了大量神经科学文献，但未直接比较神经数据（如海马体或内嗅皮层的活动模式）。
- **参数敏感性分析欠缺**：仅说明固定参数（如 α=0.05，λ=β=1），未详细分析这些参数对结果的影响。

（完）
