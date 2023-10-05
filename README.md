# FoodX-251 Classification and Similarity Retrieval

## Swin-Transformer vs ConvNext (Pytorch Edition)

**Author:** Mario Avolio

## GitHub Repository

[Repository Link](https://github.com/MarioAvolio/FoodX-251-Classification-ConvNext-vs-SwinTransformer)

## Table of Contents

01. [Introduction](#introduction)
02. [Cleaning Model](#cleaning-model)
03. [Data Augmentation and Noise Maker Model](#data-augmentation-and-noise-maker-model)
04. [Classification](#classification)
05. [Similarity Retrieval](#similarity-retrieval)

## Introduction

### FoodX-251: A Dataset for Fine-grained Food Classification

- **Dataset FoodX-251 Info**
- **Why Pytorch?**
- **Pipeline**
- **Analysis and Problems of Data**

#### FoodX-251

- A dataset of 251 fine-grained food categories with 158k images collected from the web.
- 118k images as a training set and 40k images that can be used for validation and testing (12k validation and 28k test images).
- The FoodX251 dataset has been used for organizing iFood-2019 challenge in the Fine-Grained Visual Categorization workshop (FGVC6 at CVPR 2019).

#### FoodX-251 Noise

- Web data is freely available in abundance but contains different types of noise.
- Web images collected via search engines may include images of processed and packaged food items as well as ingredients required to prepare the food items.
- The web results may also include images not belonging to any particular class.

### Why Pytorch?

Because I want to increase my skills. PyTorch is a machine learning framework based on the Torch library, used for applications such as computer vision and natural language processing.

## Cleaning Model

### InceptionV3 Based Model

- InceptionV3 Model for image and text fusion for UPMC Food-101 using BERT and CNNs.
- Modifications to the classification layer to make binary classification.
- Transfer Learning through the weights provided by the official paper.
- Problems faced during training and testing using the Food5k Dataset.

### Model - Improving Performance

- Strategies to improve model performance using new data and data integration.
- Balancing data with undersampling.
- Achieving F1-Score of 0.97.

## Data Augmentation and Noise Maker Model

### Noise Maker Neural Network

- Encoder-Decoder Neural Network used for generating degraded images.
- Challenges and parameters used.
- Data augmentation techniques applied using the Imgaug library.

## Classification

- Training and validation set details.
- Swin Transformer vs. ConvNeXt Tiny models for image classification.
- Model training details and metrics.
- Challenges faced during training.

## Similarity Retrieval

- Utilizing Swin Transformer features for similarity retrieval.
- K-Nearest Neighbors (KNN) algorithm used.
- Evaluation metrics and results for both degraded and standard datasets.

## Final Conclusions

- Summary of key findings and outcomes.
- Suggestions for future research.

