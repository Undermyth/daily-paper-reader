---
title: Coordination of turn-related activity in the superior colliculus with locomotor dynamics and hippocampal representations of possible futures
title_zh: 上丘中与转向相关的活动与步态动力学及海马体对未来路径的表征之间的协调
authors: "Wilhite, C., Frank, L. M., Scanziani, M."
date: 2026-06-16
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.12.731955v1.full.pdf"
tags: ["query:comp-neuro"]
score: 9.0
evidence: 海马表征可能的未来路径；导航与转向活动
tldr: 动物转向需与步态精确协调并依赖未来路径规划。上丘是中脑转向关键脑区，但其活动是否与步态节律及海马未来表征协调未知。本研究在小鼠Y迷宫导航中同步记录上丘转向细胞、步态动力学及海马神经活动，发现转向细胞发放严格锁定于步态节律，且其调制与海马未来路径表征动态协调。这一机制揭示了运动控制与认知规划在脑内的协同基础，使动物能流畅执行转向并导向目标。
source: biorxiv
selection_source: fresh_fetch
motivation: 探究上丘转向细胞活动是否与步态节律及海马未来路径表征相协调，以揭示运动与认知的整合机制。
method: 在小鼠Y迷宫任务中，同步记录上丘运动层转向细胞发放、步态动力学及海马神经活动，并解码未来路径表征。
result: 上丘转向细胞活动紧密锁定于步态节律，且其幅度调制与海马未来路径表征的变化相协调。
conclusion: 该多脑区协调机制使动物能在运动中流畅转向，导向计划目的地，揭示了运动控制与认知规划的神经基础。
---

## 摘要
左转或右转是动物导航的核心元素。这种转向与持续的迈步节律精确协调，并需要对动物未来路径进行内部规划。上丘（SC）是中脑参与转向的结构。上丘中与转向相关的活动是否与迈步和未来路径的内部表征相协调尚不清楚。在这里，我们从小鼠在Y迷宫导航时记录上丘运动层中偏好左或右的“转向细胞”，监测步态动力学，并从海马体解码未来路径的内部表征。我们发现，转向细胞的活动紧密锁相于迈步节律，并与海马体对未来路径的表征协调调制。上丘中与转向相关的活动与迈步和未来路径的内部表征的协调，可能使动物在朝向计划目的地导航时能够无缝地执行转向。

## Abstract
Turning left or right is a core element of animal navigation. Such turns occur in precise coordination with the ongoing stepping rhythm and require internal planning for the animals future path. The superior colliculus (SC) is a midbrain structure involved in turning. Whether turn-related activity in the SC is coordinated with stepping and internal representations of future paths is unknown. Here, while recording from left- or right-preferring "turn cells" in the motor layers of the SC as mice navigated a Y-maze, we monitored locomotor dynamics and decoded internal representations of future paths from the hippocampus. We discovered that turn cell activity was tightly phase-locked to the stepping rhythm and modulated in coordination with hippocampal representations of future paths. The coordination of turn-related activity in the SC with stepping and internal representations of future paths may allow animals to seamlessly execute turns during locomotion while navigating toward planned destinations.

---

## 论文详细总结（自动生成）

### 1. 论文的核心问题与整体含义

- **研究动机与背景**：动物在导航中需要精准协调转向与步态节律，并依靠内部认知表征规划未来路径。上丘（SC）的中深层（dSC）含有编码转向方向的“转向细胞”，但其在自由运动中的活动是否同时与步态节律和认知规划（如海马体对未来路径的表征）相协调，尚不清楚。
- **整体含义**：本研究首次揭示上丘转向细胞的发放既紧密锁相于步态相位，又受海马体未来路径表征的调制，表明运动执行与认知规划在脑内高度整合，使动物能在运动中无缝执行转向并导向预定目标。

### 2. 论文提出的方法论

- **核心思想**：在小鼠执行Y迷宫转向任务时，同步记录dSC神经元电活动、通过头部‑身体角度（head‑body angle）推断步态节律，并利用海马CA1区群体神经活动解码动物对未来路径的内部表征（“海马扫视”，hippocampal sweeps）。
- **关键技术细节**：
  - **转向细胞识别**：计算转向方向选择性指数（Turn Direction Selectivity Index, TDSI），选取在Y迷宫分岔口对不同转向有显著偏好且一致性跨臂的神经元。
  - **步态相位估计**：通过头顶摄像头追踪头部‑身体角度振荡（~5.5 Hz），利用Hilbert变换提取瞬时相位，以此作为步态节律的代理。验证了小鼠中左右前肢摆动与头部侧向运动的对应关系。
  - **海马扫视检测**：采用Denovellis等（2021）的状态空间解码算法，从CA1群体发放中实时解码线性位置，识别解码位置偏离实际位置至少15 ms并进入另一臂的事件，分为同位扫视（与即将转向同向）和对位扫视（相反方向）。
  - **统计分析**：使用Rayleigh检验评估相位锁定；利用广义线性模型（GLM，泊松回归）量化海马扫视在特定θ节律循环中对dSC转向细胞后续发放的预测能力；通过置换检验确定显著性。
- **公式/算法流程**：未使用复杂公式，主要依赖指数型指标（TDSI、SDSI）和二元回归模型。核心流程为：行为分段 → 神经元分类 → 相位对齐 → 扫视检测 → GLM预测 → 行为偏差量化。

### 3. 实验设计

- **数据集/场景**：12只C57BL/6J小鼠在Y迷宫（臂长45 cm，宽5 cm）中执行空间导航任务。任务包含多个未提示区块，每区块两个奖励端口，动物需交替往返，产生大量左/右转。
- **基准与对比**：无公开基准数据集。研究主要对转向细胞进行自身对照分析（如左右转向细胞相位对比、扫视方向选择性对比、有无扫视试次对比），并采用置换检验与shuffle控制评估统计显著性。
- **方法对比**：未与其他脑区或模型对比；主要将dSC转向细胞特性与已有文献中运动命令神经元特征进行定性比较。

### 4. 资源与算力

- **计算资源**：文中未明确说明使用的GPU型号、数量或训练时长。spike sorting使用了Kilosort 2.0（通常可运行于GPU），但具体配置未提及。解码算法及GLM分析均在CPU上执行。整体算力需求中等，未给出量化信息。

### 5. 实验数量与充分性

- **实验组数**：
  - 12只动物，共55个session，记录到1471个dSC神经元，其中411个转向细胞（28%）。
  - 5只动物同时记录海马CA1（2642个细胞）和dSC，获得167个转向细胞与海马数据。
  - 步态分析包含2只小鼠在透明直线轨道上的验证实验。
  - GLM分析涉及42个扫视选择性转向细胞，共420个可能的预测循环（5个θ周期×42细胞×2方向）。
  - 行为轨迹偏差分析基于19个session的ROC分类。
- **充分性与客观性**：实验设计较系统，每一步均使用置换检验、Bonferroni校正、交叉验证等统计手段控制假阳性。但样本量（12只小鼠，5只含海马）中等，未涉及独立复制数据集；所有实验在同一实验室、相同任务条件下完成，可能存在生态效度局限。

### 6. 论文的主要结论与发现

1. **转向细胞特性**：dSC中约30%为“转向细胞”，多数偏好对侧转向，其方向选择性在行为分岔前约283 ms出现，表现为前运动信号。
2. **与步态节律的耦合**：约47%的转向细胞发放显著锁相于步态周期，左、右转向细胞分别在相反相位（约π/2与3π/2）放电；这种相位偏好即使在直线运动期也存在，表明转向选择性已内嵌于步态耦合模式中。
3. **与海马未来路径表征的协调**：34%的转向细胞（56/167）的发放随海马扫视方向显著变化，且TDSI与SDSI强相关（r=0.61）。在双向调制分析中，细胞在偏好扫视方向试次中发放增加，在非偏好方向试次中发放减少。
4. **海马扫视预测转向细胞活动**：GLM显示，海马扫视可在分岔前最多4个θ周期（~500 ms）显著预测dSC转向细胞在分岔时的发放，且预测周期与转向细胞方向选择性出现时间正相关（r=0.71）。反之，dSC活动不能可靠预测海马扫视。
5. **行为关联**：对位扫视试次中，动物转向轨迹更偏离直线路径，累积角速度更大；扫视存在与否及方向还影响试次持续时间和运动速度。

### 7. 优点

- **创新性整合**：首次同时记录运动命令神经元（dSC）、精细步态节律和认知表征（海马未来路径扫视），揭示了运动与认知在单一试次内的动态协调。
- **方法严谨**：使用多种互补分析（相位锁定、GLM预测、行为量化），并通过置换检验、交叉验证、多重比较校正确保结果可靠。
- **生理学关联**：将神经元活动与自然行为中的相位关系（如转向发生在步态周期的特定相位）直接挂钩，解释性强。
- **开放获取与可重复性**：论文为预印本，代码与数据可能在后续公开。

### 8. 不足与局限

- **因果关系未建立**：所有结果基于相关性，未通过光遗传/化学遗传等操作验证dSC活动对步态耦合或海马扫视的必要性/充分性。
- **样本量有限**：12只小鼠（仅5只同时记录海马），神经群体规模中等，可能限制发现的泛化性。
- **步态推断的代理性**：头部‑身体角度振荡作为步态节律的代理，虽然经直线跑道部分验证，但未同时记录肌电或力板，可能有细微误差。
- **海马扫视检测局限性**：解码算法依赖线性化位置，可能漏检短时扫视或引入假阳性；仅分析分岔前单个扫视事件，未考虑多重扫视的累积效应。
- **任务单一**：仅采用Y迷宫交替任务，未测试其他类型转向（如不同角度、有无选择冲突），也未探索不同认知负荷下的表现。
- **缺乏跨物种验证**：结论基于小鼠，能否推广到其他哺乳动物（如灵长类）需进一步确认。

（完）
