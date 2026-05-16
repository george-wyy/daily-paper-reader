---
title: Causally validated phase-amplitude coupling enables high-fidelity motor decoding for next-generation brain-computer interfaces
title_zh: 经因果验证的相位-振幅耦合可实现下一代脑机接口的高保真运动解码
authors: "Ma, J., Chen, T., Wang, H., Luo, C., Yin, Y., Xie, L., Hui, R., Liu, Y., He, R., Yu, X., Cheng, G., Bai, H., Su, H., Zhang, J."
date: 2026-05-13
pdf: "https://www.biorxiv.org/content/10.64898/2026.05.11.723545v1.full.pdf"
tags: ["query:gaze-intent"]
score: 6.5
evidence: 利用相位-振幅耦合解码脑机接口的运动意图
tldr: 本研究针对脑机接口依赖粗略代谢指标导致的性能瓶颈，提出利用相位-振幅耦合（PAC）作为高保真解码特征。通过高密度皮层脑电图和机器学习，并结合罕见的人体结构损伤模型进行因果验证，证明了Beta-PAC在运动意图解码中的优越性，为下一代神经假体奠定了生理基础。
source: biorxiv
selection_source: fresh_fetch
motivation: 现有的脑机接口主要依赖粗略的频谱功率降低（ERD），限制了高维运动控制的解码精度。
method: 采用高密度皮层脑电图记录运动想象，将Beta-PAC特征引入分类器，并利用肿瘤损伤模型进行因果验证。
result: 结合Beta-PAC的解码性能显著优于传统特征，且在结构失联导致PAC消失时，解码准确率降至随机水平。
conclusion: Beta-PAC是独立于代谢指标的高保真控制信号，为开发相位依赖的下一代脑机接口提供了生理依据。
---

## 摘要
现代脑机接口（BCI）面临着根本性的性能瓶颈，原因在于其依赖宽谱功率降低（事件相关去同步，ERD）作为主要的解码特征。ERD 仅作为皮层激活的粗略代谢代理，丢弃了高维运动控制所需的高频时间语法。在此，我们证明了相位-振幅耦合（PAC）——特别是高伽马（70-150 Hz）放电与残余 Beta 振荡的相位锁定——为解码运动意图提供了一种高保真的时间特征。通过在运动想象期间使用高密度皮层脑电图（HD-ECoG），我们展示了将 Beta-PAC 纳入机器学习分类器（LDA/SVM）的效果显著优于传统的基于功率的特征。为了明确验证该特征针对数学衍生伪影的因果鲁棒性，我们利用了一个罕见的活体人类结构损伤模型。在一名运动神经束受局灶性肿瘤浸润的患者中，代谢门控（ERD）得以保留，但结构解耦完全消除了 Beta-PAC，导致网络拓扑崩溃，并将单次试验的解码准确率降低至随机水平。我们的研究结果从因果上验证了 Beta-PAC 是一种稳健、独立的控制信号，为下一代相位依赖型神经假体奠定了生理学基础。

## Abstract
Modern Brain-Computer Interfaces (BCIs) face a fundamental performance plateau due to their reliance on broad spectral power reduction (Event-Related Desynchronization, ERD) as the primary decoding feature. ERD acts as a coarse metabolic proxy for cortical activation, discarding the high-frequency temporal syntax necessary for high-dimensional motor control. Here, we demonstrate that Phase-Amplitude Coupling (PAC)--specifically, the phase-locking of high-gamma (70-150 Hz) firing to residual Beta oscillations--provides a high-fidelity temporal feature for decoding motor intent. Using high-density electrocorticography (HD-ECoG) during motor imagery, we show that incorporating Beta-PAC into machine-learning classifiers (LDA/SVM) significantly outperforms traditional power-based features. To definitively validate the causal robustness of this feature against mathematically-derived artifacts, we leveraged a rare in vivo human structural lesion model. In a patient with focal tumor infiltration of the motor tract, the metabolic gate (ERD) was preserved, yet structural uncoupling completely abolished Beta-PAC, collapsing network topology and reducing single-trial decoding accuracy to chance levels. Our findings causally validate Beta-PAC as a robust, independent control signal, establishing a physiological foundation for next-generation, phase-dependent neuroprostheses.