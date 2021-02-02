# Introduction

Image classification is the process of taking an input and returning a class or a probability that the input is a particular class. 

# Goals

You should establish a neural network involving advanced DNN modules such as convolution layers, RELU, pooling, and fully connected layers etc. in order to determine the
specific category of an input image.

# Dataset

The CIFAR-10 dataset consists of 60000 32x32 color images in 10 classes, with 6000 images
per class. There are 50000 training images and 10000 test images.
The dataset is divided into five training batches and one test batch, each with 10000 images.
The test batch contains exactly 1000 randomly-selected images from each class. The training
batches contain the remaining images in random order, but some training batches may contain
more images from one class than another. Between them, the training batches contain exactly
5000 images from each class.

# Requirements
1. Program a data loader for CIFAR-10 dataset:

    a. You are supposed to split the dataset into train data and test data
  
    b. Dataset predefined by Pytorch can be applied in your implementation
  
    c. Both training data loader and testing data loader need to be established by torch.utils.data.DataLoader
    
2. Build a CNN model for classification:

    a. The model should be established based on torch.nn.Module and torch.nn.functional
    
    b. The model (base model) should be built upon the same architecture of the GoogLeNet structure
    
    c. You can add more layers in the base model to push performance: OPTIONAL
    
3. Write training frameworks to implement the classification pipeline:

    a. Apply the dataloader you wrote in the first step
    
    b. Apply the CNN model you wrote written in the second step
    
    c. Define a Cross-Entropy criterion function
    
    d. Define an Adam Optimizer function
    
4. Write testing frameworks to evaluate your classification pipeline:

    a. Apply the dataloader you wrote in the first step
    
    b. Apply the CNN model you wrote in the second step
    
    c. Define the accuracy of your model’s prediction
