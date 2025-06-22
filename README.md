# Autonomous Vehicle Object Detection using YOLOv8, YOLOv11, and YOLOv12

This project explores object detection models for autonomous driving by evaluating and comparing YOLOv8, YOLOv11, and YOLOv12 on the KITTI dataset. The goal is to accurately detect road objects like cars, pedestrians, cyclists, and other traffic elements in real-time conditions.

## Project Overview

- Dataset: KITTI (7-class object detection version)
- Models Used: YOLOv8, YOLOv11, YOLOv12 , MobileVIT+YOLO
- Backbones: Standard YOLO + transformer hybrids (e.g., MobileViT, SwinViT)
- Task: Real-time object detection for autonomous vehicles
- Evaluation Metric: mAP (Mean Average Precision), Precision, Recall, FPS

## Tech Stack

- Python, PyTorch
- YOLOv8/YOLOv11/YOLOv12 (Ultralytics and custom)
- Google Colab Pro (for training on GPU)
- KITTI dataset (converted to COCO format)
- TensorBoard for logging
- OpenCV for visualization

## Results Summary

| Model   | mAP@0.5 | Inference Speed | Notes                      |
|---------|---------|------------------|----------------------------|
| YOLOv8  | 87.3%   | Fast             | Lightweight baseline       |
| YOLOv11 | 89.8%   | Moderate         | Enhanced transformer-based |
| YOLOv12 | 91.4%   | Fast             | Custom hybrid (ViT + YOLO) |

## Folder Structure

├── data/ # KITTI dataset (in YOLO/COCO format)
├── models/ # YOLOv11 and YOLOv12 custom configs
├── notebooks/ # Training and evaluation notebooks
├── weights/ # Best model checkpoints
├── results/ # Inference images and videos
└── utils/ # Helper scripts


## Key Learnings

- Compared performance of YOLO variants on real-world driving data
- Addressed challenges in small object detection and occlusions
- Improved mAP through data augmentation and anchor tuning

## References
- KITTI Dataset: http://www.cvlibs.net/datasets/kitti/
