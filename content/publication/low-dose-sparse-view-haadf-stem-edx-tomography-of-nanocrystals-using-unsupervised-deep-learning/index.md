---
title: "Low-dose sparse-view HAADF-STEM-EDX tomography of nanocrystals using unsupervised deep learning"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- Eunju Cha
- admin
- Jaeduck Jang,
- Junho Lee,
- Eunha Lee,
- Jong Chul Ye

# Author notes (optional)
author_notes: 
- "Equal contribution"
- "Equal contribution"

date: "2022-06-01T00:00:00Z"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: "2022-06-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

# Publication name and optional abbreviated publication name.
publication: In ACS Nano
publication_short: In ACS Nano

abstract: High-angle annular dark-field (HAADF) scanning transmission electron microscopy (STEM) can be acquired together with energy-dispersive X-ray spectroscopy (EDX) to give complementary information of the nano-particles being imaged. Recent  deep learning approaches show potential for accurate 3D tomographic reconstruction  for these  applications, but large number of high-quality electron micrographs are usually required for supervised training, which may be difficult to collect due to the damage on the  particles from the electron beam. To overcome these limitations and enable tomographic reconstruction even in low-dose sparse-view conditions, here we present an unsupervised deep learning method for HAADF-STEM-EDX tomography. Specifically, to improve EDX image quality from low dose condition, a HAADF-constrained unsupervised denoising approach is proposed. Additionally, to enable extreme sparse-view tomographic reconstruction, unsupervised view enrichment scheme is proposed in the projection domain. Extensive experiments with different types of quantum dots show that the proposed method offers a high quality reconstruction even with only three projection views recorded under low dose conditions.
# Summary. An optional shortened abstract.
summary: Unsupervised deep learning enables low-dose extreme sparse view HAADF-STEM-EDX tomography reconstruction.

tags: [Unsupervised Learning, ProjectionGAN, HAADF-STEM-EDX]

# Display this page in the Featured widget?
featured: false

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: ''
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