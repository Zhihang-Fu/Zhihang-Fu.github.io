---
title: "Enhancing LLM’s Cognition via Structurization"
collection: publications
category: conferences
permalink: /publication/StruXGPT
excerpt: 'This paper is about the number 1. The number 2 is left for future work.'
date: 2024-10-31
venue: 'Conference on Neural Information Processing Systems (<b>NeurIPS</b>)'
slidesurl: 'https://github.com/alibaba/struxgpt'
paperurl: 'https://arxiv.org/pdf/2407.16434'
authors: 'Kai Liu, <b><u>Zhihang Fu</u><sup>&sect;</sup></b>, Chao Chen, Wei Zhang, Rongxin Jiang, Fan Zhou, Yaowu Chen, Yue Wu, and Jieping Ye'

#citation: 'Your Name, You. (2009). &quot;Paper Title Number 1.&quot; <i>Journal 1</i>. 1(1).'
---

When reading long-form text, human cognition is complex and structurized. While large language models (LLMs) process input contexts through a causal and sequential perspective, this approach can potentially limit their ability to handle intricate and complex inputs effectively. To enhance LLM’s cognition capability, this paper presents a novel concept of context structurization. Specifically, we transform the plain, unordered contextual sentences into well-ordered and hierarchically structurized elements. By doing so, LLMs can better grasp intricate and extended contexts through precise attention and information-seeking along the organized structures. Extensive evaluations are conducted across various model architectures and sizes (including a series of auto-regressive LLMs as well as BERT-like masking models) on a diverse set of NLP tasks (e.g., context-based question-answering, exhaustive hallucination evaluation, and passage-level dense retrieval). Empirical results show consistent and significant performance gains afforded by a singleround structurization. In particular, we boost the open-sourced LLaMA2-70B model to achieve comparable performance against GPT-3.5-Turbo as the hallucination evaluator. Besides, we show the feasibility of distilling advanced LLMs’ language processing abilities to a smaller yet effective StruXGPT-7B to execute structurization, addressing the practicality of our approach.