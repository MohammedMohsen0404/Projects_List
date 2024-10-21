# Aerial Semantic Segmentation by Drone


<p align="center">
  <img src="https://github.com/user-attachments/assets/3a1526b4-fa75-4b47-baf5-b8c9c626bb10" height="300"/>
</p>


## Summary
This project aims to enhance the safety of autonomous drone flights by developing models for semantic segmentation and person detection using the Aerial Semantic Segmentation Drone Dataset. The dataset contains high-resolution images of urban scenes, annotated with 20 semantic classes, such as trees, roofs, and vehicles. The goal is to create accurate models that can interpret these complex scenes, improving drone navigation and landing procedures.

## About Dataset

The Semantic Drone Dataset focuses on semantic understanding of urban scenes to increase the safety of autonomous drone flight and landing procedures. Imagery depicts more than 20 houses from a nadir (bird's eye) view, acquired at an altitude of 5 to 30 meters above ground. A high-resolution camera captured images at a size of 6000x4000px (24Mpx). The training set contains 400 publicly available images, and the test set consists of 200 private images.



## Semantic Classes
- Tree
- Grass
- Other vegetation
- Dirt
- Gravel
- Rocks
- Water
- Paved area
- Pool
- Person
- Dog
- Car
- Bicycle
- Roof
- Wall
- Fence
- Fence-pole
- Window
- Door
- Obstacle

## Tools and Technologies
- **Programming Language:** Python
- **Libraries:** TensorFlow/Keras, NumPy, Matplotlib
- **Metrics:** Accuracy, Precision, Recall, F1 Score, Confusion Matrix
- 
## Model Architecture
| Layer (type)                   | Output Shape         | Param #   | Connected to             |
|--------------------------------|----------------------|-----------|--------------------------|
| conv2d_transpose_3             | (None, 768, 512, 32) | 18,464    | activation_15[0]        |
| concatenate_3                   | (None, 768, 512, 64) | 0         | conv2d_transpose_3[0]   |
| conv2d_16 (Conv2D)             | (None, 768, 512, 32) | 18,464    | concatenate_3[0]        |
| batch_normalization_16          | (None, 768, 512, 32) | 128       | conv2d_16[0][0]         |
| activation_16                   | (None, 768, 512, 32) | 0         | batch_normalization_16[0]|
| conv2d_17 (Conv2D)             | (None, 768, 512, 32) | 9,248     | activation_16[0][0]     |
| batch_normalization_17          | (None, 768, 512, 32) | 128       | conv2d_17[0][0]         |
| activation_17                   | (None, 768, 512, 32) | 0         | batch_normalization_17[0]|
| conv2d_18 (Conv2D)             | (None, 768, 512, 24) | 792       | activation_17[0][0]     |

- **Total params:** 8,643,032 (32.97 MB)  
- **Trainable params:** 8,637,144 (32.95 MB)  
- **Non-trainable params:** 5,888 (23.00 KB)  

## Model Performance
- **Training Accuracy:** 68.30%
- **Training Loss:** 0.95
- **Test Accuracy:** 67.56%
- **Test Loss:** 0.99

## Samples 
<p align="center">
  <img src="https://github.com/user-attachments/assets/0d1212d8-4d11-4bc0-bc59-9b81db00e8fc"/>
</p>
