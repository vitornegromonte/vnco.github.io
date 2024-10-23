---
title: "Convolutional Neural Networks in Breast Cancer Diagnosis - A Comparative Study with CBIS-DDSM Data"
date: 2023-11-27
lastmod: 2024-01-06
aliases:
    - /projects/project3/keynote.pdf
tags: ["Python", "TensorFlow", "Keras", "Computer Vision", "Healthcare"]
author: ["Vitor Negromonte", "Eduardo Medeiros"]
description: "Cancer diagnosis using AI Methods."
summary: "The goal of this project is to compare CNN models to improve early breast cancer detection using mammography images."
cover:
    image: "project3.png"
    alt: "Convolutional Neural Networks in Breast Cancer Diagnosis"
---

----

##### Introduction

The objective of this project is to undertake a thorough comparative analysis of CNN models with the aim of enhancing early detection capabilities for breast cancer through the utilization of mammography images. 

----
##### Dataset

The dataset used was available on [Kaggle](https://www.kaggle.com/datasets/skooch/ddsm-mammography) and was based in the [CBIS-DDSM dataset](http://www.eng.usf.edu/cvprg/Mammography/Database.html) from the University of South Florida (in colaboration with Washington University, Wake Forest University and Sandia National Laboratories).

The dataset consists of negative images from the DDSM dataset and positive images from the CBIS-DDSM dataset. The data was pre-processed to convert it into 299x299 images.

The negative (DDSM) images were tiled into 598x598 tiles, which were then resized to 299x299.

The positive (CBIS-DDSM) images had their ROIs extracted using the masks with a small amount of padding to provide context. Each ROI was then randomly cropped three times into 598x598 images, with random flips and rotations, and then the images were resized down to 299x299.

##### Our approach

The objective of this project is to undertake a thorough comparative analysis of various CNN models with the aim of enhancing early detection capabilities for breast cancer through the utilization of mammography images.

- Models:

    - VGG;
    - GoogLeNet;
    - ResNet;
    - DenseNet;

The code was developed using Jupyter Notebooks (Google Colab) and the Python language, incorporating essential libraries such as PyTorch, Plotly, Pandas, SciKit Learn, and Numpy. We used Nvidia GPUs during the training, specifically the Nvidia A100 80GB. We didn't exported the models best weights and also didn't made hyperparameters fine-tune.

##### Results

    Hyperparameters:
    - Optimizer: ADAM
    - lr: 0.001
    - Loss: Binary cross-entropy
    - Epochs: 5
---

    Model       | Acc     | F1-Score     | Training time (minutes)
    VGG16       | 0.9563  | 67           | 22
    DenseNet121 | 0.9569  | 67           | 24
    ResNet50    | 0.96    | 70           | 22.4

##### Details
+ [Keynote](keynote.pdf)
+ [Code and data](https://github.com/vitornegromonte/breast_cancer-classification)