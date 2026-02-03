# Iris Flower Classification using Logistic Regression

## Overview  
This project implements a machine learning model to classify Iris flowers into different species using their sepal and petal measurements. 
The Iris dataset contains three species: Setosa, Versicolor, and Virginica. Since the target variable is categorical, I have used classification approach.
Logistic Regression is applied here.


## Dataset Description  
The Iris dataset consists of 150 samples with four numerical features:

- Sepal Length  
- Sepal Width  
- Petal Length  
- Petal Width  

Target variable:
- Species (Setosa, Versicolor, Virginica)  stored in X

The dataset does not contain any missing values so we dont require cleaning of Data here.

## Approach  

1. Data Loading and Inspection  
   The dataset is loaded using pandas and checked for missing values to ensure data quality.

2. Feature and Target Separation  
   - Features (X): Sepal and petal measurements  
   - Target (y): Species of the flower  

3. Label Encoding  
   I have used label encoding in this in order to classify the three different categories as Model can only understand the numbers
   Encoding used:
   - 0 → Setosa  
   - 1 → Versicolor  
   - 2 → Virginica
     
4. The dataset is divided int train and test with 80:20 ratio. A random state is also choosen in order to get the consistent result

5. Logisitic regeression Model is used here in order to handle multiClassification Variables

6. The trained model is evaluated on the test dataset using accuracy score import from sklearn.metrics.

7. Feature Importance Analysis  
   The absolute values of the Logistic Regression coefficients are used to determine the importance of each feature in predicting the flower species. The results are visualized using a bar chart.


## Model Used  

- Logistic Regression (Multiclass Classification)

This Problem involves more than two classes and performs effectively on the Iris dataset.


## Results  
The model achieves high accuracy on the test dataset, indicating that Logistic Regression can successfully classify Iris flower species based on their measurements.
Feature importance analysis shows that petal-related features contribute more significantly to classification than sepal-related features.

## Libraries Used  

- pandas  
- numpy  
- scikit-learn  
- matplotlib  
## Conclusion  
This project demonstrates a complete machine learning workflow, including data preprocessing, label encoding, model training, evaluation, and interpretation of results. Logistic Regression proves to be a simple and effective approach for multiclass classification using the Iris dataset.
