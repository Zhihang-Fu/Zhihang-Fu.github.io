---
title: "Rethinking Out-of-Distribution Detection on Imbalanced Data Distribution"
collection: publications
category: conferences
permalink: /publication/ImOOD
excerpt: 'This paper is about the number 1. The number 2 is left for future work.'
date: 2024-10-20
venue: 'Conference on Neural Information Processing Systems (<b>NeurIPS</b>)'
slidesurl: 'https://github.com/alibaba/imood'
paperurl: 'https://arxiv.org/pdf/2407.16430'
authors: 'Kai Liu, <b><u>Zhihang Fu</u><sup>&sect;</sup></b>, Sheng Jin, Chao Chen, Ze Chen, Rongxin Jiang, Fan Zhou, Yaowu Chen, Jieping Ye'

#citation: 'Your Name, You. (2009). &quot;Paper Title Number 1.&quot; <i>Journal 1</i>. 1(1).'
---

Detecting and rejecting unknown out-of-distribution (OOD) samples is critical for deployed neural networks to void unreliable predictions. In real-world scenarios, however, the efficacy of existing OOD detection methods is often impeded by the inherent imbalance of in-distribution (ID) data, which causes significant performance decline. Through statistical observations, we have identified two common challenges faced by different OOD detectors: misidentifying tail class ID samples as OOD, while erroneously predicting OOD samples as head class from ID. To explain this phenomenon, we introduce a generalized statistical framework, termed ImOOD, to formulate the OOD detection problem on imbalanced data distribution. Consequently, the theoretical analysis reveals that there exists a class-aware bias item between balanced and imbalanced OOD detection, which contributes to the performance gap. Building upon this finding, we present a unified training-time regularization technique to mitigate the bias and boost imbalanced OOD detectors across architecture designs. Our theoretically grounded method translates into consistent improvements on the representative CIFAR10-LT, CIFAR100-LT, and ImageNet-LT benchmarks against several state-of-the-art OOD detection approaches.