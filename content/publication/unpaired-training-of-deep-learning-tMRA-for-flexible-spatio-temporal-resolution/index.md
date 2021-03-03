---
title: "Unpaired training of deep learning tMRA for flexible spatio-temporal resolution"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- Eunju Cha
- admin
- Eung Yeop Kim
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
publication: in IEEE Transactions on Medical Imaging, 2020
publication_short: IEEE TMI

abstract: Time-resolved MR angiography (tMRA) has been
widely used for dynamic contrast enhanced MRI (DCE-MRI)
due to its highly accelerated acquisition. In tMRA, the periphery
of the k-space data are sparsely sampled so that neighbouring
frames can be merged to construct one temporal frame. However,
this view-sharing scheme fundamentally limits the temporal resolution, and it is not possible to change the view-sharing number to
achieve different spatio-temporal resolution trade-off. Although
many deep learning approaches have been recently proposed for
MR reconstruction from sparse samples, the existing approaches
usually require matched fully sampled k-space reference data
for supervised training, which is not suitable for tMRA. This
is because high spatio-temporal resolution ground-truth images
are not available for tMRA. To address this problem, here
we propose a novel unsupervised deep learning using optimal
transport driven cycle-consistent generative adversarial network
(cycleGAN). In contrast to the conventional cycleGAN with
two pairs of generator and discriminator, the new architecture
requires just a single pair of generator and discriminator, which
makes the training much simpler and improves the performance.
Reconstruction results using in vivo tMRA data set confirm that
the proposed method can immediately generate high quality
reconstruction results at various choices of view-sharing numbers, allowing us to exploit better trade-off between spatial and
temporal resolution in time-resolved MR angiography.


# Summary. An optional shortened abstract.
summary: OT-cycleGAN for the reconstruction of time resolved magnetic resonance angiography (MRA) was proposed. The derived method enables flexible control of sptial and temporal resolution.

tags: [Deep Learning, MRI, Optimal Transport]

# Display this page in the Featured widget?
featured: false

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://arxiv.org/pdf/2003.13096.pdf'
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