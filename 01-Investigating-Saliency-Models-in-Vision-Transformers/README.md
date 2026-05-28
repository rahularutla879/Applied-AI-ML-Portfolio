# Investigating the Efficiency-Enforcing Role of Biologically-Inspired Bottom-Up Saliency Models in Vision Transformers

## Overview
This project investigates whether biologically-inspired bottom-up saliency can improve the efficiency and behavior of Vision Transformers. The main idea is to guide the model toward visually important image regions instead of treating all image patches equally.

## Problem
Vision Transformers process images as sequences of patch tokens. In early layers, they often treat all tokens uniformly, which can be inefficient because not all image regions are equally informative. This project explores whether an external saliency signal can act as an inductive bias for better representation learning.

## Approach
The project uses ImgSig, a deterministic frequency-domain saliency method, to generate saliency maps from input images. These saliency maps are converted into patch-level token signals and integrated into Vision Transformers using multiple strategies:

- External saliency gating
- Adaptive input-level blending
- Feature-level injection
- Attention-level modulation

## Dataset
Experiments were conducted on CIFAR-100 for image classification.

## Key Result
Adaptive input-level blending achieved the best reported accuracy of approximately 91.44%, showing that saliency is most useful when the model can learn how much to trust it.

## Tools and Methods
- Python
- PyTorch
- Vision Transformers
- ImgSig saliency model
- CIFAR-100
- Attention modulation
- Feature injection
- Model evaluation using classification accuracy

## Key Learning
The project showed that bottom-up saliency is most effective in early transformer layers, where representations are still closely related to low-level visual structures like edges, textures, and contrast.

## Files
- `Investigating_the_Efficiency_Enforcing_Role_of_Biologically_Inspired_Bottom_Up_Saliency_Models_in_Vision_Transformers.pdf` — Full project report
