---
title: "A unified multiscale modelling framework to explore the brain excitatory-inhibitory balance: application to multiple sclerosis"
title_zh: 一个探索大脑兴奋-抑制平衡的统一多尺度建模框架：应用于多发性硬化症
authors: "Korkmaz, G., Lorenzi, R. M., Ravera, F., Alahmadi, A. A. S., Monteverdi, A., Kanber, B., Prados, F., D'Angelo, E. U., Palesi, F., Toosy, A., Gandini Wheeler-Kingshott, C. A. M."
date: 2026-08-19
pdf: "https://www.biorxiv.org/content/10.64898/2025.12.03.692031v2.full.pdf"
tags: ["query:comp-neuro"]
score: 6.0
evidence: 结合动态因果建模与虚拟大脑的统合多尺度脑建模范式，属于计算神经科学核心主题
tldr: 大脑兴奋-抑制平衡对正常功能至关重要，其失衡与多发性硬化等神经疾病相关。为表征这一平衡，提出融合动态因果建模（DCM）与虚拟大脑（TVB）的统一多尺度框架，应用于任务和静息态fMRI数据。在MS患者中，发现静息与任务态有效连接的兴奋/抑制性质显著改变，并与行为表现和残疾程度相关。该框架整合连接级与网络级信息，为探索脑网络失衡机制提供了新手段。
source: biorxiv
selection_source: fresh_fetch
motivation: 大脑兴奋-抑制平衡的破坏与神经疾病密切相关，但现有方法难以在多尺度上统一表征其变化，亟需综合建模框架。
method: 构建结合动态因果建模（DCM）与虚拟大脑（TVB）的多尺度框架，应用于MS患者的视觉运动任务和静息态fMRI数据。
result: 发现MS患者静息和任务态有效连接兴奋/抑制性质显著改变，并与反应时间和残疾程度等临床指标相关。
conclusion: 研究揭示全局兴奋性增益与任务有效连接强度相关，为理解神经疾病中的兴奋-抑制失衡提供了统一的多尺度视角。
---

## 摘要
兴奋与抑制的平衡对大脑动力学至关重要，其紊乱可导致神经系统疾病中的网络功能障碍。在此，我们提出了一个概念上统一的多尺度大脑建模框架，结合了应用于任务和静息态功能磁共振成像（fMRI）数据的动态因果建模（DCM）以及虚拟大脑（TVB），以表征大脑的兴奋/抑制平衡。我们将该框架应用于由9名健康对照者和17名多发性硬化症患者（pwMS）组成的队列中的视觉运动脑子网络。采集的数据包括具有可变握力的事件相关任务fMRI实验、静息态fMRI和弥散加权成像。视觉运动网络包括双侧初级视觉皮层（V1）、左侧初级运动皮层（M1）、辅助运动区和前运动皮层（SMAPMC）、扣带皮层（CC）、顶上小叶（SPL）以及右侧小脑小叶VI（CR）。DCM结果显示，虽然MS患者的整体网络架构得以保留，但有效连接的兴奋/抑制性质存在显著改变：在静息状态下，观察到CR到V1连接性的统计变化，其在健康志愿者中为抑制性，而在MS中为兴奋性。在任务期间，有效连接反馈（包括小脑自连接）在健康志愿者中为正，而在MS中为负，并且随着运动需求的增加而日益失调。功能性和有效连接的改变与行为表现（任务反应时间）和临床指标（残疾严重程度）相关。在整体组水平上，TVB参数将NMDA介导的兴奋性增益降低与较慢的任务反应联系起来。此外，整合DCM和TVB表明，较高的全局兴奋性增益与跨感觉运动和视觉运动通路的更强任务参与有效连接相关，将TVB捕获的网络水平兴奋性与上下文依赖的定向相互作用重构以及DCM揭示的连接水平强度联系起来。

## Abstract
Balanced excitation and inhibition are essential for brain dynamics, and their disruption can lead to network dysfunction in neurological diseases. Here, we present a conceptually unified multiscale brain modelling framework combining Dynamic Causal Modelling (DCM) applied to task and resting-state functional Magnetic Resonance Imaging (fMRI) data and The Virtual Brain (TVB) to characterise the excitatory/inhibitory balance of the brain. We applied the framework to a visuomotor brain subnetwork in a cohort of 9 healthy controls and 17 people with multiple sclerosis (pwMS). Acquired data included an event-related task fMRI experiment with variable grip force, resting-state fMRI, and diffusion-weighted imaging. The visuomotor network comprised the bilateral primary visual cortex (V1), left primary motor cortex (M1), supplementary motor and premotor cortex (SMAPMC), cingulate cortex (CC), superior parietal lobule (SPL), and right cerebellar lobule VI (CR). Results from DCM showed that while the overall network architecture was preserved in MS, there were significant alterations in the excitatory/inhibitory nature of effective connectivity: at rest, a statistical change was observed in CR-to-V1 connectivity, which was inhibitory in healthy volunteers but excitatory in MS. During task, effective connectivity feedback, including cerebellar self-connection, was positive in healthy volunteers but negative in MS and became increasingly dysregulated with higher motor demand. Alterations in functional and effective connectivity were associated with behavioural performance (task reaction time) and clinical measures (disability severity). At the overall group level, TVB parameters linked reduced NMDA-mediated excitatory gain to slower task responses. Moreover, integrating DCM and TVB demonstrated that higher global excitatory gain was associated with stronger task-engaged effective connectivity across sensorimotor and visuomotor pathways, linking network-level excitability captured by TVB to context-dependent reconfiguration of directed interactions and to connection-level strength revealed by DCM.