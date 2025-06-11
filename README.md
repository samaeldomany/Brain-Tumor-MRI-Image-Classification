# Brain-Tumor-MRI-Image-Classification
This project implements an image classification system to detect and classify different types of brain tumors (Meningioma, No Tumor, Pituitary, Glioma) using MRI scan images.


## Overview
This Jupyter Notebook demonstrates a deep learning approach for classifying brain MRI images into four categories: Meningioma, No Tumor, Pituitary, and Glioma. The project covers the entire machine learning pipeline, including dataset organization, data augmentation, model building using a pre-trained EfficientNetB0, training, and evaluation with various performance metrics and a confusion matrix.

## Features
### 1. Robust Dataset Management
- Automated Organization: Functionality to structure raw image datasets into train, val, and test directories with proper class subfolders.
- Efficient Loading: Utilizes tf.keras.utils.image_dataset_from_directory for efficient loading of image datasets.
- Data Preprocessing: Normalizes image pixel values for model readiness.

### 2. Advanced Data Augmentation
- Implements various augmentation techniques such as horizontal flips, rotations, and zooms using tf.keras.Sequential layers to prevent overfitting and improve model generalization.

### 3. Transfer Learning with EfficientNetB0
- Pre-trained Model: Uses EfficientNetB0 as a base model, pre-trained on ImageNet, to leverage learned features from a vast dataset.
- Custom Classification Head: Adds custom dense layers, batch normalization, ReLU activation, and dropout for specific brain tumor classification.
- Fine-tuning: Allows for fine-tuning of a specified number of top layers in the base model.

### 4. Comprehensive Model Evaluation
- Performance Metrics: Calculates and displays per-class and averaged precision, recall, and F1-score.
- Confusion Matrix: Generates a confusion matrix to provide a detailed view of the model's classification performance across all classes.

5. Multi-class Brain Tumor Classification
- Specifically designed to classify brain MRI images into 'meningioma', 'notumor', 'pituitary', and 'glioma' categories.
