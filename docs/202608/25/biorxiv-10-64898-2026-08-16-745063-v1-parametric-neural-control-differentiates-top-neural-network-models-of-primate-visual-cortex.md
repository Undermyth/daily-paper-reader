---
title: Parametric neural control differentiates top neural network models of primate visual cortex
title_zh: 参数化神经控制区分灵长类视觉皮层的顶级神经网络模型
authors: "Prince, J. S., Wang, B., Fel, T., Jagadeesh, A. V., Vaziri, P. A., Alvarez, G. A., Livingstone, M. S., Konkle, T."
date: 2026-08-20
pdf: "https://www.biorxiv.org/content/10.64898/2026.08.16.745063v1.full.pdf"
tags: ["query:comp-neuro"]
score: 8.0
evidence: 视觉皮层计算编码模型与参数化神经控制，属核心计算神经科学
tldr: 深度神经网络编码模型在预测视觉皮层响应上精度相近，但此相似性掩盖了模型与神经元参数化方式的差异。本文提出轴对齐特征强调，将编码轴转化为可控刺激，并对猕猴视觉皮层进行闭环实验。结果显示多数模型无法精确控制神经活动，对抗训练模型表现更优，且控制能力与输入梯度的空间频率结构相关。该方法为评估神经-模型因果对齐提供了新工具。
source: biorxiv
selection_source: fresh_fetch
motivation: 预测精度相近的模型可能未真正对齐神经元的参数化方式，需借助因果测试分辨。
method: 提出轴对齐特征强调，生成控制器刺激，在五种猕猴皮层区域进行闭环实验。
result: 模型间控制能力差异大，对抗训练模型占优，且控制能力由输入梯度的空间频率结构预测。
conclusion: 轴对齐特征强调成为评估神经-模型对齐的因果方法。
---

## 摘要
领先的深度神经网络编码模型以几乎无法区分的精度预测视觉皮层反应，这引发了强烈的推断，即这些模型已收敛到相同的、与大脑对齐的自然图像空间参数化。在这里，我们证明情况并非如此。我们引入了轴对齐特征强调，将每个模型的拟合编码轴转换为分级刺激扰动，预计这些扰动将在自然图像范围内外参数化控制神经放电。我们从十个领先的视觉模型生成了超过27,500个控制器刺激，并在针对早期、中期和高级视觉区域的闭环实验中将其呈现给五只猕猴。尽管自然图像预测性匹配，模型在使用强调刺激控制神经放电的能力上存在显著差异，揭示大多数模型编码轴未能捕捉其对应神经元的精确调谐。两个对抗训练模型表现出持续优势，尽管对抗鲁棒性在其他模型中对神经控制的预测性较弱。相反，控制更好地由输入梯度的空间频率结构预测：影响每个编码轴的像素分布。总的来说，这些结果确立了通过轴对齐特征强调进行神经控制作为一种因果方法，用于评估神经元和模型如何参数化视觉世界之间的一致性。

## Abstract
Leading deep neural network encoding models predict visual cortical responses with nearly indistinguishable accuracy, raising the strong inference that these models have converged on the same underlying brain-aligned parameterization of natural image space. Here we demonstrate that this is not the case. We introduce axis-aligned feature accentuation, which converts each model's fitted encoding axis into graded stimulus perturbations that are predicted to parametrically control neural firing within and beyond the natural-image range. We generated over 27,500 controller stimuli from ten leading vision models and presented them to five macaques in closed-loop experiments targeting early, mid-, and high-level visual areas. Despite matched natural image predictivity, models diverged strongly in their ability to control neural firing using accentuated stimuli, revealing that most model encoding axes failed to capture the precise tuning of their corresponding neurons. The two adversarially trained models showed a consistent advantage, though adversarial robustness was only weakly predictive of neural control across other models. Instead, control was better predicted by the spatial frequency structure of the input gradient: the distribution of pixels influencing each encoding axis. Overall, these results establish neural control via axis-aligned feature accentuation as a causal method to assess the alignment between how neurons and models parameterize the visual world.

---

## 论文详细总结（自动生成）

# 论文详细中文总结

## 1. 核心问题与整体含义（研究动机与背景）

- **研究背景**：当前多种深度神经网络编码模型在预测灵长类视觉皮层反应上已达到几乎无法区分的精度，这容易让人推断这些模型已经收敛到相同的、与大脑对齐的自然图像空间参数化方式。
- **核心问题**：**预测精度的高度相似是否真正意味着模型与神经元在表征参数化方式上高度一致？** 作者认为这一推断可能是错误的，预测精度相近并不能排除模型编码轴与神经元调谐方式存在实质差异。
- **整体含义**：论文试图从“预测自然图像反应”转向“因果控制神经活动”，以此检验模型编码轴是否真正对齐神经元的参数化方式，从而为神经-模型对齐提供一个更严格的评价维度。

## 2. 方法论：核心思想、关键技术细节

- **核心思想**：提出一种名为 **“轴对齐特征强调”（Axis-Aligned Feature Accentuation）** 的方法，将每个模型拟合得到的编码轴（encoding axis）转化为分级的刺激扰动。这些扰动刺激预计可以在自然图像范围之内或之外**参数化地控制神经放电率**。
- **关键技术细节**：
  - 对于每个目标神经元，先从模型中提取其对应的编码轴（即模型中对应该神经元的特征方向）。
  - 通过沿该编码轴方向对输入图像施加受控的扰动，生成“强调刺激”（accentuated stimuli），使刺激逐渐偏向或偏离该编码轴所代表的特征。
  - 刺激扰动的强度是分级的，从而产生剂量-反应式的神经控制测试。
  - 使用**闭环实验**（closed-loop）：根据实时记录到的神经响应调整后续刺激，以更精确地拟合控制曲线。
- **本质**：该方法不是用模型去预测给定自然图片的响应，而是**主动生成刺激来“操纵”神经活动**，从而检验模型编码轴是否因果性地反映神经元的真实调谐特性。

## 3. 实验设计：数据集、基准与对比方法

- **实验对象**：五只猕猴（macaques），在**闭环条件下**进行视觉刺激呈现。
- **目标脑区**：覆盖**早期、中期和高级视觉区域**（early-, mid-, and high-level visual areas）。
- **模型数量**：从 **十个领先视觉模型** 生成控制器刺激。
- **刺激规模**：共生成 **超过 27,500 个控制器刺激**。
- **对比方式**：
  - 首先比较十个模型在**自然图像预测精度**上的表现（这些模型预测精度匹配）。
  - 然后比较它们在**使用强调刺激控制神经放电**上的能力差异。
  - 额外分析了**对抗训练模型**（adversarially trained models）与其他模型的神经控制能力差异。
  - 进一步检验了**输入梯度空间频率结构**（spatial frequency structure of the input gradient，即影响每个编码轴的像素分布）对神经控制能力的预测力。

## 4. 资源与算力

- **原文未明确说明**使用的 GPU 型号、数量或训练时长等算力资源信息。
- 从摘要看，实验主要涉及刺激生成、神经数据采集与闭环控制，并未提供模型训练或在线优化的具体算力需求。因此无法基于给定文本总结具体的计算资源消耗。

## 5. 实验数量与充分性

- **实验规模较大**：27500+ 控制器刺激，5 只猕猴，10 个模型，覆盖多个视觉层级，属于较全面的因果测试。
- **多维度比较**：包括预测精度匹配下的控制能力比较、对抗训练模型与非对抗模型比较、输入梯度空间频率结构的预测性分析。
- **充分性评估**：
  - 从摘要看，实验设计具有较强的系统性和比较性，能够支撑“预测精度相近但控制能力差异大”这一核心结论。
  - 但所提供的信息中**未包含**详细的统计检验方法、刺激生成的具体参数、控制成功率的量化标准、不同脑区/神经元的样本量等细节，因此无法完全判断实验的统计功效和客观性。
  - 由于只对比了“领先模型”中的十个模型，可能不能完全代表所有视觉模型；且“控制能力”的定义和测量方式也需要更详细的描述。

## 6. 主要结论与发现

- **预测精度相近不等于模型-神经对齐**：尽管十个模型在自然图像预测上的精度几乎无法区分，但它们在用强调刺激控制神经放电的能力上存在**显著差异**。
- **大多数模型编码轴未能捕捉神经元的精确调谐**：多数模型生成的强调刺激不能可靠地控制对应神经元的放电，说明它们与神经元的参数化方式并不真正一致。
- **对抗训练模型表现持续占优**：两个对抗训练模型在神经控制上表现出明显优势。
- **对抗鲁棒性不是主要预测因子**：在其他模型中，对抗鲁棒性与神经控制能力只有较弱的关联。
- **输入梯度的空间频率结构才是关键**：神经控制能力更好地由输入梯度的空间频率结构预测，即“影响每个编码轴的像素分布”决定了该编码轴是否能驱动对应的神经元。
- **方法学贡献**：轴对齐特征强调可以作为一种**因果评价工具**，用于评估神经元与模型如何参数化视觉世界的对齐程度。

## 7. 优点：方法与实验设计的亮点

- **因果性**：超越传统的“预测”范式，采用主动刺激控制神经活动，能更直接地检验模型的因果可解释性。
- **闭环设计**：闭环实验可实时调整刺激，提升控制测试的效率和准确性。
- **跨层级覆盖**：覆盖早期、中期、高级视觉区域，能够系统评估模型在不同视觉处理阶段的神经对齐情况。
- **多模型比较**：十个领先模型的统一比较，能够揭示模型族之间的重要差异，而天然图像预测无法区分它们。
- **提出新的诊断指标**：将输入梯度的空间频率结构作为控制能力的预测指标，为该领域提供了新的分析视角。

## 8. 不足与局限

- **信息不完整**：由于全文未提供，无法获知实验的具体统计细节、刺激生成算法、神经元类型与采样数量等，限制了对其严谨性的完全评估。
- **模型覆盖范围**：仅涉及十个“领先模型”，未涵盖所有可能的架构或训练范式，结论的普适性有待进一步验证。
- **对抗训练模型的优势原因未完全解释**：摘要指出对抗鲁棒性不是主预测因子，但对抗模型为何控制优势更强，其机制尚需进一步挖掘。
- **空间频率结构预测的潜在混淆**：输入梯度空间频率与控制能力的相关性可能是间接因素所致（如某些模型更关注纹理而非形状），仍需更多消融分析来确认因果方向。
- **应用限制**：该方法需要在动物上做闭环神经记录，成本高、通量有限，难以直接推广到人类或大规模筛查模型；且刺激扰动超出自然图像范围后，可能涉及视觉感受野的非线性等复杂问题。

（完）
