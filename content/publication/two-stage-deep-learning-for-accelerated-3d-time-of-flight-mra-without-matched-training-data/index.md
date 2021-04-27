---
title: "Two-Stage Deep Learning for Accelerated 3D Time-of-Flight MRA without Matched Training Data"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- admin
- Eunju Cha
- Leonard Sunwoo
- Jong Chul Ye

# Author notes (optional)
author_notes:
- ""

date: "2020-04-05T00:00:00Z"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: "2021-04-27T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

# Publication name and optional abbreviated publication name.
publication: In Medical Image Analysis
publication_short: In Medical Image Analysis

abstract: Time-of-flight magnetic resonance angiography (TOF-MRA) is one of the most widely used non-contrast MR imaging methods to visualize blood vessels, but due to the 3-D volume acquisition highly accelerated acquisition is necessary. Accordingly, high quality reconstruction from undersampled TOF-MRA is an important research topic for deep learning. However, most existing deep learning works require matched reference data for supervised training, which are often difficult to obtain. By extending the recent theoretical understanding of cycleGAN from the optimal transport theory, here we propose a novel two-stage unsupervised deep learning approach, which is composed of the multi-coil reconstruction network along the coronal plane followed by a multi-planar refinement network along the axial plane. Specifically, the first network is trained in the square-root of sum of squares (SSoS) domain to achieve high quality parallel image reconstruction, whereas the second refinement network is designed to efficiently learn the characteristics of highly-activated blood flow using double-headed max-pool discriminator. Extensive experiments demonstrate that the proposed learning process without matched reference exceeds performance of state-of-the-art compressed sensing (CS)-based method and provides comparable or even better results than supervised learning approaches.

# Summary. An optional shortened abstract.
summary: Two-stage unsupervised reconstruction method for 3D TOF-MRA is developed. A novel projection discriminator in the axial reconstruction step drastically enhances the vessel visiblity.

tags: [Deep Learning, MRI, Optimal Transport, Projection Discriminator]

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://www.sciencedirect.com/science/article/pii/S1361841521000931?casa_token=d_SKOLkevjUAAAAA:FgTZe8yJEgAvA-A-WAPNU8J9rdF21wR5SKL81aQHIeQuidIQLARs7d29E_N2sK9GvJ6hk2LtAw'
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