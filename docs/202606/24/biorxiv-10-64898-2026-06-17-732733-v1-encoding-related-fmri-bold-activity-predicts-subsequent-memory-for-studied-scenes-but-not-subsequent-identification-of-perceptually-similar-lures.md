---
title: "Encoding-related fMRI BOLD activity predicts subsequent memory for studied scenes, but not subsequent identification of perceptually similar lures."
title_zh: 与编码相关的fMRI BOLD活动能预测学习场景的后续记忆，但不能预测知觉相似诱饵的后续识别
authors: "Aktas, A., Srokova, S., Rugg, M."
date: 2026-06-22
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.17.732733v1.full.pdf"
tags: ["query:comp-neuro"]
score: 10.0
evidence: 海马模式分离在记忆相似性任务中的作用
tldr: 本研究使用fMRI检验了召回-拒绝假说，即相似诱饵识别依赖于对已学项目的回忆。在年轻和老年人中进行三选一MST任务，发现场景图像的编码相关BOLD活动可预测后续目标识别，但无法预测诱饵识别，与假说矛盾。物体图像无预测效应。编码效应年龄不变，与目标-诱饵区分指标稳健相关。结果挑战了当前对诱饵识别神经机制的理解。
source: biorxiv
selection_source: fresh_fetch
motivation: 检验召回-拒绝假说是否成立，即编码操作是否同时支持目标回忆和诱饵识别。
method: 使用fMRI对年轻和老年人进行三选一MST任务，通过ROI单变量和多变量分析评估编码期活动对后续记忆的预测。
result: 场景编码活动预测目标识别，但不预测诱饵识别；物体图像无显著效应。
conclusion: 诱饵识别可能不依赖对已学项目的回忆，模式分离机制与召回-拒绝不同。
---

## 摘要
模式分离被广泛认为是一种海马介导的过程，可减少相似经历记忆之间的干扰。在记忆相似性任务（MST）中，要求区分学习项目（目标）和知觉相似的诱饵，其表现通常被认为依赖于模式分离。具体而言，有人提出相似诱饵的识别依赖于一种回忆-拒绝策略，即通过检索相应的学习项目来识别诱饵。因此，根据这一假设，支持成功目标回忆和成功诱饵识别的编码操作应高度相似，因为两种记忆判断都依赖于对学习项目的后续回忆。在这里，我们使用fMRI检验了这一预测。在认知健康的年轻和年长成年人样本中，我们采用了一项三选一的MST（目标/诱饵/新），以场景和物体图像作为测试项目。通过基于感兴趣区域的单变量和多体素分析，我们评估了编码相关活动是否能预测后续记忆测试中目标和相似诱饵项目的识别。与回忆-拒绝假设相反，场景图像诱发的活动能够预测后续呈现目标的记忆表现，但不能预测相应相似诱饵的识别。对于两类物体测试项目，均未发现显著效应。场景目标的编码效应量级在年龄上不变，并且，单变量场景SME与目标-诱饵辨别性指标之间存在稳健的、年龄不变的关联。

## Abstract
Pattern separation is widely regarded as a hippocampally mediated process that reduces interference between memories of similar experiences. Performance on the Mnemonic Similarity Task (MST), where the requirement is to discriminate between studied items (targets) and perceptually similar lures, is commonly held to depend on pattern separation. Specifically, it has been proposed that similar lure identification is supported by a recall-to-reject strategy, whereby lures are identified as a result of the retrieval of the corresponding studied item. According to this proposal, therefore, the encoding operations that support successful target recollection and successful lure identification should be closely similar, since both mnemonic judgments depend upon subsequent recollection of the study item. Here, using fMRI, we examined this prediction. In samples of cognitively healthy young and older adults, we employed a three-choice MST (target/lure/new) with scene and object images as test items. Using ROI-based univariate and multivoxel analyses, we assessed whether encoding-related activity was predictive of the identification of target and similar lure items on the subsequent memory test. The activity elicited by scene images predicted memory performance for subsequently presented targets but not for corresponding similar lures, contrary to the recall-to-reject hypothesis. No effects could be identified for either class of object test items. The magnitude of the encoding effects for the scene targets was age-invariant, and, moreover, the univariate scene SMEs demonstrated a robust, age-invariant association with the target-lure discriminability metric.

---

## 论文详细总结（自动生成）

# 论文详细中文总结

## 1. 核心问题与整体含义（研究动机和背景）
- **研究动机**：检验“回忆-拒绝假说”（recall-to-reject）——该假说认为，在Mnemonic Similarity Task (MST)中，正确识别知觉相似的诱饵依赖于对相应已学项目的回忆（即模式分离的海马机制）。若此假说成立，则编码操作应同时预测后续目标识别和诱饵识别，且编码相关活动应相似。
- **整体含义**：挑战当前对MST中诱饵识别神经机制的主流理解。如果编码活动只预测目标识别而不预测诱饵识别，则说明诱饵识别可能依赖不同的（非回忆性）记忆信号（如熟悉感），从而对模式分离的经典理论提出修正。

## 2. 方法论：核心思想、关键技术细节
- **核心思想**：使用fMRI的subsequent memory effect (SME) 范式，比较编码期BOLD活动在后续不同记忆结果之间的差异。
- **关键技术细节**：
  - **任务**：三选一MST（“旧”、“相似”、“新”），包含场景和物体两类图像。
  - **分析框架**：
    - 区域兴趣（ROI）分析：场景选择性PPA（parahippocampal place area），物体选择性LOC（lateral occipital complex）。
    - **单变量SME**：计算每个条件（目标正确、诱饵正确、错误）的均值，并用池化标准差标准化（类Cohen's d），公式：`(μ_correct - μ_incorrect) / pooled_SD`。
    - **多体素模式相似性分析（PSA）**：计算同一条件内与不同条件间体素活动模式的相关系数之差，得到MV-SME指标。
  - **全脑探索性分析**：mass-univariate GLM，对比目标正确>错误，诱饵正确>错误，以及目标>诱饵。
  - **回归分析**：SME指标与目标-诱饵辨别性（TLD）的关联，控制年龄组和交互项。

## 3. 实验设计
- **数据集**：23名年轻成人（18-30岁）和24名健康老年人（65-75岁）。所有参与者完成神经心理学筛查排除认知障碍。
- **刺激**：120张场景图像和120张物体图像，其中144张（每类72张）进入后续测试。测试阶段：每类36个目标、36个诱饵、36个新项目。
- **流程**：编码期在fMRI扫描仪内进行，做“室内/室外”判断；测试期在扫描仪外进行，做“旧/相似/新”判断。
- **基准（benchmark）**：主要对比目标正确识别 vs. 诱饵正确识别的SME差异，以及年龄组间差异。
- **方法对比**：无外部对比方法，仅自身条件间比较（目标/诱饵/错误）。

## 4. 资源与算力
- **文中未明确说明**使用的GPU型号、数量、训练时长等硬件信息。仅提及MRI数据采集设备（Siemens Prisma 3T，32通道头线圈）和预处理软件（SPM12，MATLAB）。未涉及深度学习模型，因此无GPU算力需求。

## 5. 实验数量与充分性
- **主要实验组数**：
  - 行为分析：2（年龄）×2（图像类别）ANOVA，计算项目记忆和TLD。
  - fMRI ROI分析：2（年龄）×2（ROI：PPA/LOC）×2（SME指标：目标/诱饵）混合ANOVA，包含单变量和MV-SME。
  - 全脑分析：六个事件类型（目标正确/诱饵正确/错误 × 场景/物体）的GLM。
  - 回归分析：4个模型（每ROI×每SME指标）预测TLD，加年龄交互。
- **充分性评价**：实验设计较充分，覆盖关键条件（目标/诱饵/错误，场景/物体，年轻/老年）。但样本量偏小（N=47），且未报告交叉验证或效应量置信区间。部分结果（如物体SME缺失）可能受统计效力不足影响。

## 6. 主要结论与发现
- **关键发现**：
  - 场景图像的编码活动（单变量和MV-SME）显著预测后续目标识别，但不预测诱饵识别。
  - 物体图像未发现任何显著的SME。
  - 全脑分析确认场景目标SME位于PPA、OPA、MPA等场景选择性区域，且目标>诱饵差异也出现在相同区域。
  - 年龄差异小：场景目标SME无年龄组间差异，且与TLD的关联年龄不变。
  - 诱饵识别可能依赖非回忆性记忆信号（如熟悉感），与回忆-拒绝假说矛盾。
- **否定假说**：编码操作和神经机制在目标和诱饵上可分离，不支持统一的回忆依赖过程。

## 7. 优点
- **方法亮点**：
  - 使用三选一MST（而非传统二选一），允许独立分析目标识别和诱饵识别。
  - 同时采用单变量和MV-SME两种互补指标，增加结论稳健性。
  - 引入标准化效应量（类Cohen's d），便于跨条件和跨组比较。
  - 采用“留一对”ROI定义法避免循环分析。
  - 包含年龄组比较，考察老化影响。
- **实验设计优点**：严格控制参与者健康状态，使用匹配刺激列表，随机化。

## 8. 不足与局限
- **统计效力**：样本量较小（N=47），尤其错误试次少，可能降低检测SME的敏感性，尤其对物体图像。
- **实验覆盖**：仅使用场景和物体两类别，未涵盖面孔、抽象图形等；且仅健康人群，未涉及MCI/AD患者。
- **方法限制**：cross-sectional设计无法推断年龄变化（aging vs. age effects）。编码期任务为“室内/室外”判断，可能非最优编码策略。
- **偏差风险**：诱饵识别缺失SME可能源于任务设计（诱饵与目标相似度固定），或统计效力不足。作者承认无法完全排除假阴性风险。
- **应用限制**：结果仅适用于MST任务的特定版本，推广至其他范式需谨慎。

（完）
