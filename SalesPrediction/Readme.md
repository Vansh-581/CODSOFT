#  SALES PREDICTION USING LINEAR REGRESSION

---

##  OVERVIEW

This project implements a machine learning model to predict Sales based on advertising expenditure. The dataset contains advertising budgets for TV, Radio and Newspaper. Since the target variable is continuous (Sales amount), I have used Regression approach. Linear Regression model is applied here.

---

##  DATASET DESCRIPTION

The Advertising dataset consists of numerical features:

- **TV** – Advertising budget spent on TV  
- **Radio** – Advertising budget spent on Radio  
- **Newspaper** – Advertising budget spent on Newspaper  

**Target variable:**

- **Sales** – Product sales amount  

The dataset does not contain any major missing values so heavy cleaning was not required. Only basic checking was done.

---

##  APPROACH

### Data Loading and Inspection  
The dataset is loaded using pandas and checked for missing values to ensure data quality.

### Feature and Target Separation  

**Features (X):**
- TV  
- Radio  
- Newspaper  

**Target (y):**
- Sales  

### Train Test Split  
The dataset is divided into train and test set using 80:20 ratio.  
Random state is used in order to get consistent results every time.

### Model Used  
Linear Regression model is used here because this is a regression problem and all input features are numerical.

The model learns the relationship between advertising spending and sales.

### Model Evaluation  

The trained model is evaluated using:

- **R2 Score** – To measure how well the model explains variation in sales  
- **Mean Absolute Error (MAE)** – To check average prediction error  

---

##  FEATURE IMPORTANCE ANALYSIS

The coefficients of Linear Regression are used to determine the impact of each advertising channel on sales.

The results are visualized using a bar chart.

From the analysis, it is observed that:

- Radio advertising has the highest impact on Sales  
- TV advertising has moderate impact  
- Newspaper advertising has least impact  

---

##  MODEL USED

**Linear Regression (Regression Problem)**  

Since the target variable is continuous, accuracy score is not used. Instead regression evaluation metrics are applied.

---

##  RESULTS

The model achieves a high R2 score, showing that it explains most of the variation in sales data.

The results indicate that advertising through Radio and TV plays a significant role in increasing sales.

---

##  LIBRARIES USED

- pandas  
- numpy  
- scikit-learn  
- matplotlib  

---

##  CONCLUSION

This project demonstrates a complete regression workflow including data loading, preprocessing, model training, evaluation and interpretation of coefficients.

Linear Regression proves to be a simple and effective approach for predicting sales based on advertising expenditure.
