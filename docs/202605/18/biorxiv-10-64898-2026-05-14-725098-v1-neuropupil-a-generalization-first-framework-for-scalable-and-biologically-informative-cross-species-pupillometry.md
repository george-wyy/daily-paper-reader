---
title: "NeuroPupil: A generalization-first framework for scalable and biologically informative cross-species pupillometry"
title_zh: NeuroPupil：一种泛化优先的框架，用于可扩展且具有生物学信息量的跨物种瞳孔测量
authors: "Ozdemirli, K., Connor, T., Dinc, b., Kim, K., Lacin, M. E., Maldonado, M., Guha, S., Hawk, K., Oksuz, C., Bell, F., Zhang, Z., Leal, T., sarn, n., Sloan, A. R., Chomyk, A., Ghasia, F., Trapp, B., Mata, I., Lathia, J., Eng, C., Yildirim, M."
date: 2026-05-18
pdf: "https://www.biorxiv.org/content/10.64898/2026.05.14.725098v1.full.pdf"
tags: ["query:gaze-intent"]
score: 8.5
evidence: 用于脑状态和神经功能的瞳孔测量
tldr: 瞳孔测量是研究脑状态和神经功能的非侵入性手段，但现有方法在跨物种和跨场景应用时面临泛化性差和效率低的挑战。本研究开发了NeuroPupil深度学习框架，通过优化U-Net架构和多受试者池化训练策略，实现了高精度、可扩展的跨物种瞳孔追踪。该框架不仅在计算效率上显著提升，还能更有效地关联瞳孔动态与皮层活动及临床表型，为大规模神经科学研究提供了有力工具。
source: biorxiv
selection_source: fresh_fetch
motivation: 现有的瞳孔测量技术在处理跨物种、多场景数据时，难以兼顾高精度、强泛化能力和大规模计算效率。
method: 提出NeuroPupil框架，结合优化的U-Net架构与多受试者池化训练策略，构建了一个高通量的深度学习追踪系统。
result: 该框架在小鼠和人类数据集上均表现出优于现有方法的准确性与效率，并显著提升了对皮层活动预测和临床特征提取的保真度。
conclusion: NeuroPupil为大规模、跨物种的瞳孔动力学研究提供了可靠的标准化工具，推动了系统神经科学与转化医学的应用。
---

## 摘要
定量瞳孔测量为大脑状态和神经功能提供了一个非侵入性的窗口，但由于在实现准确、可扩展和可泛化的测量方面存在挑战，其在实验和临床环境中的广泛应用受到了限制。在这里，我们介绍了 NeuroPupil，这是一个用于高通量、跨物种瞳孔测量的深度学习框架，强调在不同受试者、行为背景和成像条件下的鲁棒泛化。通过对训练策略和网络架构的系统基准测试，我们确定了池化多受试者训练结合优化的 U-Net 架构是实现可靠且可迁移的瞳孔追踪性能的关键因素。在多种小鼠和人类数据集上，与现有方法相比，NeuroPupil 提高了准确性并显著提升了计算效率，从而实现了对大规模数据集的实际分析。我们进一步证明，提高瞳孔追踪的保真度可以增强下游的生物学推断：源自 NeuroPupil 的瞳孔特征显著改善了对行为小鼠分布式皮层活动的预测，并保留了人类临床记录中具有诊断相关性的时间结构。这些发现强调了精确且可扩展的测量对于将瞳孔动力学与大脑活动和临床表型联系起来的重要性。通过整合基准测试、可扩展性和易于获取的软件工具，NeuroPupil 为大规模瞳孔测量提供了一个可重复的框架，并促进了其在系统和转化神经科学中的应用。

## Abstract
Quantitative pupillometry provides a noninvasive window into brain state and neurological function, but its broader use across experimental and clinical settings is limited by challenges in achieving accurate, scalable, and generalizable measurements. Here, we present NeuroPupil, a deep learning framework for high-throughput, cross-species pupillometry that emphasizes robust generalization across subjects, behavioral contexts, and imaging conditions. Through systematic benchmarking of training strategies and network architectures, we identify pooled multi-subject training combined with an optimized U-Net architecture as a key determinant of reliable and transferable pupil tracking performance. Across diverse mouse and human datasets, NeuroPupil achieves improved accuracy and substantial gains in computational efficiency compared to existing approaches, enabling practical analysis of large-scale datasets. We further demonstrate that improved pupil tracking fidelity enhances downstream biological inference: NeuroPupil-derived pupil features significantly improve prediction of distributed cortical activity in behaving mice and preserve diagnostically relevant temporal structure in human clinical recordings. These findings highlight the importance of precise and scalable measurement for linking pupil dynamics to brain activity and clinical phenotypes. By integrating benchmarking, scalability, and accessible software tools, NeuroPupil provides a reproducible framework for large-scale pupillometry and facilitates its application in systems and translational neuroscience.

---

## 论文详细总结（自动生成）

这篇论文介绍了一个名为 **NeuroPupil** 的深度学习框架，旨在解决神经科学研究中瞳孔测量（Pupillometry）的泛化性、可扩展性和生物学解释力不足的问题。以下是对该论文的深度结构化总结：

### 1. 核心问题与整体含义
*   **研究动机**：瞳孔动力学是反映大脑状态（如唤醒度、认知负荷、自主神经活动）的非侵入性“窗口”。然而，现有的瞳孔追踪工具（如 DeepLabCut, Facemap）在面对不同受试者、不同光照条件或跨物种应用时，往往需要大量的重新标注和微调，且在大规模数据集上的计算效率较低。
*   **核心问题**：如何构建一个既能实现“零样本”泛化（无需针对新受试者训练），又能高效处理海量数据，且能保留高保真生物学信息的瞳孔测量框架？

### 2. 方法论
*   **核心思想**：采用“泛化优先”的策略，通过**多受试者池化训练（Pooled Multi-subject Training）**和**优化的 U-Net 架构**来捕捉瞳孔特征的共性，而非过拟合于特定实验设置。
*   **关键技术细节**：
    *   **架构**：基于 U-Net 的编码器-解码器结构，通过跳跃连接（Skip Connections）保留空间细节，输出像素级的瞳孔分割掩码。
    *   **训练策略**：将来自不同个体、不同光照和行为背景的数据整合进一个大型训练池。研究发现，这种多样性训练比针对单一受试者的精调更能提升模型在未知数据上的鲁棒性。
    *   **后处理**：对分割出的掩码进行椭圆拟合，提取瞳孔中心坐标、长短轴及面积等参数。
    *   **工作流**：提供了一个端到端的流水线，支持从原始视频到生物学特征提取的全自动化处理。

### 3. 实验设计
*   **数据集**：
    *   **小鼠数据**：使用了 Allen Brain Institute 的大规模公开数据集以及实验室自采的多种红外光照下的视频。
    *   **人类数据**：包含来自克利夫兰医学中心（Cleveland Clinic）的临床记录，涵盖不同眼色、光照条件及神经系统疾病患者。
*   **Benchmark（基准测试）**：
    *   对比了神经科学领域主流的追踪工具：**DeepLabCut (DLC)**、**Facemap** 和 **StarDist**。
*   **评估指标**：
    *   **准确性**：像素级误差、中心点偏移。
    *   **泛化能力**：在未见过的受试者和成像设备上的表现。
    *   **生物学保真度**：瞳孔特征预测皮层活动（通过广域钙成像数据验证）的准确率。

### 4. 资源与算力
*   **算力说明**：论文强调了 NeuroPupil 的计算效率。在推理阶段，它比现有方法快数倍，能够实现高通量处理。
*   **具体细节**：文中提到在标准工作站 GPU（如 NVIDIA RTX 系列）上即可运行。虽然未详细列出总训练时长，但明确指出其架构优化使得在处理数千小时的视频数据时具有显著的时间优势。

### 5. 实验数量与充分性
*   **实验规模**：研究涵盖了跨物种（小鼠到人）、跨场景（实验室行为实验到临床诊断）的多组实验。
*   **消融实验**：系统对比了“单受试者训练”与“池化训练”的效果，验证了池化策略对泛化性的贡献。
*   **充分性评价**：实验设计非常充分且具有客观性。研究不仅关注计算机视觉指标（如 IoU），更通过下游的神经科学任务（预测皮层神经元活动）验证了工具的实际科研价值，这在同类论文中较为少见。

### 6. 主要结论与发现
*   **泛化性突破**：NeuroPupil 在无需针对新视频进行手动标注的情况下，表现优于经过精调的传统模型。
*   **效率提升**：其处理速度支持大规模筛选，使得分析数 TB 级的神经科学视频数据成为可能。
*   **生物学关联**：更高精度的瞳孔追踪显著提升了对大脑皮层状态的预测能力。在人类临床数据中，NeuroPupil 能够精准捕捉到具有诊断意义的微小瞳孔震颤和反应延迟。

### 7. 优点
*   **易用性**：实现了“开箱即用”，极大降低了神经科学家的标注负担。
*   **跨物种能力**：一套框架同时适用于啮齿类和人类，证明了瞳孔特征提取的通用性。
*   **鲁棒性**：对光照变化、遮挡（如睫毛、反光）具有极强的抵抗力。
*   **开源贡献**：提供了完整的软件工具包，促进了实验结果的可重复性。

### 8. 不足与局限
*   **极端情况限制**：虽然泛化性强，但在极度异常的病理眼球（如严重眼外伤或瞳孔畸形）上可能仍需少量数据微调。
*   **计算门槛**：尽管推理快，但初始的大规模池化训练需要较强的算力和高质量的标注数据集作为支撑。
*   **偏差风险**：如果训练池中的受试者多样性不足（例如缺乏特定族裔或特定光照条件），模型在极端边缘案例上的表现可能会下降。

（完）
