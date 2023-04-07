---
title: 可信机器学习研究项目
summary: 建立对标签噪声具有鲁棒性的神经网络
tags:
- Deep Learning
date: "2023-04-01T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: Photo by Pengwei Yang
  focal_point: Smart

---

标签噪声对深度学习模型训练来说是一个重要的难题。这种噪声可能会对图像分类模型的性能产生很大的影响，特别是对于深度神经网络，因为它们很容易记住噪声标签。在这个项目中，我们探讨了与标签噪声相关的基本原理。我们创建了一个转移矩阵估计器，并证实了它在与实际转移矩阵的比较中表现出的有效性。同时，我们还研究了两个采用LeNet和AlexNet设计的卷积神经网络分类器在面对标签噪声时的鲁棒性。通过两个FashionMINIST数据集的分析，我们发现这两个模型都具有很好的鲁棒性。然而，由于时间和计算资源的限制，我们无法正确调整复杂的卷积神经网络模型，因此不能有效地展示转移矩阵噪声校正对鲁棒性增强的贡献。在未来的研究中，我们需要付出更多努力来优化神经网络模型，并深入探讨估计的转移模型的准确性。
