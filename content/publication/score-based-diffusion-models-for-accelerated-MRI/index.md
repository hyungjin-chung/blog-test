---
title: "Score-based diffusion models for accelerated MRI"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- admin
- Jong Chul Ye

# Author notes (optional)
author_notes: ""

date: "2021-10-08T00:00:00Z"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: "2021-12-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["3"]

# Publication name and optional abbreviated publication name.
publication: In ArXiv
publication_short: In ArXiv

abstract: Score-based diffusion models provide a powerful way to model images using the gradient of the data distribution. Leveraging the learned score function as a prior, here we introduce a way to sample data from a conditional distribution given the measurements, such that the model can be readily used for solving inverse problems in imaging, especially for accelerated MRI. In short, we train a continuous time-dependent score function with denoising score matching. Then, at the inference stage, we iterate between numerical SDE solver and data consistency projection step to achieve reconstruction. Our model requires magnitude images only for training, and yet is able to reconstruct complex-valued data, and even extends to parallel imaging. The proposed method is agnostic to sub-sampling patterns, and can be used with any sampling schemes. Also, due to its generative nature, our approach can quantify uncertainty, which is not possible with standard regression settings. On top of all the advantages, our method also has very strong performance, even beating the models trained with full supervision. With extensive experiments, we verify the superiority of our method in terms of quality and practicality.
# Summary. An optional shortened abstract.
summary: Score-based diffusion models beat supervised learning methods on MRI reconstruction.

tags: [Diffusion model, Score-based model, Compressed-sensing MRI]

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://arxiv.org/abs/2110.05243'
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