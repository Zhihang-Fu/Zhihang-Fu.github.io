---
title: "ROPO: Robust Preference Optimization for Large Language Models"
collection: publications
category: conferences
permalink: /publication/ROPO
excerpt: 'This paper is about the number 1. The number 2 is left for future work.'
date: 2025-05-01
venue: 'International Conference on Machine Learning (<b>ICML</b>)'
#slidesurl: 'https://github.com/alibaba/struxgpt'
paperurl: 'https://arxiv.org/pdf/2404.04102'
authors: 'Xize Liang, Chao Chen, Shuang Qiu, Jie Wang, Yue Wu, <b><u>Zhihang Fu</u><sup>&diams;</sup></b>, Zhihao Shi, Feng Wu, Jieping Ye'
image: '/images/ropo.png'
#citation: 'Your Name, You. (2009). &quot;Paper Title Number 1.&quot; <i>Journal 1</i>. 1(1).'
---

Preference alignment is pivotal for empowering large language models (LLMs) to generate helpful and harmless responses. However, the performance of preference alignment is highly sensitive to the prevalent noise in the preference data. Recent efforts for this problem either marginally alleviate the impact of noise without the ability to actually reduce its presence, or rely on costly teacher LLMs prone to reward misgeneralization. To address these challenges, we propose the RObust Preference Optimization (ROPO) framework, a novel iterative alignment approach that integrates noise-tolerance and filtering of noisy samples without the aid of external models. Specifically, ROPO first formulates the training process with adaptive noise reduction as an optimization problem, which can be efficiently solved in an iterative paradigm. Then, to enhance this iterative solving process with noise-tolerance and noise-identification capabilities, we derive a robust loss that suppresses the gradients from samples with high uncertainty. We demonstrate both empirically and theoretically that the derived loss is key to the noise-tolerance and effective filtering of noisy samples. Furthermore, inspired by our derived loss, we propose a robustness-guided rejection sampling technique to compensate for the potential important information in discarded queries. Experiments on three widely-used datasets of dialogue and post-summarization demonstrate that ROPO significantly outperforms existing preference alignment methods in the practical noise setting and under artificial random symmetric noise, with its advantage increasing as the noise rate increases.