---
title: "Interact-RAG: Reason and Interact with the Corpus, Beyond Black-Box Retrieval"
collection: publications
category: conferences
permalink: /publication/InteractRAG
excerpt: 'This paper is about the number 1. The number 2 is left for future work.'
date: 2026-04-24
venue: 'International Conference on Learning Representations (<b>ICLR</b>)'
#slidesurl: ''
paperurl: 'https://arxiv.org/pdf/2510.27566'
authors: 'Yulong Hui, Chao Chen, <b><u>Zhihang Fu</u><sup>&diams;</sup></b>, Yihao Liu, Jieping Ye, Huanchen Zhang'
image: '/images/interact-rag.png'
#citation: 'Your Name, You. (2009). &quot;Paper Title Number 1.&quot; <i>Journal 1</i>. 1(1).'
---

Retrieval-Augmented Generation (RAG) has significantly enhanced LLMs by incorporating external information. However, prevailing agentic RAG approaches are constrained by a critical limitation: they treat the retrieval process as a black-box querying operation. This confines agents' actions to query issuing, hindering its ability to tackle complex information-seeking tasks. To address this, we introduce Interact-RAG, a new paradigm that elevates the LLM agent from a passive query issuer into an active manipulator of the retrieval process. We dismantle the black-box with a Corpus Interaction Engine, equipping the agent with a set of action primitives for fine-grained control over information retrieval. To further empower the agent on the entire RAG pipeline, we first develop a reasoning-enhanced workflow, which enables both zero-shot execution and the synthesis of interaction trajectories. We then leverage this synthetic data to train a fully autonomous end-to-end agent via Supervised Fine-Tuning (SFT), followed by refinement with Reinforcement Learning (RL). Extensive experiments across six benchmarks demonstrate that Interact-RAG significantly outperforms other advanced methods, validating the efficacy of our reasoning-interaction strategy.
