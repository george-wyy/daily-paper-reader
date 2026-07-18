---
title: Information-dependent eye-hand coordination emerges from active vision
title_zh: 信息依赖的眼手协调源于主动视觉
authors: "Zhao, J., VERDEL, D., Tan, Y., Burdet, E."
date: 2026-07-17
pdf: "https://www.biorxiv.org/content/10.64898/2026.05.29.726887v2.full.pdf"
tags: ["query:gaze-intent"]
score: 9.0
evidence: 基于随机模型预测控制的主动视觉，用于眼动驱动的预判性手部运动规划
tldr: 人类在连续任务中通过眼动获取信息以协调手部动作，但眼手协调的计算原理尚不明确。本文提出双随机模型预测控制框架，将眼动建模为连续优化以最小化任务相关不确定性并构建内部模型指导手部运动。实验显示该模型自然涌现扫视-追视模式，准确预测不同信息条件下的眼手运动特征，且提取视界保持恒定。该工作为理解主动视觉中的眼手协调提供了统一计算框架，对机器人辅助和主动感知有启示意义。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-05-29-726887-v2/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1286, \"height\": 731, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-05-29-726887-v2/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1399, \"height\": 1076, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-05-29-726887-v2/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1248, \"height\": 1106, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-05-29-726887-v2/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1169, \"height\": 1563, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-05-29-726887-v2/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1175, \"height\": 1138, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-05-29-726887-v2/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 687, \"height\": 341, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-05-29-726887-v2/fig-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 1472, \"height\": 560, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-05-29-726887-v2/fig-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 1828, \"height\": 802, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-05-29-726887-v2/fig-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 1833, \"height\": 799, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-05-29-726887-v2/fig-010.webp\", \"caption\": \"\", \"page\": 0, \"index\": 10, \"width\": 1829, \"height\": 800, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-05-29-726887-v2/fig-011.webp\", \"caption\": \"\", \"page\": 0, \"index\": 11, \"width\": 1831, \"height\": 801, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-05-29-726887-v2/fig-012.webp\", \"caption\": \"\", \"page\": 0, \"index\": 12, \"width\": 1832, \"height\": 803, \"label\": \"Figure\"}]"
tables_json: "[{\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-05-29-726887-v2/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1568, \"height\": 2216, \"label\": \"Table\"}]"
motivation: 缺乏解释连续任务中眼手协调模式涌现的统一计算原理。
method: 提出双随机模型预测控制框架，眼动连续优化不确定性并构建手部规划内部模型。
result: 模型涌现扫视-追视模式，准确预测不同信息密度和难度下的眼手运动特征。
conclusion: 为理解人类眼动调节提供原则框架，开拓机器人辅助和主动感知应用。
---

## 摘要
在日常活动中，人类依赖视觉信息来规划手部运动，因此通过眼睛注视提取任务相关信息成为运动控制的关键。行为研究揭示了特征性的扫视-追踪模式，这些模式很可能由共享的神经回路控制，能够有效降低任务相关的不确定性。然而，目前仍缺乏一个统一的计算原理来解释这些模式在连续任务（如阅读或驾驶）中的产生。本文提出了主动视觉的双随机模型预测控制框架，其中眼动被持续控制以最小化任务相关不确定性，并构建用于手部运动规划的内部模型。通过操控未来视觉信息的数量、密度和难度的实验，我们展示了眼动模式如何适应信息上下文，同时保持不变的提取视界。扫视-追踪模式自然地从模型中产生，准确预测了实验中观察到的眼动和手部运动特征。这些结果为理解人类眼动的连续调节提供了原则性框架，并为机器人辅助和主动感知应用开辟了新视角。

## Abstract
In daily activities, humans rely on visual information to plan hand movements, making the extraction of task-relevant information through eye gaze a key aspect of motor control. Behavioral studies have revealed characteristic saccade-pursuit patterns, likely governed by shared neural circuits, which enable an efficient reduction of task-related uncertainty. However, a unifying computational principle explaining the emergence of these patterns in continuous tasks such as reading or driving is still lacking. Here we propose a dual stochastic model predictive control formulation of active vision, in which eye movements are continuously controlled to minimize task-relevant uncertainty and build an internal model used for hand movement planning. Through experiments manipulating the amount, density, and difficulty of future visual information, we show how eye movement patterns adapt to the information context while maintaining an invariant extraction horizon. A saccade-pursuit pattern naturally emerges from the model, which accurately predicts both eye and hand movement features observed in experiments. These results provide a principled framework for understanding the continuous regulation of human eye movements and open new perspectives for applications in robotic assistance and active perception.

---

## 论文详细总结（自动生成）

好的，以下是对所提供论文的详细中文总结。

### 1. 论文的核心问题与整体含义（研究动机和背景）

*   **核心问题**：人类在进行连续动作（如阅读、驾驶、抓取）时，眼睛和手如何进行无缝协调？尽管学界对手部运动控制原理（如最小化能量或不确定性）已有深入理解，但控制眼动以获取信息进而指导手部动作的计算原则仍不清楚。现有的眼动模型往往将扫视和平滑追踪视为两个独立过程，无法解释它们如何在一个统一的机制下涌现。
*   **研究意义**：论文试图提出一个统一的计算框架（主动视觉原则），来解释人类如何通过控制眼动（注视）来有效地获取任务相关信息（即降低不确定性），并利用这些信息构建内部模型以规划和执行手部动作。这项工作不仅加深了对人脑运动控制底层机制的理解，也为开发更智能的机器人、辅助系统和主动感知技术提供了理论基础。

### 2. 论文提出的方法论：核心思想、关键技术细节

*   **核心思想**：论文提出了一个**双随机模型预测控制（Dual Stochastic Model Predictive Control, MPC）** 框架。该框架的核心假设是：中枢神经系统（CNS）通过一个连续优化过程来控制眼动，目标是在能量消耗的约束下，最小化与任务相关的不确定性。获取的视觉信息随后被用于构建内部模型，并指导手部运动的规划。
*   **关键技术细节**：
    1.  **眼动控制**：眼动的目标是选择一个注视点，以最小化成本和。
        *   成本函数 \( G(\mathbf{u}_g) = \int (U_e + U_h + W_g) dt \)，其中：
            *   \( U_e \)：环境不确定性，指对未来的目标轨迹估计的不确定性。
            *   \( U_h \)：手部不确定性，指对手部自身状态估计的不确定性。
            *   \( W_g \) ：眼动能量消耗。
        *   为了模拟人类的视觉特性，模型引入了**偏心度依赖的视觉噪声**：离注视中心越远，视觉噪声越大（\(\sigma(d) = a d^2 + b\)），这符合人类视网膜中央凹分辨率高、周边分辨率低的生理特点。
    2.  **内部状态估计**：中枢神经系统利用当前和过去的视觉观测（并考虑200毫秒的感觉延迟）以及自身运动指令的副本，通过一个状态估计器（如卡尔曼滤波器）来更新对环境和手部状态的估计。
    3.  **手部运动控制**：手部的运动是基于内部模型对未来状态的预测来规划的，目标是同时最小化轨迹跟踪误差和能量消耗。
        *   成本函数 \( H(\mathbf{u}_h) = \int (V_t + W_h) dt \)，其中 \( V_t \) 代表任务性能（跟踪误差），\( W_h \) 代表手部能量消耗。
    4.  **模型输出**：通过这个统一的优化过程，模型在没有显式切换机制的情况下，**自然涌现出类似人类行为的扫视-追踪模式**。扫视用于在目标漂离中央凹时，将注视点快速“重置”到高价值区域，而平滑追踪则允许在中央凹内进行连续的信息整合，以降低状态估计的不确定性。

### 3. 实验设计：数据集、场景与对比方法

*   **任务场景**：一个**轨迹追踪任务**。被试者需要控制腕部屈伸运动，移动屏幕上的光标（手）去追踪一个在有限滑动时间窗口内显示的、向下滚动的目标轨迹。
*   **数据集**：论文采集了**17名健康人类被试者**的眼动和手部运动数据。
*   **实验操纵（自变量）**：为了验证模型，实验系统地操纵了三个影响获取信息的变量，模拟了9种实验条件（3个变量 × 3个水平）：
    1.  **视界**：未来轨迹显示的时间长度（80%, 50%, 20% 的基准值）。
    2.  **运动频率**：目标轨迹的形状频率（0.5倍, 1倍, 2倍基准值）。
    3.  **滚动速度**：目标轨迹下滚的速度（0.5倍, 1倍, 2倍基准值）。
*   **Benchmark与对比方法**：
    *   论文**没有与任何其他计算方法进行对比**。核心的实验范式是将**模型的预测行为**与**真实人类的实验数据**进行对比，以验证模型的有效性。模型本身是其自身的benchmark。
    *   模型参数的选取是通过拉丁超立方体采样进行随机搜索，选出最符合6个行为指标（注视超前时间、水平距离、扫视频率、追踪持续时间、手部RMSE、总肌肉激活）的平均人类模式的参数集。

### 4. 资源与算力

*   **未明确说明**。论文中没有提及训练模型所需的GPU型号、数量或具体训练时长。模型是一个控制算法，其参数是通过搜索和拟合人类数据确定的，而不是通过深度学习训练的。

### 5. 实验数量与充分性

*   **实验数量**：相当充分。
    *   **行为实验**：17名被试者，在3个条件下的9个变体中进行了重复试验，每个被试者完成了38个试次（包括基线、试次间清洗等），数据量较为丰富。
    *   **仿真实验**：模型在同样的9种实验条件下进行了模拟，并对每个条件重复多次。
    *   **参数敏感性分析**：在附录中，论文对模型的7个超参数进行了敏感性分析，检验了参数扰动对模型输出（6个指标）的影响。
*   **充分性与客观性**：
    *   **优点**：实验条件设计系统，涵盖了信息的“数量”、“密度”和“获取难度”三个关键维度，能够全面地检验模型在不同情况下的适应性。36个预测（9个条件 × 4个眼动指标）基本被实验数据所证实，表明框架具有很强的解释力。
    *   **局限性**：实验完全依赖于一个特定的轨迹追踪任务。虽然这能很好地控制变量，但其生态效度可能有限，无法完全代表如驾驶、运动等更复杂、更自然的眼手协调场景。

### 6. 论文的主要结论与发现

1.  **统一框架**：一个基于“最小化任务相关不确定性”和“最优控制”的主动视觉原则，能够统一地解释眼-手协调中的扫视-追踪模式。
2.  **模型预测准确**：模型定量地预测了人类在不同信息条件下的眼动和手部行为，特别是保持了大约**200毫秒**的这个**相对恒定的信息提取超前时间**。
3.  **适应性行为**：
    *   当**视界减小时**，注视点被迫向当前手部位置靠近，导致手部跟踪误差增大。
    *   当**运动频率增加时**（信息密度大），眼球表现出一种“低通滤波”效应，跳过轨迹的“峰值”，只跟踪主要轮廓，这在高信息密度下是一种节省眼动能量的策略。
    *   当**滚动速度增加时**（信息获取难度大），注视点不得不抬升以获得足够的前瞻时间，但由于眼动能量成本增加，注视点与目标轨迹的距离（Dist）会增大。
4.  **统一的神经基础**：此项工作支持了神经科学中关于扫视和追踪共享神经通路的假说。

### 7. 优点：方法或实验设计上的亮点

*   **理论创新**：提出了一个真正意义上的统一计算框架，将眼动控制从传统的“反应式”模型提升为“主动、预测性”的信息采集过程，并成功模拟了扫视和追踪两种行为的内在联系，而不是将其视为离散模块。
*   **模型的可解释性**：模型的每个组成部分（视觉噪声、状态估计、成本函数）都有明确的神经生理学或生物力学依据，如偏心度噪声、感觉延迟、肌肉动力学等，使得模型预测与行为结果之间的因果关系清晰。
*   **实验设计的精巧**：通过对“视界”、“频率”、“速度”三个变量的独立操控，精准地剥离了信息采集过程的“数量”、“密度”和“难度”，从而能够有力地验证模型在不同维度上的预测，特别是发现了“恒定超前时间”和“滤波效应”这些非平凡的预测。
*   **兼顾准确率和简洁性**：模型虽然简化了眼球和手部的复杂动力学（如忽略肌肉的非线性），但其行为预测在定性和定量上都与人类数据高度吻合，证明了核心原理的有效性，避免了不必要的复杂性。

### 8. 不足与局限

*   **模型的简化**：
    *   **眼动模型**：忽略了垂直和水平方向上的运动差异，以及微扫视等精细调节。
    *   **手部模型**：使用了简单的三阶线性模型，未能捕捉到神经肌肉系统中的阻抗调节、信号依赖噪声等复杂特性。这可能是模型高估手部在最高滚动速度条件下表现的原因（低估了跟踪误差）。
*   **实验任务的局限性**：任务非常具体（屏幕上的滚动轨迹追踪）。结论是否适用于更复杂的3D空间眼手协调任务（如体育运动、外科手术）还有待验证。
*   **缺乏与其他方法的直接竞争**：论文的核心贡献是提出了一个统一框架，但没有与任何现有的、处理单一扫视或追踪问题的模型进行直接、定量的性能对比（如预测的准确性）。这限制了模型“更具优势”的说服力。
*   **计算负担**：虽然未提，但随机MPC的全过程连续求解（特别是面对高维信息空间）在实际应用中可能计算开销较大，需要进一步优化才能实现实时应用。

（完）
