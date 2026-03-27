# 🏠 California Housing Price Prediction using Ridge Regression

## 📌 Project Overview

This project aims to predict housing prices in California using demographic and geographic features.
A **Ridge Regression model** is implemented to handle multicollinearity among features and improve prediction performance.

---

## 📊 Dataset

The dataset used is the **California Housing Dataset**.

* Source: https://www.kaggle.com/datasets/camnugent/california-housing-prices

* Features:

  * MedInc → Median income
  * HouseAge → Average house age
  * AveRooms → Average rooms
  * AveBedrms → Average bedrooms
  * Population → Area population
  * AveOccup → Average occupancy
  * Latitude → Geographic latitude
  * Longitude → Geographic longitude

* Target:

  * MedHouseVal → Median house value

---

## ⚙️ Technologies Used

* Python 🐍
* NumPy
* Pandas
* Matplotlib
* Seaborn
* Scikit-learn

---

## 🚀 Project Workflow

### 1. Data Loading

* Dataset loaded using `sklearn.datasets.fetch_california_housing()`

### 2. Data Exploration

* Checked for missing values
* Viewed dataset statistics
* Visualized feature relationships using a heatmap

### 3. Data Preparation

* Selected input features and target variable
* Split dataset into training (80%) and testing (20%)
* Applied feature scaling using `StandardScaler`

### 4. Model Building

* Used **Ridge Regression** from Scikit-learn
* Set regularization parameter `alpha = 1.0`

### 5. Model Evaluation

* Mean Squared Error (MSE)
* R² Score

### 6. Visualization

* Plotted Actual vs Predicted house prices

---

## 🧠 What is Ridge Regression?

Ridge Regression is a regularized version of Linear Regression that adds a penalty term to reduce overfitting.

**Formula:**

L = Σ(y - ŷ)² + αΣw²

* α → Regularization strength
* Helps reduce multicollinearity
* Prevents large coefficient values

---

## 📈 Results

* The model achieves good prediction performance with balanced bias and variance
* Median Income (MedInc) has the strongest influence on house prices
* Geographic features also significantly impact predictions

---

## 📂 Project Structure

```
📁 housing-price-prediction
│── ridge_model.py
│── README.md
```

---

## ▶️ How to Run

1. Install dependencies:

```
pip install numpy pandas matplotlib seaborn scikit-learn
```

2. Run the script:

```
python ridge_model.py
```

---

## 🎯 Future Improvements

* Hyperparameter tuning (GridSearchCV)
* Compare with Lasso and Linear Regression
* Deploy model using Flask or Streamlit

---

## 🙌 Author

**Prathiba Devendiran**
B.Sc Computer Science with AI

---

## ⭐ Acknowledgment

* Dataset provided by Kaggle
* Scikit-learn documentation

---
