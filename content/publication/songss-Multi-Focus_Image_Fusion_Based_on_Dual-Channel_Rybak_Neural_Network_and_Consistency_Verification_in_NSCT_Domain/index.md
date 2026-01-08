---
title: "Multi-Focus Image Fusion Based on Dual-Channel Rybak Neural Network and Consistency Verification in NSCT Domain"
authors:
- 宋森森
date: "2025-05-01"





# Schedule page publish date (NOT publication's date).
publishDate: "2025-10-20T00:00:00+08:00"

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ["article-journal"]

# Publication name and optional abbreviated publication name.
publication: " Fractal and Fractional.2025"
publication_short: ""

abstract: "In multi-focus image fusion, accurately detecting and extracting focused regions remains a key challenge. Some existing methods suffer from misjudgment of focus areas, resulting in incorrect focus information or the unintended retention of blurred regions in the fused image. To address these issues, this paper proposes a novel multi-focus image fusion method that leverages a dual-channel Rybak neural network combined with consistency verification in the nonsubsampled contourlet transform (NSCT) domain. Specifically, the high-frequency sub-bands produced by NSCT decomposition are processed using the dual-channel Rybak neural network and a consistency verification strategy, allowing for more accurate extraction and integration of salient details. Meanwhile, the low-frequency sub-bands are fused using a simple averaging approach to preserve the overall structure and brightness information. The effectiveness of the proposed method has been thoroughly evaluated through comprehensive qualitative and quantitative experiments conducted on three widely used public datasets: Lytro, MFFW, and MFI-WHU. Experimental results show that our method consistently outperforms several state-of-the-art image fusion techniques, including both traditional algorithms and deep learning-based approaches, in terms of visual quality and objective performance metrics.These results clearly demonstrate the robustness and superiority of the proposed fusion framework in handling multi-focus image fusion tasks."

# Summary. An optional shortened abstract.
summary: Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis posuere tellus ac convallis placerat. Proin tincidunt magna sed ex sollicitudin condimentum.

links:
  - name: DOI
    url: "https://doi.org/10.3390/fractalfract9070432"
url_pdf: "/publication/songss-Multi-Focus_Image_Fusion_Based_on_Dual-Channel_Rybak_Neural_Network_and_Consistency_Verification_in_NSCT_Domain/fractalfract-09-00432-v2.pdf"




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