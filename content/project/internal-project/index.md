---
title: Trustworthy Machine Learning Research Project
summary: Establishment of Neural Networks Robust to Label Noise
tags:
- Deep Learning
date: "2023-04-01T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: "https://arxiv.org/abs/2211.15279"

image:
  caption: Photo by Pengwei Yang
  focal_point: Smart

links:
- icon: twitter
  icon_pack: fab
  name: Follow
  url: https://twitter.com/pengwei_yang_
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

Label noise is a significant obstacle in deep learning model training. It can have a considerable impact on the performance of image classification models, particularly deep neural networks, which are especially susceptible because they have a strong propensity to memorise noisy labels. In this project, we have examined the fundamental concept underlying related label noise approaches. A transition matrix estimator has been created, and its effectiveness against the actual transition matrix has been demonstrated. In addition, we examined the label noise robustness of two convolutional neural network classifiers with LeNet and AlexNet designs. The two FashionMINIST datasets have revealed the robustness of both models. We are not efficiently able to demonstrate the influence of the transition matrix noise correction on robustness enhancements due to our inability to correctly tune the complex convolutional neural network model due to time and computing resource constraints. There is a need for additional effort to fine-tune the neural network model and explore the precision of the estimated transition model in future research.
