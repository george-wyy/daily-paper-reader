---
title: Fixation-evoked potentials reveal neural signatures of hierarchical belief-updating during decision-making
title_zh: 注视诱发电位揭示决策中层次信念更新的神经特征
authors: "Deakin, J., Frömer, R., Gluth, S."
date: 2026-07-20
pdf: "https://www.biorxiv.org/content/10.64898/2026.07.15.738682v1.full.pdf"
tags: ["query:gaze-intent"]
score: 9.0
evidence: 使用眼动追踪和脑电图研究决策中的信念更新，直接相关于人类注视的概率建模
tldr: 决策涉及从信息采样到行动计划的层级信念更新。本研究结合EEG和眼动追踪，使用多属性搜索与选择模型（MASC）生成注视级预测，分析注视诱发电位（FEPs）。结果发现属性级、选项级和偏好级更新分别在前中央正波、中央顶正波和侧化运动准备活动中体现。研究揭示了层级信念更新的神经机制，为自然自由观看范式下的注意和选择动力学提供了新方法。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-15-738682-v1/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1666, \"height\": 1064, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-15-738682-v1/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1608, \"height\": 986, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-15-738682-v1/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1769, \"height\": 1089, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-15-738682-v1/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1875, \"height\": 952, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-15-738682-v1/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1686, \"height\": 1486, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-15-738682-v1/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1480, \"height\": 1283, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-15-738682-v1/fig-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 1804, \"height\": 469, \"label\": \"Figure\"}]"
motivation: 探究自然自由观看条件下多层级信念更新的神经机制。
method: 结合EEG和眼动追踪，利用MASC模型生成注视级预测并分析FEPs。
result: FEPs显示属性级、选项级和偏好级分别对应前中央正波、中央顶正波和运动准备活动。
conclusion: 阐明了从信息采样到决策形成的层级信念更新神经过程。
---

## 摘要
许多决策需要在多个表征层次上维持信念，从采样和整合信息到形成行动计划。为了阐明这些过程并揭示在自然自由观看条件下支持它们的神经机制，我们在多属性选择任务中结合了脑电图和眼动追踪。利用我们最近开发的多属性搜索与选择（MASC）模型，我们生成了针对价值信念更新过程（涵盖属性、选项和偏好状态）的注视级别预测。行为和眼动追踪数据证实了MASC预测的搜索和选择动态。关键的是，注视诱发电位（FEPs）揭示了处理层次上的不同神经特征。属性级和选项级更新分别反映在早期的额中央正电位和中央顶叶正电位，而新兴的偏好则表现为侧化的运动准备活动。我们预先注册的研究阐明了将信息采样与决策形成联系起来的层次神经信念更新过程，并为在自然自由观看范式中研究神经注意和选择动态开辟了新的研究途径。

## Abstract
Many decisions require maintaining beliefs across multiple levels of representation, from sampling and integrating information to forming action plans. To elucidate these processes and reveal the neural mechanisms supporting them under naturalistic free-viewing conditions, we combined EEG and eye-tracking in a multi-attribute choice task. Leveraging our recently developed Multi-Attribute Search and Choice (MASC) model, we generated fixation-level predictions for value-belief updating processes encompassing attribute, option, and preference states. Behavioral and eye-tracking data confirmed search and choice dynamics as predicted by MASC. Crucially, fixation-evoked potentials (FEPs) revealed distinct neural signatures along the processing hierarchy. While attribute-level and option-level updates were reflected in an early fronto-central positivity and a centro-parietal positivity, respectively, emerging preferences were expressed in lateralized motor-preparatory activity. Our preregistered study elucidates a hierarchy of neural belief-updating processes linking information sampling to decision formation and opens new research avenues for investigating neural attention and choice dynamics in naturalistic free-viewing paradigms.

---

## 论文详细总结（自动生成）

# 论文中文总结

## 1. 论文的核心问题与整体含义

- **研究动机**：多属性决策（如选购手机）需要在信息采样、整合和行动之间维持多级信念（属性、选项、偏好）。现有研究多依赖非人灵长类或fMRI（时间分辨率低），而EEG因眼动伪迹和时序变异难以用于自然自由观看任务。本文旨在结合EEG和眼动追踪，利用多属性搜索与选择(MASC)计算模型揭示层次信念更新的神经机制。
- **整体含义**：阐明了信息采样到决策形成的**分层神经过程**——属性级更新、选项级集成和偏好形成分别对应不同的时空特征（前中央正波、中央顶正波、侧化运动准备活动）。为自由观看范式下研究注意与选择动态提供了新框架。

## 2. 论文提出的方法论

- **核心思想**：以MASC（层次贝叶斯信念更新模型）生成注视级别的预测——属性级信念更新（KL散度）、选项级信念更新（KL散度）、当前偏好（Jeffrey距离），然后通过线性反卷积模型将这些预测与注视诱发电位(FEPs)关联。
- **关键技术细节**：
  - 同步EEG（1000Hz，64通道）和眼动追踪（1000Hz，EyeLink 1000 Plus），离线降采样至500Hz，同步误差<2ms。
  - 使用OPTICAT算法去除眼动伪迹（包括棘波电位），保留脑信号。
  - 线性反卷积模型(Unfold.jl)建模重叠的神经活动，每个注视的FEP分解为：
    \[ \text{FEP} \sim 1 + \text{FixatedVal} + \text{AttUpd} + \text{OptUpd} + \text{Preference} + \text{FixNum} + \text{spl(振幅)} + \text{spl(时长)} \]
    其中AttUpd和OptUpd基于KL散度（测前后分布差异），Preference基于Jeffrey距离并标记主导选项侧。
  - 模型拟合：网格搜索三个自由参数（采样标准差\(\sigma_s\)、容忍度增量\(\Delta\)、搜索灵敏度\(\alpha\)），优化选择一致性和注视比例等摘要统计。

## 3. 实验设计

- **数据集/场景**：自创智能手机多属性选择任务。参与者（N=57）先对45款手机（3属性：屏幕、电池、存储，0-5星）进行评分（1-10），之后在420个试次中（140个易/中/难各等份）自由观看并按键选择偏好的选项（左右手分别对应左右选项）。选项为两两配对，使用颜色区分（绿/蓝）。
- **Benchmark**：无外部基准。文中主要将MASC的行为预测（如注视数、选择一致性、注意力偏好、属性权重动态）与实际行为对比验证模型拟合度；神经层面则检验MASC生成预测对FEP的解释力。
- **对比方法**：未与其他决策模型（如aDDM、DBM）进行直接对比，而是通过统计检验证明MASC预测与观察数据吻合。

## 4. 资源与算力

- 文中未明确提及GPU型号、数量或训练时长等算力信息。实验采用MATLAB R2021b/R2024b和Psychtoolbox，在标准台式机上运行；眼动和EEG设备为商用科研设备（EyeLink 1000 Plus, Brain Products ActiCap）。
- 仅提及模型拟合使用网格搜索（31个等距值×3参数），无高算力消耗。

## 5. 实验数量与充分性

- **预注册**：项目在OSF预注册，明确假设、排除标准和EEG预处理流程，提高客观性。
- **样本量**：基于先验功效分析要求至少52人，实际57人（剔除13人因技术/质量/随机按键）。足够检测预设效应。
- **实验组**：
  - 行为验证：4个主要分析（注视数随难度变化、选择一致性、注意-选择关联、属性权重随时间衰减、跨个体搜索模式），均通过t检验或相关性报告，显著且效应量适中到高。
  - 神经分析：对FEP的4个主要预测器（FixatedVal、AttUpd、OptUpd、Preference）进行阈值自由聚类置换检验，均达到显著（p<.001）。后续还分析了属性权重对Option更新与Attribute更新的差异化效应（重复测量ANOVA），以及Preference与Choice的分离。
- **充分性与客观性**：实验覆盖行为与神经两个层面，验证了MASC的层次预测；但缺乏与其他模型（如aDDM）的竞争性比较，且未做交叉验证或泛化测试。总体而言，实验较为系统，但未对比基准方法，公平性有限。

## 6. 论文的主要结论与发现

- **行为发现**：MASC成功解释了：
  - 难度增加导致注视增多、选择一致性降低。
  - 高价值选项被更频繁关注，且这种偏向随时间增强。
  - 高权重属性在早期被优先关注，后衰减。
  - 属性权重分散度与搜索模式（Payne指数）负相关。
- **神经发现**：
  - **属性级更新 (AttUpd)**：前中央正电位（192-1062 ms），线性缩放更新幅度；不受属性权重调节。
  - **选项级更新 (OptUpd)**：中央顶正电位（208-1050 ms），非对称受属性权重影响（早期高权属性更新更大，后减弱）。
  - **偏好 (Preference)**：侧化运动准备活动（LRP样），区分为方向效应（持续）与强度效应（晚期出现）。
  - **注视值 (FixatedVal)**：短暂的前中央正波（230-374 ms），非线性编码（高值主导）。

## 7. 优点

- **方法创新**：首次在**自由观看价值决策**中结合EEG与眼动追踪，利用线性反卷积处理重叠和伪迹，提取注视诱发电位。
- **计算建模驱动**：基于MASC理论生成层次信念更新的定量预测，直接解释神经信号，超越传统ERP分析。
- **预注册+严格伪迹处理**：使用OPTICAT去除眼动伪迹，同步误差<2ms，增强结果可靠性。
- **时空分辨率优势**：EEG提供毫秒级时间分辨率，揭示不同层次的更新时序（属性→选项→偏好）。

## 8. 不足与局限

- **模型覆盖**：MASC未直接实现属性间比较（如逐属性交替），但参与者行为以选项间为主；未来可扩展。
- **源定位有限**：EEG空间分辨率低，无法精确确定脑区；虽提及P3a/CPP的源（前扣带、顶叶），但缺乏源分析验证。
- **实验对比不足**：未与其他决策模型（如aDDM、DBM）进行模型比较或联合分析，难以说明MASC的独特优势。
- **泛化性**：仅测试了智能手机多属性情境，未验证到其他领域（如感知决策、风险选择）。
- **统计偏差风险**：仅对单一模型预测做显著性检验，未进行交叉验证或预测误差分析，可能高估模型解释力。

（完）
