---
title: "Deep Diffusion Image Prior for Efficient OOD Adaptation in 3D Inverse Problems"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- admin
- Jong Chul Ye

# Author notes (optional)
author_notes:
- ""

date: "2024-06-15T00:00:00Z"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: "2024-07-15T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: ECCV 2024
publication_short: ECCV 2024

abstract: We propose a new method for solving imaging inverse problems using text-to-image latent diffusion models as general priors. Existing methods using latent diffusion models for inverse problems typically rely on simple null text prompts, which can lead to suboptimal performance. To address this limitation, we introduce a method for prompt tuning, which jointly optimizes the text embedding on-the-fly while running the reverse diffusion process. This allows us to generate images that are more faithful to the diffusion prior. In addition, we propose a method to keep the evolution of latent variables within the range space of the encoder, by projection. This helps to reduce image artifacts, a major problem when using latent diffusion models instead of pixel-based diffusion models. Our combined method, called P2L, outperforms both image- and latent-diffusion model-based inverse problem solvers on a variety of tasks, such as super-resolution, deblurring, and inpainting.

# Summary. An optional shortened abstract.
summary: By generalizing DIP, we can design an adaptation algorithm that corrects the PF-ODE trajectory of posterior sampling with diffusion models, such that one can reconstruct from OOD measurements.

tags: [Diffusion model, Deep Image Prior, OOD Adaptation]

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://arxiv.org/abs/2407.10641'
url_code: 'https://github.com/HJ-harry/DDIP3D'
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