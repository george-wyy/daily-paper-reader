---
title: Behavioral evidence challenges species-specific ocular morphology as a primary constraint on human gaze-following
title_zh: 行为证据挑战了物种特异性眼部形态作为人类注视跟随主要约束因素的观点
authors: "Shafiei, M., Arnous, Y., Taubert, N., Giese, M., Thier, P."
date: 2026-05-13
pdf: "https://www.biorxiv.org/content/10.64898/2026.05.11.705002v1.full.pdf"
tags: ["query:gaze-intent"]
score: 8.0
evidence: 人类对指向物体的视线关注的敏感性
tldr: 本研究探讨了人类对视线追踪的高敏感性是否由其独特的眼部形态决定。通过对比人类在面对人类和猕猴头像视线引导时的空间注意转移，发现尽管猕猴眼睛缺乏人类眼睛的显著特征，人类对两者的视线线索均表现出显著且相当的注意增强效应。这挑战了“人类特有眼部形态是视线跟随主要约束”的观点，证明了人类对视线信号具有极高的感知灵敏度。
source: biorxiv
selection_source: fresh_fetch
motivation: 探究人类独特的眼部形态是否是导致人类与非人灵长类动物在视线追踪敏感度上存在差异的主要原因。
method: 实验测量了人类受试者在面对人类或猕猴头像视线引导时，其隐蔽空间注意转移的反应时差异。
result: 结果显示人类对猕猴视线和人类视线产生的注意引导效果相当，并未受限于猕猴眼睛缺乏显著特征的形态。
conclusion: 眼部形态并非人类视线驱动注意定向的主要限制因素，人类对不同物种的视线信号均具有极强的感知能力。
---

## 摘要
先前的研究表明，人类对指向物体的视线注视极其敏感，这能有效地引导他们的注意力转向共同感兴趣的物体。这与非人灵长类动物形成对比，后者通常需要更显著的视线注视线索才能实现相当的注意力定向。然而，目前尚不清楚眼部形态的跨物种差异是否是造成这种表现差距的原因。为了探讨这一问题，我们研究了人类在面对由逼真的人类或恒河猴头部化身提供的视线注视线索时，空间注意力的隐蔽转移。结果显示，与注视不一致的试验相比，注视一致试验中的目标检测能力得到了显著增强，且两种化身类型的注视提示效应相当，尽管猴子的眼睛缺乏人类眼睛所特有的许多显著特征。因此，单纯的眼部形态并不会显著调节人类由注视驱动的注意力定向，而人类对猴子视线注视线索的可靠利用，突显了在视线信号感知灵敏度方面明显的物种差异。

## Abstract
Previous research suggests that humans are extremely sensitive to object-directed eye gaze, which effectively guides their attention toward objects of shared interest. This contrasts with non-human primates, who typically require much more salient eye-gaze cues to achieve comparable attentional orienting. However, it remains unclear whether cross-species differences in ocular morphology account for this performance gap. To address this question, we examined humans' covert shifts of spatial attention in response to eye-gaze cues provided by either realistic human or rhesus monkey head avatars. Target detection was reliably enhanced on gaze-congruent compared to gaze-incongruent trials, with comparable gaze-cueing effects for both avatar types, despite the fact that monkey eyes lack many of the conspicuous features characteristic of human eyes. Hence, eye morphology alone does not substantially modulate gaze-driven attentional orienting in humans, whereas humans' reliable use of monkey eye-gaze cues highlights a clear species difference in perceptual sensitivity to eye gaze signals.

---

## 论文详细总结（自动生成）

这篇论文对人类注视跟随（Gaze-following）能力的机制进行了深入探讨，挑战了长期存在的“合作之眼假说”（Cooperative Eye Hypothesis）。以下是该研究的结构化总结：

### 1. 核心问题与整体含义（研究动机和背景）
*   **核心问题**：人类在注视跟随能力上显著优于非人灵长类动物（NHPs），这种差异究竟是因为人类独特的**眼部形态**（如显著的白色巩膜、细长的眼裂），还是因为人类具有更高的**感知灵敏度**？
*   **背景**：传统观点认为，人类眼睛的高对比度形态是进化出的社交工具，旨在方便他人追踪自己的视线。然而，近期形态学研究发现某些猴类也具有类似特征，且人类内部也存在形态差异，这使得“形态决定论”受到质疑。

### 2. 论文提出的方法论
*   **核心思想**：通过“注视提示范式”（Gaze-cueing paradigm），比较人类受试者对“人类头像”和“猕猴头像”视线线索的反应。如果形态是主要约束，人类对猴子眼睛（缺乏白色巩膜、形状较圆）的反应应显著弱于对人类眼睛的反应。
*   **关键技术细节**：
    *   **逼真头像**：利用 Unreal Engine 5 开发了超写实的 3D 人类和猕猴头部化身（Avatar），确保两者的视线移动轨迹、动力学特征完全一致。
    *   **隐蔽注意测量**：受试者需在保持中央注视的同时，检测外围 LED 灯微弱的亮度变化。
    *   **非预测性线索**：头像的视线方向与目标出现位置无关（50%一致性），以测量自发的、反射性的注意转移，而非策略性选择。

### 3. 实验设计
*   **受试者**：23 名神经发育正常的成年人。
*   **实验阶段**：
    1.  **训练阶段**：熟悉任务流程。
    2.  **感知阈值估计（PTE）**：为每位受试者量身定制 LED 亮度变化值，确保基准检测准确率在 75% 左右。
    3.  **正式实验**：包含人类和猴子两种头像块，设置了 5 种不同的刺激偏移异步时间（SOA：50, 100, 200, 300, 400 ms）。
*   **Benchmark（基准对比）**：
    *   **内部对比**：人类对人类头像 vs. 人类对猴子头像。
    *   **跨物种对比**：将本实验数据与作者之前在恒河猴身上进行的相同实验（使用相同猴子头像和设备）进行对比。

### 4. 资源与算力
*   **硬件设备**：使用 EyeLink 1000 Plus 高速眼动仪（2 KHz 采样率）监控注视稳定性；BenQ 144Hz 显示器。
*   **软件工具**：Unreal Engine 5（生成头像）、CapCut（视频处理）、MATLAB（实验控制与数据预处理）、R 语言（统计建模）。
*   **算力说明**：文中未提及具体的 GPU 训练时长或算力规模，因为该研究属于行为神经科学实验，不涉及深度学习模型的训练，重点在于高精度眼动数据采集和统计分析。

### 5. 实验数量与充分性
*   **实验规模**：每位受试者完成约 2000 次试验（1000 次/头像类型），总计分析了数万次试验数据。
*   **统计方法**：采用广义线性混合效应模型（GLMM），充分考虑了受试者间的个体差异（随机截距和随机斜率）。
*   **充分性评价**：实验设计严谨，通过 PTE 阶段排除了个体感知差异的干扰，并设置了多个 SOA 时间点来捕捉注意力的动态变化。对比实验使用了完全相同的刺激物，确保了跨物种比较的公平性。

### 6. 主要结论与发现
*   **形态不敏感性**：人类对人类和猴子头像表现出**几乎相同**的注视提示效应（Gaze-cueing effect）。尽管猴子眼睛缺乏显著的对比度特征，人类依然能高效提取其空间信息。
*   **感知灵敏度差异**：对比发现，同样的微弱视线线索能驱动人类的注意转移，但无法驱动猴子的注意转移。
*   **结论**：眼部形态并非限制人类注视跟随能力的主要因素。人类的优势在于对视线信号极高的**感知灵敏度**，这可能源于发育过程中的社交学习经验。

### 7. 优点
*   **高生态效度**：使用了高度逼真的 3D 头像，克服了以往研究中使用简笔画或低质量照片的局限。
*   **严谨的跨物种比较**：通过完全相同的实验设置和刺激物，直接量化了人类与猴子在处理相同视觉信号时的性能差异。
*   **排除干扰**：通过非预测性设计和强制性中央注视，成功分离了“反射性注意”与“自愿性注意”。

### 8. 不足与局限
*   **单向测试**：研究仅测试了人类对猴子视线的反应，尚未测试猴子对人类视线的反应（虽然推测猴子表现会更差，但缺乏直接证据）。
*   **面部背景干扰**：虽然匹配了眼睛动力学，但人类和猴子的面部轮廓、毛发等背景信息仍存在差异，未来需进一步通过“换眼实验”（如猴脸人眼）来彻底分离面部背景与眼部形态的影响。
*   **发育因素未深究**：论文推测灵敏度差异源于社会化经验，但未对不同年龄段或社交背景的人群进行对比。

（完）
