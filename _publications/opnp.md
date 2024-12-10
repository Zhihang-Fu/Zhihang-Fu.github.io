---
title: "Optimal Parameter and Neuron Pruning for Out-of-Distribution Detection"
collection: publications
category: conferences
permalink: /publication/OPNP
excerpt: 'This paper is about the number 1. The number 2 is left for future work.'
date: 2023-10-20
venue: 'Conference on Neural Information Processing Systems (<b>NeurIPS</b>)'
#slidesurl: 'https://github.com/alibaba/catex'
paperurl: 'https://proceedings.neurips.cc/paper_files/paper/2023/file/a4316bb210a59fb7aafeca5dd21c2703-Paper-Conference.pdf'
authors: 'Chao Chen, <b><u>Zhihang Fu</u><sup>&sect;</sup></b>, Kai Liu, Ze Chen, Mingyuan Tao, Jieping Ye'

#citation: 'Your Name, You. (2009). &quot;Paper Title Number 1.&quot; <i>Journal 1</i>. 1(1).'
---
For a machine learning model deployed in real world scenarios, the ability of detecting out-of-distribution (OOD) samples is indispensable and challenging. Most existing OOD detection methods focused on exploring advanced training skills or training-free tricks to prevent the model from yielding overconfident confidence score for unknown samples. The training-based methods require expensive training cost and rely on OOD samples which are not always available, while most trainingfree methods can not efficiently utilize the prior information from the training data. In this work, we propose an Optimal Parameter and Neuron Pruning (OPNP) approach, which aims to identify and remove those parameters and neurons that lead to over-fitting. The main method is divided into two steps. In the first step, we evaluate the sensitivity of the model parameters and neurons by averaging gradients over all training samples. In the second step, the parameters and neurons with exceptionally large or close to zero sensitivities are removed for prediction. Our proposal is training-free, compatible with other post-hoc methods, and exploring the information from all training data. Extensive experiments are performed on multiple OOD detection tasks and model architectures, showing that our proposed OPNP consistently outperforms the existing methods by a large margin.