---
title: fMRI-Based Prediction of Eye Gaze During Naturalistic Movie Viewing Reveals Eye-Movement-Related Brain Activity
title_zh: 基于 fMRI 的自然电影观看期间视线预测揭示了眼动相关的脑活动
authors: "Gao, L., Wei, Z., Biswal, B. B., Di, X."
date: 2026-04-12
pdf: "https://www.biorxiv.org/content/10.64898/2026.01.10.698820v2.full.pdf"
tags: ["query:gaze-intent"]
score: 8.0
evidence: 利用深度学习预测自然观看过程中的眼动注视
tldr: 本研究探讨了在缺乏眼动追踪数据的情况下，利用深度学习模型（DeepMReye）从fMRI眼球信号中预测自然观影时视线轨迹的可行性。通过在三个独立数据集上进行零样本测试，发现该模型在个体层面预测精度有限，但在群体平均层面表现出极高的可靠性，并能成功识别出额叶和顶叶眼动区等大脑激活区域。这为分析缺乏眼动记录的自然神经影像数据提供了有效工具。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-01-10-698820-v2/fig-001.webp\", \"caption\": \"Figure 4. Intersubject similarity and variability of gaze patterns in the Partly Cloudy dataset. 319 (a–b) Intersubject correlation matrices within the PC dataset revealed increasingly structured alignment of 320 predicted gaze trajectories with increasing age for horizontal (a) and vertical (b) gaze components. (c–d) 321 Scatter plots showing the relationship between age and correlation strength for horizontal (c) and vertical 322 (d) gaze components. Solid lines indicate linear regression fits, and shaded regions represent 95% 323 confidence intervals. Red lines indicate statistically significant age effects (p < 0.05). 324\", \"page\": 15, \"index\": 1, \"width\": 1054, \"height\": 339}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-01-10-698820-v2/fig-002.webp\", \"caption\": \"Table 1. Summary of datasets used in this study. 145\", \"page\": 7, \"index\": 2, \"width\": 979, \"height\": 221}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-01-10-698820-v2/fig-003.webp\", \"caption\": \"Figure 3. Cross-dataset comparison of group-mean gaze trajectories and age-related correlation 292 patterns between the ground-truth of the Natural Viewing (NV) dataset and the predicted gaze of 293 the Healthy Brain Network (HBN) dataset. 294 (a, d) Group-averaged gaze trajectories for the cross-dataset comparison between NV ground-truth eye 295 tracking (blue) and HBN predicted gaze signals (red) in the Despicable Me (DM) and The Present (TP) 296 tasks, respectively. Solid lines represent the mean across subjects within each dataset, and shaded regions 297 indicate ±1 standard deviation. Horizontal and vertical gaze components are shown separately. 298\", \"page\": 14, \"index\": 3, \"width\": 1054, \"height\": 612}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-01-10-698820-v2/fig-004.webp\", \"caption\": \"Figure 6. Modulation of Gaze-Related Brain Activity by Age. 412\", \"page\": 19, \"index\": 4, \"width\": 1054, \"height\": 365}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-01-10-698820-v2/fig-005.webp\", \"caption\": \"Figure 5. Main Effect of Gaze Displacement on Whole-Brain Activation. The figure shows regions 356 where brain activity was significantly and positively correlated with individual-level and group-averaged 357 gaze displacement. Activation using group-averaged gaze prediction of (a) Despicable Me (DM) stimulus 358 of the Healthy Brain Network (HBN) dataset, (b) The Present (TP) stimulus of the HBN dataset, and (c) 359 Partly Cloudy (PC) dataset. Activation using individual gaze prediction of (d) DM stimulus of the HBN 360 dataset, (e) TP stimulus of the HBN dataset, and (f) PC dataset. Warm colors indicate a stronger positive 361 correlation, and cold colors indicate negative correlations. 362\", \"page\": 17, \"index\": 5, \"width\": 1054, \"height\": 448}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-01-10-698820-v2/fig-006.webp\", \"caption\": \"Figure 2. Validation of DeepMReye gaze predictions against ground-truth eye-tracking data. 260 (a, d) Group-averaged horizontal and vertical gaze trajectories for the Natural Viewing (NV) dataset in 261 the Despicable Me (DM) and The Present (TP) tasks. Solid lines represent the mean across subjects, and 262 shaded regions indicate ±1 standard deviation. 263 (b, e) Subject-level Pearson correlation coefficients between predicted and ground-truth gaze signals for 264 horizontal and vertical components. 265 (c, f) Subject-level mean absolute error (MAE) in degrees of visual angle, reported separately for 266 horizontal and vertical components. 267\", \"page\": 12, \"index\": 6, \"width\": 1054, \"height\": 492}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-01-10-698820-v2/fig-007.webp\", \"caption\": \"Figure 1. Study workflow for fMRI-based gaze decoding and downstream analyses. Eyeball fMRI 102 voxels were extracted from three naturalistic viewing datasets—Natural Viewing (NV; brown), Healthy 103 Brain Network (HBN; green), and Partly Cloudy (PC; purple)—following motion correction and template 104 alignment. A pre-trained DeepMReye model then performed zero-shot inference to extract predicted gaze 105 paths. These predictions underwent several levels of evaluation and downstream analysis: (1) Validation:106 NV predictions were compared against ground-truth camera-based eye-tracking data using correlation and107 Mean Absolute Error (MAE). (2) Consistency: Cross-dataset consistency was evaluated by correlating 108 HBN predictions with NV ground-truth data for shared video stimuli, while inter-subject correlation (ISC109 assessed cross-individual consistency in the independent PC dataset. (3) Brain Mapping: Gaze 110\", \"page\": 5, \"index\": 7, \"width\": 1054, \"height\": 494}]"
motivation: 旨在评估预训练深度学习模型在无需特定数据集微调的情况下，从fMRI信号预测自然观影视线轨迹的泛化能力及其实用性。
method: 采用DeepMReye框架的预训练模型，在三个独立fMRI数据集上进行零样本视线预测，并结合广义线性模型分析相关的脑活动。
result: 个体预测准确度较低，但群体平均预测与真实值高度相关（r达0.73-0.84），且能准确映射出经典的动眼神经控制脑区。
conclusion: 零样本fMRI视线预测虽不适用于个体推断，但能有效捕捉群体共享的观看行为，是研究无眼动记录数据集脑活动的可靠手段。
---

## 摘要
背景：在自然电影观看过程中，视线为感知和认知过程提供了关键见解，但在功能磁共振成像（fMRI）研究中，同步眼动追踪往往不可用。虽然深度学习模型可以直接从 fMRI 眼球信号中估计视线，但其在异质数据集上的开箱即用泛化能力仍需实证评估。方法：我们在零样本（zero-shot）设置下（即不进行特定数据集的微调），应用了 DeepMReye 框架中的特定预训练模型，来估计三个独立 fMRI 数据集在电影观看期间的视线。通过与基于摄像头的眼动追踪数据对比以及受试者间相关性来评估模型准确性。此外，我们从预测的视线信号中推导出眼动相关的时间序列，以绘制相关的脑激活图。结果：在个体层面，预测的视线与实测的地面真值（ground-truth）数据表现出中等程度的相关性（r ≈ 0.24-0.37），生成的脑激活图主要局限于视觉皮层。相比之下，群体平均的视线预测表现出显著更高的可靠性（r ≈ 0.73-0.84）。基于群体平均预测的一级广义线性模型（GLMs）成功揭示了已确定的动眼神经控制区域的广泛激活，包括额叶和顶叶眼动区。关于年龄对视线预测和脑活动影响的探索性分析在不同数据集中得出了不一致的结果。结论：在零样本应用下，预训练模型在个体层面的推断中表现出局限性，这可能反映了缺乏特定数据集的训练。然而，基于 fMRI 的群体平均视线估计成功捕捉到了共同的观看行为，并有力地支持了对眼动相关脑活动的研究。这些发现为在缺乏地面真值眼动追踪记录的自然神经影像数据集中，如何恰当使用基于 fMRI 的视线解码提供了参考。

## Abstract
Background: Eye gaze provides crucial insights into perceptual and cognitive processes during naturalistic movie viewing, yet concurrent eye tracking is often unavailable in functional MRI (fMRI) research. While deep learning models can estimate gaze directly from fMRI eyeball signals, their out-of-the-box generalizability across heterogeneous datasets requires empirical evaluation. Methods: We applied a specific pre-trained model from the DeepMReye framework in a zero-shot setting (without dataset-specific fine-tuning) to estimate gaze during movie watching across three independent fMRI datasets. Model accuracy was evaluated against camera-based eye-tracking data and via inter-subject correlations. Furthermore, we derived eye-movement-related time series from the predicted gaze signals to map their associated brain activation. Results: At the individual level, predicted gaze showed modest correspondence with measured ground-truth data (r {approx} 0.24-0.37), yielding brain activation maps largely restricted to the visual cortex. In contrast, group-averaged gaze predictions exhibited substantially higher reliability (r {approx} 0.73-0.84). First-level General Linear Models (GLMs) derived from group-averaged predictions successfully revealed widespread activation across established oculomotor control regions, including the frontal and parietal eye fields. Exploratory analyses of age-related effects on gaze prediction and brain activity yielded inconsistent results across datasets. Conclusions: Under a zero-shot implementation, the pre-trained model exhibits limitations for individual-level inference, likely reflecting the absence of dataset-specific training. However, group-averaged fMRI-based gaze estimates successfully capture shared viewing behaviors and robustly support the investigation of eye-movement-related brain activity. These findings inform the appropriate use of fMRI-based gaze decoding for naturalistic neuroimaging datasets lacking ground-truth eye-tracking logs.

---

## 论文详细总结（自动生成）

这篇论文对基于 fMRI 信号预测自然观影期间视线轨迹的技术进行了深入评估，以下是详细的结构化总结：

### 1. 核心问题与整体含义
*   **研究动机**：眼动行为是理解人类感知和认知的关键窗口，但在许多大规模公开的 fMRI 数据集或早期研究中，往往缺乏同步的眼动追踪记录。
*   **核心问题**：评估深度学习模型（如 DeepMReye）在“零样本”（Zero-shot，即不进行特定数据集微调）设置下，从 fMRI 眼球信号中预测视线轨迹的泛化能力，以及这些预测信号在揭示眼动相关脑活动方面的有效性。

### 2. 方法论
*   **核心思想**：利用预训练的卷积神经网络（CNN）模型，将 fMRI 扫描中眼球区域的信号变化解码为屏幕上的视线坐标（x, y）。
*   **关键技术流程**：
    1.  **眼球体素提取**：对 fMRI 数据进行运动校正和模板对齐，提取标准化的眼球区域体素信号。
    2.  **零样本推理**：直接应用 DeepMReye 官方提供的预训练权重进行预测，模拟在完全没有眼动真值的数据集上的应用场景。
    3.  **视线位移计算**：计算相邻时间点预测坐标之间的欧几里得距离（Euclidean distance），作为眼动强度的指标。
    4.  **脑活动映射**：将视线位移时间序列与 BOLD 信号进行卷积，利用广义线性模型（GLM）识别与眼动相关的脑区。

### 3. 实验设计
*   **数据集**：
    *   **NV (Natural Viewing)**：22名成年人，包含同步摄像头眼动追踪数据（作为地面真值/Benchmark）。
    *   **PC (Partly Cloudy)**：82名受试者（3-39岁），无眼动数据，用于发育研究。
    *   **HBN (Healthy Brain Network)**：约80名受试者（5-21岁），无眼动数据，具有高时间分辨率（TR=0.8s）。
*   **对比维度**：
    *   **个体 vs. 群体**：对比个体预测精度与群体平均预测精度。
    *   **跨数据集一致性**：用 HBN 的预测结果与 NV 的真值进行跨样本比对。
    *   **脑图对比**：对比基于个体预测和群体平均预测生成的脑激活图。

### 4. 资源与算力
*   **说明**：论文中**未明确说明**具体的 GPU 型号、数量或训练时长。由于该研究主要采用预训练模型进行推理（Inference）而非从头训练，其对算力的需求相对较低，主要集中在 fMRI 图像预处理和 GLM 统计建模上。

### 5. 实验数量与充分性
*   **实验规模**：涵盖了三个独立数据集，涉及不同的电影刺激（《The Present》、《Despicable Me》、《Partly Cloudy》）、不同的扫描参数（TR 从 0.8s 到 2.1s）以及广泛的年龄跨度。
*   **充分性评价**：实验设计较为充分且客观。作者不仅验证了预测精度，还通过下游的脑功能分析验证了预测信号的生物学意义。通过受试者间相关性（ISC）和跨数据集验证，增强了结论的稳健性。

### 6. 主要结论与发现
*   **精度差异**：在零样本设置下，个体层面的预测精度中等（相关性 $r \approx 0.24-0.37$），但**群体平均预测表现出极高的可靠性**（相关性 $r \approx 0.73-0.84$）。
*   **脑网络识别**：基于群体平均预测的回归分析成功识别出了经典的**动眼神经控制网络**（包括额叶眼动区 FEF 和顶内沟 IPS），而个体层面的预测仅能识别出视觉皮层。
*   **发育效应**：发现视线同步性随年龄增长而增加；眼动相关的脑活动随年龄呈现非线性变化（如倒 U 型或持续下降），且这种变化受电影内容的影响。

### 7. 优点
*   **实用性强**：为缺乏眼动追踪硬件的实验室提供了一种“事后补偿”的低成本方案。
*   **群体平均策略**：巧妙地证明了通过群体平均可以抵消个体预测中的解剖和运动噪声，从而提取出稳健的刺激驱动信号。
*   **生物学验证**：不仅停留在算法精度上，还通过脑图谱验证了预测信号的神经生理一致性。

### 8. 不足与局限
*   **个体推断受限**：由于缺乏特定数据集的微调，该模型目前不适用于需要精确个体视线分析的临床诊断（如个体注视点分析）。
*   **时间分辨率瓶颈**：fMRI 的采样率（TR）远低于眼动发生的频率，无法捕捉快速扫视（Saccades）的细节。
*   **领域偏移（Domain Shift）**：不同扫描仪、序列参数和人群解剖差异对个体预测精度影响显著，零样本模型的泛化边界仍清晰可见。

（完）
