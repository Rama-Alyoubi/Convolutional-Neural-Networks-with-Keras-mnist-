# Convolutional-Neural-Networks-with-Keras-mnist-

This repository contains an implementation of a Convolutional Neural Network (CNN) using Keras framework to classify the MNIST dataset. The MNIST dataset consists of 60,000 training images of handwritten digits (0-9) and 10,000 test images, each of size 28x28 pixels.

## Requirements
To run the code, you need the following dependencies installed:

- Python (3.6 or higher)
- Keras (2.6.0 or higher)
- TensorFlow (2.6.0 or higher)
- NumPy (1.19.5 or higher)
- Matplotlib (3.4.3 or higher)
## Dataset
The MNIST dataset is automatically downloaded and preprocessed by Keras. It is split into training and test sets, with the training set used for model training and the test set for evaluation.

## Model Architecture
The CNN model is defined using Keras Sequential API. It consists of several layers:

- Convolutional layers: These layers extract features from the input images using convolutional filters.
- MaxPooling layers: These layers downsample the input by selecting the maximum value in each region.
- Flatten layer: This layer flattens the output from the previous layer into a 1-dimensional vector.
- Dense layers: These fully connected layers take the flattened vector as input and perform classification.

The CNN model architecture used in this code is as follows:

```
Model: "CNN Model"
_________________________________________________________________
Layer (type)                 Output Shape              Param #
=================================================================
conv2d (Conv2D)              (None, 26, 26, 32)        320
_________________________________________________________________
max_pooling2d (MaxPooling2D) (None, 13, 13, 32)        0
_________________________________________________________________
flatten (Flatten)            (None, 5408)              0
_________________________________________________________________
dense (Dense)                (None, 128)               692352
_________________________________________________________________
dense_1 (Dense)              (None, 10)                1290
=================================================================
Total params: 693,962
Trainable params: 693,962
Non-trainable params: 0
_________________________________________________________________
```

## Acknowledgments
The code implementation in this repository is based on the knowledge and skills acquired from the IBM course titled "Introduction to Deep Learning & Neural Networks with Keras." We would like to express our gratitude to IBM for providing valuable educational resources and guidance in the field of deep learning.

We also acknowledge the contributions of various tutorials, guides, and examples available in the Keras documentation and the wider deep learning community, which have influenced the development of this code implementation.

If you find this code useful, consider giving a star to the repository or acknowledging it in your project's documentation.

## References
- MNIST dataset: http://yann.lecun.com/exdb/mnist/
- Keras documentation: https://keras.io/
