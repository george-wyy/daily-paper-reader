---
title: "Seamless interaction in VR: decoding user intent with eye gaze and passive brain-computer interfaces"
title_zh: VR中的无缝交互：利用视线和被动脑机接口解码用户意图
authors: "Pan, Y., Rabe, L., Zander, T., Klug, M."
date: 2026-07-10
pdf: "https://www.biorxiv.org/content/10.64898/2026.07.06.736575v1.full.pdf"
tags: ["query:gaze-intent"]
score: 9.0
evidence: 在VR中使用眼动和被动脑机接口解码用户意图
tldr: "VR交互依赖显式运动输入，限制了无缝自适应交互。本研究结合EEG被动脑机接口与眼动追踪，在动态VR游戏中解码交互意图，包括可负担性评估和趋避评估。离线分类准确率66.28%，在线达69.64%；明确正负效价分类准确率80.84%，模糊情境近随机。首次实现实时EEG解码VR交互意图，推动生理信号驱动的沉浸式交互。"
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-06-736575-v1/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1358, \"height\": 837, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-06-736575-v1/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1290, \"height\": 1011, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-06-736575-v1/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 783, \"height\": 1375, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-06-736575-v1/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1283, \"height\": 1045, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-06-736575-v1/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1241, \"height\": 1036, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-06-736575-v1/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1189, \"height\": 1409, \"label\": \"Figure\"}]"
tables_json: "[{\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-07-06-736575-v1/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1359, \"height\": 414, \"label\": \"Table\"}, {\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-07-06-736575-v1/table-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1330, \"height\": 434, \"label\": \"Table\"}, {\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-07-06-736575-v1/table-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1214, \"height\": 739, \"label\": \"Table\"}]"
motivation: VR交互依赖显式运动输入，缺乏自适应能力。
method: 结合EEG被动BCI与眼动追踪，解码交互意图的趋避与可负担性评估。
result: "离线准确率66.28%，在线69.64%；明确效价分类80.84%，模糊效价59.03%。"
conclusion: 首次实现实时EEG解码VR交互意图，有效但个体差异大，用户认为更有趣。
---

## 摘要
虚拟现实（VR）交互在很大程度上仍然依赖于明确的外部运动输入，限制了无缝和自适应交互。本研究探讨了基于脑电图（EEG）的被动脑机接口（BCI）结合视线，是否能在动态VR游戏过程中直接从其潜在的神经生理相关性中解码交互意图。我们将交互意图操作化为两个组成部分：可供性相关评估，指示被注意对象是否提供交互，以及趋近-回避评估，指示交互朝向期望或不期望结果的倾向性。23名参与者完成了一项VR游戏，包括两次校准环节和一次在线BCI环节。离线分析显示，在所有可操作试验中，对二元趋近-回避决策分类的解码高于随机水平，跨参与者的总平均准确率为66.28%。这种解码转移到了在线闭环游戏中，总平均准确率仍高于随机水平，达到69.64%。类别层面分析进一步揭示了分类可分性的显著变异。对于趋近-回避相关分类，在明确效价的奖励与惩罚类别之间最清晰的配对中，准确率达到80.84%，但在动机效价模糊、更依赖语境的配对中，准确率降至接近随机的59.03%。非可操作与可操作物品类别之间的可供性相关分类一直很高，范围从77.76%到83.50%。用户体验问卷结果表明，尽管存在导致感知失去控制感和易用性降低的局限性，但参与者发现基于BCI的交互范式本身比控制器基线更有趣。据我们所知，这是在动态VR游戏过程中实时EEG解码交互意图的首次演示，有助于在沉浸式环境中由生理信号驱动的直觉用户自适应界面。

## Abstract
Virtual reality (VR) interaction remains largely dependent on explicit motor input, limiting seamless and adaptive interaction. This study investigated whether electroencephalography (EEG)-based passive brain-computer interfaces (BCIs), combined with eye gaze, can decode interaction intent directly from its underlying neurophysiological correlates during dynamic VR gameplay. We operationalized interaction intent as comprising two components: affordance-related evaluation, indicating whether an attended object affords interaction, and approach-avoidance evaluation, indicating the directional tendency of interaction toward desirable or undesirable outcomes. Twenty-three participants completed a VR game with two calibration sessions and one online BCI session. Offline analyses showed above-chance decoding of the binary approach-avoidance decision classification across all actionable trials, with a grand-average accuracy of 66.28% across participants. This decoding transferred to online closed-loop gameplay, where grand-average accuracy remained above chance at 69.64%. Category-level analyses further revealed substantial variability in classification separability. For approach-avoidance-related classifications, accuracy reached 80.84% for the most distinct pairing between clearly valenced reward and punishment categories, but dropped to near chance at 59.03% for the more context-dependent pairing with ambiguous motivational valence. Affordance-related classifications between non-actionable and actionable item categories were consistently high, ranging from 77.76% to 83.50%. User Experience questionnaire results showed that, despite limitations leading to perceived loss of control and reduced ease of use, participants found the BCI-based interaction paradigm itself more fun than the controller baseline. To our knowledge, this is the first demonstration of real-time EEG decoding of interaction intent during dynamic VR gameplay, contributing toward intuitive user-adapted interfaces driven by physiological signals in immersive environments.

---

## 论文详细总结（自动生成）

# VR中基于视线与被动脑机接口的无缝交互：解码用户意图

## 1. 论文的核心问题与整体含义（研究动机和背景）

- **核心问题**：当前VR交互严重依赖显式运动输入（如手柄、手部追踪），导致交互摩擦、影响沉浸感，且无法感知用户隐式的认知状态（如意图、工作负荷等）。为了解决“Midas touch问题”（即视线注视即被当作命令），亟需一种能自动解码用户交互意图的方法，实现无缝、自适应的交互。
- **研究背景**：被动脑机接口（pBCI）可解码自发的神经活动，结合眼动追踪形成混合BCI，有望直接解码交互意图而无需显式输入。以往工作多依赖事件相关电位（如SPN、P300）作为代理信号，且局限于离线分析或简单选择任务。本研究首次在动态VR游戏中实现实时EEG解码交互意图，并将其分为可供性评估（是否可交互）和趋避评估（采取或丢弃）两个成分。

## 2. 论文提出的方法论：核心思想、关键技术细节、算法流程

- **核心思想**：将交互意图操作化为两个二元分类问题：①可供性评估（可操作 vs. 不可操作物品）；②趋避评估（采取 vs. 丢弃）。通过EEG信号解码决策期间的神经活动，结合眼动实现空间定位，从而在VR游戏中替代手柄输入。
- **关键技术细节**：
  - **实验范式**：VR防御游戏，玩家注视飞来的岩石以停止并揭示内部物品，经历1秒决策期（仅可评估思考，不能操作）、1.5秒行动期（校准阶段用手柄反馈，在线阶段由预训练分类器自动执行）。
  - **EEG预处理**：64通道有源电极，500Hz采样；带通滤波0.1–15 Hz，参考FCz，后重参考为全脑平均；分段-200~1000ms相对于物品出现，基线校正-200~0ms。
  - **特征提取与分类**：采用0–800ms决策窗口，分为16个50ms非重叠时间窗，每个窗口内计算各通道均值，得到1024维特征向量。分类器为正则化线性判别分析（rLDA），带自动协方差收缩和类别平衡，5折时间交叉验证。
  - **在线分类**：校准阶段（2次）训练好分类器后，在线阶段实时处理EEG流，预测采取/丢弃并通过Lab Streaming Layer发送到Unity执行，参与者仅在对系统错误时按键纠正，以此获取标签。
  - **事后分析**：使用AMICA进行独立成分分析（ICA）去除眼动和肌肉伪迹，再应用相同分类流程分析不同物品类别配对。
- **算法流程**：校准数据采集 → 离线训练rLDA模型 → 在线实时特征提取与分类 → 行动执行 → 参与者纠正反馈 → 在线准确率评估。

## 3. 实验设计：数据集/场景、benchmark、对比方法

- **场景**：自建的VR游戏（Unity开发），包含岩石、金币、炸弹、食物、盔甲、岩石碎片等多种物品，具有不同的可供性和动机效价（奖励、惩罚、情境依赖）。
- **数据集**：19名有效参与者（最初23人，排除4名校准问题和1名在线错误率超额者）。校准阶段2次，每次约20分钟，4波难度递增；在线BCI阶段1次，类似结构但间隔更长以便标签反馈。
- **基准**：控制器基线（手柄操作），用于对比用户体验问卷。
- **对比方法**：离线分类性能与仿真随机机会水平对比；在线分类准确率与机会水平对比；用户体验问卷中当前BCI系统与控制器、理想化完美BCI系统对比。未与其他类似方法（如纯眼动、SPN方法）直接比较，但引用相关领域文献说明创新性。

## 4. 资源与算力

- **文中明确说明**：未提及使用的GPU型号、数量或训练时长。实验采用台式计算机（AMD Ryzen 7 5800X, NVIDIA GeForce RTX 3070 Ti），用于VR渲染和在线BCI处理。EEG信号处理及分类在MATLAB中使用EEGLAB和BCILAB完成，未说明特定硬件加速。整体算力需求较低，属于标准PC级别。

## 5. 实验数量与充分性

- 实验数量：离线分析19名参与者，在线分析18名（1名因错误率>15%排除）。离线每个参与者约493个有效试验，在线约260个试验。事后分析对所有物品类别配对进行了分类，包括6个二元分类（可操作 vs 不可操作：4种；趋避内部：2种）。用户体验问卷含8个维度双条件对比。
- **充分性与公平性**：
  - 采用了仿真随机机会水平（25000次模拟），确保统计显著性评估。
  - 在线标签通过参与者纠正获取，存在一定噪声（平均错误率4.35%），但已使用阈值排除不可靠参与者。
  - 用户体验问卷为探索性分析，未做多重比较校正，样本量较小，结论需谨慎。
  - 控制器基线非完全匹配（固定顺序），可能引入顺序效应。
  - 实验设计合理，覆盖多种难度的物品类别，但物品视觉特征差异可能混淆神经信号，未完全控制感知因素。

## 6. 论文的主要结论与发现

- **离线解码可行**：趋避二元分类（采取 vs 丢弃）总平均准确率66.28%（>机会水平55.85%）。可供性相关分类（可操作 vs 不可操作）均较高（77.76%–83.50%）。
- **在线解码成功**：在线准确率69.64%（>机会58.61%），金币命中率76.23%，炸弹正确拒绝率64.66%。首次证明实时EEG解码VR交互意图可行。
- **类别差异显著**：明确效价的物品（金币vs炸弹）分类准确率达80.84%；情境依赖的模糊物品（非金币采取vs非炸弹丢弃）仅59.03%（接近随机）。
- **用户体验**：当前BCI系统相比控制器更有趣，但控制感、易用性、满意度显著降低。理想化完美BCI系统在所有维度更优，表明当前限制主要源于技术性能而非概念本身。
- **交互意图结构**：可供性评估和趋避评估是两个部分可分离的成分，前者更稳健，后者受情境模糊性制约。

## 7. 优点：方法或实验设计上的亮点

- **创新性**：首次在动态VR游戏中实现实时EEG解码交互意图，克服了以往离线研究以及依赖代理信号（SPN）的限制。
- **直接解码**：通过受控决策期隔离评估响应，从神经活动直接解码意图，而非通过预期反馈的间接信号。
- **混合BCI架构**：将眼动用于空间定位，EEG解码意图，两者互补，解决了眼动的Midas touch问题。
- **操作化结构**：将交互意图分解为可供性和趋避两个成分，提供了可解析的认知模型，有利于针对不同成分设计自适应策略。
- **在线至闭环验证**：从离线校准到在线闭环的游戏全过程演示，验证了实际可行性。
- **用户体验探索**：对比当前BCI与理想化条件，有助于区分概念接受度与技术缺陷。

## 8. 不足与局限

- **实验覆盖**：
  - 仅使用一种VR游戏范式，物品类别存在视觉差异（如金币更亮），难以完全归因于认知评估。
  - 样本量较小（最终19/18人），统计功效有限；用户体验问卷为探索性，未校正多重比较。
- **偏差风险**：
  - 在线标签依赖参与者主观纠正，可能存在误报或漏报（平均错误率4.35%），即使调整后准确率仍低于机会水平。
  - 固定顺序设计（先校准后在线），可能存在学习效应或疲劳效应。
- **应用限制**：
  - 当前分类精度中等（~70%），在控制感、易用性上不如传统手柄，实际应用需更高准确率或置信度自适应策略。
  - 未集成实时伪迹去除方法（ICA仅用于事后分析），对强运动伪迹的鲁棒性未知。
  - 硬件设置复杂（64通道湿电极、Meta Quest Pro），实用性受限；未来需向干电极、轻量化系统推进。
- **神经机制理解局限**：仅依据分类性能推断认知过程，未进行源定位或详细时间频率分析，分类特征的具体神经起源未明确。

（完）
