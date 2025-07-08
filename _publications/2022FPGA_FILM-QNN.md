---
title: "FILM-QNN: Efficient FPGA Acceleration of Deep Neural Networks with Intra-Layer, Mixed-Precision Quantization"
collection: publications
category: conferences
permalink: /publication/2022FPGA_FILM-QNN
excerpt: ''
date: 2022-02-13
venue: 'ACM/SIGDA International Symposium on Field-Programmable Gate Arrays'
paperurl: 'http://mengshus.github.io/files/2022FPGA_FILM-QNN.pdf'
bibtexurl: 'http://mengshus.github.io/files/2022FPGA_FILM-QNN.bib'
---

With the trend to deploy Deep Neural Network (DNN) inference models on edge devices with limited resources, quantization techniques have been widely used to reduce on-chip storage and improve computation throughput. However, existing DNN quantization work deploying quantization below 8-bit may be either suffering from evident accuracy loss or facing a big gap between the theoretical improvement of computation throughput and the practical inference speedup.

In this work, we propose a general framework, called FILM-QNN, to quantize and accelerate multiple DNN models across different embedded FPGA devices. First, we propose the novel intra-layer, mixed-precision quantization algorithm that assigns different precisions onto the filters of each layer. The candidate precision levels and assignment granularity are determined from our empirical study with the capability of preserving accuracy and improving hardware parallelism. Second, we apply multiple optimization techniques for the FPGA accelerator architecture in support of quantized computations, including DSP packing, weight reordering, and data packing, to enhance the overall throughput with the available resources.
Moreover, a comprehensive resource model is developed to balance the allocation of FPGA computation resources (LUTs and DSPs) as well as data transfer and on-chip storage resources (BRAMs) to accelerate the computations in mixed precisions within each layer.
Finally, to improve the portability of FILM-QNN, we implement it using Vivado High-Level Synthesis (HLS) on Xilinx PYNQ-Z2 and ZCU102 FPGA boards.
Our experimental results of ResNet-18, ResNet-50, and MobileNet-V2 demonstrate that the implementations with intra-layer, mixed-precision (95% of 4-bit weights and 5% of 8-bit weights, and all 5-bit activations) can achieve comparable accuracy (70.47%, 77.25%, and 65.67% for the three models) as the 8-bit (and 32-bit) versions and comparable throughput (214.8 FPS, 109.1 FPS, and 537.9 FPS on ZCU102) as the 4-bit designs.
