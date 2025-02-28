# Solar Panel Detection using YOLOv8

## Introduction
This project focuses on detecting solar panels in aerial imagery using YOLOv8. The workflow includes data preparation, model training, evaluation, and performance metrics computation.

---

## Step 1: Data Exploration and Understanding
### 1.1 Mount Google Drive & Install Dependencies

### 1.2 Verify Dataset Structure
- Dataset is stored in Google Drive: `/content/drive/MyDrive/Dataset`
- Image folder: `image_chips_native`
- Label folder: `labels_merged`

### 1.3 Count Number of Images & Labels

### 1.4 Compute Solar Panel Instances & Area
- Count number of bounding boxes per label file
- Compute the average solar panel area in square meters
- Plot histogram of area distribution

---

## Step 2: Implementing IoU & Average Precision Calculation
### 2.1 IoU Calculation

### 2.2 Average Precision (AP) Calculation
- Pascal VOC 11-point Interpolation
- COCO 101-point Interpolation
- Area Under Precision-Recall Curve (AUC-PR)

## Step 3: Model Building and Evaluation
### 3.1 Data Preprocessing
- Convert `.tif` images to `.jpg`
- Split dataset into `train`, `val`, and `test` (80-10-10 split)

### 3.2 Create YOLOv8 Configuration File

### 3.3 Train YOLOv8 Model

### 3.4 Model Evaluation
- Plot validation loss over epochs
- Compute mAP50 and display results

### 3.5 Visualize Predictions

## Results & Conclusion
- The model was trained and evaluated on solar panel detection.
- Key performance metrics:
  - **mAP50:** Computed on validation and test datasets.
  - **Precision, Recall, F1-score:** Evaluated across multiple IoU and confidence thresholds.
- Future improvements:
  - Enhance dataset quality
  - Experiment with different YOLO versions and hyperparameters
  - Optimize post-processing for better detection

---
**Author:** Ananya Kumari 
**Date:** 28-02-2025 

