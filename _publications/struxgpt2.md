---
title: "Structure-aware Domain Knowledge Injection for Large Language Models"
collection: publications
category: conferences
permalink: /publication/StruXGPT2
excerpt: 'This paper is about the number 1. The number 2 is left for future work.'
date: 2025-05-15
venue: 'Annual Meeting of the Association for Computational Linguistics (<b>ACL</b>)'
slidesurl: 'https://github.com/alibaba/struxgpt'
paperurl: 'https://arxiv.org/pdf/2407.16724'
authors: 'Kai Liu, Ze Chen, <b><u>Zhihang Fu</u><sup>&sect;</sup></b>, Wei Zhang, Rongxin Jiang, Fan Zhou, Yaowu Chen, Yue Wu, Jieping Ye'
image: '/images/struxgpt2.png'
#citation: 'Your Name, You. (2009). &quot;Paper Title Number 1.&quot; <i>Journal 1</i>. 1(1).'
---

This paper introduces a pioneering methodology, termed StructTuning, to efficiently transform foundation Large Language Models (LLMs) into domain specialists. It significantly reduces the training corpus needs to a mere 5% while achieving an impressive 100% of traditional knowledge injection performance. Motivated by structured human education, we propose a novel two-stage strategy for knowledge injection and alignment: Structure-aware Continual Pre-Training (SCPT) and Structureaware Supervised Fine-Tuning (SSFT). In the SCPT phase, we automatically extract the domain knowledge taxonomy and reorganize the training corpora, enabling LLMs to effectively link textual segments to targeted knowledge points within the taxonomy. In the SSFT phase, we explicitly prompt models to elucidate the underlying knowledge structure in their outputs, leveraging the structured domain insight to address practical problems. Our ultimate method was extensively evaluated across model architectures and scales on LongBench and MMedBench datasets, demonstrating superior performance against other knowledge injection methods. We also explored our method’s scalability across different training corpus sizes, laying the foundation to enhance domain-specific LLMs with better data utilization.