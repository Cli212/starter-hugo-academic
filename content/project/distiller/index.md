---
title: Distiller:A Systematic Study of Model Distillation Methods in Natural Language Processing
tags:
- Natural Language Processing
- Deep Learning
date: "2021-08-6T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: Photo by rawpixel on Unsplash
  focal_point: Smart

links:
- icon: twitter
  icon_pack: fab
  name: Follow
  url: https://twitter.com/HaoyuHe212
url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: example
---

Knowledge Distillation (KD) offers a natural way to reduce the latency and memory/energy usage of massive pretrained models that have come to dominate Natural Language Processing (NLP) in recent years. While numerous sophisticated variants of KD algorithms have been proposed for NLP applications, the key factors underpinning the optimal distillation performance are often confounded and remain unclear. We aim to identify how different components in the KD pipeline affect the resulting performance and how much the optimal KD pipeline varies across different datasets/tasks, such as the data augmentation policy, the loss function, and the intermediate representation for transferring the knowledge between teacher and student. To tease apart their effects, we propose Distiller, a meta KD framework that systematically combines a broad range of techniques across different stages of the KD pipeline, which enables us to quantify each component's contribution. Within Distiller, we unify commonly used objectives for distillation of intermediate representations under a universal mutual information (MI) objective and propose a class of MI-\alpha objective functions with better bias/variance trade-off for estimating the MI between the teacher and the student. On a diverse set of NLP datasets, the best Distiller configurations are identified via large-scale hyperparameter optimization. Our experiments reveal the following:1) the approach used to distill the intermediate representations is the most important factor in KD performance, 2) among different objectives for intermediate distillation, MI-\alpha performs the best, and 3) data augmentation provides a large boost for small training datasets or small student networks. Moreover, we find that different datasets/tasks prefer different KD algorithms, and thus propose a simple AutoDistiller algorithm that can recommend a good KD pipeline for a new dataset.
