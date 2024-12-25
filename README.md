# Abnormal Bone Detection

This project aims to detect abnormalities in bones using medical imaging data. The goal is to classify X-ray images into two categories:
- **Normal**
- **Abnormal**

## Dataset
We used the **MURA (Musculoskeletal Radiographs)** dataset for this project. MURA is a large dataset of musculoskeletal X-rays that contains images labeled as either normal or abnormal.

### Key Features of the Dataset:
- Contains X-ray images from various body parts such as the wrist, elbow, shoulder, etc.
- Binary labels: normal and abnormal.
- Designed for the task of automated abnormality detection in radiographs.

## Problem Statement
The objective is to develop a machine learning model that can accurately classify X-ray images as either normal or abnormal, assisting radiologists in diagnosis and treatment planning.

## Approach
1. **Data Preprocessing**:
   - Images were resized to ensure uniform input dimensions.
   - Normalization was applied to standardize the pixel values.
   - Data augmentation techniques were used to improve model generalization.

2. **Model Architecture**:
   - A ResNet50 was used to extract features from the X-ray images.
   - The model was trained on labeled data to learn patterns associated with abnormalities.

   ![Model Architecture](path/to/model_architecture_image.png)

3. **Training**:
   - The dataset was split into training, validation, and test sets.
   - BinaryCross-entropy loss was used as the loss function.
   - Adam optimizer was employed to minimize the loss and improve performance.

4. **Evaluation**:
   - Accuracy, precision, recall, and F1-score were used as evaluation metrics.
   - Confusion matrix analysis was performed to understand model performance.

## Results
The model achieved satisfactory performance in distinguishing between normal and abnormal X-ray images. Detailed results and performance metrics can be found in the results section of this repository.

## Future Work
- Extend the model to handle multi-class classification for different types of abnormalities.
- Incorporate more datasets to improve robustness and generalization.
- Explore other architectures such as Vision Transformers or hybrid models.


