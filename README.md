# Masked Autoencoders (MAE) Mini-ImageNet

## Overview

This project implements **Masked Autoencoders (MAE)** in PyTorch, based on the CVPR 2022 paper [Masked Autoencoders Are Scalable Vision Learners](https://arxiv.org/abs/2111.06377).

The objective is to explore **self-supervised visual representation learning** using a Vision Transformer (ViT).

MAE learns visual representations by randomly masking a large portion of an input image and training the model to reconstruct the missing image patches from the remaining visible patches.

This project focuses on understanding and implementing the MAE architecture, including its masking strategy, Vision Transformer encoder, lightweight decoder, and image reconstruction objective.

## Dataset

The project uses **Mini-ImageNet**, a subset of ImageNet commonly used in computer vision research.

Images are resized and processed at a resolution of **224 × 224 pixels**. During MAE pretraining, **75% of image patches are randomly masked**, leaving the remaining 25% visible to the encoder.

**Dataset reference and download instructions:** [Mini-ImageNet — Kaggle](https://www.kaggle.com/datasets/ctrnngtrung/miniimagenet)

The dataset is stored locally and is not included in this repository.