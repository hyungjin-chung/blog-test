---
title: "Simultaneous super-resolution and motion artifact removal in diffusion-weighted MRI using unsupervised deep learning"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- admin
- Jaehyun Kim
- Jeong Hee Yoon
- Jeong Min Lee
- Jong Chul Ye

# Author notes (optional)
author_notes:

date: "2020-05-01T00:00:00Z"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: "2021-05-21T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["3"]

# Publication name and optional abbreviated publication name.
publication: In ArXiv
publication_short: In ArXiv

abstract: Diffusion-weighted MRI is nowadays performed routinely due to its prognostic ability, yet the quality of the scans are often unsatisfactory which can subsequently hamper the clinical utility. To overcome the limitations, here we propose a fully unsupervised quality enhancement scheme, which boosts the resolution and removes the motion artifact simultaneously. This process is done by first training the network using optimal transport driven cycleGAN with stochastic degradation block which learns to remove aliasing artifacts and enhance the resolution, then using the trained network in the test stage by utilizing bootstrap subsampling and aggregation for motion artifact suppression. We further show that we can control the trade-off between the amount of artifact correction and resolution by controlling the bootstrap subsampling ratio at the inference stage. To the best of our knowledge, the proposed method is the first to tackle super-resolution and motion artifact correction simultaneously in the context of MRI using unsupervised learning. We demonstrate the efficiency of our method by applying it to both quantitative evaluation using simulation study, and to in vivo diffusion-weighted MR scans, which shows that our method is superior to the current state-of-the-art methods. The proposed method is flexible in that it can be applied to various quality enhancement schemes in other types of MR scans, and also directly to the quality enhancement of apparent diffusion coefficient maps.

# Summary. An optional shortened abstract.
summary: Unsupervised deep learning for simultaneous super-resolution and motion artifact removal of diffusion-weighted MRI scans is proposed.

tags: [Unsupervised Learning, MRI, DWI, Super resolution, Motion artifact correction]

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://arxiv.org/abs/2105.00240'
url_code: ''
url_dataset: ''
url_poster: ''
url_project: ''
url_slides: ''
url_source: ''
url_video: ''

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: 'Image credit: Hyungjin Chung'
  focal_point: ""
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects:
- []

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ""
---