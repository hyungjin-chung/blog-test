---
title: "Unpaired deep learning for accelerated MRI using optimal transport driven cycleGAN"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- Gyutaek Oh
- Byeongsu Sim
- admin
- Leonard Sunwoo
- Jong Chul Ye

# Author notes (optional)
author_notes:
- ""

date: "2020-08-21T00:00:00Z"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: "2021-03-02T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

# Publication name and optional abbreviated publication name.
publication: in IEEE Transactions on Computational Imaging, 2020
publication_short: IEEE TCI

abstract: Recently, deep learning approaches for accelerated
MRI have been extensively studied thanks to their high performance reconstruction in spite of significantly reduced runtime complexity. These neural networks are usually trained
in a supervised manner, so matched pairs of subsampled and
fully sampled k-space data are required. Unfortunately, it is
often difficult to acquire matched fully sampled k-space data,
since the acquisition of fully sampled k-space data requires
long scan time and often leads to the change of the acquisition
protocol. Therefore, unpaired deep learning without matched
label data has become a very important research topic. In this
paper, we propose an unpaired deep learning approach using a
optimal transport driven cycle-consistent generative adversarial
network (OT-cycleGAN) that employs a single pair of generator
and discriminator. The proposed OT-cycleGAN architecture is
rigorously derived from a dual formulation of the optimal
transport formulation using a specially designed penalized least
squares cost. The experimental results show that our method
can reconstruct high resolution MR images from accelerated kspace data from both single and multiple coil acquisition, without
requiring matched reference data.

# Summary. An optional shortened abstract.
summary: A novel unpaired learning scheme for accelerated MRI, OT-cycleGAN was extensively applied and was found effective for the reconstruction of multi-coil static MRI.

tags: [Deep Learning, MRI, Optimal Transport]

# Display this page in the Featured widget?
featured: false

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://arxiv.org/pdf/2008.12967.pdf'
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