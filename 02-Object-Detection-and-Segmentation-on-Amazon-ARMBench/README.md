# Object Detection and Segmentation on Amazon ARMBench

## Overview
This project focuses on object detection and instance segmentation using the Amazon ARMBench dataset. The goal was to compare multiple computer vision models for robotic object understanding in crowded tote/bin environments.

## Problem
In warehouse and robotic automation, models need to detect and segment objects accurately even when objects are cluttered, overlapping, or visually similar. This project evaluates how different detection and segmentation architectures perform on this type of real-world object understanding task.

## Approach
We compared multiple deep learning models for object detection and segmentation:

- Mask R-CNN
- DeepLabV3+
- RetinaNet
- YOLOv8

The models were evaluated using quantitative metrics and qualitative visualizations.

## Dataset
Amazon ARMBench object segmentation dataset.

## Tools and Methods
- Python
- PyTorch
- OpenCV
- pycocotools
- MS-COCO style annotations
- Google Colab Pro with T4 GPU
- mAP, IoU, precision, recall, and F1 score evaluation

## Key Results
- Mask R-CNN with ResNet50 achieved strong bounding box and mask performance.
- DeepLabV3+ achieved high Mean IoU on validation and test splits.
- YOLOv8 showed strong detection performance with high mAP50 scores.

## Key Learning
This project helped compare the trade-offs between two-stage models, one-stage detectors, and segmentation-based pipelines for robotic vision tasks.

## Files
- 'Object Detection and Segmentation on Amazon ARMBench.pdf' — Full project report
