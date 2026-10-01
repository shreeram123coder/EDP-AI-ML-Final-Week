# EDP-AI-ML Week 6–7 – Hyperparameter Tuning

## Project Title

Hyperparameter Tuning of KNN and Decision Tree Models using the Iris Dataset

## Objective

The objective of Week 6–7 is to understand hyperparameter tuning in machine learning. KNN and Decision Tree models are tuned using different parameter values, and their performance is compared with the original models from Week 5.

## Dataset

The Iris dataset from Scikit-learn is used.

The dataset contains:

- 150 samples
- 4 input features
- 3 flower classes

### Features

- Sepal Length
- Sepal Width
- Petal Length
- Petal Width

### Target Classes

- Setosa
- Versicolor
- Virginica

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

KNN classifies a data point based on the classes of its nearest neighboring data points.

The `n_neighbors` parameter was tuned using different K values:

```text
1, 3, 5, 7, 9, 11, 13, 15