# CIFAR-100 Transfer Learning with InceptionV3

## Overview
This repository contains code for a deep learning model using transfer learning with InceptionV3 on the CIFAR-100 dataset. The model achieves a testing accuracy of 76.66%.

## Dataset
The CIFAR-100 dataset consists of 60,000 32x32 color images in 100 different classes. It is divided into 50,000 training images and 10,000 testing images.

## Model Architecture
The model utilizes the InceptionV3 architecture pretrained on ImageNet. The top layers are fine-tuned for the CIFAR-100 classification task. Key features include global average pooling, dropout, batch normalization, and a dense output layer.

## Data Preprocessing
The dataset is preprocessed by normalizing pixel values to the range [0, 1]. Image data augmentation techniques, such as rotation, zooming, and flipping, are applied using the Keras ImageDataGenerator.

## Training
The model is trained for 50 epochs with a learning rate reduction strategy. If the validation accuracy does not improve for 3 consecutive epochs, the learning rate is decreased by a factor of 0.6.

## Results
The training and validation accuracy and loss are visualized using matplotlib. The final testing accuracy achieved by the model is 76.66%. A confusion matrix is generated to assess the model's performance on individual classes.

## Usage
1. Clone the repository: `git clone https://github.com/your-username/cifar-100-transfer-learning.git`
2. Run the Jupyter notebook or Python script to train and evaluate the model.

Feel free to explore and modify the code to experiment with different architectures, hyperparameters, or datasets. If you find this project helpful, consider giving it a star!

*Note:* This readme assumes that the dataset link is not provided due to potential licensing or size constraints. Please make sure to comply with the dataset's terms of use if you decide to use it.
