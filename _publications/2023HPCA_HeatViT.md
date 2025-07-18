---
title: "HeatViT: Hardware-Efﬁcient Adaptive Token Pruning for Vision Transformers"
collection: publications
category: conferences
permalink: /publication/2023HPCA_HeatViT
excerpt: ''
date: 2023-02-25
venue: 'IEEE International Symposium on High-Performance Computer Architecture (HPCA)'
paperurl: 'http://mengshus.github.io/files/2023HPCA_HeatViT.pdf'
bibtexurl: 'http://mengshus.github.io/files/2023HPCA_HeatViT.bib'
---

While vision transformers (ViTs) have continuously achieved new milestones in the field of computer vision, their sophisticated network architectures with high computation and memory costs have impeded their deployment on resource-limited edge devices.
In this paper, we propose a hardware-efficient image-adaptive token pruning framework, called HeatViT, for efficient yet accurate ViT acceleration on embedded FPGAs.
Based on the inherent computational patterns in ViTs, we first adopt an effective, hardware-efficient, and learnable head-evaluation token selector, which can be progressively inserted before transformer blocks to dynamically identify and consolidate the non-informative tokens from input images.
Moreover, we implement the token selector on hardware by adding miniature control logic to heavily reuse existing hardware components built for the backbone ViT.
To improve the hardware efficiency, we further employ 8-bit fixed-point quantization and propose polynomial approximations with regularization effect on quantization error for the frequently used nonlinear functions in ViTs.
Compared to existing ViT pruning studies, under the similar computation cost, HeatViT can achieve 0.7%$$\sim$$8.9% higher accuracy; while under the similar model accuracy, HeatViT can achieve more than 28.4%$$\sim$$65.3% computation reduction, for various widely used ViTs, including DeiT-T, DeiT-S, DeiT-B, LV-ViT-S, and LV-ViT-M, on the ImageNet dataset.
Compared to the baseline hardware accelerator, our implementations of HeatViT on the Xilinx ZCU102 FPGA achieve 3.46$$\times \sim$$4.89$$\times$$ speedup with a trivial resource utilization overhead of 8%$$\sim$$11% more DSPs and 5%$$\sim$$8% more LUTs.
