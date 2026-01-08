---
title: "Image Segmentation Based on Fuzzy Low-Rank Structural Clustering"
authors:
- 宋森森
date: "2023-07-01"





# Schedule page publish date (NOT publication's date).
publishDate: "2025-10-20T00:00:00+08:00"

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ["article-journal"]

# Publication name and optional abbreviated publication name.
publication: " IEEE Transactions on Fuzzy Systems"
publication_short: ""

abstract: Fuzzy clustering is an essential algorithm in image segmentation, and most of them are based on fuzzy c-mean algorithms. However, it is sensitive to noise, center point selection, cluster number, and distance metric. To address this problem, we propose a new fuzzy clustering method based on low-rank representation (LRR) for image segmentation, which integrates low-rank structure with fuzzy theory. First, we improve the morphological reconstruction superpixel method based on edge detection by introducing anisotropy to enhance the image edge. Thus, on the one hand, the improved morphological reconstruction superpixel method can improve its noise-resistance performance; on the other hand, the complexity of the subsequent low-rank computation can be reduced by enhancing the superpixels constructed by the edges. Second, inspired by the fact that rank can represent correlation, we propose the concept of fuzzy low-rank structure, which is not dealing with data directly but with the relationship between data. Specifically, we perform rank minimization on the constructed membership matrix to obtain the optimal matrix. To obtain better clustering results, we added the Frobenius norm of the fuzzy matrix as a fuzzy regularization term in the LRR model to achieve global convergence and obtain a membership matrix with a strong element correlation. Finally, we obtain the final clustering results by clustering the processed membership matrix using a subspace clustering with a low-rank structure constraint. Experiments performed on artificial and real-world images show that the proposed method is more effective and efficient than the current state-of-the-art methods.

# Summary. An optional shortened abstract.
summary: Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis posuere tellus ac convallis placerat. Proin tincidunt magna sed ex sollicitudin condimentum.

links:
  - name: DOI
    url: "https://doi.org/10.1109/TFUZZ.2022.3220925"
url_pdf: "/publication/songss-fuzzy-low-rank-structural-clustering/Image_Segmentation_Based_on_Fuzzy_Low-Rank_Structural_Clustering.pdf"



  





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