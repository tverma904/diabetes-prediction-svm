# Diabetes Prediction Using Support Vector Machine (SVM)

## Overview

This project demonstrates a binary classification workflow using a Support Vector Machine (SVM) classifier and Scikit-learn's diabetes dataset.

The original dataset contains a continuous disease-progression target. For this project, the target is converted into two classes using its median value.

**Important:** This is an educational classification exercise, not a clinical diabetes prediction or diagnosis model.

## Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Scikit-learn

## Project Workflow

1. Load the diabetes dataset.
2. Convert the continuous target into two classes using the median.
3. Split the dataset into training and testing sets.
4. Standardize the features using `StandardScaler`.
5. Train an SVM classifier with an RBF kernel.
6. Evaluate the model using classification metrics.
7. Plot the ROC curve and calculate the AUC score.
8. Compare training and testing accuracy.
9. Visualize a separate two-dimensional linear SVM decision boundary.

## Model Performance

| Metric | Score |
|---|---:|
| Training Accuracy | 81.30% |
| Testing Accuracy | 74.16% |
| Weighted F1-score | 0.74 |
| ROC-AUC | 0.826 |

### Classification Report

| Class | Precision | Recall | F1-score |
|---|---:|---:|---:|
| 0 | 0.78 | 0.69 | 0.73 |
| 1 | 0.71 | 0.80 | 0.75 |

## Visualizations

The notebook includes:

- Classification report
- Confusion matrix
- ROC curve with AUC score
- Training and testing accuracy comparison
- Two-dimensional linear SVM decision boundary

## Key Learnings

- Understanding Support Vector Machine classification
- Applying feature standardization
- Evaluating classification models using precision, recall, F1-score, and ROC-AUC
- Interpreting ROC curves
- Identifying possible overfitting through training and testing performance
- Visualizing decision boundaries in two-dimensional feature space

## Limitations

- The original dataset is designed for regression, not diabetes diagnosis.
- The binary target is artificially created using the median of the disease-progression target.
- The difference between training and testing accuracy suggests possible overfitting.
- The decision-boundary plot uses a separate linear SVM trained on only two features, not the main RBF model.

## How to Run

1. Open `diabetes_prediction_svm.ipynb` in Google Colab or Jupyter Notebook.
2. Install the required libraries if they are not already available.
3. Run the notebook cells in order.

## Disclaimer

This project is intended for educational purposes only. It must not be used for medical diagnosis, treatment, or clinical decision-making.
