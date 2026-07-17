---
title: Functional imaging of hippocampal layers using VASO and BOLD on the Next Generation (NexGen) 7T Scanner
title_zh: 使用VASO和BOLD在下一代(NexGen)7T扫描仪上进行海马层的功能成像
authors: "Häkkinen, S., Beckett, A., Walker, E., Huber, L., Feinberg, D. A."
date: 2026-07-17
pdf: "https://www.biorxiv.org/content/10.1101/2025.08.29.673151v3.full.pdf"
tags: ["query:comp-neuro"]
score: 7.0
evidence: 记忆任务中海马层的特异性功能成像
tldr: 针对mesoscale fMRI中海马体层特异性成像面临灵敏度低、生理噪声大和血管复杂等挑战，本研究在NexGen 7T扫描仪上优化了CBV VASO序列。通过自传体记忆任务，VASO与BOLD均在宏观层面检测到前海马显著激活，但在下托层别上BOLD表现出偏向深层静脉的偏差。优化后的有效TR为3.2秒，支持检索阶段和皮层功能连接的探索，证实了海马前后功能分离。该工作实现了海马体层功能的高精度成像，为神经心理学研究提供了新工具。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-08-29-673151-v3/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1700, \"height\": 1094, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-08-29-673151-v3/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1713, \"height\": 1678, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-08-29-673151-v3/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1718, \"height\": 1213, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-08-29-673151-v3/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1588, \"height\": 1043, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-08-29-673151-v3/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1210, \"height\": 2005, \"label\": \"Figure\"}]"
motivation: 海马体fMRI面临灵敏度低、生理噪声大及复杂血管导致的层特异性偏差，需优化VASO以实现精准的层功能成像。
method: 在NexGen 7T上优化CBV VASO参数，结合BOLD同时采集，采用自传体记忆任务进行海马体层特异性激活分析。
result: 宏观上VASO和BOLD均显示前海马激活；层级别上下托区BOLD偏向内层静脉，VASO无此偏差；优化TR支持功能连接分析。
conclusion: 优化VASO可实现海马体层功能的高精度映射，有效避免静脉偏倚，为神经心理疾病机制研究提供可靠手段。
---

## 摘要
空间准确性和静脉偏倚是介观尺度fMRI的核心问题，由于灵敏度较低、生理噪声高和血管结构复杂，皮层下脑区域面临额外挑战。在此，我们在NexGen 7T扫描仪上优化了CBV VASO，用于人脑海马层特异性研究。VASO和BOLD（从同一采集）均在既定的自传体记忆任务中检测到显著的海马激活。在宏观尺度上，激活模式趋同，显示前海马有显著的记忆任务激活，并且额顶叶新皮层持续参与。然而，在层状尺度上，下托内深度依赖的轮廓出现了差异：BOLD表现出朝向内层的明显偏倚，与该亚区的已知静脉引流模式一致。最后，优化的有效TR为3.2秒，允许探索性研究检索阶段和新皮层功能连接，两者均使用VASO和BOLD支持海马前后分离。因此，海马fMRI能够以高精度绘制层功能，并为许多神经心理学现象和疾病提供更深入的见解。

## Abstract
Spatial accuracy and venous biases are a central concern in mesoscale fMRI, with subcortical brain regions facing additional challenges due to lower sensitivity, high physiological noise, and complicated vasculature. Here, we optimized CBV VASO on the NexGen 7T scanner for layer-specific investigations of the human hippocampus. Both VASO and BOLD (from the same acquisition) detected significant hippocampal activation during an established autobiographical memory task. At the macroscale, activation patterns converged, showing pronounced memory task activation in the anterior hippocampus and consistent engagement across the frontoparietal neocortex. At the laminar scale, however, differences in depth-dependent profiles emerged within the subiculum: BOLD exhibited a pronounced bias toward the inner layers, consistent with the known venous drainage pattern in the subfield. Finally, the optimized effective TR of 3.2 s allowed exploratory study of retrieval stages and neocortical functional connectivity, which both supported hippocampal anterior-posterior dissociation using both VASO and BOLD. Thus, hippocampal fMRI allows mapping layer function with high accuracy and can provide deeper insights into a number of neuropsychological phenomena and disorders.