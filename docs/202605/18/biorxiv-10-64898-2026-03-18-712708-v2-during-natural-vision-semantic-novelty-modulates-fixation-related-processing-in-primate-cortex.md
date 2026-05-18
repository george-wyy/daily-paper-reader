---
title: "During natural vision, semantic novelty modulates fixation-related processing in primate cortex"
title_zh: 在自然视觉过程中，语义新颖性调节灵长类动物皮层中与注视相关的处理
authors: "Raghavan, V. S., Madsen, J., Nentwich, M., Leszczynski, M., Falchier, A., Bickel, S., Russ, B. E., Parra, L. C."
date: 2026-05-14
pdf: "https://www.biorxiv.org/content/10.64898/2026.03.18.712708v2.full.pdf"
tags: ["query:gaze-intent"]
score: 8.0
evidence: 自然视觉中语义新颖性调节注视相关的处理
tldr: 本研究探讨了灵长类动物在自然视觉中如何跨注视点整合语义信息。研究者利用深度网络量化注视点的语义新颖性，并通过人类EEG及灵长类颅内记录发现，语义新颖性会调节额叶和枕叶的注视相关电位。结果显示额叶活动先于枕叶，暗示了自上而下的处理机制，揭示了大脑通过整合注视表征来构建场景理解的神经基础。
source: biorxiv
selection_source: fresh_fetch
motivation: 旨在揭示大脑在自然视觉过程中如何跨越多次眼动注视来整合并处理语义信息。
method: 结合深度学习量化语义新颖性，并分析了人类及非人灵长类在观看电影时的EEG和颅内电生理信号。
result: 发现语义新颖性会调节额叶和枕叶的神经活动，且额叶的反应在时间上领先于枕叶。
conclusion: 研究证明了灵长类大脑通过跨注视点的语义整合及自上而下的反馈机制来构建对自然场景的表征。
---

## 摘要
我们通过由扫视分隔的短时间注视来采样视觉场景。虽然低级整合已为人所知，但跨多次注视的中央凹视觉语义整合仍不清楚。我们假设大脑会对从一次注视到下一次注视的语义信息变化做出反应，因此假设每次扫视都存在一个与语义新颖性相关的神经信号。新颖性是利用深度网络对中央凹视觉进行测量的。在观看完整电影的自然视觉过程中（3.4x10^6次扫视），新颖性调节了人类脑电图（EEG）中的额叶和枕叶注视相关电位。人类（9.0x10^4次扫视）和非人灵长类动物（3.3x10^4次扫视）的颅内记录显示，腹内侧视觉区和额叶脑区的宽带高频活动受到调节。这种调节在电影中比在静态图像中更强，且额叶调节先于枕叶调节，表明存在自上而下的效应。这种随新颖性而变化的注视相关活动调节表明，在灵长类动物的自然观察过程中，中央凹表征跨扫视进行了整合，以构建场景表征。

## Abstract
We sample visual scenes with short gaze fixations separated by saccades. While low-level integration is known, semantic integration of foveal vision across multiple fixations remains unclear. We hypothesized that the brain responds to changes in semantic information from one fixation to the next, and therefore postulated a neural signal associated with semantic novelty for each saccade. Novelty was measured using a deep network on foveal vision. Novelty modulated frontal and occipital fixation-related potentials in human EEG during natural viewing of full-length movies (3.4x106 saccades). Intracranial recordings in humans (9.0x104 saccades) and non-human primates (3.3x104 saccades) revealed broadband high-frequency activity modulations in ventromedial visual and frontal brain areas. This modulation was stronger for movies than static images, and frontal modulation preceded occipital modulation, suggesting top-down effects. This modulation of fixation-related activity with novelty suggests that foveal representations are integrated across saccades to construct scene representations during natural viewing in primates.

---

## 论文详细总结（自动生成）

这篇论文探讨了灵长类动物在自然视觉（如观看电影）过程中，大脑如何跨越多次眼动注视（Fixations）来整合语义信息。以下是对该研究的深度结构化总结：

### 1. 核心问题与整体含义（研究动机和背景）
*   **核心问题**：人类和灵长类动物通过频繁的扫视（Saccades）来观察世界，每次注视仅持续几百毫秒。虽然科学界对低级视觉特征（如亮度、对比度）的跨注视整合已有研究，但大脑如何**在语义层面整合**连续注视点之间的信息，并构建连贯的场景理解，其神经机制尚不明确。
*   **研究动机**：研究者假设大脑会监测相邻两次注视之间语义信息的变化（即“语义新颖性”），并产生相应的神经信号来驱动场景表征的更新。

### 2. 论文提出的方法论
*   **核心思想**：利用深度神经网络（DNN）作为计算模型，量化自然视觉中每一次注视所包含的语义信息，并计算相邻注视间的“新颖性”。
*   **关键技术细节**：
    *   **语义特征提取**：使用在 ImageNet 上预训练的 **ResNet-50** 网络。针对每次注视，提取其中心凹区域（视觉中心约 3° 范围）的图像特征向量。
    *   **语义新颖性（Semantic Novelty）定义**：计算当前注视点 $t$ 的特征向量与前一次注视点 $t-1$ 的特征向量之间的**余弦距离**。距离越大，表示语义变化越剧烈，即新颖性越高。
    *   **神经信号分析**：分析注视相关电位（FRPs）和宽带高频活动（BHA，60-150Hz）。使用线性混合效应模型（LMM）排除亮度、对比度、扫视幅度等低级物理特征的干扰。

### 3. 实验设计
*   **数据集与场景**：
    *   **人类 EEG 实验**：125 名受试者观看完整电影（如《神探夏洛克》），累计分析了约 340 万次扫视。
    *   **人类颅内记录（iEEG/ECoG）**：10 名癫痫患者在临床监测期间观看电影，累计约 9 万次扫视。
    *   **非人灵长类（NHP）实验**：2 只猕猴植入电极，观看电影及静态图像，累计约 3.3 万次扫视。
*   **对比维度**：
    *   **动态 vs. 静态**：对比观看电影（有上下文逻辑）与观看静态图像时语义新颖性的调节效应。
    *   **脑区对比**：重点分析额叶（Frontal）与枕叶（Occipital）在时间序列上的反应先后。

### 4. 资源与算力
*   论文中**未明确说明**具体的 GPU 型号、数量或训练时长。
*   考虑到使用了预训练的 ResNet-50 进行特征提取，且处理了数百万次注视点的图像切片，该研究在数据预处理和统计建模（尤其是大规模 LMM 模型拟合）上具有较高的计算需求。

### 5. 实验数量与充分性
*   **实验规模极大**：涵盖了从宏观（EEG）到微观（颅内电生理），从人类到非人灵长类的多维度数据。
*   **充分性**：340 万次扫视的数据量在同类研究中属于顶级规模，确保了统计效力。
*   **客观性**：通过跨物种（人与猴）的一致性发现，增强了结论的普遍性；通过控制低级视觉变量，排除了物理特征对语义信号的混淆。

### 6. 论文的主要结论与发现
*   **语义新颖性调节**：语义新颖性显著调节了额叶和枕叶的神经活动。新颖性越高，注视后的神经反应越强。
*   **自上而下的处理**：在时间上，**额叶的调节效应先于枕叶**（领先约数十毫秒）。这表明大脑可能存在一种自上而下的机制，由高级脑区识别语义变化并反馈给视觉皮层。
*   **上下文依赖性**：语义新颖性的调节效应在观看电影时比观看静态图像时更强，说明这种整合机制与场景的动态演变和上下文逻辑密切相关。

### 7. 优点
*   **生态效度高**：采用自然观看电影的任务，而非实验室中枯燥的简单刺激，更接近真实的视觉体验。
*   **跨学科结合**：成功将计算机视觉的深度学习模型（ResNet）应用于认知神经科学，量化了难以定义的“语义”概念。
*   **跨物种验证**：在人类和猕猴身上发现了相似的神经表征模式，证明了该机制在灵长类进化中的保守性。

### 8. 不足与局限
*   **模型偏差**：ResNet-50 虽然能提取语义，但其处理方式与生物大脑视觉系统仍有差异（如缺乏反馈连接），可能无法完全模拟人类的语义理解。
*   **时间分辨率限制**：尽管使用了 iEEG，但对于极其复杂的语义加工过程，毫秒级的时间分辨率仍可能难以完全拆解所有反馈环路。
*   **应用限制**：研究主要集中在中心凹视觉，忽略了周边视觉（Peripheral Vision）在扫视计划和语义预取中的作用。

（完）
