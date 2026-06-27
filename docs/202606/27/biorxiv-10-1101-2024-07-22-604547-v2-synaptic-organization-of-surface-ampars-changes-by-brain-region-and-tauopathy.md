---
title: Synaptic Organization of Surface AMPARs Changes by Brain Region and Tauopathy
title_zh: 表面AMPA受体的突触组织随脑区和tau蛋白病的变化
authors: "Vaidya, R. M., Zhang, J., Nall, D., Pendharkar, R., Lee, Y., Kim, E. C., Ma, D., Huang, F., Nonaka, H., Kiyonaka, S., Hamachi, I., Chung, H. J., Selvin, P. R."
date: 2026-06-23
pdf: "https://www.biorxiv.org/content/10.1101/2024.07.22.604547v2.full.pdf"
tags: ["query:comp-neuro"]
score: 8.0
evidence: 海马体和tau病变中AMPAR的突触组织
tldr: 表面AMPAR的突触分布与学习记忆相关，但缺乏脑区或病理下的高分辨率测量。本研究采用活标记和双色STORM超分辨成像（精度<10 nm），在厚脑切片中测量表面AMPAR与突触后蛋白的距离。发现海马中表面AMPAR的突触簇比例比皮层小两倍，且在tauopathy模型早期海马分布被破坏而皮层保持正常。该方法为纳米尺度蛋白分布变化提供新工具。
source: biorxiv
selection_source: fresh_fetch
motivation: 探究不同脑区和tauopathy病理下表面AMPAR纳米级组织的变化。
method: 使用活标记和双色STORM超分辨成像，在厚脑切片中精确测量表面AMPAR与突触后蛋白的距离。
result: 海马表面AMPAR突触簇比例是皮层的三分之一；tauopathy模型中海马分布异常而皮层正常。
conclusion: 新方法可识别疾病或学习范式下的AMPAR纳米分布变化。
---

## 摘要
神经元质膜上突触和突触外AMPA受体（AMPARs）的分布与学习和记忆相关。尽管在神经元培养中进行了广泛研究，但缺乏对AMPARs细胞表面分布随脑区或病理变化的高分辨率测量。通过独特的标记方法和优化的双色超分辨率STORM成像（横向<10 nm，轴向<25 nm精度），我们在厚小鼠脑切片中测量了来自活体标记表面AMPARs的各种突触后蛋白在纳米尺度上的距离。我们发现，与附近的运动和体感皮层相比，海马中组织成突触簇的表面AMPARs比例小两倍，这可能是因为两个脑区的突触动力学和功能作用不同。在神经退行性变发生前的tau蛋白病小鼠模型中，我们发现AMPARs的突触-突触外分布及其在突触纳米域中的组织在海马中受到破坏，但在皮层中没有。本工作建立的新方法可用于识别AMPARs以及可能其他蛋白质在病理疾病模型中或作为学习范式功能的纳米尺度分布变化。

## Abstract
The distribution of synaptic and extra-synaptic AMPA receptors (AMPARs) on neuronal plasma membranes is correlated with learning and memory. Despite extensive investigation in neuronal cultures, a high-resolution measurement of the cell-surface distribution of AMPARs as a function of brain regions or pathology is lacking. Via a unique labeling approach and optimized 2-color super-resolution STORM imaging (<10 nm lateral and <25 nm axial precision), we have measured the distances between various post-synaptic proteins from live-labeled surface AMPARs in thick mouse brain slices at the nanoscale level. We find that the fraction of surface AMPARs organized in synaptic clusters is two times smaller in the hippocampus compared to the nearby motor and somatosensory cortex, possibly because of different synaptic dynamics and functional roles of the two brain regions. In a mouse model of tauopathy at an age before the onset of neurodegeneration, we find the synaptic to extra-synaptic distribution of AMPARs, as well as its organization in synaptic nanodomains, are disrupted in the hippocampus, but not the cortex. The novel method established in this work can be applied to identify alterations in nanoscale distributions of AMPARs and possibly other proteins in pathological disease models or as a function of learning paradigms.

---

## 论文详细总结（自动生成）

### 1. 论文的核心问题与整体含义（研究动机和背景）

- **核心问题**：神经元质膜上突触和突触外 AMPA 受体（AMPARs）的纳米级分布如何随脑区（海马 vs. 皮层）和 tau 蛋白病病理发生变化？  
- **背景意义**：AMPARs 是兴奋性突触可塑性的核心，其表面分布与学习记忆密切相关。此前研究多局限于离体神经元培养，缺乏在完整脑组织中高分辨率（纳米级）测量 AMPARs 表面组织的方法。理解其脑区差异和病理改变，能揭示学习记忆的分子基础及神经退行性疾病的早期突触病变。

### 2. 论文提出的方法论

- **核心思想**：利用化学探针 CAM2 活体标记天然表面 AMPARs，结合优化的双色三维 dSTORM 超分辨成像，在厚脑切片中对 AMPARs 与突触后蛋白（PSD-95、Homer-1）实现<10 nm 横向、<25 nm 轴向精度的纳米级定位与距离测量。  
- **关键技术细节**：  
  1. **CAM2 探针**：基于配体导向酰基咪唑（LDAI）化学，将 Alexa Fluor 647 共价连接到所有 GluA1-4 亚基的配体结合域附近，小尺寸确保快速扩散进入 200 μm 脑切片。  
  2. **双色 dSTORM**：使用 CF568 标记的纳米抗体或二抗标记 PSD-95/Homer-1；采用折射率匹配液、自适应光学（变形镜）和原位 PSF 检索（INSPR）校正像差和多步漂移校正（实时台漂移 + 2D 互相关），获得高精度定位。  
  3. **数据分析**：DBSCAN 算法识别 AMPAR 和 PSD-95 簇，进一步识别簇内的纳米域；通过凹包和最近邻分析计算 AMPAR 到 PSD-95 的距离。  
- **公式/算法流程**（文字说明）：  
  - 定位提取：INSPR 提取单分子定位。  
  - 簇检测：DBSCAN（minPts=120，ε=120 nm）从定位点中识别 AMPAR 簇；纳米域检测：DBSCAN（minPts=mean+1.5σ，ε=30 nm）。  
  - 距离计算：AMPAR 簇与 PSD-95 簇的三维主成分分析（PCA）方向距离；AMPAR 点到 PSD-95 簇凹包的最短距离。  
  - 配对联相关函数（PCF）用于分析簇内空间相关性。

### 3. 实验设计

- **样本与数据集**：  
  - 6 月龄 Thy1-YFP-H 小鼠（WT）和 PS19:Thy1-YFP-H 小鼠（tau 蛋白病模型），各 3 只（每组 2 雄 1 雌）。  
  - 脑区：海马 CA1 区 vs. 运动/体感皮层（冠状切片相邻区域）。  
  - 原代神经元培养：E18 大鼠胚胎的海马和皮层神经元（DIV 16），作为离体对照。  
- **验证基准**：文献中已知的 AMPAR-PSD-95 簇距离（~14 nm）、AMPAR-Homer-1 距离（~64 nm）、AMPAR 纳米域大小（~69 nm）等，与 EM 或培养实验数据一致。  
- **对比方法**：  
  - 不同 CAM2 浓度（2 μM vs. 5 μM）和颅内注射方案验证趋势稳定性。  
  - 原代培养与脑片结果对比。  
  - PSD-95 在有/无 CAM2 标记时的比较（排除干扰）。  
  - 对 PS19 海马使用降低 1.6 倍的 DBSCAN 参数以补偿总定位减少。

### 4. 资源与算力

- **论文未明确说明**所使用的 GPU 型号、数量或训练时长。仅描述了显微镜系统（EMCCD、变形镜、LabVIEW/MATLAB 控制）、INSPR 算法和 ThunderSTORM 插件等。无深度学习模型训练细节。

### 5. 实验数量与充分性

- **数量**：  
  - 每基因型/脑区：3 只小鼠，每只≥6 FOV；累计每脑区检测>1500 个 AMPAR 簇（全 FOV）或≥15 根 YFP 阳性神经元（神经元水平分析）。  
  - 额外实验：增加 CAM2 浓度（5 μM）、颅内注射、原代培养对比、PSD-95 对照实验。  
- **充分性**：  
  - 统计检验使用配对 t 检验（WT 内脑区对比）或 Welch t 检验（WT vs. PS19）。多数主结论显著（p<0.05），部分接近显著（如图 4g，p=0.055）。  
  - 实验设计较严谨，但样本量较小（n=3 小鼠），可能增加方差。离体培养与脑片趋势相反，表明培养模型不能完全替代原位。  
  - 未进行多重比较校正，但关键差异较小且一致，结论合理。  
  - **总体充分，但需更大样本和独立验证**。

### 6. 论文的主要结论与发现

1. **脑区差异**：  
   - 海马总表面 AMPAR 密度比皮层高 1.9 倍，但突触簇比例低 2.9 倍（全 FOV）或 2.5 倍（沿 YFP 神经元）；突触内 AMPAR 数目和簇数相同，差异主要来自突触外池增大。  
2. **tau 蛋白病（PS19）变化**：  
   - 海马总 AMPAR 密度下降 1.6 倍（p=0.023），但突触簇比例反而升高（p=0.02-0.03）；突触外池缩小更显著。  
   - 突触簇内 AMPAR 纳米域组织被破坏：纳米域内 AMPAR 比例下降（p=0.001-0.002），每纳米域定位数减少（p=0.027）。  
   - 皮层无显著变化。表明 tau 蛋白病早期（6 月龄，尚未神经退行）已导致海马 AMPAR 纳米级分布失调，可能解释学习记忆缺陷。

### 7. 优点

- **方法创新**：首次在成年脑切片中实现天然表面 AMPAR 纳米级成像，结合化学活体标记（CAM2）与先进显微技术（INSPR、自适应光学、多步漂移校正），分辨率高（<10 nm 横向、<25 nm 轴向）。  
- **生理相关性**：在完整神经回路中研究，结果更贴近生理状态，比离体培养更真实。  
- **发现新现象**：揭示海马与皮层 AMPAR 突触分布根本差异（突触外池大小），以及 tau 蛋白病中 AMPAR 的复杂重组（突触比例增加但纳米域破坏）。  
- **可推广性**：方法能用于其他膜蛋白或疾病模型，为研究纳米尺度蛋白动态提供工具。

### 8. 不足与局限

- **样本量小**：每组仅 3 只小鼠，个体方差大，部分统计边缘显著。  
- **选择偏差**：仅分析有 PSD-95 富集簇的突触（约 1/3 棘），可能遗漏无 PSD-95 簇的弱突触或抑制性突触。  
- **病理模型局限**：仅使用 P301S 突变 tau 小鼠，不能代表所有 tau 蛋白病；未涉及 Aβ 病理。  
- **未测量绝对蛋白数**：使用定位点数而非绝对分子数，定量不确定。  
- **机制缺失**：未探究 tau 如何导致 AMPAR 重分布（如与 PACSIN1、Stargazin 的相互作用），也未与电生理/行为学直接关联。  
- **离体培养反向趋势**：原代培养中海马 vs 皮层趋势相反（海马突触比例更高），提示培养条件可能改变 AMPAR 组织，需谨慎外推。  
- **技术限制**：dSTORM 通量低，不能大规模统计；成像深度有限（30 μm 切片），可能遗漏深层结构。  
- **未校正多重比较**：多个假设检验，部分显著性可能因多重性而减弱。

（完）
