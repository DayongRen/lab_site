---
title: "A Fuzzy C-Means Clustering Algorithm for Real Medical Image Segmentation"
authors:
  - 张飞飞
date: "2024-11-01"
# Schedule page publish date (NOT publication's date).
publishDate: "2025-10-20T00:00:00+08:00"

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ["paper-conference"]

# Publication name and optional abbreviated publication name.
publication: "ICASSP 2025"
publication_short: ""

abstract: In the field of medical image processing, the presence of noise can often result in the obfuscation of crucial details, which in turn can have a detrimental impact on the accuracy of clinical diagnoses. In order to effectively remove noise and improve segmentation performance, this paper proposes a refined Fuzzy C-Means (FCM) algorithm, designated as MKL-FCM. The method commences with Poisson denoising, which enables more effective handling of the noise characteristics inherent to medical images. Subsequently, multi-scale Kullback-Leibler divergence is utilised to analyse local image information across varying scales, facilitating the differentiation between tissues and pathological regions. Furthermore, tight wavelet frames are capable of capturing fine image details, while reverse optimisation of the objective function serves to correct errors in feature reconstruction, thereby enhancing the accuracy of the segmentation process. The experimental results demonstrate that MKL-FCM enhances both image clarity and segmentation accuracy, and outperforms existing methods in terms of efficiency.

# Summary. An optional shortened abstract.
summary: Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis posuere tellus ac convallis placerat. Proin tincidunt magna sed ex sollicitudin condimentum.

# links:
#   - name: DOI
#     url: "https://doi.org/10.1016/j.ins.2022.10.103"
url_pdf: "/publication/zff_FCM/icassp2025.pdf"





# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  filename: featured.jpg 
  caption: ''
  focal_point: ""
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects:
- internal-project

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: example
share: false
comments: false   # 也顺便关掉评论（如果主题支持评论）

---