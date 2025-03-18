---
title: "ROUTE: Robust Multitask Tuning and Collaboration for Text-to-SQL"
collection: publications
category: conferences
permalink: /publication/ROUTE
excerpt: 'This paper is about the number 1. The number 2 is left for future work.'
date: 2025-02-11
venue: 'International Conference on Learning Representations (<b>ICLR</b>)'
slidesurl: 'https://github.com/alibaba/Route'
paperurl: 'https://openreview.net/pdf?id=BAglD6NGy0'
authors: 'Yang Qin, Chao Chen, <b><u>Zhihang Fu</u><sup>&diams;</sup></b>, Ze Chen, Dezhong Peng, Peng Hu, Jieping Ye'
image: '/images/route.png'

#citation: 'Your Name, You. (2009). &quot;Paper Title Number 1.&quot; <i>Journal 1</i>. 1(1).'
---

Despite the significant advancements in Text-to-SQL (Text2SQL) facilitated by large language models (LLMs), the latest state-of-the-art techniques are still trapped in the in-context learning of closed-source LLMs (e.g., GPT-4), which limits their applicability in open scenarios. To address this challenge, we propose a novel RObust mUltitask Tuning and collaboration mEthod (ROUTE) to improve the comprehensive capabilities of open-source LLMs for Text2SQL, thereby providing a more practical solution. Our approach begins with multi-task supervised fine-tuning (SFT) using various synthetic training data related to SQL generation. Unlike existing SFT-based Text2SQL methods, we introduced several additional SFT tasks, including schema linking, noise correction, and continuation writing. Engaging in a variety of SQL generation tasks enhances the model’s understanding of SQL syntax and improves its ability to generate high-quality SQL queries. Additionally, inspired by the collaborative modes of LLM agents, we introduce a Multitask Collaboration Prompting (MCP) strategy. This strategy leverages collaboration across several SQL-related tasks to reduce hallucinations during SQL generation, thereby maximizing the potential of enhancing Text2SQL performance through explicit multitask capabilities. Extensive experiments and in-depth analyses have been performed on eight open-source LLMs and five widely-used benchmarks. The results demonstrate that our proposal outperforms the latest Text2SQL methods and yields promising performance.