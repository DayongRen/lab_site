---
title: "Adaptive Gaussian Regularization Constrained Sparse Subspace Clustering for Image Segmentation"
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
publication: "ICASSP"
publication_short: ""

abstract: Sparse Subspace Clustering (SSC) is integral to image processing, drawing from spectral clustering foundations. However, prevalent methods, relying on an l1-norm constraint, fail to capture nuanced inter-region correlations, affecting segmentation efficacy. To remedy this, we introduce an Adaptive Gaussian Regularization Constrained SSC for enhanced image segmentation. This method begins with superpixel preprocessing to enrich local information. Given the Gaussian nature of the SSC’s sparse coefficient matrix, a Gaussian probability density function is infused as a regularization term, reinforcing regional image ties and facilitating similarity matrix creation. Using spectral clustering, we then define superpixel clusters leading to the final segmentation. When tested against the BSDS500 and SBD datasets and other leading algorithms, our model showcases marked improvements in natural image segmentation.

# Summary. An optional shortened abstract.
summary: Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis posuere tellus ac convallis placerat. Proin tincidunt magna sed ex sollicitudin condimentum.

links:
  - name: DOI
    url: "https://doi.org/10.1109/ICASSP48485.2024.10446289"
url_pdf: "/publication/songss-Adaptive_Gaussian_Regularization_Constrained_Sparse_Subspace_Clustering_for_Image_Segmentation/Adaptive_Gaussian_Regularization_Constrained_Sparse_Subspace_Clustering_for_Image_Segmentation.pdf"






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