# Vehicle Detection in Road Images Using Deep Learning

This project develops and evaluates a computer vision system for detecting vehicles in roadway images using deep learning. The project uses the KITTI 2D Object Detection dataset and focuses primarily on cars, vans, and trucks.

## Project Objective

The goal is to determine how effectively a YOLO-based object detector can identify vehicles in road scenes and how preprocessing, augmentation, and fine-tuning affect model performance.

## Dataset

The project uses the KITTI 2D Object Detection dataset. The labeled dataset contains 7,481 roadway images with object annotations. For this project, the labeled images will be divided into training, validation, and held-out test sets so that model performance can be evaluated consistently.

Primary vehicle classes:
- Car
- Van
- Truck

## Project Workflow

1. Dataset access and inspection
2. Exploratory data analysis
3. Data cleaning and preprocessing
4. Train/validation/test split
5. Baseline YOLO model
6. Fine-tuned YOLO model
7. Data augmentation experiment
8. Model evaluation
9. Error analysis and visualization
10. Technical report and presentation

## Planned EDA

The exploratory data analysis will examine:
- image dimensions and aspect ratios
- class distribution
- number of objects per image
- bounding-box widths, heights, and areas
- relative object size
- class imbalance
- small or distant vehicles
- occluded and truncated objects
- invalid or missing annotations
- representative annotated images

## Evaluation Metrics

The project will evaluate object detection performance using:
- Precision
- Recall
- F1-score
- mAP@0.5
- mAP@0.5:0.95

## Repository Structure

```text
vehicle-detection-cnn/
├── README.md
├── notebooks/
│   └── vehicle_detection_kitti.ipynb
├── src/
│   ├── eda.py
│   ├── preprocessing.py
│   ├── train.py
│   └── evaluate.py
├── config/
│   └── kitti_vehicle.yaml
├── results/
├── report/
├── requirements.txt
└── .gitignore
```

## Environment

The primary development environment is Google Colab with Python. Training will use Ultralytics YOLO with PyTorch.

## Notes

The KITTI images, trained model weights, and generated experiment outputs are not committed to this repository because they are large files. The notebook and scripts will document how to reproduce the dataset preparation, training, and evaluation workflow.
