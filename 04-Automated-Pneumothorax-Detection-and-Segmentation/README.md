# Automated Pneumothorax Detection and Segmentation from Chest X-rays Using Multi-task Learning

## Overview
This project focuses on automated pneumothorax detection and segmentation from chest X-ray images using deep learning. The goal was to build a model that can both detect whether pneumothorax is present and segment the affected lung region.

## Problem
Pneumothorax is a serious medical condition where air collects in the pleural cavity and can cause lung collapse. Chest X-rays are commonly used for diagnosis, but interpretation can be difficult due to subtle visual patterns, human error, and variation between cases.

## Approach
We built a multi-task learning framework that performs both:

- Binary classification for pneumothorax detection
- Image segmentation for localizing the pneumothorax region

The model uses an EfficientNet-based encoder with a U-Net-style decoder. Intermediate encoder and decoder features are also used for the classification branch.

## Dataset
The project used the SIIM-ACR Pneumothorax Segmentation dataset, which contains chest X-ray images with segmentation masks and binary pneumothorax labels.

## Tools and Methods
- Python
- PyTorch
- EfficientNet
- U-Net
- Multi-task learning
- Binary cross-entropy loss
- Jaccard loss / IoU loss
- Chest X-ray preprocessing
- Data augmentation
- Segmentation and classification evaluation

## Key Results
The model was evaluated using segmentation metrics such as IoU and Dice score, along with classification metrics such as accuracy, precision, recall, and F1-score.

## Key Learning
This project showed how multi-task learning can combine classification and segmentation in a single medical imaging pipeline. It also helped demonstrate how segmentation outputs can support more interpretable clinical AI predictions.

## Files
- `Pneumothorax Detection and Segmentation.pdf` — Full project report
