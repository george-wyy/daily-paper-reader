---
title: "Web-based eye-tracking for remote cognitive assessments: The anti-saccade task as a case study"
title_zh: 基于 Web 的眼动追踪用于远程认知评估：以反向眼跳任务为案例研究
authors: "Juantorena, G. E., Figari, F., Petroni, A., Kamienkowski, J. E."
date: 2026-04-30
pdf: "https://www.biorxiv.org/content/10.1101/2023.07.11.548447v2.full.pdf"
tags: ["query:gaze-intent"]
score: 8.0
evidence: 用于远程认知任务的基于网络摄像头的眼动追踪原型，无需持续鼠标交互
tldr: 本研究开发了一种新型基于网页摄像头的远程眼动追踪原型，旨在解决远程认知评估中设备质量低和环境噪声大的挑战。该原型改进了现有技术，无需频繁鼠标交互，并具有稳定的校准性能。通过反向眼跳任务的实验验证，成功复现了实验室高精度眼动仪的结果，证明了其在远程医疗和大规模认知研究中的应用潜力。
source: biorxiv
selection_source: fresh_fetch
motivation: 旨在克服传统实验室眼动追踪的局限性，开发一种适用于远程认知评估和临床应用的高效网页端眼动追踪工具。
method: 提出了一种改进的网页摄像头眼动追踪原型，并通过反向眼跳任务评估其时空分辨率、可靠性及在抑制性控制测量中的表现。
result: 实验成功复现了反向眼跳错误率高于正向眼跳的经典发现，且该原型在长时间实验中表现出稳定的校准能力。
conclusion: 该网页端眼动追踪原型在认知实验中具有良好的功能性和可靠性，为远程临床评估和大规模心理学研究提供了可行方案。
---

## 摘要
过去几年中，出现了几种基于远程网络摄像头的眼动追踪（ET）原型，旨在测试其在基于 Web 的实验中的可行性和潜力。这种日益增长的关注主要源于远程执行任务的可能性，这使得研究更大规模且难以触及的人群以及在远程医疗中的潜在应用成为可能。然而，摄像头质量的下降和更复杂的环境噪声带来了新的实施挑战。在本研究中，我们提出了一种新型的基于远程网络摄像头的 ET 原型。首先，我们对用于认知和临床任务的最先进远程 ET 原型进行了改进，例如消除了持续鼠标交互的必要性。其次，我们评估了其时空分辨率及其在实验中的可靠性。第三，我们运行了一个经典实验——反向眼跳（anti-saccade）任务，以评估其功能和局限性。这一认知测试通过比较朝向目标（正向眼跳）或背离目标（反向眼跳）的水平眼动，作为抑制控制的一种衡量指标。我们的结果复现了以往使用高质量实验室 ET 设备获得的研究结果。简而言之，观察到反向眼跳的错误率高于正向眼跳，且错误反应表现出更快的反应时间。我们的 Web-ET 原型显示出随时间稳定的校准性能，并在经典认知实验中表现良好。最后，我们讨论了该原型在临床应用中的潜力及其在实验使用中的局限性。

## Abstract
Over the last years, several developments of remote webcam-based eye tracking (ET) prototypes have emerged, testing their feasibility and potential for web-based experiments. This growing interest is mainly explained by the possibility to perform tasks remotely, which allows the study of larger and hard-to-reach populations and potential applications in telemedicine. Nevertheless, a decrease in the quality of the camera and a noisier environment brings new implementation challenges. In this study, we present a new prototype of remote webcam-based ET. First, we introduced improvements to the state-of-the-art remote ET prototypes for cognitive and clinical tasks, e.g. without the necessity of constant mouse interactions. Second, we assessed its spatiotemporal resolution and its reliability within an experiment. Third, we ran a classical experiment, the anti-saccade task, to assess its functionality and limitations. This cognitive test compares horizontal eye movements toward (pro-saccades) or away from (anti-saccades) a target, as a measure of inhibitory control. Our results replicated previous findings obtained with high-quality laboratory ETs. Briefly, higher error rates in anti-saccades compared to pro-saccades were observed, and incorrect responses presented faster reaction times. Our web-ET prototype showed a stable calibration over time and performed well in a classic cognitive experiment. Finally, we discussed the potential of this prototype for clinical applications and its limitations for experimental use.

---

## 论文详细总结（自动生成）

这篇论文介绍了一种用于远程认知评估的新型基于 Web 的眼动追踪（Eye-Tracking, ET）原型，并以“反向眼跳任务”为例验证了其有效性。以下是对该论文的结构化总结：

### 1. 核心问题与整体含义（研究动机和背景）
*   **核心问题**：传统的眼动追踪研究依赖昂贵的实验室设备，限制了样本量和人群覆盖面（如偏远地区或行动不便的临床患者）。虽然现有的基于网页摄像头的 ET 技术（如 WebGazer.js）提供了远程可能性，但在**空间精度、校准稳定性以及对用户交互的依赖性**（如频繁点击鼠标）方面存在不足。
*   **研究背景**：随着远程医疗和大规模在线心理学实验的需求增加，开发一种无需特殊硬件、低侵入性且能可靠捕捉认知指标（如抑制性控制）的工具变得至关重要。

### 2. 论文提出的方法论
*   **核心思想**：基于现有的开源库 **WebGazer.js** 进行改进，构建了一个专门用于认知任务的 Web-ET 原型，重点优化了用户体验和数据质量。
*   **关键技术细节**：
    *   **改进校准机制**：传统的 WebGazer 需要用户在实验中不断点击鼠标来维持校准。本研究改进了算法，使其在初始 9 点校准后，无需持续的鼠标交互即可维持较长时间的稳定性。
    *   **数据预处理流程**：包括坐标平滑处理、眨眼检测与剔除、以及基于速度和位置阈值的眼跳（Saccade）检测算法。
    *   **任务集成**：将眼动追踪逻辑与基于 JavaScript 的心理学实验框架（如 jsPsych）集成，确保刺激呈现与眼动数据采集的同步。

### 3. 实验设计
*   **实验场景**：远程在线环境，参与者在自己的电脑上通过浏览器完成任务。
*   **核心任务：反向眼跳任务（Anti-saccade Task）**：
    *   **正向眼跳（Pro-saccade）**：看向屏幕上突然出现的目标（本能反应）。
    *   **反向眼跳（Anti-saccade）**：看向目标的镜像对称位置（需要抑制本能反应，衡量抑制控制能力）。
*   **Benchmark（基准）**：对比实验室环境下高精度眼动仪（如 EyeLink）的经典研究结果。
*   **参与者**：30 名健康成年人。

### 4. 资源与算力
*   **算力说明**：论文未明确提到高性能 GPU 或大规模训练时长。
*   **技术栈**：该原型主要基于客户端 JavaScript 运行，利用参与者本地设备的 CPU 进行实时面部特征检测和坐标映射。这体现了该方法对计算资源要求较低，具有良好的普适性。

### 5. 实验数量与充分性
*   **实验规模**：30 名参与者，每人完成 240 次试验（120 次正向，120 次反向），总计产生数千个眼跳数据点。
*   **充分性评价**：
    *   **统计效力**：实验成功复现了显著的“反向眼跳效应”，证明了样本量足以捕捉核心认知指标。
    *   **稳定性测试**：通过在实验开始、中期和结束设置校准检查点，验证了系统在 20 分钟实验流程中的稳定性。
    *   **客观性**：采用了自动化的数据清洗和分析脚本，减少了人为干预。

### 6. 论文的主要结论与发现
*   **成功复现经典效应**：反向眼跳的错误率显著高于正向眼跳（符合预期）；且错误反应（看向目标）的反应时间比正确反应（看向反方向）更快。
*   **校准稳定性**：改进后的原型在无需中途干预的情况下，空间精度在整个实验过程中保持稳定，平均误差维持在可接受范围内（约 2-4 度视角）。
*   **可行性验证**：证明了普通网页摄像头（约 30Hz 采样率）足以捕捉到足以区分认知状态的眼动特征。

### 7. 优点
*   **低成本与高可及性**：无需额外硬件，极大降低了临床筛查和大规模心理学研究的门槛。
*   **用户体验优化**：消除了实验过程中繁琐的鼠标点击，使任务更接近自然认知状态。
*   **鲁棒性**：在参与者设备多样、光照环境不一的远程条件下，依然获得了可靠的统计结果。

### 8. 不足与局限
*   **时空分辨率限制**：相比实验室设备（500-1000Hz），网页摄像头（30Hz）无法捕捉微小的眼动细节（如微眼跳）或精确的眼跳动力学特征。
*   **环境敏感性**：极差的光照条件或参与者剧烈的头部运动仍会显著降低数据质量。
*   **人群偏差**：远程实验可能排除掉不熟悉电脑操作或没有网络设备的特定人群。
*   **精度瓶颈**：空间精度（约 2° 以上）尚不足以支持需要极高精细注视分析的任务（如阅读研究）。

（完）
