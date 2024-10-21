# CAMvid Semantic Segmentation

<p align="center">
  <img src="https://github.com/user-attachments/assets/7c054854-baec-4d5f-8553-fdba25b4a25e" height="300"/>
</p>

## Summary
This project aims to utilize the Cambridge-driving Labeled Video Database (CamVid) for real-time semantic segmentation research. By analyzing pixel-level ground truth labels across 32 semantic classes, the goal is to develop advanced segmentation models that can accurately classify and segment various elements in driving scenes. This work contributes to the broader field of autonomous driving and real-time image processing.

## Dataset
**N.B.** The owner of this dataset is The University of Cambridge. I'm not in any way affiliated with The University of Cambridge. I just thought it would be nice for people to have this dataset available on Kaggle.

### Context
The Cambridge-driving Labeled Video Database (CamVid) provides ground truth labels that associate each pixel with one of 32 semantic classes. This dataset is often used in (real-time) semantic segmentation research.

## Tools and Technologies
- **Programming Language:** Python
- **Libraries:** TensorFlow/Keras, NumPy, Matplotlib
- **Metrics:** Accuracy, Precision, Recall, F1 Score, Confusion Matrix

## Model Architecture

| Layer (type)        | Output Shape      | Param #   | Connected to            |
|---------------------|-------------------|-----------|-------------------------|
| image_input         | (None, 256, 256, 3) | 0         | -                       |
| (InputLayer)        |                   |           |                         |
| conv2d (Conv2D)     | (None, 256, 256, 64) | 1,792     | image_input[0][0]      |
| batch_normalization  | (None, 256, 256, 64) | 256       | conv2d[0][0]           |
| activation          | (None, 256, 256, 64) | 0         | batch_normalization[0][0] |
| conv2d_1 (Conv2D)   | (None, 256, 256, 64) | 36,928    | activation[0][0]       |
| batch_normalization  | (None, 256, 256, 64) | 256       | conv2d_1[0][0]         |
| activation_1        | (None, 256, 256, 64) | 0         | batch_normalization[1][0] |
| max_pooling2d       | (None, 128, 128, 64) | 0         | activation_1[0][0]     |
| (MaxPooling2D)      |                   |           |                         |
| conv2d_2 (Conv2D)   | (None, 128, 128, 128) | 73,856    | max_pooling2d[0][0]    |
| batch_normalization  | (None, 128, 128, 128) | 512       | conv2d_2[0][0]         |
| activation_2        | (None, 128, 128, 128) | 0         | batch_normalization[2][0] |
| conv2d_3 (Conv2D)   | (None, 128, 128, 128) | 147,584   | activation_2[0][0]     |
| batch_normalization  | (None, 128, 128, 128) | 512       | conv2d_3[0][0]         |
| activation_3        | (None, 128, 128, 128) | 0         | batch_normalization[3][0] |
| max_pooling2d_1     | (None, 64, 64, 128)   | 0         | activation_3[0][0]     |
| (MaxPooling2D)      |                   |           |                         |
| conv2d_4 (Conv2D)   | (None, 64, 64, 256)   | 295,168   | max_pooling2d_1[0][0]  |
| batch_normalization  | (None, 64, 64, 256)   | 1,024     | conv2d_4[0][0]         |
| activation_4        | (None, 64, 64, 256)    | 0         | batch_normalization[4][0] |
| conv2d_5 (Conv2D)   | (None, 64, 64, 256)    | 590,080   | activation_4[0][0]     |
| batch_normalization  | (None, 64, 64, 256)    | 1,024     | conv2d_5[0][0]         |
| activation_5        | (None, 64, 64, 256)    | 0         | batch_normalization[5][0] |
| max_pooling2d_2     | (None, 32, 32, 256)    | 0         | activation_5[0][0]     |
| (MaxPooling2D)      |                   |           |                         |
| conv2d_6 (Conv2D)   | (None, 32, 32, 512)    | 1,180,160 | max_pooling2d_2[0][0]  |
| batch_normalization  | (None, 32, 32, 512)    | 2,048     | conv2d_6[0][0]         |
| activation_6        | (None, 32, 32, 512)    | 0         | batch_normalization[6][0] |
| conv2d_7 (Conv2D)   | (None, 32, 32, 512)    | 2,359,808 | activation_6[0][0]     |
| batch_normalization  | (None, 32, 32, 512)    | 2,048     | conv2d_7[0][0]         |
| activation_7        | (None, 32, 32, 512)    | 0         | batch_normalization[7][0] |
| max_pooling2d_3     | (None, 16, 16, 512)    | 0         | activation_7[0][0]     |
| (MaxPooling2D)      |                   |           |                         |
| dropout (Dropout)   | (None, 16, 16, 512)    | 0         | max_pooling2d_3[0][0]  |
| conv2d_8 (Conv2D)   | (None, 16, 16, 1024)   | 4,719,616 | dropout[0][0]          |
| batch_normalization  | (None, 16, 16, 1024)   | 4,096     | conv2d_8[0][0]         |
| activation_8        | (None, 16, 16, 1024)   | 0         | batch_normalization[8][0] |
| conv2d_9 (Conv2D)   | (None, 16, 16, 1024)   | 9,438,208 | activation_8[0][0]     |
| batch_normalization  | (None, 16, 16, 1024)   | 4,096     | conv2d_9[0][0]         |
| activation_9        | (None, 16, 16, 1024)   | 0         | batch_normalization[9][0] |
| dropout_1 (Dropout) | (None, 16, 16, 1024)   | 0         | activation_9[0][0]     |
| conv2d_transpose    | (None, 32, 32, 512)    | 4,719,104 | dropout_1[0][0]        |
| (Conv2DTranspose)   |                   |           |                         |
| concatenate         | (None, 32, 32, 1024)   | 0         | conv2d_transpose[0][0] |
| (Concatenate)       |                   |           | activation_7[0][0]     |
| conv2d_10 (Conv2D)  | (None, 32, 32, 512)    | 4,719,104 | concatenate[0][0]      |
| batch_normalization  | (None, 32, 32, 512)    | 2,048     | conv2d_10[0][0]        |
| activation_10       | (None, 32, 32, 512)    | 0         | batch_normalization[10][0] |
| conv2d_11 (Conv2D)  | (None, 32, 32, 512)    | 2,359,808 | activation_10[0][0]    |
| batch_normalization  | (None, 32, 32, 512)    | 2,048     | conv2d_11[0][0]        |
| activation_11       | (None, 32, 32, 512)    | 0         | batch_normalization[11][0] |
| dropout_2 (Dropout) | (None, 32, 32, 512)    | 0         | activation_11[0][0]    |
| conv2d_transpose_1  | (None, 64, 64, 256)    | 1,179,904 | dropout_2[0][0]        |
| (Conv2DTranspose)   |                   |           |                         |
| concatenate_1       | (None, 64, 64, 512)    | 0         | conv2d_transpose_1[0][0] |
| (Concatenate)       |                   |           | activation_5[0][0]     |
| conv2d_12 (Conv2D)  | (None, 64, 64, 256)    | 1,179,904 | concatenate_1[0][0]    |
| batch_normalization  | (None, 64, 64, 256)    | 1,024     | conv2d_12[0][0]        |
| activation_12       | (None, 64, 64, 256)    | 0         | batch_normalization[12][0] |
| conv2d_13 (Conv2D)  | (None, 64, 64, 256)    | 590,080   | activation_12[0][0]    |
| batch_normalization  | (None, 64, 64, 256)    | 1,024     | conv2d_13[0][0]        |
| activation_13       | (None, 64, 64, 256)    | 0         | batch_normalization[13][0] |
| dropout_3 (Dropout) | (None, 64, 64, 256)    | 0         | activation_13[0][0]    |
| conv2d_transpose_2  | (None, 128, 128, 128) | 295,168   | dropout_3[0][0]        |
| (Conv2DTranspose)   |                   |           |                         |
| concatenate_2       | (None, 128, 128, 256) | 0         | conv2d_transpose_2[0][0] |
| (Concatenate)       |                   |           | activation_3[0][0]     |
| conv2d_14 (Conv2D)  | (None, 128, 128, 128) | 147,584   | concatenate_2[0][0]    |
| batch_normalization  | (None, 128, 128, 128) | 512       | conv2d_14[0][0]        |
| activation_14       | (None, 128, 128, 128) | 0         | batch_normalization[14][0] |
| conv2d_15 (Conv2D)  | (None, 128, 128, 128) | 147,584   | activation_14[0][0]    |
| batch_normalization  | (None, 128, 128, 128) | 512       | conv2d_15[0][0]        |
| activation_15       | (None, 128, 128, 128) | 0         | batch_normalization[15][0] |
| dropout_4 (Dropout) | (None, 128, 128, 128) | 0         | activation_15[0][0]    |
| conv2d_transpose_3  | (None, 256, 256, 64)   | 73,792    | dropout_4[0][0]        |
| (Conv2DTranspose)   |                   |           |                         |
| concatenate_3       | (None, 256, 256, 128) | 0         | conv2d_transpose_3[0][0] |
| (Concatenate)       |                   |           | activation_1[0][0]     |
| conv2d_16 (Conv2D)  | (None, 256, 256, 64)   | 73,792    | concatenate_3[0][0]    |
| batch_normalization  | (None, 256, 256, 64)   | 256       | conv2d_16[0][0]        |
| activation_16       | (None, 256, 256, 64)   | 0         | batch_normalization[16][0] |
| conv2d_17 (Conv2D)  | (None, 256, 256, 64)   | 36,928    | activation_16[0][0]    |
| batch_normalization  | (None, 256, 256, 64)   | 256       | conv2d_17[0][0]        |
| activation_17       | (None, 256, 256, 64)   | 0         | batch_normalization[17][0] |
| conv2d_18 (Conv2D)  | (None, 256, 256, 3)    | 1,737     | activation_17[0][0]    |
| (Conv2D)            |                   |           |                         |

**Total params:** 31,307,057  
**Trainable params:** 31,297,057  
**Non-trainable params:** 10,000


## Model Performance
- **Training Accuracy:** 78.28%
- **Training Loss:** 0.56
- **Test Accuracy:** 78.57%
- **Test Loss:** 0.85

## samples

<p align="center">
  <img src="https://github.com/user-attachments/assets/67bc9ee6-2290-4fd6-9d5f-4677ef87ebb1"/>
</p>
