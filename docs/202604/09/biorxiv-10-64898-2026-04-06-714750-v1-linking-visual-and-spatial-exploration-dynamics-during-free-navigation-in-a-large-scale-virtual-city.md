---
title: Linking visual and spatial exploration dynamics during free navigation in a large-scale virtual city
title_zh: 在大规模虚拟城市自由导航期间关联视觉与空间探索动态
authors: "Schmidt, V., Nolte, D., Walter, J. L., Sanchez Pacheco, T., König, P."
date: 2026-04-08
pdf: "https://www.biorxiv.org/content/10.64898/2026.04.06.714750v1.full.pdf"
tags: ["query:gaze-intent"]
score: 9.0
evidence: 用于探索意图的多模态眼动追踪与运动追踪
tldr: 本研究探讨了人类在大型虚拟城市导航时，视觉采样与空间运动之间的关联。通过记录26名参与者的眼动和全身运动数据，研究发现行走速度、空间覆盖率与视觉动态性之间存在显著的正相关。这表明存在一个跨领域的“探索”因子，共同塑造了个体在复杂环境中的移动和注意力分配方式。
source: biorxiv
selection_source: fresh_fetch
motivation: 旨在探究视觉采样与空间运动在探索行为中是受单一跨领域特质驱动还是独立运行。
method: 在大型虚拟城市中记录参与者的眼动和运动轨迹，并利用主成分分析和典型相关分析处理视觉与空间描述符。
result: 发现行走速度和空间占用熵与视觉动态性之间存在强耦合关系，而探索性路径选择对这种耦合的贡献较小。
conclusion: 研究结果支持存在一个通用的“探索”因子，该因子同步调节个体在复杂环境中的运动速度、空间覆盖及视觉注意力风格。
---

## 摘要
平衡探索与利用是适应性行为面临的一项基本挑战，然而目前尚不清楚视觉采样与空间运动是反映了单一的跨领域特质，还是独立运行。我们通过记录26名参与者在五个阶段共计150分钟内自由导航大规模虚拟城市“Westbrook”时的头戴式眼动追踪和全身运动追踪数据，探讨了这一问题。我们从运动轨迹中推导出三个空间描述指标：中值步行速度、占用熵以及探索性路线选择的比例。从注视数据中，我们计算了38个稳健的视觉描述指标，涵盖注视动态、瞳孔大小、扫视幅度、眼头对齐和转移熵。主成分分析将视觉描述指标简化为三个成分，解释了58%的方差，其中第一主成分（PC1）反映了“注视活力”（频繁的切换、更大的扫视和更高的转移熵）。典型相关分析揭示了空间行为与视觉行为之间的强耦合：第一对典型变量的相关系数为r=0.68（交叉验证r=0.45），这主要由高步行速度和占用熵与高注视活力的关联所驱动。相比之下，探索性路线选择的比例对这种耦合的贡献较小。这些研究结果表明，低水平运动速度和空间覆盖范围的个体差异与探索性视觉风格共同变化，支持了存在一种领域通用的“探索”因子，该因子塑造了人们在复杂环境中移动和关注的方式。

## Abstract
Balancing exploration and exploitation is a fundamental challenge for adaptive behavior, yet it remains unclear whether visual sampling and spatial locomotion reflect a single cross-domain trait or operate independently. We addressed this question by recording head-mounted eye-tracking and full-body motion tracking while 26 participants freely navigated "Westbrook", a large-scale virtual city for a total of 150min across five sessions. From the movement trajectories we derived three spatial descriptors: median walking speed, occupancy entropy, and the proportion of explorative route choices. From the gaze data, we computed 38 robust visual descriptors encompassing fixation dynamics, pupil size, saccadic amplitude, gaze-head alignment, and transition entropy. Principal-component analysis reduced the visual descriptors to three components that captured 58% of variance, with the first component (PC1) reflecting "gaze dynamism" (frequent shifts, larger saccades, higher transition entropy). Canonical correlation analysis revealed a strong coupling between spatial and visual behaviours: the first pair of canonical variates correlated at r=0.68 (cross-validated r=0.45), driven primarily by the association of high walking speed and occupancy entropy with elevated gaze dynamism. In contrast, the proportion of explorative route choices contributed little to this coupling. These findings demonstrate that individual differences in low-level locomotor speed and spatial coverage co-vary with an exploratory visual style, supporting the existence of a domain-general "exploration" factor that shapes both how people move through, and attend to, complex environments.

---

## 论文详细总结（自动生成）

这篇论文探讨了人类在复杂环境中导航时，视觉注意力（看哪里）与空间运动（往哪走）之间的内在联系。以下是对该研究的详细总结：

### 1. 核心问题与整体含义
*   **研究动机**：在陌生环境中，生物体必须在“探索”（获取新信息）与“利用”（利用已知资源）之间取得平衡。过去的研究通常将视觉搜索和空间导航作为独立领域对待。
*   **核心问题**：个体的探索行为是受一个统一的、跨领域的“探索特质”驱动，还是由视觉和运动系统各自独立控制？
*   **整体含义**：研究揭示了视觉采样动态与空间移动速度/范围之间存在强耦合，支持了存在一种通用的“探索因子”来同步调节多模态行为。

### 2. 方法论
*   **核心思想**：通过高维度的行为描述符捕捉视觉和空间的细微特征，并利用降维和相关性分析寻找跨模态的关联。
*   **关键技术细节**：
    *   **空间描述符（3个）**：中值步行速度、占用熵（衡量空间覆盖的均匀度/广度）、探索性路线选择比例（基于路径的新颖性）。
    *   **视觉描述符（38个）**：包括注视持续时间、瞳孔大小、扫视幅度、眼头协调性（Gaze-head alignment）、转移熵（衡量视觉扫描的复杂性）等。
    *   **算法流程**：
        1.  **PCA（主成分分析）**：对38个视觉指标进行降维，提取出反映“注视活力”（Gaze Dynamism）的核心成分。
        2.  **CCA（典型相关分析）**：将空间描述符矩阵与视觉描述符矩阵进行关联，寻找能最大化两者相关性的线性组合。
        3.  **交叉验证**：使用留一法（Leave-one-subject-out）验证相关性的稳健性。

### 3. 实验设计
*   **场景与数据集**：使用名为“Westbrook”的大规模虚拟城市（约 1 平方公里，包含街道、建筑、公园等复杂元素）。
*   **参与者**：26名健康成年人。
*   **实验流程**：每位参与者进行5个阶段的自由导航，总时长达150分钟。
*   **硬件设备**：HTC Vive Pro 头显（集成眼动追踪）、Cyberith Virtualizer ELITE 2 全向跑步机（实现全身运动追踪）。
*   **Benchmark/对比**：本研究属于探索性实证研究，主要对比了不同个体间的行为差异，并利用置换检验（Permutation testing）建立统计基准。

### 4. 资源与算力
*   **算力说明**：论文未明确提及具体的 GPU 型号或训练时长。由于该研究侧重于实验数据采集与统计分析（PCA/CCA），而非深度学习模型训练，因此对算力的需求主要集中在 VR 环境的实时渲染和后期数据处理上，通常普通的科研工作站即可满足。

### 5. 实验数量与充分性
*   **实验规模**：26名参与者，每人150分钟数据，累计约65小时的多模态高频采样数据。
*   **充分性评价**：
    *   **样本量**：对于此类高精度的实验室行为研究，26人的样本量属于标准水平，但对于建立普适性的个体差异模型稍显局限。
    *   **数据深度**：150分钟的自由导航远超同类研究（通常为10-20分钟），提供了极高的统计效能来观察稳定的行为风格。
    *   **客观性**：采用了交叉验证和置换检验，确保了发现的相关性不是由于过拟合或随机噪声引起的。

### 6. 主要结论与发现
*   **视觉成分提取**：视觉 PC1（解释 32% 方差）代表了“注视活力”，即高频切换、大扫视和高信息熵。
*   **跨模态耦合**：空间行为与视觉行为显著相关（$r = 0.68$，$p < 0.001$；交叉验证 $r = 0.45$）。
*   **核心驱动力**：这种耦合主要由**步行速度**和**空间占用熵**驱动。简单来说，走得快且空间覆盖广的人，其视觉扫描也更活跃、更具探索性。
*   **路线选择的独立性**：令人意外的是，高层次的“探索性路线选择”（选择新路径）与低层次的视觉/运动动态关联较弱，暗示高层决策可能受不同机制控制。

### 7. 优点
*   **高生态效能**：在大型、复杂的虚拟城市中进行长时程自由导航，比传统的实验室简易任务更接近真实世界。
*   **多模态整合**：同步记录眼动、头部运动和全身位移，提供了全方位的行为画像。
*   **统计严谨**：使用了 CCA 和交叉验证，有效处理了高维行为数据中的共线性问题。

### 8. 不足与局限
*   **硬件限制**：全向跑步机虽然实现了行走，但其运动学特征（如步态、阻力）与真实地面行走仍有差异，可能影响运动速度与视觉的自然耦合。
*   **样本多样性**：参与者多为年轻人，可能无法代表老年人或具有导航障碍的群体。
*   **因果关系不明**：CCA 只能证明相关性，无法确定是“活跃的视觉引导了快速移动”，还是“快速移动迫使视觉系统更频繁采样”。
*   **缺乏认知负荷控制**：实验为自由导航，未考虑在有特定任务压力（如限时寻宝）下这种耦合是否会发生变化。

（完）
