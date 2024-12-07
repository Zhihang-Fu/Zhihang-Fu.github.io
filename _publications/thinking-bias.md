---
title: "Delving into the Reversal Curse: How Far Can Large Language Models Generalize?"
collection: publications
category: conferences
permalink: /publication/Thinking-Bias
excerpt: 'This paper is about the number 1. The number 2 is left for future work.'
date: 2024-10-30
venue: 'Conference on Neural Information Processing Systems (<b>NeurIPS</b>)'
slidesurl: 'https://github.com/alibaba/thinking_bias'
paperurl: 'https://arxiv.org/pdf/2410.18808'
authors: 'Zhengkai Lin, <b><u>Zhihang Fu</u><sup>&diams;</sup></b>, Kai Liu, Liang Xie, Binbin Lin, Wenxiao Wang, Deng Cai, Yue Wu, Jieping Ye'

#citation: 'Your Name, You. (2009). &quot;Paper Title Number 1.&quot; <i>Journal 1</i>. 1(1).'
---

While large language models (LLMs) showcase unprecedented capabilities, they also exhibit certain inherent limitations when facing seemingly trivial tasks. A prime example is the recently debated "reversal curse", which surfaces when models, having been trained on the fact "A is B", struggle to generalize this knowledge to infer that "B is A". In this paper, we examine the manifestation of the reversal curse across various tasks and delve into both the generalization abilities and the problem-solving mechanisms of LLMs. This investigation leads to a series of significant insights: (1) LLMs are able to generalize to "B is A" when both A and B are presented in the context as in the case of a multiple-choice question. (2) This generalization ability is highly correlated to the structure of the fact "A is B" in the training documents. For example, this generalization only applies to biographies structured in "\[Name\] is \[Description\]" but not to "\[Description\] is \[Name\]". (3) We propose and verify the hypothesis that LLMs possess an inherent bias in fact recalling during knowledge application, which explains and underscores the importance of the document structure to successful learning. (4) The negative impact of this bias on the downstream performance of LLMs can hardly be mitigated through training alone. These findings offer a novel perspective on interpreting LLMs' generalization through their intrinsic mechanisms and provide insights for developing more effective learning methods.