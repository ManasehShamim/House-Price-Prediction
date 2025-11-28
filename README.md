# House Price Prediction

This project predicts house prices using machine learning techniques based on features such as **square footage, number of bedrooms, and location.  
The model is trained using the House Price Prediction Dataset from Kaggle.
DATASET LINK:
https://www.kaggle.com/datasets/zafarali27/house-price-prediction-dataset/data

---

## Project Objective
To build a regression model that can accurately estimate the price of a house based on important property features.

---

## Dataset
Dataset used: House Price Prediction Dataset(Kaggle)
LINK:
https://www.kaggle.com/datasets/zafarali27/house-price-prediction-dataset/data

Features include:
- `square_feet` – Total area of the house  
- `bedrooms` – Number of bedrooms  
- `location` – City/area  
- `price` – Target variable (House price)

---

## Data Preprocessing
The following preprocessing steps were applied:
- Removed missing values using `dropna()`
- Selected important features for training
- One-hot encoded the **location** column using `OneHotEncoder`
- Split dataset into **train (80%)** and **test (20%)**

---

## Model Used
Two models were prepared (you can switch between them):

✔ **Linear Regression**  
✔ **Gradient Boosting Regressor**

Pipeline used:
- Preprocessing (One-Hot Encoding)
- Regression Model

---

## Model Training
The model was trained using:
```python
pipeline.fit(X_train, y_train)
