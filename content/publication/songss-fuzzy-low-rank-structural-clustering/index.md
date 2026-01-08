---
title: "Salient detection via the fusion of background-based and multiscale frequency-domain features"
authors:
- 宋森森
date: "2022-11-01"





# Schedule page publish date (NOT publication's date).
publishDate: "2025-10-20T00:00:00+08:00"

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ["article-journal"]

# Publication name and optional abbreviated publication name.
publication: "Information Sciences"
publication_short: ""

abstract: Salient object detection is a fundamental problem in image processing and computer vision. Many saliency detection algorithms based on the background and frequency domain are used to extract salient object clues. However, the former causes the real object to be submerged in the detected object areas, especially in complex or small object scenes. While the latter will lead to the loss of some object information when detecting large objects. To solve these problems and achieve better object detection results, we propose a fusion framework for salient object detection by fusing background and frequency domain features. The background features of the image are extracted by an improved back ground model. This model represents the spatial layout of the image area with respect to the image boundaries. Meanwhile, we present a new frequency-domain processing method to obtain multiscale frequency-domain features and mark the saliency of the object at different scales. Within our framework, inspired by human visual attention, we use the idea of a self-attention mechanism to capture the intrinsic relation between back ground and multiscale frequency-domain features. In addition, this fusion framework pro vides a three-dimensional Gaussian convolution kernel, which expands two-dimensional local information to three dimensions for feature fusion, thus producing more accurate salient objects. Experiment results demonstrate that the proposed method consistently outperforms eleven state-of-the-art methods on five challenging and complicated datasets in terms of four evaluation metrics.

# Summary. An optional shortened abstract.
summary: Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis posuere tellus ac convallis placerat. Proin tincidunt magna sed ex sollicitudin condimentum.

links:
  - name: DOI
    url: "https://doi.org/10.1016/j.ins.2022.10.103"
url_pdf: "/publication/songss-salient-detection-bg-multiscale-frequency/salient-detection-bg-multiscale-frequency.pdf"



  





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