---
title: "Adaptive fuzzy weighted C-mean image segmentation algorithm combining a new distance metric and prior entropy"
authors:
- 宋森森
date: "2024-05-01"





# Schedule page publish date (NOT publication's date).
publishDate: "2025-10-20T00:00:00+08:00"

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ["article-journal"]

# Publication name and optional abbreviated publication name.
publication: "Engineering Applications of Artificial Intelligence"
publication_short: ""

abstract: The fuzzy C-mean clustering algorithm (FCM) is effective in image segmentation. However, its sensitivity to initialization settings and the limitation of the Euclidean distance metric in measuring similarity lead to unsatisfactory image segmentation. To overcome these shortcomings, we propose an adaptive fuzzy weighted C-mean image segmentation algorithm that combines a new distance metric and prior entropy. This algorithm significantly contributes in three aspects. First, we employ an improved sparse subspace clustering (SSC) algorithm based on the superpixel image for initialization settings. This step aims to obtain the initial number of clusters and the membership matrix, ensuring the algorithm’s convergence to the optimal solution. Second, to better capture differences between image regions, we introduce a novel distance metric that combines Euclidean and non-Euclidean distances. Simultaneously, the fuzzy weight is introduced to mitigate redundant feature interference, making the clustering result more reasonable. Finally, leveraging prior entropy – a maximum entropy under conditional constraints – we refine the algorithm’s adaptability to unknown features, thereby improving clustering accuracy. Comparative experiments with several state-of-the-art algorithms validate the effectiveness and robustness of our proposed algorithm.

# Summary. An optional shortened abstract.
summary: Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis posuere tellus ac convallis placerat. Proin tincidunt magna sed ex sollicitudin condimentum.

links:
  - name: DOI
    url: "https://doi.org/10.1016/j.engappai.2023.107776"
url_pdf: "/publication/songss-Adaptive-fuzzy-weighted-C-mean-image-segmentation-algorithm-combining-a-new-distance-metric-and-prior-entropy/Adaptive_fuzzy_weighted .pdf"



  





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