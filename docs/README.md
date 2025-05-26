---
layout: home
permalink: index.html

# Please update this with your repository name and title
repository-name: e20-co543-Super-Resolution-For-Image-Enhancement
title: Super Resolution For Image Enhancement
---

[comment]: # "This is the standard layout for the project, but you can clean this and use your own template"

# Resolution For Image Enhancement

---

<!-- 
This is a sample image, to show how to add images to your page. To learn more options, please refer [this](https://projects.ce.pdn.ac.lk/docs/faq/how-to-add-an-image/)

![Sample Image](./images/sample.png)
 -->

## Team
-  E/20/271, Nirmani K.G.H, [email](mailto:e200271@eng.pdn.ac.lk)
-  E/20/093, Edirisooriya D.M.B, [email](mailto:e20093@eng.pdn.ac.lk)
-  E/20/244, Malshan P.G.P, [email](mailto:e200244@eng.pdn.ac.lk)
-  E/20/367, Senavirathna D. B. C. M., [email](mailto:e20367@eng.pdn.ac.lk)


## Table of Contents
1. [Introduction](#introduction)
2. [Problem & Motivation](#problem)
3. [Solution Overview](#solution)
4. [Links](#links)

---

## Introduction
Image Super-Resolution (SR) enhances the resolution of low-quality images by reconstructing high-resolution (HR) versions. This technique is crucial in fields like medical imaging, surveillance, and satellite analysis. This project explores deep learning approaches—specifically Convolutional Neural Networks (CNNs)—to improve SR performance. We compare two strategies:

  1.Mean Squared Error (MSE): Focused on pixel-level accuracy.
  
  2.Perceptual Loss: Uses a pre-trained VGG19 network to preserve high-level features and texture details.
  
By optimizing hyperparameters and evaluating both pixel fidelity and perceptual quality, we demonstrate how CNNs can effectively generate detailed HR images.

## Problem & Motivation
Traditional SR methods, such as bicubic interpolation, often result in blurry images and fail to preserve structural detail. Major challenges include High computational demands for HR image processing, Loss of texture and fine details and Difficulty in identifying optimal training duration. These limitations are significant in domains requiring precise visual information, such as diagnostics in healthcare, land-use interpretation in satellite imagery, and accurate identification in surveillance footage. Our goal is to balance pixel-level precision with perceptual realism using deep learning.

## Solution Overview
We implemented a CNN-based SR model with residual blocks and upsampling layers, trained on paired LR-HR image datasets.
we prepared the dataset by generating low-resolution (LR) images through 3x downsampling of high-resolution (HR) inputs and applied data augmentation techniques such as flipping, rotation, and brightness adjustments to improve model generalization. The CNN architecture consisted of five residual blocks with skip connections to address the vanishing gradient problem, followed by transposed convolution layers for upsampling and resolution enhancement. Two loss functions were employed: Mean Squared Error (MSE), which optimizes pixel-level accuracy, and Perceptual Loss, which combines MSE with feature-based loss using a pre-trained VGG19 network to better preserve textures and high-level details. Experimental comparisons were conducted by training MSE-based models for 20 and 30 epochs, and by evaluating models trained with MSE versus Perceptual Loss for 10 epochs each to assess the trade-off between pixel accuracy and perceptual quality.


## Links

- [Project Repository](https://github.com/cepdnaclk/{{ page.repository-name }}){:target="_blank"}
- [Project Page](https://cepdnaclk.github.io/{{ page.repository-name}}){:target="_blank"}
- [Department of Computer Engineering](http://www.ce.pdn.ac.lk/)
- [University of Peradeniya](https://eng.pdn.ac.lk/)


[//]: # (Please refer this to learn more about Markdown syntax)
[//]: # (https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
