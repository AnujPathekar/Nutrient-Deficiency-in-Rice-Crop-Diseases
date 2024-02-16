# Nutrient-Deficiency-in-Rice-Crop-Diseases

![Rice Leaf Disease](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTEze8YtXObKeMjVl-uUvzkZItnMN-F6kSVnGP29aqvMPju8FNudEKgaScPMC6bLatHlTM&usqp=CAU)
## Project Description
The "Nutrient Deficiency in Rice Crop Diseases" project aims to develop a deep learning-based solution for identifying and diagnosing nutrient deficiency in rice crops. The project focuses on leveraging computer vision and machine learning techniques to assist farmers and agricultural experts in detecting and addressing nutrient-related issues in rice fields. The main objective is to demonstrate the use of deep learning for image classification tasks.

## Table of Contents
- [Installation](#installation)
- [Usage](#usage)
- [Dataset](#dataset)
- [Model Architecture](#model-architecture)
- [Training](#training)
- [Evaluation](#evaluation)
- [Results](#results)
- [Pre-trained Models](#pre-trained-models)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)
- [Acknowledgments](#acknowledgments)

## Installation
To use this image classifier, you need to have Python 3.6 or higher installed. Clone this repository and install the required packages using pip:

```bash
git clone https://github.com/your-username/deep-learning-image-classifier.git
cd deep-learning-image-classifier
pip install -r requirements.txt
```


## Dataset
The image classifier uses the CIFAR-10 dataset for training and validation. The dataset is automatically downloaded and preprocessed during the first run.

## Model Architecture
The deep learning model used in this project is a Convolutional Neural Network (CNN) with the following architecture:

```bash

Model: "sequential_2"
_________________________________________________________________
 Layer (type)                Output Shape              Param #   
=================================================================
 sequential (Sequential)     (32, 256, 256, 3)         0         
                                                                 
 conv2d (Conv2D)             (32, 254, 254, 32)        896       
                                                                 
 max_pooling2d (MaxPooling2D  (32, 127, 127, 32)       0         
 )                                                               
                                                                 
 conv2d_1 (Conv2D)           (32, 125, 125, 64)        18496     
                                                                 
 max_pooling2d_1 (MaxPooling  (32, 62, 62, 64)         0         
 2D)                                                             
                                                                 
 conv2d_2 (Conv2D)           (32, 60, 60, 64)          36928     
                                                                 
 max_pooling2d_2 (MaxPooling  (32, 30, 30, 64)         0         
 2D)                                                             
                                                                 
 conv2d_3 (Conv2D)           (32, 28, 28, 64)          36928     
                                                                 
 max_pooling2d_3 (MaxPooling  (32, 14, 14, 64)         0         
 2D)                                                             
                                                                 
 conv2d_4 (Conv2D)           (32, 12, 12, 64)          36928     
                                                                 
 max_pooling2d_4 (MaxPooling  (32, 6, 6, 64)           0         
 2D)                                                             
                                                                 
 conv2d_5 (Conv2D)           (32, 4, 4, 64)            36928     
                                                                 
 max_pooling2d_5 (MaxPooling  (32, 2, 2, 64)           0         
 2D)                                                             
                                                                 
 flatten (Flatten)           (32, 256)                 0         
                                                                 
 dense (Dense)               (32, 32)                  8224      
                                                                 
 dense_1 (Dense)             (32, 5)                   165       
                                                                 
=================================================================
Total params: 175,493
Trainable params: 175,493
Non-trainable params: 0
_________________________________________________________________
```
