---
title: Pupil and Neural Dynamics Reveal Belief-Dependent Decision Making Under Ambiguity
title_zh: 瞳孔与神经动力学揭示模糊情境下基于信念的决策
authors: "Qin, Y., Rungratsameetaweemana, N., Lauharatanahirun, N., Sajda, P."
date: 2026-04-23
pdf: "https://www.biorxiv.org/content/10.64898/2026.04.21.719818v1.full.pdf"
tags: ["query:gaze-intent"]
score: 8.5
evidence: 结合瞳孔测量和脑电数据的多模态决策研究
tldr: 本研究探讨了人类在模糊性（概率未知）下的决策机制。通过结合行为学、瞳孔测量和脑电图（EEG）的多模态方法，研究发现个体在面对模糊结果时会采用不同的决策策略，这些策略反映了其内部的主观信念。研究揭示了瞳孔唤醒水平追踪的是主观信念而非客观任务结构，证明了模糊规避并非统一的偏差，而是异质性内部信念模型的体现，为理解价值决策提供了生理学视角。
source: biorxiv
selection_source: fresh_fetch
motivation: 旨在探究个体在模糊环境下如何内部表征未知结果，以及这些表征如何影响其行为和生理反应。
method: 采用结合行为实验、瞳孔测量和脑电图（EEG）的多模态研究方法，分析风险与模糊条件下的价值决策。
result: 发现个体的决策策略反映了不同的内部信念，且瞳孔唤醒水平与主观信念而非客观任务结构紧密相关。
conclusion: 模糊规避并非单一的认知偏差，而是源于异质性的内部信念模型，多模态生理数据为揭示这些信念引导决策的机制提供了重要窗口。
---

## 摘要
人类每天在模糊情境下做出数千次决策，在大多数情况下，获得有利结果的概率并不完全已知。尽管模糊规避在群体层面已得到很好的刻画，但个体如何在内部表征模糊结果，以及这些表征如何塑造行为和生理，目前尚不清楚。为了解决这些问题，我们采用结合了行为、瞳孔测量和脑电图（EEG）数据的多模态方法，研究了风险和模糊情境下基于价值的决策。我们表明，个体采取了不同的决策策略，反映了对未知结果的不同内部信念。这些信念差异不仅体现在选择中，还体现在决策形成过程中的瞳孔相关唤醒中。关键的是，不同策略之间的生理差异在模糊选项的客观估值规则下持续存在，但在使用每个个体的主观信念计算估值时消失，这表明唤醒追踪的是主观信念而非客观任务结构。总之，我们的研究结果表明，模糊规避并非一种统一的偏差，而是反映了异质的内部信念模型，多模态生理学为理解这些信念引导基于价值的选择的机制提供了一个窗口。

## Abstract
Humans make thousands of decisions under ambiguity every day, where most times the probabilities of getting beneficial outcomes are not fully known. Although ambiguity aversion is well characterized at the aggregate level, it remains unclear how individuals internally represent ambiguous outcomes and how these representations shape behavior and physiology. To address these questions, we investigate value-based decision-making under risk and ambiguity using a multimodal approach that combines behavioral, pupillometric, and electroencephalographic (EEG) data. We show that individuals adopt distinct decision strategies that reflect different internal beliefs about unknown outcomes. These belief differences are expressed not only in choice but also in pupil-linked arousal during decision formation. Crucially, physiological differences across strategies persist under an objective valuation rule for ambiguous options but disappear when valuation is computed using each individuals subjective beliefs, indicating that arousal tracks subjective belief rather than objective task structure. Together, our findings show that ambiguity aversion is not a uniform bias but reflects heterogeneous internal belief models, and that multimodal physiology provides a window into the mechanisms through which these beliefs guide value-based choice.

---

## 论文详细总结（自动生成）

这篇论文题为《瞳孔与神经动力学揭示模糊情境下基于信念的决策》，由哥伦比亚大学的研究团队发表。以下是对该论文的结构化总结：

### 1. 核心问题与整体含义（研究动机和背景）
*   **核心问题**：人类在面对“模糊性”（Ambiguity，即结果概率未知）时，往往表现出规避行为。然而，传统的决策理论通常将其视为一种统一的群体偏差，忽略了个体在内部如何表征这些未知概率。
*   **研究动机**：研究旨在探索个体在模糊情境下是否存在不同的内部信念模型，以及这些模型如何通过生理信号（瞳孔唤醒和脑电动力学）得到体现。
*   **整体含义**：论文试图证明模糊规避并非单一的认知偏差，而是由异质的、基于主观信念的决策策略驱动的，且这些策略与个体的领导力等社会特质相关。

### 2. 核心方法论
*   **核心思想**：结合行为实验、生理测量（瞳孔+EEG）和计算建模（漂移扩散模型 DDM），从多模态角度解析决策过程。
*   **关键技术细节**：
    *   **行为分层**：根据参与者在无模糊（纯风险）条件下的表现，将其分为三类：**理想型（Ideal）**、**进取型（Aggressive）**和**保守型（Conservative）**。
    *   **主观信念推断**：引入参数 $k$，代表个体对模糊区域中出现高回报概率的主观估计。
    *   **生理信号处理**：
        *   **瞳孔**：使用广义线性模型（GLM）去除亮度诱发的瞬态反应，提取与决策相关的唤醒信号。
        *   **EEG**：分析 Fz（额叶）和 Pz（顶叶）电极的波谱功率，特别是 Delta、Theta 和 Alpha 频段。
    *   **漂移扩散模型 (DDM)**：公式为 $v = \beta_0 + b_k \cdot K + b_{pupil} \cdot Pupil + b_{eeg} \cdot EEG + \dots$，将主观价值、瞳孔唤醒和 EEG 特征整合进证据积累过程的漂移率（Drift Rate）中。

### 3. 实验设计
*   **实验场景**：
    *   **前置任务**：三人协作的航天器控制任务（用于评估领导力和团队表现）。
    *   **核心任务**：彩票选择任务（LCT）。参与者在“确定收益”和“概率彩票”之间做出选择。
*   **实验变量**：
    *   **模糊水平**：0%（无模糊）、30%（低模糊）、60%（高模糊）。
    *   **刺激类型**：社交（人脸）与非社交（轮盘）。
*   **对比基准**：以期望价值（EV）最优决策作为基准，对比不同策略组在不同模糊程度下的行为和生理差异。

### 4. 资源与算力
*   **硬件设备**：使用了 HTC VIVE Pro Eye 虚拟现实头显（内置 120Hz 眼动仪）、B-Alert X24 无线脑电系统（20 电极）。
*   **算力说明**：文中未明确提及高性能计算集群或 GPU 型号。由于涉及的是传统的信号处理和 DDM 模型拟合（使用 PyDDM 框架），通常在标准工作站上即可完成，不涉及大规模深度学习训练。

### 5. 实验数量与充分性
*   **样本量**：招募 57 名健康成年人，共进行 108 个实验场次。最终有效数据包含 96 组行为数据、95 组瞳孔数据和 79 组 EEG 数据。
*   **充分性评价**：
    *   实验设计涵盖了从行为分类到生理验证，再到计算建模的完整闭环。
    *   通过滑动窗口 Wilcoxon 符号秩检验和 FDR 校正处理生理信号，统计方法严谨。
    *   **消融/对比**：对比了“固定模糊模型”与“主观信念模型”对瞳孔数据的解释力，证明了主观模型更符合生理实测。

### 6. 主要结论与发现
*   **策略异质性**：进取型投资者持有乐观信念（高 $k$ 值），决策快；保守型持有悲观信念（低 $k$ 值），决策慢且对模糊不敏感。
*   **生理追踪信念**：瞳孔唤醒水平并不直接追踪客观的模糊程度，而是追踪基于个体主观信念的估值。当使用主观信念重新计算价值时，不同组间的生理差异消失。
*   **神经动力学差异**：理想型表现出强烈的额叶 Beta 信号；进取型具有广泛的预判性神经活动；保守型则表现出较弱的顶叶 Alpha 调制。
*   **社会特质关联**：在个人决策中表现“进取”的个体，在之前的团队协作任务中往往获得更高的领导力评分。

### 7. 优点与亮点
*   **多模态整合**：成功将瞬时生理信号（瞳孔、EEG）与长期认知模型（DDM）结合，提供了决策过程的动态视图。
*   **超越群体平均**：挑战了“模糊规避是统一偏差”的传统观点，揭示了策略背后的计算机制。
*   **跨情境一致性**：发现实验室内的价值决策风格与复杂的社会行为（领导力）之间存在关联，增加了研究的生态效度。

### 8. 不足与局限
*   **模糊水平有限**：仅设置了 30% 和 60% 两个模糊梯度，可能无法完全捕捉连续的信念变化。
*   **EEG 空间分辨率**：受限于 20 通道 EEG，无法进行精确的源定位分析，难以确定具体的脑区贡献。
*   **VR 环境影响**：虽然 VR 增加了沉浸感，但头显重量和佩戴舒适度可能对长时间实验中的生理信号产生干扰。
*   **因果关系**：研究揭示的是相关性，尚不能断定是生理状态决定了信念，还是信念塑造了生理反应。

（完）
