# FoodX-251 Classification and Similarity Retrieval

## Swin-Transformer vs ConvNext (Pytorch Edition)

**Author:** Mario Avolio

## GitHub Repository

[Access the Repository](https://github.com/MarioAvolio/FoodX-251-Classification-ConvNext-vs-SwinTransformer)

## Table of Contents

1. [Introduction](#introduction)
2. [Cleaning Model](#cleaning-model)
3. [Data Augmentation and Noise Maker Model](#data-augmentation-and-noise-maker-model)
4. [Classification](#classification)
5. [Similarity Retrieval](#similarity-retrieval)

## Introduction

### FoodX-251: A Dataset for Fine-grained Food Classification

- **FoodX-251 Dataset Overview**
- **Choice of Pytorch Framework**
- **Methodology Pipeline**
- **Data Analysis and Challenges**

#### FoodX-251 Dataset

- The FoodX-251 dataset comprises 251 fine-grained food categories with a collection of 158,000 images sourced from the web.
- It features a training set of 118,000 images and a validation and testing set of 40,000 images (12,000 for validation and 28,000 for testing).
- This dataset served as the foundation for the iFood-2019 challenge within the Fine-Grained Visual Categorization workshop (FGVC6 at CVPR 2019).

#### Noise in FoodX-251

- The abundance of freely available web data comes with inherent noise.
- Images collected from search engines may encompass processed and packaged food items as well as raw ingredients.
- The dataset might also include images featuring multiple food items assigned to a single category (cross-category noise).
- Additionally, it may contain images unrelated to any specific class.

### The Choice of Pytorch

The decision to employ PyTorch as our machine learning framework was driven by a desire to enhance our skill set. PyTorch is a versatile framework rooted in the Torch library, well-suited for applications ranging from computer vision to natural language processing. It boasts a user-friendly, open-source architecture licensed under the modified BSD license, offering flexibility, rapid training, and robust debugging capabilities.

## Cleaning Model

### InceptionV3 Based Model

- We employed an InceptionV3-based model for image and text fusion in the context of UPMC Food-101, utilizing BERT and CNNs.
- Customizations to the classification layer facilitated binary classification.
- Transfer Learning was harnessed via weights provided by the official paper.
- This phase entailed challenges encountered during both training and testing with the Food5k Dataset.

### Enhancing Model Performance

- Strategies for model performance enhancement were devised, including data integration and the balancing of imbalanced data via undersampling.
- The outcome yielded an impressive F1-Score of 0.97.

## Data Augmentation and Noise Maker Model

### Noise Maker Neural Network

- The implementation of an Encoder-Decoder Neural Network was pivotal for generating degraded images.
- Pertinent challenges and parameterization details are documented.
- Data augmentation techniques, facilitated by the Imgaug library, played a significant role in the process.

## Classification

- In this section, we delve into the specifics of our training and validation sets.
- A comparative analysis between Swin Transformer and ConvNeXt Tiny models is presented in the context of image classification.
- Details regarding model training, accompanied by relevant metrics, are outlined.
- Obstacles encountered during the training process are discussed.

## Similarity Retrieval

- We explore the utilization of Swin Transformer features for similarity retrieval.
- The K-Nearest Neighbors (KNN) algorithm is employed.
- Evaluation metrics, alongside results for both degraded and standard datasets, are provided.

## Final Conclusions

- A concise summary of key findings and insights.
- Recommendations for prospective research directions.

