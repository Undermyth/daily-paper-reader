---
title: Hierarchical substrates of prediction in visual cortical spiking
title_zh: 视觉皮层尖峰预测的分层基底
authors: "Westerberg, J. A., Xiong, Y. S., Sennesh, E., Nejat, H., Ricci, D., Azmi, M., Durand, S., Hardcastle, B., Cabasco, H., Belski, H., Bawany, A., Gillis, R., Loeffler, H., Peene, C. R., Han, W., Nguyen, K., Ha, V., Johnson, T., Grasso, C., Young, A., Swapp, J., Ouellette, B., Caldejon, S., Williford, A., Groblewski, P. A., Olsen, S. R., Kiselycznyk, C., Koch, C., Lecoq, J. A., Maier, A., Bastos, A. M."
date: 2026-06-17
pdf: "https://www.biorxiv.org/content/10.1101/2024.10.02.616378v5.full.pdf"
tags: ["query:comp-neuro"]
score: 9.0
evidence: 层次预测编码作为视觉皮层推理的计算机制
tldr: 层级预测编码模型认为视觉皮层通过反馈和预测误差处理信息，但以往研究难以区分反馈与局部计算。本研究利用多物种、多区域高密度层状电生理和全局/局部异常刺激无报告任务发现：全局异常响应仅出现在高级皮层；抑制性中间神经元不介导预测抑制；多数神经元对可预测的局部异常响应占主导。这些发现挑战了现有模型的预测抑制假设，揭示了预测塑造视觉处理的新回路机制。
source: biorxiv
selection_source: fresh_fetch
motivation: 检验层级预测编码是否是视觉皮层处理的关键机制，并解决以往研究无法解析反馈与局部计算的混淆。
method: 使用多物种多区域高密度层状电生理，结合无报告任务和全局/局部异常刺激，以及抑制性中间神经元靶向光遗传。
result: 全局异常响应仅限高级皮层；抑制性中间神经元不介导预测抑制；多数神经元对高度可预测刺激的响应占主导。
conclusion: 结果挑战现有层级预测编码模型，需构建更神经约束的预测处理模型。
---

## 摘要
分层预测编码（HPC）模型近年来在神经科学中蓬勃发展1-9。前馈和反馈处理是HPC模型的核心。以往的fMRI、EEG/MEG和LFP实验研究9-11无法可靠地将反馈调节与局部计算和前馈输出区分开来。这里，利用开放科学8、多物种、多区域、高密度12、层状神经生理学13，我们实验性地检验了分层预测编码是否是塑造视觉刺激皮层处理的关键组成部分。为了隔离视觉信息处理并消除运动/奖赏混杂因素9-11，我们采用无报告任务。我们的任务利用所谓的全局异常刺激（GO）作为不可预测的偏差刺激，从而规避低级适应。我们研究了它们相对于局部异常刺激（LO）的反应，后者已被习惯化为高度可预测的先验。该数据集中的四个惊人发现挑战了许多现有的分层预测编码模型。首先，GO反应仅限于高阶、更认知的区域，而非早期到中期视觉皮层。其次，在灵长类和小鼠中进行的抑制性中间神经元靶向光遗传学以及灵长类中的波形形状分析没有发现预测抑制通过这些中间神经元实现的证据。第三，高度可预测的LO反应在超过50%的所有神经元中占主导地位，包括高阶皮层，而后者本应预期它们，这表明预测抑制的证据有限。最后，由GO引发的预测错误反应并未引发前馈处理。这些结果揭示了控制预测如何塑造视觉处理的回路动态，激励了更多神经约束的预测处理模型。

## Abstract
Hierarchical predictive coding (HPC) models have recently flourished in neuroscience1-9. Feedforward and feedback processing are at the heart of HPC models. Previous experimental studies using fMRI, EEG/MEG, and LFP9-11 do not reliably resolve feedback modulation from local computations and feedforward outputs. Here, using open-science8, multi-species, multi-area, high-density12, laminar neurophysiology13, we empirically test whether hierarchical predictive coding is a key component shaping cortical processing of visual stimuli. To isolate visual information processing and eliminate motor/reward confounders9-11, we use a no-report task. Our task leveraged so-called global oddballs (GO) as unpredictable, deviant stimuli that circumvent low-level adaptation. We examined their responses relative to local oddballs (LO) that we habituated into highly predictable priors. Four surprising findings in this dataset challenge many existing hierarchical predictive coding models. First, GO responses were exclusive to higher-order, more cognitive areas rather than early-to-mid visual cortex. Second, inhibitory interneuron-targeted optogenetics in primates and mice and waveform shape analysis in primates revealed no evidence that predictive suppression was implemented via these interneurons. Third, highly predictable LO responses dominated in over 50% of all neurons, including in higher-order cortex, which should have anticipated them, indicating limited evidence for predictive suppression. Lastly, prediction error responses evoked by GOs did not evoke feedforward processing. These results reveal circuit dynamics that govern how prediction shapes visual processing, motivating more neurally constrained predictive processing models.

---

## 论文详细总结（自动生成）

# 论文详细中文总结

## 1. 核心问题与整体含义（研究动机和背景）

- **研究动机**：层级预测编码（Hierarchical Predictive Coding, HPC）模型提出大脑通过预测与预测误差的机制处理感觉信息，其中前馈和反馈处理是核心。然而，以往研究（fMRI、EEG/MEG、LFP）难以区分反馈调节、局部计算与前馈输出，因此无法明确检验HPC的关键假设。
- **核心问题**：本文旨在利用多物种、多区域、高密度层状电生理记录，并采用无报告任务的全局/局部异常刺激范式，直接检验HPC模型的三个核心假设：
  - H1：预测具有抑制性或通过抑制性中间神经元实现减法消减；
  - H2：预测误差信号通过前馈通路（特别是浅层2/3锥体神经元）向上传递；
  - H3：HPC回路在皮层中普遍存在（从初级视皮层到高级联合皮层）。
- **整体含义**：实验结果对经典HPC模型形成了系统性挑战，揭示了预测处理在视觉皮层中的实际回路动态，呼吁构建更符合神经数据的预测处理模型。

## 2. 方法论：核心思想、关键技术细节

- **核心思想**：采用**无报告任务**（no-report task）以消除运动和奖赏的混杂效应，通过**习惯化**（habituation）建立对局部异常（LO）序列（如 x-x-x-y）的高度可预测先验，然后引入不可预测的**全局异常（GO）**（x-x-x-x）作为预测误差刺激。GO不受低级适应影响，能更纯净地反映高阶预测误差。
- **关键技术细节**：
  - **多区域高密度层状电生理（MaDeLaNe）**：使用Neuropixels探针（小鼠）和线性阵列探针（猴）同时记录多个视觉皮层区域（小鼠：V1、LM、RL、AL、PM、AM；猴：V1、V2、V3、V4、MT、MST、8A、PFC）的神经元尖峰活动。
  - **层识别**：结合MUA、CSD、光谱层状模式及MRI解剖图像，将神经元定位到不同皮层。
  - **细胞类型特异性光遗传学**：在小鼠中标记PV+和SST+抑制性中间神经元；在猴中使用AAV-Dlx-ChR2靶向所有GABA能抑制性中间神经元，结合光标记和波形形状分析识别抑制性中间神经元。
  - **统计对比方法**：主对比为（P4-P3）主块 vs （P4-P3）控制块，以控制时间效应和适应。使用非参数簇置换检验（cluster-based permutation test）确定显著性。
  - **Granger因果分析**：在小鼠中计算区域间尖峰活动的Granger因果关系，比较前馈与反馈方向的偏侧性。
  - **多LLM文献对比**：利用10个大型语言模型组成的委员会对25篇文献和本文结果进行标准化评分，量化与三个假设的一致性。

## 3. 实验设计：数据集、基准、对比方法

- **数据集**：
  - **小鼠实验**：16只转基因小鼠（SST-Cre;Ai32和PV-Cre;Ai32），记录6个视觉皮层区域。最终分析纳入14只小鼠、4807个高质量单单元。
  - **猴实验**：2只雄性猕猴（1只恒河猴、1只食蟹猴），记录8个皮层区域。多单元活动（MUAe）来自6592个记录位点，视觉响应限定的单元约2495个。
- **任务范式**：
  - **主块**：80% x-x-x-y（局部异常LO），20% x-x-x-x（全局异常GO）。
  - **控制块**：50% x-x-x-x，50% y-y-y-y（两种序列交替，使GO刺激变为可预测的规则刺激）。
  - **随机块**：所有4刺激序列等概率呈现（用于计算选择性指数）。
  - 为建立先验，小鼠/猴在记录前经过多天（2000-3000次）LO序列习惯化。
- **对比方法**：主要对比是主块中GO/LO的P4-P3与控制块中对应刺激的P4-P3的差异。此外还比较了不同概率条件下的LO响应，以及有无习惯化时的GO响应。没有与其他模型进行端到端对比，但通过LLM文献比较将结果置于HPC文献坐标系中。

## 4. 资源与算力

- **文中未明确说明使用的GPU型号、数量或训练时长**。仅提及数据采集使用了Neuropixels探针（小鼠）和自定义的128/32通道线性探针（猴），并通过Open Ephys GUI、Kilosort2等软件进行离线处理。
- **多LLM评估**使用10个本地执行的模型（Gemma、DeepSeek、Mistral等），在Apple Silicon硬件上通过MLX-LM框架运行，但未给出具体GPU或时长。
- **综上**：论文主要贡献为实验发现，计算资源细节不足，这是常见情况。

## 5. 实验数量与充分性

- **实验数量**：
  - 小鼠：14只，4807个单单元，分布在6个视觉区域。
  - 猴：2只，约2495个视觉响应多单元，分布在8个皮层区域。
  - 主块400试次（含80次GO），控制块200试次，随机块100试次（每种序列约6.25%概率）。
  - 光遗传标记：小鼠9只SST+细胞215个、7只PV+细胞262个；猴1只17个标记单元。
  - 行为指标：猴瞳孔直径变化、小鼠跑步速度变化。
  - 补充实验：概率操纵（12.5%、80%、100% LO概率）、习惯化程度对比、试次位置效应分析、CSD、Granger因果、功能聚类等。
- **充分性与公平性**：
  - 实验设计严密：使用无报告任务、长时间习惯化、控制块、多重对比控制、非参数统计检验。
  - 多物种、多区域、多层级记录增强了结果的普适性。
  - 对选择性偏差进行了分层（stratification）处理。
  - 通过嵌套模型验证（考虑动物间变异）确认了主要结果（LM、PM、AM的GO检测）。
  - 但也存在局限：仅两只猴且仅一只有光遗传数据，小鼠物种单一；未操纵注意力（precision）变量；未涵盖所有皮层区域（如更高级的MTL）；电生理样本量虽大但 GO 响应稀疏，统计效力可能受限于极低比例的响应单元。

## 6. 主要结论与发现

- **发现1（挑战H3，普遍性）**：可预测的局部异常（LO）引起广泛、强烈、前馈方向的尖峰响应，涉及50%以上神经元，遍布所有记录皮层区域，且强度随层级升高而增大（小鼠）。但这不是预测误差，因为其幅度不随偏差概率升高而增大，甚至相反。
- **发现2（挑战H2，前馈预测误差）**：不可预测的全局异常（GO）仅在一小部分高阶皮层区域（小鼠LM、AM、PM；猴V3、MT、8A、PFC）产生稀疏、延迟的响应（＜10%神经元）。GO响应未显示出前馈时序（层级间无显著延时梯度），且在反馈接收层（extragranular layers）更明显。Granger因果分析未发现GO期间前馈连接增强。
- **发现3（挑战H1，预测抑制）**：光标记的PV+、SST+抑制性中间神经元（以及猴的pan-inhibitory细胞）在GO刺激下并未显著降低活动（以允许预测误差表达），相反某些PV群体在GO时活动增加。波形鉴别的猴抑制性神经元同样无显著GO调制。
- **发现4（支持反馈机制）**：GO响应的层分布（主要在L2/3和L5/6中的非颗粒层）、延时模式（高阶较早、低阶较迟）以及缺乏前馈Granger因果，均支持GO信号通过反馈通路从高阶皮层向下传递，而非经典HPC所设想的前馈预测误差传播。
- **文献对比结果**：多LLM评分表明，本文发现与HPC经典文献在三项假设上均显著相悖（尤其对GO而言），因此需要更受神经数据约束的新模型。

## 7. 优点

- **技术创新**：结合多物种、多区域、高密度层状电生理与细胞类型特异性光遗传学，首次在尖峰水平系统检验HPC的精细回路假说。
- **实验设计严谨**：采用无报告任务、长时间习惯化、全局与局部异常的双重对比、控制块和随机块，有效分离了刺激适应与预测、感觉与奖赏/运动相关信号。
- **全面性**：同时记录多个层级、多个区域、多个层、多种细胞类型，并进行Granger因果、CSD、功能聚类等多种分析，多维证伪。
- **开放性**：所有小鼠数据已公开（DANDI Archive），代码开源，便于独立验证。
- **客观性**：使用非参数统计检验和多模型LLM文献比较，减少人为偏差。

## 8. 不足与局限

- **物种与样本限制**：猴实验仅2只动物，光遗传仅1只猴；小鼠为单一品系；未涉及非人灵长类更高级的前额叶-颞叶环路。
- **任务限制**：无报告任务虽然消除了运动/奖赏混淆，但也可能减弱了动物的注意水平，而一些理论认为预测误差受precision（注意）调制，可能影响GO的大小。未来需直接操纵注意。
- **未测试所有预测形式**：本研究仅涉及时间序列预测，未覆盖空间预测、感觉运动预测等其他HPC提议的核心内容。
- **抑制性细胞类型覆盖不全**：未单独研究VIP+中间神经元的作用（尽管部分工作引用了相关文献）。
- **统计效力问题**：GO响应稀疏（7-8%神经元），多数对比在特定子集（如PV细胞在LM/PM/AM深层）可能出现假阴性或假阳性。虽然用了多层级核验，但样本量在特定分层后减小。
- **缺乏计算建模**：本文主要为实验证伪，没有构建替代的量化模型来验证提出观点的可解释性，作者承认这一点并鼓励社区后续建模。
- **潜在偏差**：依赖于从LFP/CSD层定位，猴层识别基于MRI和功能指标，可能引入解剖对应误差；光遗传标记可能漏掉未表达ChR2的抑制性神经元。

（完）
