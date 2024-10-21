# Ships Object Detection using YOLOv8

<p align="center">
  <img src="https://github.com/user-attachments/assets/a7c12e22-750c-41c9-be54-f2dabd8232d5" height="300"/>
</p>

## Summary
This project aims to develop efficient ship detection models using a carefully curated dataset of 26.9k annotated images. The dataset, labeled in the YOLO format, focuses exclusively on detecting ships, which has crucial applications in maritime safety, fisheries management, marine pollution monitoring, and maritime security. By leveraging this dataset, researchers can create precise models that contribute to preventing accidents, monitoring fishing activities, and enhancing overall maritime operations.

## Dataset Overview
- **Total Images:** 26,900
- **Training Frames:** 9,697
- **Validation Frames:** 2,165
- **Test Frames:** 1,573
- **Total Frames:** 13,435

## Model Configuration
- **Model Type:** YOLOv8
- **Number of Classes:** 1 (Ships)


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

#### Evaluation Metrics

| Metric                          | Value   |
|---------------------------------|---------|
| Total Images                    | 1,573   |
| Total Instances                 | 2,872   |
| Box Precision (P)              | 0.688   |
| Recall (R)                     | 0.264   |
| mAP @ IoU=0.50                 | 0.494   |
| mAP @ IoU=0.50-0.95            | 0.328   |

#### Speed Metrics

| Phase           | Time (ms) |
|-----------------|-----------|
| Preprocess      | 0.2       |
| Inference       | 7.6       |
| Postprocess     | 0.9       |

## Samples 
<p align="center">
  <img src=""/>
</p>

![Uploading download.png…]()
