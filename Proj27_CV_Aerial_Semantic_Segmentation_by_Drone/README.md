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
#### Model: U-Net

| Layer (type)               | Output Shape        | Param #   | Connected to          |
|----------------------------|---------------------|-----------|-----------------------|
| image_input                | (None, 768, 512, 3) | 0         | -                     |
| conv2d (Conv2D)           | (None, 768, 512, 32) | 896       | image_input[0][0]    |
| batch_normalization        | (None, 768, 512, 32) | 128       | conv2d[0][0]         |
| activation                 | (None, 768, 512, 32) | 0         | batch_normalization[0]|
| conv2d_1 (Conv2D)         | (None, 768, 512, 32) | 9,248     | activation[0][0]     |
| batch_normalization_1      | (None, 768, 512, 32) | 128       | conv2d_1[0][0]       |
| activation_1               | (None, 768, 512, 32) | 0         | batch_normalization_1[0]|
| max_pooling2d             | (None, 384, 256, 32) | 0         | activation_1[0][0]   |
| conv2d_2 (Conv2D)         | (None, 384, 256, 64) | 18,496    | max_pooling2d[0][0]  |
| ...                        | ...                 | ...       | ...                   |
| conv2d_17 (Conv2D)        | (None, 768, 512, 32) | 9,248     | activation_16[0][0]   |
| batch_normalization_17     | (None, 768, 512, 32) | 128       | conv2d_17[0][0]      |
| activation_17              | (None, 768, 512, 32) | 0         | batch_normalization_17[0]|
| conv2d_18 (Conv2D)        | (None, 768, 512, 24) | 792       | activation_17[0][0]   |

**Total params:** 8,643,032  
**Trainable params:** 8,637,144  
**Non-trainable params:** 5,888


## Model Performance
- **Training Accuracy:** 68.30%
- **Training Loss:** 0.95
- **Test Accuracy:** 67.56%
- **Test Loss:** 0.99

## Samples 
<p align="center">
  <img src="https://github.com/user-attachments/assets/0d1212d8-4d11-4bc0-bc59-9b81db00e8fc"/>
</p>
