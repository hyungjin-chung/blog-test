---
title: 2 papers accepted to ICLR 2025

event: 2 papers accepted to ICLR 2025
event_url: 

# location: Wowchemy HQ
# address:
#   street: 450 Serra Mall
#   city: Stanford
#   region: CA
#   postcode: '94305'
#   country: United States

summary: CFG++ and TReg are accepted to ICLR 2025.
abstract: Classifier-free guidance (CFG) is a fundamental tool in modern diffusion models for text-guided generation. Although effective, CFG has notable drawbacks. For instance, DDIM with CFG lacks invertibility, complicating image editing; furthermore, high guidance scales, essential for high-quality outputs, frequently result in issues like mode collapse. This paper reveals that the problems may stem from the off-manifold phenomenon associated with CFG, rather than the diffusion models themselves.
 More specifically, inspired by the recent advancements of diffusion model-based inverse problem solvers (DIS),  we reformulate text-guidance as an inverse problem with a text-conditioned score matching loss and
develop CFG++, a novel approach that tackles the off-manifold challenges inherent in traditional CFG. CFG++ features a surprisingly simple fix to CFG, yet it offers significant improvements, including 
better sample quality for text-to-image generation, invertibility, smaller guidance scales, etc. Furthermore, CFG++ enables seamless interpolation between unconditional and conditional sampling at lower guidance scales, consistently outperforming traditional CFG at all scales. 
Moreover, CFG++ can be easily integrated into high-order diffusion solvers and naturally extends to distilled diffusion models.
Experimental results confirm that our method significantly enhances performance in 
text-to-image generation, DDIM inversion, editing, and solving inverse problems, suggesting a wide-ranging impact and potential applications in various fields that utilize text guidance.

# Talk start and end times.
#   End time can optionally be hidden by prefixing the line with `#`.
# date: "2030-06-01T13:00:00Z"
# date_end: "2030-06-01T15:00:00Z"
# all_day: false

# Schedule page publish date (NOT talk date).
publishDate: "2025-01-24T00:00:00Z"

authors: [admin]
tags: []

# Is this a featured talk? (true/false)
featured: false

image:
  caption: 
  focal_point: 

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
