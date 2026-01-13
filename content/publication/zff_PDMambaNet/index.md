---
title: "PDMambaNet: Poisson Denoising-Aided Twin-Path Mamba for Brain MRI Image Segmentation"
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
publication: "ICME 2024"
publication_short: ""

abstract: Brain tissue segmentation is critical for diagnosing and treating brain diseases, but noise introduced during MRI image acquisition can compromise downstream tasks. To address this, we introduce a Poisson denoising module to eliminate Poisson and mixed noise. However, Poisson denoising may blur local brain tissue details and edges, impacting segmentation accuracy. To overcome this, we propose PDMambaNet, which integrates Poisson denoising, the Mamba architecture, and a Twin-Path Decoder (TPD). One decoder focuses on global detail recovery, while the other restores texture and edge information. This structure minimizes detail loss and improves the model’s ability to capture multi-level features. The collaborative effect of TPD reduces over-smoothing and artifact generation, ensuring the preservation of cross-scale spatial information. Extensive subjective and objective evaluations demonstrate that PDMambaNet outperforms existing methods in segmentation performance. The code is available in the supplementary material.

# Summary. An optional shortened abstract.
summary: Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis posuere tellus ac convallis placerat. Proin tincidunt magna sed ex sollicitudin condimentum.

# links:
#   - name: DOI
#     url: "https://doi.org/10.1016/j.ins.2022.10.103"
url_pdf: "/publication/zff_PDMambaNet/icme2025.pdf"







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