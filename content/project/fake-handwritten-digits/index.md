---
title: Fake Handwritten Digits
date: 2021-03-10T13:13:47.650Z
summary: Built a GAN (Generative Adversarial Networks) model that learns from real handwritten digits to generate its own handwritten digits.
draft: false
featured: false
tags:
  - ml
external_link: ""
links:
  - url: https://github.com/pollmix/fake-handwritten-digits
    name: Link
    icon_pack: fab
    icon: github
image:
  filename: ""
  focal_point: Smart
  preview_only: false
---

In this project, we will train a model that will eventually learn to write handwritten digits.

INPUT: we will use torchvision dataset that is built-in in PyTorch
![input](https://i.ibb.co/2Sd6RSk/input.png "input")

OUTPUT: generated data
![output](https://i.ibb.co/qxVFwmx/Output.png "output")

### Tools Used

- Python
- PyTorch
- Torchvision
- Matplotlib

### Concepts covered

- GAN (Generative Adversarial Networks)
- Generator
- Discriminator
- Leaky ReLU Activation Function

### Details

We used PyTorch built-in torchvision module as a data source which called MNIST handwritten digit. We implemented a GAN (Generative Adversarial Networks) model that implemented the Leaky ReLU activation function. We trained the Discriminator and Generator Neural Networks. The purpose of the Generator is to create fake images and the Discriminator to identify between the fake and real images. They worked together to finally generate some very realistic fake images which are hard to differentiate.
