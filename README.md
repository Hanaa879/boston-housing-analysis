# boston-housing-analysis
This is a linear regression data analysis model for a sample dataset taken from a course on infosys springboard related to boston housing analysis. It was my first try so I did have to ask ai for partial assistance. I used python in Jupyter lab to run this code
# Boston Housing Price Prediction: Single Linear Regression Model

## 1. Project Overview

This project focuses on the implementation of a **Single Linear Regression Model** using the Boston Housing Prices dataset. The goal is to predict the median value of owner-occupied homes (MEDV) based on a single selected independent variable. This serves as a foundational exercise in machine learning model development, data preparation, and results interpretation.

## 2. Methodology and Objectives

### **2.1 Key Objectives**

* To successfully apply the concepts of linear regression for predictive modeling.
* To perform **Feature Selection** to isolate the most influential independent variable for predicting home value.
* To train and evaluate the model using standard metrics.
* To clearly interpret the model's coefficients and understand their real-world impact on housing prices.

## 3. Dataset and Feature Selection

The project utilizes the classic **Boston Housing Prices Dataset**.

| Feature Name | Description | Role in Model |
| :--- | :--- | :--- |
| **RM** | **Average number of rooms per dwelling** | Independent Variable (X) |
| MEDV | Median value of owner-occupied homes in $1000s | Dependent Variable (Y) |

## 4. Key Results and Interpretation

### **4.1 Model Performance Metrics**

The model was tested on an unseen subset of the data, yielding the following performance metrics:

| Metric | Value |
| :--- | :--- |
| **$R^2$ Score** | **0.483** |
| **Mean Squared Error (MSE)** | **39.091** |

### **4.2 Model Coefficients**

The fitted linear equation takes the form: $Y = \beta_0 + \beta_1 X$

| Parameter | Value | Interpretation |
| :--- | :--- | :--- |
| **Intercept ($\beta_0$)** | **-34.222** | The predicted median home value when the average number of rooms (RM) is zero. |
| **Coefficient ($\beta_1$)** | **9.039** | The change in MEDV (in $1000s$) for every one-unit increase in the average number of rooms (RM). |

### **4.3 Insight**

The model reveals a **positive** linear relationship between **RM** and the median home value. Specifically, a one-unit increase in the average number of rooms is associated with an approximate **$9,039** increase in the median home value.

### **4.4 Visualization**

A scatter plot illustrating the positive linear relationship between RM and MEDV, along with the calculated line of best fit.

![Scatter Plot: RM vs. MEDV with Line of Best Fit]

## 5. Technical Requirements

### **5.1 Environment**

* **Language:** Python
* **Environment:** JupyterLab 

### **5.2 Libraries**

The following Python libraries are required:
* `pandas`
* `numpy`
* `scikit-learn` (`sklearn`)
* `matplotlib` (for visualizations)
* `seaborn` (for visualizations)

## 6. Repository Structure

The core files of this repository include:

* `LinearRegressionsample.ipynb`: The main Jupyter Notebook containing all data cleaning, EDA, model training, and evaluation steps.
* `boston_housing.csv` : The raw dataset used for the analysis.
* `README.md`: This documentation file.

1.  Expanding the analysis to a **Multiple Linear Regression Model** to assess the combined predictive power of all features.
2.  Implementing **Feature Scaling** and **Regularization Techniques** (Ridge, Lasso) to improve model generalization and combat potential overfitting.
