---
title: Effect of Large Language Models on P300 Speller Performance with Cross-Subject Training
title_zh: 大语言模型对跨被试训练下 P300 拼写器性能的影响
authors: "Parthasarathy, N., Soetedjo, J., Panchavati, S., Lee, D., Arnold, C., Pouratian, N., Speier, W."
date: 2026-05-05
pdf: "https://www.biorxiv.org/content/10.1101/2025.10.28.685216v2.full.pdf"
tags: ["query:gaze-intent"]
score: 6.0
evidence: 用于人机交互和通信的 P300 拼写器脑机接口
tldr: 本研究针对渐冻症患者使用的P300拼写器脑机接口，旨在解决其通信效率低和跨受试者训练难的问题。通过引入先进的多受试者分类器训练方法，并集成Llama、Mistral和GPT2等大语言模型进行单词预测，显著提升了打字速度。研究还构建了理想LLM以确定性能上限，证明了现代LLM在提升BCI交互效率方面的巨大潜力。
source: biorxiv
selection_source: fresh_fetch
motivation: 旨在提高P300拼写器脑机接口的通信效率，并优化跨受试者分类器的训练效果。
method: 结合了先进的多受试者分类器训练技术，并集成多种大语言模型进行刺激呈现优化和单词预测。
result: "字符级模型提升约10%的打字速度，而Llama等大语言模型通过高效单词预测使速度提升约40%。"
conclusion: 大语言模型能显著提升P300拼写器的性能，且该改进在不同分类器中具有良好的泛化性。
---

## 摘要
肌萎缩侧索硬化症（ALS）是一种渐进性神经肌肉变性疾病，在发病后数年内会迅速损害患者的沟通能力。这种沟通能力的丧失使得恢复互动和独立性的辅助技术变得至关重要。P300 拼写器脑机接口（BCI）便是这样一种技术，它通过追踪受试者对屏幕上高亮字符的神经反应，将脑电图（EEG）信号转化为文本。P300 研究的一个核心挑战是提升性能，以实现更快速、更高效的用户交互。在此背景下，本研究解决了关键局限性，特别是多被试分类器的训练，以及集成先进语言模型以优化刺激呈现和词预测，从而提高沟通效率。具体而言，我们引入了三项关键创新：先进的多被试分类器训练；集成并评估了多种大语言模型（LLM）对拼写器性能的影响；利用具有完美预测能力的理想 LLM 确定了 P300 LLM 的性能边界。我们使用随机采样的 EEG 数据进行了广泛的模拟。结果表明，在输入包含罕见词和词汇表外（OOV）词汇的段落时，打字速度得到了显著提升。提升幅度取决于所使用的语言模型类型。具体而言，字符级模型使打字速度提升了约 10%，而 Llama、Mistral 和 GPT2 等开源 LLM 通过高效的词预测实现了约 40% 的提升。此外，我们构建了一个理想 LLM 以确立理论性能极限，并证明许多现代 LLM 的性能已达到该极限的 10% 以内。此外，我们还证明了这些由 LLM 驱动的速度提升在不同分类器中具有通用性，包括那些旨在减少特定被试训练的分类器。

## Abstract
Amyotrophic lateral sclerosis (ALS), a progressive neuromuscular degenerative disease, rapidly impairs communication within years of onset. This loss of communication necessitates assistive technologies to restore interaction and independence. One such technology, the P300 speller brain-computer interface (BCI), translates EEG signals into text by tracking a subjects neural responses to highlighted characters on a screen. A central challenge in P300-based research is enhancing performance to enable faster and more efficient user interaction. In this context, this study addresses key limitations, particularly in the training of multi-subject classifiers, and integrating advanced language models to optimize stimuli presentation and word prediction, thereby improving communication efficiency. Specifically, we introduce three key innovations:- Advanced multi-subject classifier training- Integrating and evaluating impact of numerous large language models (LLMs) on speller performance- Determining P300 LLM performance bounds using an ideal LLM with perfect prediction We conduct extensive simulations using randomly sampled EEG data. Our results demonstrate substantial speed improvements in typing passages that include rare and out-of-vocabulary (OOV) words. The magnitude of improvement depends on the type of language model used. More specifically, character-level models provide typing speed improvements of approximately 10%, while open-source LLMs such as Llama, Mistral and GPT2 achieve around 40% improvement through efficient word prediction. Additionally, we construct an ideal LLM to establish theoretical performance limits and show that many modern LLMs achieve performance levels within 10% of it. Further, we show that these LLM-driven speed improvements generalize across classifiers, including those designed to reduce subject-specific training.