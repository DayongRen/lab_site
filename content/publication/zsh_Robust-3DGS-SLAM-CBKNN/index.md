---
title: "Robust 3DGS-based SLAM via Adaptive Kernel Smoothing"
authors:
  - 张守贺
date: "2026-03-05"
publishDate: "2026-07-05T00:00:00+08:00"

publication_types: ["paper-conference"]
publication: "ECCV 2026 Submission"
publication_short: "ECCV 2026"

abstract: In this paper, we challenge the conventional notion in 3DGS-SLAM that rendering quality is the primary determinant of tracking accuracy. We argue that, compared to solely pursuing a perfect scene representation, it is more critical to enhance the robustness of the rasterization process against parameter errors to ensure stable camera pose tracking. To address this challenge, we propose a novel approach that leverages a smooth kernel strategy to enhance the robustness of 3DGS-based SLAM. Unlike conventional methods that focus solely on minimizing rendering error, our core insight is to make the rasterization process more resilient to imperfections in the 3DGS parameters. We hypothesize that by allowing each Gaussian to influence a smoother, wider distribution of pixels during rendering, we can mitigate the detrimental effects of parameter noise from outlier Gaussians. This approach intentionally introduces a controlled blur to the rendered image, which acts as a regularization term, stabilizing the subsequent pose optimization. While a complete redesign of the rasterization pipeline is an ideal solution, we propose a practical and effective alternative that is readily integrated into existing 3DGS frameworks. Our method, termed Corrective Blurry KNN (CB-KNN), adaptively modifies the RGB values and locations of the K-nearest neighboring Gaussians within a local region. This dynamic adjustment generates a smoother local rendering, reducing the impact of erroneous GS parameters on the overall image. Experimental results demonstrate that our approach, while maintaining the overall quality of the scene reconstruction (mapping), significantly improves the robustness and accuracy of camera pose tracking.

summary: 提出 Corrective Blurry KNN (CB-KNN) 自适应核平滑策略，通过在关键帧阶段对高斯近邻进行瞬时位置与颜色校正，降低 3DGS 参数噪声对位姿优化的干扰，在保持重建质量的同时提升跟踪鲁棒性。

url_pdf: "/publication/zsh_Robust-3DGS-SLAM-CBKNN/Robust-3DGS-based-SLAM-via-Adaptive-Kernel-Smoothing.pdf"
url_code: "https://github.com/xju-zsh/Robust-3DGS-based-SLAM-via-Adaptive-Kernel-Smoothing"

image:
  filename: featured.png
  caption: ""
  focal_point: "Center"
  preview_only: false

projects: []
slides: ""
share: false
comments: false
---

这项工作面向 3DGS-based SLAM 中一个非常关键但常被忽略的问题: 渲染结果越锐利, 并不一定越有利于位姿跟踪。当高斯参数受到噪声、外点或局部估计误差影响时, 栅格化过程会放大这些误差, 进而在优化时制造尖锐的局部极值和不稳定梯度。该工作提出 **Corrective Blurry KNN (CB-KNN)**, 通过自适应核平滑让渲染对参数误差更不敏感, 从而获得更稳健的相机跟踪结果。

资源链接:

- [Paper PDF](Robust-3DGS-based-SLAM-via-Adaptive-Kernel-Smoothing.pdf)
- [GitHub Repository](https://github.com/xju-zsh/Robust-3DGS-based-SLAM-via-Adaptive-Kernel-Smoothing)

## Method Overview

CB-KNN 的核心不是永久改写地图中的高斯参数, 而是在 **keyframe** 阶段引入一种瞬时的局部正则化:

- 自适应选择邻域大小 `K`
- 对局部高斯的位置做轻量对齐, 减少空洞和几何跳变
- 对颜色做邻域平滑, 抑制高频伪影和异常颜色扰动

这样做的直接效果是: 渲染得到的颜色图与深度图更平滑、更稳定, 光度误差曲面也更容易优化, 从而降低 tracking drift 和 pose jitter。

{{< figure src="figure-2.png" caption="CB-KNN framework overview. The method inserts adaptive kernel smoothing into the keyframe stage of a 3DGS-SLAM pipeline, while keeping the canonical Gaussian map unchanged." numbered="true" >}}

## Why Smoothing Helps

论文给出的一个直观解释是: 当 3DGS 参数里存在高频噪声时, 原始损失面往往崎岖且不连续, 梯度下降很容易被局部极小值卡住。CB-KNN 通过让高斯对像素的影响更平滑, 把原本尖锐的优化景观“抹平”, 使跟踪过程更容易收敛到稳定解。

{{< figure src="figure-1.png" caption="Optimization landscape comparison. Adaptive smoothing suppresses high-frequency irregularities and expands the basin of attraction for pose optimization." numbered="true" >}}

## Experimental Results

从定性结果看, 该方法在多组场景中都表现出更稳定的轨迹和更少的局部伪影。

{{< figure src="figure-3.png" caption="Trajectory comparison on Replica, TUM-RGBD, and ScanNet scenes. The CB-KNN variant follows ground-truth trajectories more closely and exhibits less jitter." numbered="true" >}}

{{< figure src="figure-4.png" caption="Artifact suppression examples. Compared with the baseline, CB-KNN reduces high-frequency rendering artifacts and geometric discontinuities in challenging local regions." numbered="true" >}}

{{< figure src="figure-5.png" caption="Convergence analysis on Room0. The smoothed objective converges faster and avoids the oscillatory behavior of the baseline tracker." numbered="true" >}}

## Takeaway

这篇工作强调的不是“把图渲染得更漂亮”, 而是让 **3DGS 渲染过程对参数误差更鲁棒**。对于 3DGS-based SLAM 来说, 这类面向 tracking stability 的设计非常有价值, 也让该方法更适合继续扩展到真实动态场景和移动端算力受限环境。
