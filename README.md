# Semantic Segmentation Project

## Overview
This project focuses on semantic segmentation using a U-net model with the ResNet34 architecture. The goal is to label each pixel in an image with a corresponding class label.

## Dataset
- The dataset is obtained from the Cityscapes website.
- It contains 2400 images, totaling approximately 17 GB.
- The images and corresponding masks are used for training the model.

## Preprocessing
1. Load the images and masks from the dataset.
2. Store the paths of the images and masks in a data frame.
3. Perform preprocessing on the images and masks.

## Data Normalization
- Normalize the input images to ensure consistent and standardized input for the model.

## Model Building
- Utilize the U-net model architecture with ResNet34 as the backbone.
- Compile the model using the Adam optimizer.
- Use Dice Loss as the loss function for training the model.
- Evaluate the model using the IOU (Intersection over Union) score.

## Training
- Fit the compiled model on the input images and their corresponding masks.
- Train the model to learn pixel-wise semantic labels.

## Results
- After training, the model achieved an IOU score of 43%.
- Evaluate and analyze the performance of the model based on the IOU score.

## Future Improvements
- Experiment with different model architectures and backbones.
- Explore advanced data augmentation techniques to improve performance.
- Increase the dataset size for better generalization.
