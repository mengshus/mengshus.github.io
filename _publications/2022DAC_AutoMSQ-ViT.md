---
title: "FPGA-Aware Automatic Acceleration Framework for Vision Transformer with Mixed-Scheme Quantization: Late Breaking Results"
collection: publications
category: conferences
permalink: /publication/2022DAC_AutoMSQ-ViT
excerpt: ''
date: 2022-07-10
venue: '59th ACM/IEEE Design Automation Conference'
paperurl: 'http://mengshus.github.io/files/2022DAC_AutoMSQ-ViT.pdf'
bibtexurl: 'http://mengshus.github.io/files/2022DAC_AutoMSQ-ViT.bib'
---

Vision transformers (ViTs) are emerging with significantly improved accuracy in computer vision tasks. However, their complex architecture and enormous computation/storage demand impose urgent needs for new hardware accelerator design methodology. This work proposes an FPGA-aware automatic ViT acceleration framework based on the proposed mixed-scheme quantization. To the best of our knowledge, this is the first FPGA-based ViT acceleration framework exploring model quantization.
Compared with state-of-the-art ViT quantization work (algorithmic approach only without hardware acceleration), our quantization achieves 0.31% to 1.25% higher Top-1 accuracy under the same bit-width. Compared with the 32-bit floating-point baseline FPGA accelerator, our accelerator achieves around 5.6$$\times$$ improvement on the frame rate (i.e., 56.4 FPS vs. 10.0 FPS) with 0.83% accuracy drop for DeiT-base.
