# Investigating U-Net Pretraining with SimCLR for Image Segmentation

### Introduction
This paper explores the implementation of the U-Net architecture on self-supervised learning (SSL) for image segmentation on the Oxford-IIIT Pet dataset.

As of 2024, image segmentation is becoming increasingly popular in computer vision applications. The U-Net architecture has gained significant interest, due to its unique encoder-decoder structure, enabling it to effectively use both local and global information. Typically, supervised training of U-Net models requires large amount of labelled data, which can be expensive to obtain. We turn towards self-supervised learning as a promising alternative, which allows models to learn meaningful representations from unlabelled data via defined pretraining tasks.

In this paper, we focus on evaluating the Simplied Contrastive Framework for Contrasting Learning (SimCLR) for pretraining U-Net architectures. SimCLR maximises agreement between differently augmented views of an image, offering robust visual representations. We chose SimCLR over other methods like BYOL or DINO due to its proven performance and compatibility with U-Nets.

We compare SimCLR with Masked image Modeling (MIM) using Masked Autoencoders (MAEs). MIM predicts masked image regions to capture fine-grained contextual information. While SimMIM applies MIM to vision transformers (ViTs), we extend this to U-Nets. We experiment with various masking techniques like random square patches and pixels.

We conclude with an open-ended investigation into architectural variations and training strategies of SimCLR, including skip connections, freezing encoder weights, and fine-tuning dataset size. Through these analyses, we aim to optimise SimCLR-based pretraining for U-Nets.

Our study aims to provide insights into SimCLR's effectiveness within U-Net architectures for image segmentation tasks, contributing to understanding self-supervised learning frameworks for such tasks.

### Report

View the full report [here](https://github.com/jain-hl/u-net-simclr-image-segmentation/blob/main/Investigating%20U-Net%20Pretraining%20with%20SimCLR%20for%20Image%20Segmentation.pdf)
