# Crop Disease Prediction System

## Overview
Welcome to the Crop Disease Prediction System repository! This project focuses on leveraging deep learning models, DenseNet121 and MobileNetV2, to accurately detect crop diseases. With our models, you can achieve up to 98% accuracy using DenseNet121 and 91% accuracy using MobileNetV2.

## Contents
- [Introduction](#introduction)
- [Models Used](#models-used)
- [Dataset](#dataset)
- [Usage](#usage)
- [Results](#results)
- [License](#license)

## Introduction
Accurate detection of crop diseases is essential for maintaining healthy crops and maximizing agricultural yield. This repository contains two state-of-the-art deep learning models, DenseNet121 and MobileNetV2, designed to identify various crop diseases effectively. Both models have been trained and fine-tuned to deliver high accuracy in disease prediction.

## Models Used
### DenseNet121
DenseNet121 (Dense Convolutional Network) is a deep learning architecture known for its efficient parameter usage and improved feature propagation. It connects each layer to every other layer in a feed-forward manner, enhancing gradient flow and reducing the risk of vanishing gradients.

- *Accuracy*: 98%
- *Paper*: [Densely Connected Convolutional Networks](https://arxiv.org/abs/1608.06993)

### MobileNetV2
MobileNetV2 is a lightweight and efficient neural network designed for mobile and embedded vision applications. It uses depthwise separable convolutions and inverted residuals with linear bottlenecks to achieve a good trade-off between accuracy and computational cost.

- *Accuracy*: 91%
- *Paper*: [MobileNetV2: Inverted Residuals and Linear Bottlenecks](https://arxiv.org/abs/1801.04381)

## Dataset
The models were trained on a dataset comprising thousands of images of healthy and diseased crops. Each image is labeled with the corresponding disease category. The dataset includes a diverse range of crop species and disease types to ensure robust model performance.

## Usage
To use the crop disease prediction models, follow these steps:

1. Clone the repository:
bash
git clone https://github.com/yashashvisri/Crop-disease-prediction.git
cd Crop-disease-prediction


2. Install the required dependencies:
bash
pip install -r requirements.txt


3. Load and preprocess the dataset (ensure you have the dataset in the appropriate format and path).

4. Run the prediction script:
bash
python predict_crop_disease.py --model densenet121 --image_path path/to/image.jpg

Or for MobileNetV2:
bash
python predict_crop_disease.py --model mobilenetv2 --image_path path/to/image.jpg


5. The script will output the predicted disease along with the confidence score.

## Results
### DenseNet121
- *Accuracy*: 98%

### MobileNetV2
- *Accuracy*: 91%

## License
This project is licensed under the [MIT License](LICENSE). Feel free to use, modify, and distribute the code for any purpose.
