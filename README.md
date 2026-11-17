# CLIPTraVeLGAN – Monet Style Transfer

An implementation of **CLIPTraVeLGAN** for transforming real-world photographs into images inspired by Claude Monet's impressionist painting style.

## Overview

This project explores image-to-image translation using Generative Adversarial Networks (GANs) and CLIP-based visual representations.

The goal is to learn the visual characteristics of Monet's paintings and apply those characteristics to ordinary photographs while preserving the original scene's semantic content.

The implementation is based on the research paper [CLIPTraVeLGAN for Semantically Robust Unpaired Image Translation](https://floc-conference.org/publications/preprint/kvnf).

## How It Works

CLIPTraVeLGAN combines adversarial image translation with semantic guidance from a pretrained CLIP model.

The approach builds on TraVeLGAN by replacing its Siamese network with a pretrained, frozen CLIP model. This allows the model to leverage visual and semantic representations learned from large-scale image-text training.

The main components include:

- **Generator:** Learns to transform photographs into Monet-inspired images.
- **Discriminator:** Distinguishes generated Monet-style images from real Monet paintings.
- **CLIP:** Provides pretrained visual representations to guide semantic consistency.
- **Adversarial training:** Encourages generated images to resemble the target artistic style while retaining meaningful image content.

## Dataset

The project is associated with Kaggle's *I'm Something of a Painter Myself* competition.

The dataset contains two unpaired image collections:

| Dataset | Description |
|---|---|
| Monet paintings | Artwork by Claude Monet |
| Photographs | Real-world photographs to be transformed |

The original competition dataset provides 300 Monet paintings and 7,028 photographs in JPEG format, with corresponding TFRecord versions.

Dataset: [Kaggle – I'm Something of a Painter Myself](https://www.kaggle.com/competitions/gan-getting-started/data)

## Implementation

The project is implemented in Python using the Kaggle notebook environment.

The notebook explores the CLIPTraVeLGAN approach for unpaired image-to-image translation, using pretrained visual representations to guide the transformation process.

## Technologies

- Python
- Deep Learning
- Generative Adversarial Networks (GANs)
- CLIP (Contrastive Language–Image Pretraining)
- Computer Vision
- Image-to-Image Translation
- Kaggle Notebooks

## Run the Project

The complete implementation is available on Kaggle:

**[Open CLIPTraVeLGAN – Monet Article Implementation](https://www.kaggle.com/code/unfriendlyai/cliptravelgan-monet-article-implementation/notebook)**

To explore the project:

1. Open the Kaggle notebook.
2. Sign in to your Kaggle account.
3. Select **Copy & Edit** to create your own notebook.
4. Configure the required dataset and runtime.
5. Execute the notebook cells to explore the implementation.

## Research Reference

Bodyanskiy, Y., Ryabova, N., & Lavrynenko, R. (2023).

*CLIPTraVeLGAN for Semantically Robust Unpaired Image Translation.*

[Read the Research Paper](https://floc-conference.org/publications/preprint/kvnf)

## Project Objective

This project explores how pretrained vision-language representations can improve generative image translation by combining semantic understanding with adversarial learning.
