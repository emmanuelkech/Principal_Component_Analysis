# Principal Component Analysis
*BAN6420 Module 5 Milestone Assignment*

## Overview
This project aims to develop a model to identify essential variables for securing donor funding at the Anderson Cancer Center. Principal Component Analysis (PCA) is used for dimensionality reduction, and a logistic regression model is implemented for prediction.

## Dataset
The dataset used in this project is gotten from ***sklearn.datasets***. It includes a cancer-related dataset called the Breast Cancer Wisconsin (Diagnostic) Dataset which can be loaded using the *load_breast_cancer()* function.

## Explanation of Implemented Steps
#### Imports 
I began by importing specific functions and classes from *sklearn.datasets* that are required for the project.

#### Load Dataset 
The *load_breast_cancer()* function loads the dataset, which I then split into features (X) and the target variable (y).

#### Standardization 
The *StandardScaler()* function is used to normalize the features so that each feature contributes equally to the analysis.

#### PCA
Principal Component Analysis is applied to reduce the number of features to 2, capturing the most important variance in the data.

#### Train/Test Split 
The dataset is split into training and testing sets to evaluate the performance of the logistic regression model.

#### Logistic Regression
A logistic regression model is trained on the training data and then used to predict the labels of the test set.

#### Accuracy
The accuracy of the model's predictions is calculated and displayed along with the explained variance of the PCA components.

## Usage
#### Step 1: Run the Analysis
Execute the main script to perform PCA and logistic regression:

#### Step 2: Check the Results
The script will output the explained variance ratio of the PCA components and the accuracy of the logistic regression model.

## Conclusion
This project successfully demonstrates the application of Principal Component Analysis (PCA) for dimensionality reduction and logistic regression for predictive modeling using the Breast Cancer Wisconsin (Diagnostic) dataset. By reducing the dataset to just two principal components, we retained a significant portion of the variance of approximately 63% while simplifying the model. The logistic regression model trained on these components achieved a high accuracy of around 97%.
