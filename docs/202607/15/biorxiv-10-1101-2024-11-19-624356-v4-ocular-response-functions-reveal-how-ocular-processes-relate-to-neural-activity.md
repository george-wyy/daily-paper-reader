---
title: Ocular Response Functions reveal how ocular processes relate to neural activity
title_zh: 眼响应函数揭示眼部过程如何与神经活动相关
authors: "Gehmacher, Q., Schubert, J., Kaltenmaier, A., Weisz, N., Press, C."
date: 2026-07-08
pdf: "https://www.biorxiv.org/content/10.1101/2024.11.19.624356v4.full.pdf"
tags: ["query:gaze-intent"]
score: 8.0
evidence: 眼动响应函数联系眼动与神经活动
tldr: 眼动信号对认知与健康至关重要，却常作为伪迹被丢弃。本研究采用时间分辨回归方法，结合静息态MEG与眼动追踪，建模眼动响应函数（ORF），揭示扫视、眨眼、瞳孔扩张的特异神经编码，涉及感觉皮层、小脑和额叶区域。进一步从脑活动重建眼动事件，并将静息态ORF应用于被动听觉任务，表明部分任务相关神经标记可能间接源于眼动贡献。该框架促进了眼动与神经交互的理解，对认知与临床神经科学具有应用价值。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2024-11-19-624356-v4/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1610, \"height\": 912, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2024-11-19-624356-v4/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1619, \"height\": 1261, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2024-11-19-624356-v4/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 780, \"height\": 1410, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2024-11-19-624356-v4/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 786, \"height\": 1417, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2024-11-19-624356-v4/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1587, \"height\": 545, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2024-11-19-624356-v4/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1640, \"height\": 1239, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2024-11-19-624356-v4/fig-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 1587, \"height\": 545, \"label\": \"Figure\"}]"
motivation: 眼动信号常被视为伪迹而移除，导致其神经机制研究不足；本工作旨在通过建模眼动响应函数揭示眼动与神经活动的因果关系。
method: 采用时间分辨回归方法，结合静息态MEG和眼动追踪数据，建模扫视、眨眼、瞳孔扩张的Ocular Response Functions (ORFs)。
result: 发现不同眼动事件具有特异神经编码（如感觉皮层、小脑），可从脑活动重构眼动事件，且静息态ORFs能解释任务中部分神经活动。
conclusion: 提供系统框架分析眼动与神经交互，揭示眼动对神经信号的潜在贡献，为认知和临床研究提供新视角。
---

## 摘要
眼动活动为认知和健康提供了关键见解，越来越多的证据表明其参与注意力、记忆和感觉处理等多种认知功能，且是精神病理学和神经疾病的重要指标。尽管眼动在多个领域至关重要，但支持眼动的神经机制尚未得到充分探索，这主要是因为眼动通常被视为需要从神经信号中去除的伪迹。虽然这种方法有助于数据清洗，但有可能丢弃关于眼动控制的宝贵信息，因此最近有研究兴趣转向对这些信号进行建模以理解它们。因此，我们在此使用时间分辨回归方法，结合静息状态下的脑磁图（MEG）和眼动追踪，来模拟眼响应函数（ORFs），这些函数表征不同眼动事件（特别是扫视、眨眼和瞳孔扩张）的神经特征。我们展示了眼动与神经活动之间的关系（编码），揭示了在这些眼动事件前后出现的一系列感觉皮层、小脑和前额叶特征。相反，我们展示了如何从大脑活动重建眼动事件，并进一步将静息状态推导的ORFs应用于被动聆听任务——表明一些被解释为直接与感觉相关的神经标记原则上可能间接源于眼动对任务相关神经处理的贡献。通过提供一个可访问的框架来检查眼动与神经过程之间的相互作用，我们提供了一系列见解，具有认知和临床神经科学中的潜在应用。

## Abstract
Oculomotor activity provides critical insights into cognition and health, with growing evidence demonstrating its involvement in various cognitive functions such as attention, memory, and sensory processing, and that it is a significant indicator of psychopathologies and neurological disorders. Despite its crucial importance across domains, the neural mechanisms supporting oculomotion have been underexplored, largely because eye movements are typically treated as artefacts to be removed from the neural signal. While useful for data cleaning, this approach risks discarding valuable information about oculomotor control, and there has been recent interest in modelling these signals instead to understand them. Using time-resolved regression methods with magnetoencephalography (MEG) and eye tracking during the resting state, we thus here sought to model  Ocular Response Functions (ORFs), that characterise the neural signatures of distinct oculomotor events, specifically saccades, blinks, and pupil dilation. We demonstrate the relationships between ocular action and neural activity (encoding), revealing a range of sensory cortical, cerebellar and frontal signatures preceding and following such ocular events. We conversely show how we can reconstruct ocular events from brain activity, and further apply resting-state derived ORFs to a passive listening task - demonstrating how some neural markers interpreted as directly related to sensation may in principle indirectly result from oculomotor contributions to task-related neural processing. By providing an accessible framework for examining the interplay between eye movements and neural processes, we offer a range of insights with potential applications across cognitive and clinical neuroscience.

---

## 论文详细总结（自动生成）

### 论文核心问题与整体含义（研究动机和背景）

- **核心问题**：眼动活动（扫视、眨眼、瞳孔扩张）在认知加工和临床诊断中具有重要价值，但传统上在脑成像分析中被当作伪迹移除，导致其背后的神经机制研究不足。本研究旨在解决如何在不丢弃眼动信息的前提下，系统刻画眼动与神经活动的因果/时序关系。
- **整体含义**：通过建立眼响应函数（ORF），将眼动信号转化为可解释的神经响应，不仅揭示了不同眼动事件（扫视、眨眼、瞳孔）各自独特的空间-时间神经特征（涉及感觉皮层、小脑、前额叶等），还展示了这些函数可从静息态迁移至任务态（被动听觉），提示部分看似由刺激驱动的神经反应实际上可能源于眼动过程的间接贡献。该框架为认知和临床神经科学提供了研究眼-脑交互的新工具。

### 方法论：核心思想、关键技术细节

- **核心思想**：借鉴时间响应函数（TRF）框架，将眼动事件（扫视、眨眼、瞳孔扩张）视为“刺激”，通过时间分辨的回归模型（deconvolution）估计每个眼动事件对应的神经冲激响应，称为眼响应函数（ORF）。该函数可正向预测脑活动（编码），也可时间反转后用于从脑活动重建眼动事件（重建）。
- **关键技术细节**：
  - 数据采集：同步MEG（306通道，102个磁力计+204个梯度计）和眼动追踪（瞳孔直径、水平和垂直注视），采样率1 kHz，后降采样至100 Hz。
  - 预处理：分两套数据——一套仅做常规滤波（no-ICA），另一套用ICA去除眼动和心电伪迹（ICA）。眼动事件检测：眨眼基于瞳孔噪声算法；扫视基于二维速度阈值法（5倍中位数速度，最小间隔100 ms）。
  - 源空间投影：使用LCMV波束成形将MEG传感器数据投影至个体解剖空间（1 cm网格，约2982个源点），并配准至MNI模板。
  - ORF估计：使用Eelbrain工具包中的boosting算法（基于稀疏性先验的deconvolution），对每个源点拟合多变量TRF，输入三个眼动预测变量（瞳孔扩张、眨眼、扫视），输出该源点的神经信号，时间延迟范围为-1 s至+1 s（以100 ms汉明窗为基）。采用4折交叉验证，并利用选择性停止防止过拟合。
  - 编码评估：将眼动时间序列与ORF卷积得到预测神经信号，与实际神经信号计算皮尔逊相关系数r（连续）或马修斯相关系数MCC（二元事件）。
  - 重建评估：将ORF时间反转后与神经信号卷积得到预测眼动信号，对二元事件用sigmoid阈值化（0.5），再计算MCC或r。
  - 降维：对每个参与者的源空间ORF进行PCA（基于绝对值），取前三个主成分分析空间-时间模式。
- **算法流程文字说明**：  
  ① 准备静息态MEG源空间数据 y 和眼动预测变量 x（瞳孔、眨眼、扫视）；  
  ② 对每个源点，用boosting算法拟合模型 y = x * h + ε，其中h为ORF；  
  ③ 在测试集上，用眼动x_test卷积h得到预测神经活动y_pred，与实际y_test对比；  
  ④ 重建：将h时间反转，与y_test卷积得到预测眼动x_pred，与实际眼动对比；  
  ⑤ 对每个参与者的ORF做PCA提取主要成分，并在组水平平均权重图。

### 实验设计：数据集、场景与对比

- **数据集**：两个实验（同一批被试）：
  1. **静息态**（5分钟，共29名参与者，12女，17男，平均年龄25.7岁）——用于估计ORF的基准数据。
  2. **被动听觉任务**（同一批被试中28名有效参与者，1名因眼动仪故障排除）——用于验证ORF迁移性。任务：被试听有序（ordered）或随机（random）的音调序列（4个纯音，3 Hz呈现速率，每500个音调切换条件，共2个block，每条件1500个trial），同时眼动记录。
- **基准与对比**：
  - ICA vs. no-ICA预处理：对比是否去除眼动伪迹对ORF空间模式的影响，验证ORF究竟反映神经源还是伪迹。
  - 编码与重建均使用交叉验证评估，并在静息态和任务态分别执行。
  - 重建时对比使用所有源（All）与仅使用第一主成分（PC1）的效果。
  - 在被动听觉任务中，使用MVPA（线性判别分析LDA，5折交叉验证）对实际MEG数据、预测的扫视相关MEG数据进行听觉规律性（ordered vs. random）解码，并与打乱标签对照。
- **未明确对比其他方法**：论文未与Back-to-Back回归等其他解相关方法做直接定量对比，但讨论了其局限（刺激与眼动高度时间相关时难以分离），强调静息态ORF的优势。

### 资源与算力

- **文中未明确提及**：论文未说明使用的GPU型号、数量或训练时长。仅提到使用MATLAB和FieldTrip、Eelbrain工具包，以及MVPA-Light。所有分析均在常规工作站上可运行（数据量<250 GB，预处理后共享约几十GB）。隐式表明计算资源要求不高。

### 实验数量与充分性

- **实验数量**：
  - 静息态编码/重建：每个参与者约2982个源点×3个眼动特征，4折交叉验证，对每个特征计算组水平统计（t检验，N=29）。
  - PCA：每个特征取前3个主成分，在组水平报告。
  - 任务态MVPA：时域（-0.1至0.4 s）每个时间点分类，使用cluster置换检验（10000次置换）。
  - 任务态重建：每个眼动特征在有序/随机条件下分别评估。
  - 对比了ICA/no-ICA两种预处理，并比较All sources和PC1的重建效果。
- **充分性评估**：
  - 实验设计全面：静息态估计ORF（无干扰）、任务态验证迁移性，覆盖主要眼动事件。
  - 统计方法合理（交叉验证、置换检验、效应量Cohen's d）。
  - 样本量中等（N=29/28），但足以检测中等以上的效应（大多数t值>7，d>1.0）。
  - 局限性：未进行跨数据集（如其他任务、不同设备）的泛化验证；未与复杂非线性模型（如深度TRF）对比性能；未在更大规模的独立样本上验证稳定性；眼动检测算法可能影响ORF精度。

### 论文的主要结论与发现

1. **ORF的可行性**：从静息态MEG和眼动数据中可稳定提取源空间特异的ORF，对于扫视、眨眼、瞳孔扩张均有显著高于随机的编码和重建能力。
2. **神经特征时空特异性**：
   - 扫视 → 视觉皮层（枕叶），+100 ms峰，反映视觉回传（reafference）。
   - 眨眼 → 小脑（经ICA去除伪迹后），+150-200 ms峰，与眨眼条件反射相关；以及视觉区。
   - 瞳孔扩张 → 视觉皮层及后内侧区域（如楔前叶），-300~-400 ms峰（活动先于瞳孔变化），提示视觉系统参与准备或预测性调节。
3. **ICA的效果**：去除眼动伪迹后，额叶伪影消失，而真实的神经源（如小脑、视觉皮层）保留，表明ORF能分离伪迹与神经活动。
4. **迁移性**：静息态ORFs可应用于被动听觉任务，并能从中重建眼动（显著高于随机），且MVPA解码听觉规律性在预测的扫视相关MEG中也达到显著，表明眼动可能贡献于听觉定规处理的神经信号。
5. **模块化应用**：ORF可将眼动信号转化为神经空间，便于与其他神经分析方法（相干、连通性、因果建模）结合。

### 优点

- **创新性**：将传统作为伪迹移除的眼动信号转化为可解释的神经响应函数，填补了眼动神经机制研究的空白。
- **方法学严谨**：采用静息态避免刺激-眼动时间相关性干扰；使用源空间定位和PCA降维提供空间特异性；同时验证编码和重建（双向映射）。
- **实用性强**：ORF可迁移至其他任务，为研究认知任务中眼动的间接贡献提供量化工具。
- **结果解释清晰**：通过ICA对比区分了伪迹与神经源，并给出了生理学合理的解释（如小脑与眨眼、视觉皮层与扫视回传）。
- **代码和数据公开**：促进可重复性。

### 不足与局限

- **线性模型限制**：仅使用线性TRF（boosting），可能无法捕捉眼-脑关系中非线性和非平稳的动态。作者也承认若主要目的是最大化预测精度，非线性方法（如深度神经网络）会更优。
- **迁移效果较弱**：任务态重建的精度（r/MCC）虽然显著但数值不高（如瞳孔r~0.05-0.07，扫视MCC~0.05-0.06），表明静息态ORF到主动任务场景下可能丢失一部分任务特异信息。
- **样本量中等**：N≈29，对于个体差异分析和临床推广可能不足。
- **未评估跨范式泛化**：仅测试了一个被动听觉任务，未检视在视觉任务或自然场景下的迁移效果。
- **可能的偏差风险**：眼动检测算法（速度阈值5倍中位数）可能遗漏或误检某些微扫视/眨眼；MEG源定位对小脑等深部结构的可靠性有限（尽管有文献支持）。
- **缺乏系统消融实验**：例如，未检验单独使用某一眼动特征与联合模型的效果差异；未评估不同时间延迟窗口对ORF的影响。
- **计算资源未报告**：可能影响结果可重复性的描述完整性。

（完）
