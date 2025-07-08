---
title: "Hardware-Friendly 3-D CNN Acceleration With Balanced Kernel Group Sparsity"
collection: publications
category: manuscripts
permalink: /publication/2024TCAD_3D-KGS
excerpt: ''
date: 2024-04-16
venue: 'IEEE Transactions on Computer-Aided Design of Integrated Circuits and Systems'
paperurl: 'http://mengshus.github.io/files/2024TCAD_3D-KGS.pdf'
bibtexurl: 'http://mengshus.github.io/files/2024TCAD_3D-KGS.bib'
---

Being capable of extracting more information than 2D Convolutional Neural Networks (CNNs), 3D CNNs have been playing a vital role in video analysis tasks like human action recognition, but their massive operations hinder the real-time execution on edge devices with constrained computation and memory resources. Although various model compression techniques have been applied to accelerate 2D CNNs, there are rare efforts in investigating hardware-friendly pruning of 3D CNNs and acceleration on customizable edge platforms like FPGAs. This work starts from proposing a kernel group row-column (KGRC) weight sparsity pattern, which is fine-grained to achieve high pruning ratios with negligible accuracy loss, and balanced across kernel groups to achieve high computation parallelism on hardware. The reweighted pruning algorithm for this sparsity is then presented and performed on 3D CNNs, followed by quantization under different precisions. Along with model compression, FPGA-based accelerators with four modes are designed in support of the kernel group sparsity in multiple dimensions. The co-design framework of the pruning algorithm and the accelerator is tested on two representative 3D CNNs, namely C3D and R(2+1)D, with the Xilinx ZCU102 FPGA platform for action recognition. The experimental results indicate that the accelerator implementation with the KGRC sparsity and 8-bit quantization achieves a good balance between the speedup and model accuracy, leading to acceleration ratios of 4.12$$\times$$ for C3D and 3.85$\times$ for R(2+1)D compared with the 16-bit baseline designs supporting only dense models.
