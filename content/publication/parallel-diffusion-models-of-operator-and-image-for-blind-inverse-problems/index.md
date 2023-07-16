---
title: "Parallel Diffusion Models of Operator and Image for Blind Inverse Problems"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- admin
- Jeongsol Kim
- Sehui Kim
- Jong Chul Ye

# Author notes (optional)
author_notes:
- "Equal contribution"
- "Equal contribution"

date: "2023-02-28T00:00:00Z"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: "2023-02-27T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: In IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR), 2023
publication_short: In CVPR 2023

abstract: Diffusion model-based inverse problem solvers have demonstrated state-of-the-art performance in cases where the forward operator is known (i.e. non-blind). However, the applicability of the method to blind inverse problems has yet to be explored. In this work, we show that we can indeed solve a family of blind inverse problems by constructing another diffusion prior for the forward operator. Specifically, parallel reverse diffusion guided by gradients from the intermediate stages enables joint optimization of both the forward operator parameters as well as the image, such that both are jointly estimated at the end of the parallel reverse diffusion procedure. We show the efficacy of our method on two representative tasks -- blind deblurring, and imaging through turbulence -- and show that our method yields state-of-the-art performance, while also being flexible to be applicable to general blind inverse problems when we know the functional forms.

# Summary. An optional shortened abstract.
summary: We propose a method to perform posterior sampling with diffusion models on blind inverse problems.

tags: [Diffusion model, Blind Inverse problem, Posterior sampling]

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://arxiv.org/abs/2211.10656v1'
url_code: 'https://github.com/BlindDPS/blind-dps'
url_dataset: 'https://blinddps.github.io/blind-dps-project/'
url_poster: ''
url_project: ''
url_slides: ''
url_source: ''
url_video: 'https://youtu.be/uQx63WUOIj0'

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