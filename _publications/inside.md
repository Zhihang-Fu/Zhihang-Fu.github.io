---
title: "INSIDE: LLMs' Internal States Retain the Power of Hallucination Detection"
collection: publications
category: conferences
permalink: /publication/INSIDE
excerpt: 'This paper is about the number 1. The number 2 is left for future work.'
date: 2024-02-01
venue: 'International Conference on Learning Representations (<b>ICLR</b>)'
slidesurl: 'https://github.com/alibaba/eigenscore'
paperurl: 'https://arxiv.org/pdf/2402.03744'
authors: 'Chao Chen, Kai Liu, Ze Chen, Yi Gu, Yue Wu, Mingyuan Tao, <b><u>Zhihang Fu</u><sup>&sect;</sup></b>, Jieping Ye'

#citation: 'Your Name, You. (2009). &quot;Paper Title Number 1.&quot; <i>Journal 1</i>. 1(1).'
---

Knowledge hallucination have raised widespread concerns for the security and reliability of deployed LLMs. Previous efforts in detecting hallucinations have been employed at logit-level uncertainty estimation or language-level self-consistency evaluation, where the semantic information is inevitably lost during the token-decoding procedure. Thus, we propose to explore the dense semantic information retained within LLMs' \textbf{IN}ternal \textbf{S}tates for halluc\textbf{I}nation \textbf{DE}tection (\textbf{INSIDE}). In particular, a simple yet effective \textbf{EigenScore} metric is proposed to better evaluate responses' self-consistency, which exploits the eigenvalues of responses' covariance matrix to measure the semantic consistency/diversity in the dense embedding space. Furthermore, from the perspective of self-consistent hallucination detection, a test time feature clipping approach is explored to truncate extreme activations in the internal states, which reduces overconfident generations and potentially benefits the detection of overconfident hallucinations. Extensive experiments and ablation studies are performed on several popular LLMs and question-answering (QA) benchmarks, showing the effectiveness of our proposal.