---
title: "Unsupervised Missing Cone Deep Learning in Optical Diffraction Tomography"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- admin
- Jaeyoung Huh
- Geon Kim
- Yong Keun Park
- Jong Chul Ye

# Author notes (optional)
author_notes:
- "Equal contribution"
- "Equal contribution"

date: "2020-03-16T00:00:00Z"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: "2021-04-27T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["3"]

# Publication name and optional abbreviated publication name.
publication: In ArXiv
publication_short: In ArXiv

abstract: Optical diffraction tomography (ODT) produces three dimensional distribution of refractive index (RI) by measuring scattering fields at various angles. Although the  distribution of RI index is highly informative, due to the missing cone problem stemming from the limited-angle acquisition of holograms, reconstructions have very poor resolution along axial direction compared to the horizontal imaging plane. To solve this issue, here we present a novel unsupervised deep learning framework, which learns the probability distribution of missing projection views through optimal transport driven cycleGAN. Experimental results show that missing cone artifact in ODT can be significantly resolved by the proposed method.

# Summary. An optional shortened abstract.
summary: Two-stage unsupervised reconstruction method for 3D TOF-MRA is developed. A novel projection discriminator in the axial reconstruction step drastically enhances the vessel visiblity.

tags: [Deep Learning, Unsupervised Learning, Optimal Transport, Optical Diffraction Tomography]

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://arxiv.org/pdf/2103.09022.pdf'
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