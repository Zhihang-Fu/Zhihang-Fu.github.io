---
title: "ESOD: Efficient Small Object Detection on High-Resolution Images"
collection: publications
category: conferences
permalink: /publication/ESOD
excerpt: 'This paper is about the number 1. The number 2 is left for future work.'
date: 2024-11-21
venue: 'IEEE Transactions on Image Processing (<b>TIP</b>)'
slidesurl: 'https://github.com/alibaba/esod/tree/main'
paperurl: 'https://arxiv.org/pdf/2407.16424'
authors: 'Kai Liu, <b><u>Zhihang Fu</u><sup>&diams;</sup></b>, Sheng Jin, Ze Chen, Fan Zhou, Rongxin Jiang, Yaowu Chen, Jieping Ye.'

#citation: 'Your Name, You. (2009). &quot;Paper Title Number 1.&quot; <i>Journal 1</i>. 1(1).'
---

Enlarging input images is a straightforward and effective approach to promote small object detection. However, simple image enlargement is significantly expensive on both computations and GPU memory. In fact, small objects are usually sparsely distributed and locally clustered. Therefore, massive feature extraction computations are wasted on the non-target background area of images. Recent works have tried to pick out target-containing regions using an extra network and perform conventional object detection, but the newly introduced computation limits their final performance. In this paper, we propose to reuse the detector's backbone to conduct feature-level object-seeking and patch-slicing, which can avoid redundant feature extraction and reduce the computation cost. Incorporating a sparse detection head, we are able to detect small objects on high-resolution inputs (e.g., 1080P or larger) for superior performance. The resulting Efficient Small Object Detection (ESOD) approach is a generic framework, which can be applied to both CNN- and ViT-based detectors to save the computation and GPU memory costs. Extensive experiments demonstrate the efficacy and efficiency of our method. In particular, our method consistently surpasses the SOTA detectors by a large margin (e.g., 8% gains on AP) on the representative VisDrone, UAVDT, and TinyPerson datasets. Code will be made public soon.