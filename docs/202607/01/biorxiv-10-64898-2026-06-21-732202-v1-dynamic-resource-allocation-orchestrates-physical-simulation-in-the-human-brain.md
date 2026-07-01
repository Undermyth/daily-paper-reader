---
title: Dynamic resource allocation orchestrates physical simulation in the human brain
title_zh: 动态资源分配协调人脑中的物理模拟
authors: "Long, L., Wang, Q., Yang, Q., Chang, L."
date: 2026-06-25
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.21.732202v1.full.pdf"
tags: ["query:comp-neuro"]
score: 6.0
evidence: 大脑中物理推理的计算机制
tldr: 人类大脑能灵活预测物理事件，而当前AI缺乏此能力。本研究结合fMRI与MEG，利用球碰撞范式揭示了层级空间分离和双时间尺度的神经过程：高阶皮层编码关系变量，低阶区编码对象特征；早期预测信号在碰撞前700毫秒出现。动态资源直觉物理引擎(IPE)模型通过优化精度-成本权衡，统一解释了行为和神经数据，并预测了另一个自适应控制变量的早期编码，经MEG和瞳孔反应证实。该工作揭示了大脑通过分层预测控制动态分配资源实现高效物理推理的机制，为AI系统设计提供生物启发。
source: biorxiv
selection_source: fresh_fetch
motivation: 当前AI缺乏人类灵活预测物理事件的能力，亟需揭示大脑实现物理模拟的神经机制。
method: 采用视觉遮挡的球碰撞范式，结合fMRI和MEG多模态成像，并构建动态资源直觉物理引擎(IPE)模型。
result: 发现层级空间分离（高阶皮层编码关系变量）与双时间尺度过程（实时模拟与早期预测信号），并验证了自适应控制变量的早期编码。
conclusion: 大脑通过分层预测控制动态分配认知资源实现高效物理推理，该框架为AI物理模拟提供生物启发。
---

## 摘要
人类能够通过在大脑中内部模拟物体动力学来灵活预测物理事件——这是当前人工智能系统所缺乏的能力。利用带有视觉遮挡的球碰撞范式结合多模态神经成像（fMRI/MEG），我们揭示了用于物理模拟的时空组织神经架构。fMRI揭示了层次化的空间分离：高阶皮层区域编码关系性物理变量，不同于低阶感觉运动区域编码的物体特定特征。MEG揭示了两个时间上不同的神经过程：一个实时模拟，跟踪物体的演化状态，与碰撞动力学对齐；以及一个早期预测信号，预测碰撞发生（接触前约700毫秒）。我们提出这种早期预测控制机制在模拟过程中动态分配认知资源。这通过动态资源直观物理引擎（IPE）模型形式化，该模型通过优化准确度-成本权衡来捕捉行为数据和双重神经时间尺度。关键的是，这一框架预测了除碰撞发生之外的另一个自适应控制变量的早期编码，MEG和瞳孔反应均证明了这一点。这些发现揭示了大脑如何通过层次化组织的预测控制实现高效的物理推理，并动态分配认知资源。

## Abstract
Humans can flexibly predict physical events by internally simulating object dynamics in the brain--a capacity lacking in current AI systems. Using a ball collision paradigm with visual occlusion combined with multimodal neuroimaging (fMRI/MEG), we uncover a spatiotemporally organized neural architecture for physical simulation. fMRI reveals hierarchical spatial segregation: higher-order cortical regions encode relational physical variables, distinct from object-specific features encoded in the lower-order sensorimotor regions. MEG uncovers two temporally distinct neural processes: a real-time simulation tracking the evolving state of the object, in alignment with collision dynamics, and an early predictive signal anticipating collision occurrence ([~]700 ms before contact). We propose that this early predictive control mechanism dynamically allocates cognitive resources during simulation. This is formalized by a Dynamic Resource Intuitive Physics Engine (IPE) model, which captures both behavioral data and the dual neural timescales by optimizing accuracy-cost tradeoffs. Crucially, this framework predicts early encoding of another adaptive control variable separate from collision occurrence, as evidenced by both MEG and pupillary responses. These findings reveal how the brain achieves efficient physical inference through hierarchically organized predictive control that dynamically allocates cognitive resources.