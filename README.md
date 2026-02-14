# Knee X-ray Anatomy Segmentation

Multi-class semantic segmentation of knee anatomical structures from X-ray images using deep learning.

## Overview

This project addresses the problem of multi-class anatomical segmentation
of knee joint structures from X-ray images.

The input is a single-channel knee X-ray image, and the output is a pixel-wise
segmentation map consisting of K anatomical classes and one background class.

## Method / Pipeline

The overall pipeline of the proposed knee X-ray anatomy segmentation framework
is illustrated in the following figure.

![Overall pipeline of knee X-ray anatomy segmentation](assets/pipeline.png)

![OAI data annotation and review workflow](assets/pipeline_oai_segmentation.png)

## Dataset

The dataset consists of knee X-ray images collected from the
Osteoarthritis Initiative (OAI).

Due to licensing restrictions, the dataset is not included in this repository.

## Label Definition

tus
Each pixel is assigned to one of the following classes:

## Label Definition

Each pixel is assigned to one of the following classes:

| ID | Class Name               | Description                 |
|----|--------------------------|-----------------------------|
| 0  | _background_             | Non-anatomical region       |
| 1  | Distal femur             | Distal femur region         |
| 2  | Fibular head             | Fibular head region         |
| 3  | Proximal tibia           | Proximal tibia region       |
| 4  | Intercondylar eminence   | Tibial intercondylar eminence |

## Results

Qualitative results on the test set (example predictions from the trained U-Net):
![results](assets/viz_results.png)