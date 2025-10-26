---
title: "Learning Instructive Frequency Spectral and Curvature Features for Cloud Detection"
collection: publications
permalink: /publication/2009-10-01-paper-title-number-1
excerpt: 'Learning Instructive Frequency Spectral and Curvature Features for Cloud Detection'
date: 2025-01-01
venue: 'IEEE Geoscience and Remote Sensing Letters'
paperurl: 'http://dx.doi.org/10.1109/LGRS.2025.3561935'
citation: 'Wanjuan Hu, Guanyi Li, <b>Guoguo Zhang</b>, Liang Chang, Dan Zeng. "Learning Instructive Frequency Spectral and Curvature Features for Cloud Detection." <i>IEEE Geoscience and Remote Sensing Letters</i>, vol. 22, Art. 5001605, pp. 1–5, 2025. DOI: 10.1109/LGRS.2025.3561935.'
---

## Abstract

Current cloud detection methods often treat all spectral bands equally, which limits their ability to capture instructive clues necessary for accurate detection. As a result, distinguishing clouds from snow in coexisting environments remains challenging. Moreover, most approaches struggle to adaptively model the boundaries of clouds, which is crucial for detecting thin clouds with ambiguous edges. To address these challenges, we propose a novel approach for cloud detection called FSCFNet, which captures guiding visual features from frequency and curvature computations. FSCFNet comprises two key modules: the frequency spectral feature enhancement module (FSFEM) and the curvature-based edge-awareness module (CEAM). The FSFEM leverages the distinct characteristics of spectral bands to extract instructive visual cues, enabling the network to learn robust discriminative features for ice, snow, and clouds. In contrast, the CEAM adaptively identifies texture-rich regions using curvature, enhancing the ability to delineate thin cloud boundaries. Comprehensive quantitative and qualitative experiments on the Landsat 8 and MODIS datasets demonstrate that FSCFNet consistently outperforms state-of-the-art methods. Our code is publicly available at https://github.com/wanjuanhu/FSCFNet/tree/main.

[Download paper here](files/paper1.pdf)