# Titanic Survival Prediction 

## Overview
This project is about predicting whether a passenger survived the Titanic disaster or not using basic Machine Learning techniques.  
It is a Small-Beginner-focussed data science project and helped me understand the complete ML workflow — from data cleaning to model evaluation.

---

## Objective
The goal of this project is to build a machine learning model that can predict passenger survival based on factors such as:
- Passenger class
- Gender
- Age
- Fare
- Family size
- Embarkation port

---

## Dataset
The dataset used is the **Titanic dataset**, which contains information about passengers aboard the Titanic, including whether they survived.

Some important columns in the dataset:
- `Survived` – Target variable (0 = No, 1 = Yes)
- `Pclass` – Passenger class
- `Sex` – Gender
- `Age` – Age of passenger
- `Fare` – Ticket price
- `Embarked` – Port of embarkation

---

## Approach
I followed the below steps to complete the project:

1. **Data Understanding**
   - Checked dataset structure and column meanings
   - Identified missing values and data types

2. **Data Cleaning & Preprocessing**
   - Filled missing `Age` values using median
   - Filled missing `Embarked` values using mode as it was categorical with 3 categories i required mode for char values to fill then Null values
   - Encoded categorical variables:
     - `Sex` using binary encoding(0 or 1)
     - `Embarked` using one-hot encoding(i dropped the first column after one-hot encoding as two are enough
        to produce result if both give 0 then it means the left over category was what person belonged to)
   - Removed unnecessary columns not required for prediction

3. **Exploratory Data Analysis**
   - Visualized survival counts
   - Observed relationships between survival and features like gender and class

4. **Model Training**
   - Split data into training and testing sets
   - Trained a **Logistic Regression** model

5. **Model Evaluation**
   - Evaluated the model using accuracy score
   - Analyzed feature importance using model coefficients

---

## Model Used
- **Logistic Regression**

This model was chosen because:
- The target variable is binary as it returns answers in 0 or 1 format 0 means did not survive, 1 means survived
- It is simple and interpretable

---

## Results
- The model achieved an accuracy of approximately **79-81%** (may vary slightly depending on split i took it as 42).
- Gender and passenger class were among the most important features affecting survival.

---

## Tools & Libraries Used
- Python
- Pandas
- Matplotlib
- Scikit-learn

---

## What I Learned
- How important data cleaning is for machine learning
- How to handle categorical variables properly
- How train-test split works and why it is necessary
- How to train, evaluate, and interpret a machine learning model

---

## Conclusion
This project helped me understand the end-to-end machine learning process.  
It strengthened my foundation in data preprocessing, model training, and result interpretation, and gave me confidence to work on more ML projects.

---
 This project is part of the **CodSoft Data Science Internship**.
