# Deep Learning Based Medical Image Analysis with U-Net

## Overview
This project focuses on medical image analysis using deep learning techniques, specifically employing the U-Net architecture for segmentation tasks. It is implemented using TensorFlow and Keras, and it targets the segmentation of medical images (MRI scans).
 - ![Image 2: B&W Conversion](/results/img.png)


## Key Features
- **Data Loading and Preprocessing:**
  - Load medical images and corresponding masks from NIfTI format (`.nii.gz`).
  - Preprocess data for neural network training, including normalization and reshaping.
  
- **U-Net Model Implementation:**
  - Custom U-Net architecture for image segmentation.
  - Configurable dropout and input size.

- **Training and Validation:**
  - K-Fold Cross-Validation to enhance model generalization.
  - Monitoring training process with accuracy and loss metrics.

- **Performance Evaluation:**
  - Custom functions to calculate Dice Coefficient and Hausdorff Distance for model evaluation.
  - Visualization of model predictions alongside ground truth data.
  - ![Image 2: B&W Conversion](/results/dieccoff.png)
  - ![Image 2: B&W Conversion](/results/accuracyvalid.png)
  - ![Image 2: B&W Conversion](/results/prediction.png)

- **Google Colab Integration:**
  - Utilization of Google Colab for model training and evaluation, with Google Drive integration for data storage and retrieval.

## Requirements
- Python 3.x
- TensorFlow and Keras
- Nibabel for NIfTI format handling
- Scikit-learn for model validation
- Matplotlib for data visualization
- Scipy for distance calculation

## Usage
1. Mount your Google Drive to access the dataset.
2. Run the notebook cells in sequence to load data, define the U-Net model, and perform training.
3. Evaluate the model performance with the provided metrics and visualization tools.

## Dataset
The dataset consists of MRI scans along with their respective segmentation masks. It's important to ensure the dataset is correctly formatted and stored in Google Drive for seamless integration.

## Limitations and Considerations
- The model's performance is heavily reliant on the quality and quantity of the data.
- Computational resources can be a limiting factor; running on Google Colab provides access to better hardware.



