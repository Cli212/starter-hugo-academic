---
title: BERNICE and SAM, Metrics for Automatic Text Simplification
summary: Language model-powered metrics for automatic text simplification (ATS).
tags:
- Natural Language Processing
- Deep Learning
date: "2021-08-18T00:00:00Z"

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
url_code: http://afba-34-221-99-194.ngrok.io/
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

Automatic text simplification (ATS) transforms text such that it becomes easier to read, comprehend, and process. In lexical simplification simpler synonyms are substituted for complicated words, and in syntactic simplification, complex sentences are split into simpler sentences while preserving meaning. ATS is typically a mixture of both. 

While ATS has taken great strides in recent years, simplified text does not always preserve the cohesiveness and meaning of the original text. We propose the first metrics to directly measure the preservation of sentence-to-sentence cohesion and meaning during automatic simplification. Our metrics use state-of-the-art transformer technology. BERNICE (BERt Nsp Inference for Cohesion Evaluation) compares sentence-to-sentence cohesion between source and simplified text. SAM (Sentence-level question-Answering as Meaning-preservation metric) measures meaning preservation by comparing simulated reading comprehension on original and simplified text. 

We have coded and integrated both metrics with the Easier Automatic Sentence Simplification Evaluation (EASSE) package for convenience. We additionally provide a web app to visualize BERNICE and SAM results. We believe direct measurements of cohesion and meaning preservation will empower researchers to develop improved ATS systems. 
