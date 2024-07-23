---
title: Paper accepted to ECCV 2024

event: 
event_url: https://arxiv.org/abs/2407.10641

# location: Wowchemy HQ
# address:
#   street: 450 Serra Mall
#   city: Stanford
#   region: CA
#   postcode: '94305'
#   country: United States

summary: Deep Diffusion Image Prior (DDIP), a generalized use of deep image prior (DIP) in diffusion sampling, which enables efficient 3D OOD reconstruction, is accepted to ECCV 2024.
abstract: Recent inverse problem solvers that leverage generative diffusion priors have garnered significant attention due to their exceptional quality. However, adaptation of the prior is necessary when there exists a discrepancy between the training and testing distributions. In this work, we propose deep diffusion image prior (DDIP), which generalizes the recent adaptation method of SCD by introducing a formal connection to the deep image prior. Under this framework, we propose an efficient adaptation method dubbed D3IP, specified for 3D measurements, which accelerates DDIP by orders of magnitude while achieving superior performance. D3IP enables seamless integration of 3D inverse solvers and thus leads to coherent 3D reconstruction. Moreover, we show that meta-learning techniques can also be applied to yield even better performance. We show that our method is capable of solving diverse 3D reconstructive tasks from the generative prior trained only with phantom images that are vastly different from the training set, opening up new opportunities of applying diffusion inverse solvers even when training with gold standard data is impossible.

# Talk start and end times.
#   End time can optionally be hidden by prefixing the line with `#`.
# date: "2030-06-01T13:00:00Z"
# date_end: "2030-06-01T15:00:00Z"
# all_day: false

# Schedule page publish date (NOT talk date).
publishDate: "2024-07-15T00:00:00Z"

authors: [admin, Jong Chul Ye]
tags: []

# Is this a featured talk? (true/false)
featured: true

image:
  caption: 'DDIP'
  focal_point: Right

# links:
# - icon: twitter
#   icon_pack: fab
#   name: Follow
#   url: https://twitter.com/georgecushen
# url_code: ""
# url_pdf: ""
# url_slides: ""
# url_video: ""

# Markdown Slides (optional).
#   Associate this talk with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
# slides: example

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects:
- internal-project
---

<!-- {{% callout note %}}
Click on the **Slides** button above to view the built-in slides feature.
{{% /callout %}}

Slides can be added in a few ways:

- **Create** slides using Wowchemy's [*Slides*](https://wowchemy.com/docs/managing-content/#create-slides) feature and link using `slides` parameter in the front matter of the talk file
- **Upload** an existing slide deck to `static/` and link using `url_slides` parameter in the front matter of the talk file
- **Embed** your slides (e.g. Google Slides) or presentation video on this page using [shortcodes](https://wowchemy.com/docs/writing-markdown-latex/).

Further event details, including [page elements](https://wowchemy.com/docs/writing-markdown-latex/) such as image galleries, can be added to the body of this page. -->
