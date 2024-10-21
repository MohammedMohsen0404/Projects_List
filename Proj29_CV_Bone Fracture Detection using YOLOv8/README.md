# Bone Fracture Detection using YOLOv8

<p align="center">
  <img src="https://github.com/user-attachments/assets/2ecc0c38-d0b5-4dd5-9a7c-a5bb3713c7e8" height="300"/>
</p>

## Summary
This project aims to advance automated bone fracture detection using a comprehensive dataset of X-ray images, categorized into various fracture types, such as Elbow Positive, Fingers Positive, Forearm Fracture, Humerus Fracture, Shoulder Fracture, and Wrist Positive. The dataset includes annotated images with bounding boxes or pixel-level segmentation masks, aiding in the development and evaluation of object detection algorithms like YOLO. By leveraging this dataset, the project seeks to enhance computer vision solutions for medical diagnostics, ultimately improving patient care through accurate and efficient fracture detection.

## About Dataset
### Bone Fracture Detection
A comprehensive dataset of X-ray images was created for bone fracture detection, specifically designed for computer vision projects. The primary goal of this dataset is to aid in developing and evaluating algorithms for automated bone fracture detection.

The dataset contains images categorized into different classes, each representing a specific type of bone fracture. These classes include Elbow Positive, Fingers Positive, Forearm Fracture, Humerus Fracture, Shoulder Fracture, and Wrist Positive.

Each image in the dataset is annotated with either bounding boxes or pixel-level segmentation masks to indicate the location and extent of the detected fracture. This facilitates the training and evaluation of bone fracture detection algorithms.

The bone fracture detection dataset is a useful resource for researchers and developers who want to train machine learning models, specifically focusing on object detection algorithms, to automatically detect and classify bone fractures in X-ray images. The dataset's diversity of fracture classes enables the development of robust models capable of accurately identifying fractures in different regions of the upper extremities.

The aim of creating this dataset is to accelerate the development of computer vision solutions for automated fracture detection, supporting advancements in medical diagnostics and improving patient care.

## Model Configuration
- **Model Type:** YOLOv8
- **Number of Classes:** 1 (Bone Fractures)

### Model Architecture Summary
| Layer Type                           | Output Shape  | Parameters |
|--------------------------------------|---------------|------------|
| Conv                                 | -             | 928        |
| Conv                                 | -             | 18,560     |
| C2f                                  | -             | 29,056     |
| Conv                                 | -             | 73,984     |
| C2f                                  | -             | 197,632    |
| Conv                                 | -             | 295,424    |
| C2f                                  | -             | 788,480    |
| Conv                                 | -             | 1,180,672  |
| C2f                                  | -             | 1,838,080  |
| SPPF                                 | -             | 656,896    |
| Upsample                             | -             | 0          |
| Concat                               | -             | 0          |
| C2f                                  | -             | 591,360    |
| Upsample                             | -             | 0          |
| Concat                               | -             | 0          |
| C2f                                  | -             | 148,224    |
| Conv                                 | -             | 147,712    |
| Concat                               | -             | 0          |
| C2f                                  | -             | 493,056    |
| Conv                                 | -             | 590,336    |
| Concat                               | -             | 0          |
| C2f                                  | -             | 1,969,152  |
| Detect                               | -             | 2,116,435  |

- **Total Layers:** 225
- **Total Parameters:** 11,135,987
- **GFLOPs:** 28.6

## Model Evaluation

| Metric                          | Value   |
|---------------------------------|---------|
| Total Images                    | 53      |
| Total Instances                 | 53      |
| Box Precision (P)              | 1.000   |
| Recall (R)                     | 1.000   |
| mAP @ IoU=0.50                 | 0.995   |
| mAP @ IoU=0.50-0.95            | 0.986   |

### Speed Metrics

| Phase           | Time (ms) |
|-----------------|-----------|
| Preprocess      | 0.2       |
| Inference       | 8.8       |
| Postprocess     | 3.3       |

## Samples 
<p align="center">
  <img src="https://github.com/user-attachments/assets/0ebff5a1-e404-44c8-8619-a02d5a2fc9cd"/>
</p>

