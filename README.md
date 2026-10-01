# EDP-AI-ML Week 6–7 – Hyperparameter Tuning

## Project Title

Hyperparameter Tuning of KNN and Decision Tree Models using the Iris Dataset

## Objective

The objective of this project is to understand hyperparameter tuning in machine learning.

In this project, K-Nearest Neighbors (KNN) and Decision Tree classification models are tuned using different hyperparameter values. The tuned models are compared with the original models to observe the improvement in accuracy.

## Dataset

The Iris dataset from Scikit-learn is used for this project.

- Total samples: 150
- Number of features: 4
- Number of classes: 3
- Training samples: 120
- Testing samples: 30

## Features

The dataset contains the following four features:

- Sepal Length (cm)
- Sepal Width (cm)
- Petal Length (cm)
- Petal Width (cm)

## Target Classes

The Iris dataset contains three target classes:

- Class 0 – Setosa
- Class 1 – Versicolor
- Class 2 – Virginica

## Technologies Used

- Python
- Jupyter Notebook
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn

## Models Used

### 1. K-Nearest Neighbors (KNN)

KNN is a classification algorithm that predicts the class of a data point based on its nearest neighboring data points.

The `n_neighbors` parameter was tuned using the following values:

`1, 3, 5, 7, 9, 11, 13, 15`

### 2. Decision Tree

Decision Tree is a classification algorithm that makes predictions using a tree-like structure of decision rules.

The `max_depth` parameter was tested using values from:

`1 to 10`

## Data Preprocessing

The dataset was divided into training and testing sets using an 80:20 ratio.

- Training data: 120 samples
- Testing data: 30 samples
- Random state: 42
- Stratified splitting was used to maintain class distribution.

Feature scaling using StandardScaler was applied for the KNN model.

## Hyperparameter Tuning

### KNN Tuning

Different values of K were tested to identify the value that produced the highest accuracy.

Best result:

- Best K: **1**
- Accuracy: **96.67%**

### Decision Tree Tuning

Different values of `max_depth` were tested from 1 to 10.

Best result:

- Best max_depth: **3**
- Accuracy: **96.67%**

## Results

The original models from Week 5 achieved:

- Original KNN Accuracy: **93.33%**
- Original Decision Tree Accuracy: **93.33%**

After hyperparameter tuning:

- Tuned KNN Accuracy: **96.67%**
- Tuned Decision Tree Accuracy: **96.67%**

Both models improved by approximately **3.34 percentage points** on the test dataset.

## Model Comparison

| Model | Original Accuracy | Tuned Accuracy | Best Hyperparameter |
|---|---:|---:|---|
| KNN | 93.33% | 96.67% | K = 1 |
| Decision Tree | 93.33% | 96.67% | max_depth = 3 |

## Analysis

Hyperparameter tuning helped improve the performance of both classification models.

For KNN, changing the number of neighbors affected the classification accuracy. The best result was obtained with K = 1.

For the Decision Tree, changing the maximum tree depth affected the model performance. The best result was obtained with max_depth = 3.

The experiment demonstrates that selecting suitable hyperparameter values can improve model performance.

## Conclusion

In Week 6–7, hyperparameter tuning was performed on KNN and Decision Tree models using the Iris dataset.

The best KNN model used K = 1 and achieved 96.67% accuracy. The best Decision Tree model used max_depth = 3 and also achieved 96.67% accuracy.

Both tuned models improved from the original accuracy of 93.33% to 96.67% on the test dataset.

This experiment helped in understanding how hyperparameter selection can affect machine learning model performance.

## Project Structure

```text
EDP-AI-ML-Week6-7/
│
├── week6_7.ipynb
└── README.md