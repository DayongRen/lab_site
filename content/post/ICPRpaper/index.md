---
title: 实验室论文发表于 ICPR 2024
date: 2025-10-10
image:
  focal_point: 'top'
profile: false
share: false
---

实验室一项关于医学图像分割的研究工作发表于 ICPR 2024（International Conference on Pattern Recognition）。

<!--more-->

该论文 《Dual-MambaNet: A Lightweight Dual-Branch Brain Image Segmentation Network Based on Local Attention and Mamba》 关注高分辨率脑部 MRI 图像分割中局部纹理信息易丢失、模型部署成本较高的问题，提出了一种轻量化的双分支分割网络 Dual-MambaNet。

方法在编码阶段结合 局部注意力机制（Outlook Attention） 与 Mamba 状态空间模型，同时建模局部结构细节与全局上下文信息；在解码阶段引入双分支结构，并通过多层级像素级对比损失促进不同层级特征的有效融合。在保证较低参数量与计算复杂度的前提下，该模型在多个公开脑 MRI 数据集上取得了具有竞争力的分割性能。

该工作体现了实验室在 模式识别与轻量化视觉模型设计 方向上的持续探索。