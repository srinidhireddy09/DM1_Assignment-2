# DM1_Assignment-2

## Overview
This project focuses on classifying four dog breeds using edge histograms derived from images. The breeds included in this assignment are:
- Border Collie
- Irish Terrier
- Tibetan Terrier
- Scottish Deerhound

The dataset is processed to extract edge features, which are then used to train and evaluate multiple classification algorithms, including Naive Bayes, Decision Trees, and Random Forests. Additionally, a Support Vector Machine (SVM) model is evaluated for a binary classification scenario.

## Table of Contents
- Requirements
- Dataset Preparation
- Model Training and Evaluation
- Results
- License

## Requirements
- Python 3.x
- Libraries: `numpy`, `opencv-python`, `scikit-learn`, `matplotlib`, `seaborn`

You can install the required libraries using:
```bash
pip install numpy opencv-python scikit-learn matplotlib seaborn

## Dataset Preparation

The dataset is prepared by converting images to edge histograms using the following steps:

Load Images: Images are loaded from the specified directory.
Edge Detection: Canny edge detection is applied to extract edges from the images.
Histogram Calculation: Histograms of the edge-detected images are computed and normalized.
Data Storage: The edge histograms and corresponding labels are stored in numpy arrays and saved to disk.
The images are organized in folders corresponding to their respective classes.

## Model Training and Evaluation
Classifiers Used
Naive Bayes
Decision Tree
Random Forest
Support Vector Machine (SVM) for binary classification
Process
Data Splitting: The dataset is split into training (80%) and testing (20%) sets.
Standardization: The training data is standardized using StandardScaler for improved model performance.
Cross-Validation: Stratified 5-fold cross-validation is used to evaluate each classifier's accuracy.
Confusion Matrix
After fitting the models, confusion matrices are plotted to visualize performance across the classifiers.

## Results
The results include accuracy, precision, recall, and F1 scores for each classifier. The Decision Tree model showed the best performance based on the confusion matrix, while Naive Bayes achieved the highest F1 score.

