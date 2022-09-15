---
title: "Deep Learning Fast MRI Using Channel Attention in Magnitude Domain"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- Joonhyung Lee
- Hyunjong Kim
- Hyungjin Chung
- Jong Chul Ye

# Author notes (optional)
author_notes:
- "Equal contribution"
- "Equal contribution"
- "Equal contribution"

date: "2020-03-22T00:00:00Z"
doi: "10.1109/ISBI45749.2020.9098416"

# Schedule page publish date (NOT publication's date).
publishDate: "2021-03-02T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

# Publication name and optional abbreviated publication name.
publication: in 2020 17th International Symposium on Biomedical Imaging (ISBI)
publication_short: IEEE ISBI

abstract: Magnetic resonance imaging (MRI) acquisition is an inherently slow process whose acceleration has been the subject of much investigation. In recent years, the explosive advance of deep learning techniques for computer vision and image reconstruction has led to the investigation of deep neural networks for the reconstruction of MRI with under-sampled k-space. In this work, we propose a new image domain architecture that directly produces a sum-of-squares image from under-sampled multi-coil MRI acquisition. This model, called BarbellNet, is a fully convolutional neural network architecture that utilizes the channel attention mechanism using the residual channel attention block (RCAB). Through extensive experiments with the fastMRI data set, we confirm the efficacy of BarbellNet.

# Summary. An optional shortened abstract.
summary: BarbellNet, which consists of long stack of residual channel attention block(RCAB) was proposed for the reconstruction of fast MRI reconstruction. Reconstruction results through this model was placed 6th in the NeurIPS2020 fastMRI challenge.

tags: [Deep Learning, MRI, Attention]

# Display this page in the Featured widget?
featured: false

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://ieeexplore.ieee.org/document/9098416'
url_code: 'https://github.com/veritas9872/fastMRI-kspace'
url_dataset: ''
url_poster: ''
url_project: ''
url_slides: ''
url_source: ''
url_video: ''

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/pLCdAaMFLTE)'
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