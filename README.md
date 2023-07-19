# Semantic Segmentation Project

## Objective
The objective of this project is to develop a semantic segmentation model for precise pixel-level image classification. This technology finds practical applications in diverse fields such as autonomous driving, medical imaging, and augmented reality, enabling more accurate understanding resulting in improved decision-making and visual perception.

The dataset contains high-quality, pixel-level annotations for 30 classes, including road, sidewalk, building, vegetation, person, car, etc.

Practical Usage:
1. **Autonomous Driving and Robotics:** Semantic segmentation is crucial for autonomous vehicles and robots to understand the surrounding environment accurately. By segmenting different objects and obstacles on the road, autonomous vehicles can plan their trajectory, avoid collisions, and make safe driving decisions.
2. **Augmented Reality and Virtual Reality:** Semantic segmentation can be applied to enhance augmented reality (AR) and virtual reality (VR) experiences. By segmenting the real-world scene, virtual objects can be better integrated into the environment, providing a more immersive experience.

## Overview
This project focuses on semantic segmentation using a U-net model with the ResNet34 architecture. The goal is to label each pixel in an image with a corresponding class label.

## Dataset
- The dataset is obtained from the Cityscapes website.
- It contains 2400 images, totaling approximately 17 GB.
- The images and corresponding masks are used for training the model.

## Preprocessing
1. Load the images and masks from the dataset.
2. Store the paths of the images and masks in a data frame.
3. Perform preprocessing ( read and resize to 256 * 256 ) on the images and masks.
4. Find all the unique classes in the masked image ( different int values ) and replace them with continues series starting from 0.

## Data Normalization
- Normalize the input images to ensure consistent and standardized input for the model.

## Encoding the masks
- Encode the masks to one-hot encoding with respected class found in preprocessing step.

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
