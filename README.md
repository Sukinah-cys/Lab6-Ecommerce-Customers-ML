# Lab6-Ecommerce-Customers-ML

## E-commerce Customers: A Linear Regression Approach

## Introduction

In the era of digital commerce, understanding customer behavior is essential for improving business performance and maximizing revenue. This project analyzes customer interaction data from an e-commerce platform that provides services through both a website and a mobile application. The study aims to leverage Machine Learning techniques to predict customer spending patterns and support strategic decision-making.

---

## Problem Statement

The company seeks to determine whether greater emphasis should be placed on improving the **mobile application** or the **website** to enhance customer spending. To address this, a predictive model is developed to estimate the **Yearly Amount Spent** by customers based on their interaction with the platform.

---

## Dataset Description

The dataset, titled **Ecommerce Customers**, contains information about customers and their engagement with the company’s services. Each record represents a single customer.

### Key Features:

* Avg. Session Length
* Time on App
* Time on Website
* Length of Membership
* Yearly Amount Spent *(Target Variable)*

Non-numeric features such as **Email**, **Address**, and **Avatar** were excluded from the modeling process as they are not suitable for regression analysis.

---

## Methodology

The project follows a structured Machine Learning workflow:

### 1. Data Loading and Exploration

The dataset was loaded into a Pandas DataFrame and explored using:

* Head (preview)
* Info (data types)
* Describe (statistical summary)

### 2. Data Cleaning

The dataset was checked for missing values, and no significant issues were found.

### 3. Feature Selection

Relevant numerical features were selected, while categorical/text features were excluded to ensure compatibility with the Linear Regression model.

### 4. Data Preparation

The data was divided into:

* **X (features)**
* **y (target variable)**

Then split into training and testing sets.

### 5. Model Training

A **Linear Regression** model from Scikit-learn was trained using the training dataset.

### 6. Model Evaluation

The model performance was evaluated using:

* Mean Absolute Error (MAE)
* Mean Squared Error (MSE)
* Root Mean Squared Error (RMSE)

Visualization techniques such as scatter plots and residual distributions were also used to assess model performance.

---

## Results and Discussion

The model demonstrated a reasonable ability to predict customer spending behavior. Analysis of the regression coefficients indicated that:

* **Length of Membership** has the strongest influence on yearly spending
* Time spent on the **mobile application** contributes more significantly than the website
* Long-term customer engagement plays a key role in increasing revenue

These findings suggest that improving customer retention and enhancing the mobile application experience could lead to increased profitability.

---

## Conclusion

This project highlights the effectiveness of Linear Regression in modeling customer spending behavior. By analyzing key features, the model provides valuable insights that can guide business decisions and optimize digital strategies.

---

## Tools and Technologies

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn

