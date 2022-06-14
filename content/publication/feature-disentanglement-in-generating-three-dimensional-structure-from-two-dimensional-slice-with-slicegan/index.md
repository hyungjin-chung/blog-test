---
title: "Feature Disentanglement in generating three-dimensional structure from two-dimensional slice with sliceGAN"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- admin
- Jong Chul Ye

# Author notes (optional)
author_notes: ""

date: "2020-05-01T00:00:00Z"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: "2021-05-21T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

# Publication name and optional abbreviated publication name.
publication: In Nature Machine Intelligence
publication_short: In Nat. Mach. Int.

abstract: Deep generative models are known to be able to model arbitrary probability distributions. Among these, a recent deep generative model, dubbed sliceGAN, proposed a new way of using the generative adversarial network (GAN) to capture the micro-structural characteristics of a two-dimensional (2D) slice and generate three-dimensional (3D) volumes with similar properties. While 3D micrographs are largely beneficial in simulating diverse material behavior, they are often much harder to obtain than their 2D counterparts. Hence, sliceGAN opens up many interesting directions of research by learning the representative distribution from 2D slices, and transferring the learned knowledge to generate arbitrary 3D volumes. However, one limitation of sliceGAN is that latent space steering is not possible. Hence, we combine sliceGAN with AdaIN to endow the model with the ability to disentangle the features and control the synthesis.

# Summary. An optional shortened abstract.
summary: SliceGAN, stochastic model to synthesize 3D microstructures from 2D images, is endowed with the ability to disentangle features, and continuously control these features via AdaIN.

tags: [Feature disentanglement, AdaIN, SliceGAN]

# Display this page in the Featured widget?
featured: false

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://www.nature.com/articles/s42256-021-00400-4'
url_code: 'https://github.com/HJ-harry/SliceGAN_AdaIN'
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