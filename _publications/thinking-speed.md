---
title: "Controlling Thinking Speed in Reasoning Models"
collection: publications
category: conferences
permalink: /publication/ThinkingSpeed
excerpt: 'This paper is about the number 1. The number 2 is left for future work.'
date: 2025-12-10
venue: 'Conference on Neural Information Processing Systems (<b>NeurIPS Spotlight</b>)'
slidesurl: 'https://github.com/D2I-ai/thinking-speed-control'
paperurl: 'https://arxiv.org/pdf/2507.03704'
authors: 'Zhengkai Lin, <b><u>Zhihang Fu</u><sup>&sect;</sup></b>, Ze Chen, Chao Chen, Liang Xie, Wenxiao Wang, Deng Cai, Zheng Wang, Jieping Ye'
image: '/images/control.png'
#citation: 'Your Name, You. (2009). &quot;Paper Title Number 1.&quot; <i>Journal 1</i>. 1(1).'
---

Human cognition is theorized to operate in two modes: fast, intuitive System 1 thinking and slow, deliberate System 2 thinking. While current Large Reasoning Models (LRMs) excel at System 2 thinking, their inability to perform fast thinking leads to high computational overhead and latency. In this work, we enable LRMs to approximate human intelligence through dynamic thinking speed adjustment, optimizing accuracy-efficiency trade-offs. Our approach addresses two key questions: (1) how to control thinking speed in LRMs, and (2) when to adjust it for optimal performance. For the first question, we identify the steering vector that governs slow-fast thinking transitions in LRMs' representation space. Using this vector, we achieve the first representation editing-based test-time scaling effect, outperforming existing prompt-based scaling methods. For the second question, we apply real-time difficulty estimation to signal reasoning segments of varying complexity. Combining these techniques, we propose the first reasoning strategy that enables fast processing of easy steps and deeper analysis for complex reasoning. Without any training or additional cost, our plug-in module delivers an average +1.3% accuracy with -8.6% token usage across leading LRMs and advanced reasoning benchmarks. All of our algorithms are implemented based on vLLM and are expected to support broader applications and inspire future research.
