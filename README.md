# House Price Prediction Using Linear Regression

## Machine Learning CIE 2 Activity

This project implements a **Simple Linear Regression** model to predict house prices based on the living area of a house (`sqft_living`).

The activity demonstrates the complete machine learning workflow, including data loading, data exploration, data preprocessing/validation, visualization, model training, evaluation, and prediction on a new house.

---

## 📌 Project Objective

The main objective of this activity is to build a Simple Linear Regression model that predicts house prices using the **living area of the house in square feet (`sqft_living`)** as the input feature.

The target variable used for prediction is **`price`**.

---

## 📊 Dataset

**Dataset:** House Price Prediction Dataset

**Source:** Kaggle – House Price Prediction Dataset

**Dataset Link:**  
https://www.kaggle.com/code/mahmoudhassanmahmoud/house-price-regression/input

The dataset contains information about residential properties, including:

- Bedrooms
- Bathrooms
- Living area
- Lot area
- Number of floors
- Waterfront status
- View
- Condition
- Grade
- Above-ground living area
- Basement area
- Year built
- Year renovated
- Zipcode
- Latitude
- Longitude
- Living area of nearby houses
- House price

For this activity, only **`sqft_living`** was selected as the input feature and **`price`** was used as the target variable.

---

## 🛠️ Technologies and Libraries Used

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Scikit-learn

### Machine Learning Algorithm

**Simple Linear Regression**

---

## 🔍 Project Workflow

The following steps were performed in the notebook:

1. Imported the required Python libraries.
2. Loaded the House Price Prediction dataset.
3. Examined the first and last records of the dataset.
4. Checked dataset information and data types.
5. Performed descriptive statistical analysis.
6. Checked for missing values.
7. Checked for duplicate records.
8. Selected `sqft_living` as the input feature.
9. Selected `price` as the target variable.
10. Visualized the relationship between living area and house price.
11. Split the dataset into training and testing sets.
12. Trained a Simple Linear Regression model.
13. Calculated the model intercept and coefficient.
14. Derived the Linear Regression equation.
15. Generated predictions on the test dataset.
16. Compared actual and predicted house prices.
17. Evaluated the model using MAE, MSE, RMSE, and R².
18. Visualized actual versus predicted prices.
19. Used the trained model to predict the price of a new house.
20. Documented the observations, limitations, and conclusion.

The dataset contains **999 observations and 18 columns**, with no missing values and no duplicate records identified during the analysis. 

---

## 📈 Model Details

The dataset was divided into:

| Dataset | Number of Observations |
|---|---:|
| Total | 999 |
| Training | 799 |
| Testing | 200 |

An **80:20 train-test split** was used with `random_state=42`.

### Linear Regression Equation

The trained model produced the following equation:

```text
price = -3.3101 + (0.0271 × sqft_living)
```

The model intercept was approximately **-3.3101**, while the coefficient for `sqft_living` was approximately **0.0271**.

---

## 📊 Model Evaluation

The trained model was evaluated on the test dataset using four metrics:

| Metric | Result |
|---|---:|
| MAE | 14.9228 |
| MSE | 469.8139 |
| RMSE | 21.6752 |
| R² Score | 0.4774 |

The model achieved an **R² score of 0.4774**, meaning that approximately **47.74% of the variation in house prices** is explained by `sqft_living` in this simple model.

---

## 🏠 New House Prediction

The trained model was also tested with a new house having a living area of:

```text
Living Area = 2000 sqft
```

### Prediction

```text
Predicted House Price = 50.9668 price units
```

The prediction was generated using the learned regression equation:

```text
price = -3.3101 + (0.0271 × sqft_living)
```

This is an estimate based only on the living area of the house.

---

## 📌 Key Observations

- There is a positive relationship between living area and house price.
- The model captures the general relationship between `sqft_living` and `price`.
- Some predictions differ considerably from the actual prices.
- Higher-priced houses show some larger prediction errors.
- Using only `sqft_living` is not sufficient to explain all variations in house prices.
- Other factors such as location, condition, grade, bedrooms, waterfront status, and year built can influence house prices.

---

## ⚠️ Limitations

This project uses only one feature, `sqft_living`, for prediction.

The model does not consider other potentially important factors such as:

- Location
- Number of bedrooms
- Number of bathrooms
- Property condition
- Property grade
- Waterfront status
- Year built
- Lot size
- View

Therefore, the model provides a basic demonstration of Simple Linear Regression rather than a complete real-world house price prediction system.

Using multiple relevant features and more advanced regression techniques could potentially improve prediction performance.

---

## 📁 Repository Contents

```text
House-Price-Prediction/
│
├── ML_Activity-2.ipynb
├── houses.csv
└── README.md
```

> Make sure that `houses.csv` is permitted to be uploaded publicly. Do not upload confidential, restricted, or personally sensitive data.

---

## 👩‍🏫 Faculty Reference & Acknowledgement

Faculty GitHub Profile:

**[Princy2129](https://github.com/Princy2129)**

This project was completed as part of the Machine Learning CIE 2 activity. Faculty reference and Machine Learning learning resources:

**https://github.com/Princy2129**

---

## 📚 Learning Outcome

Through this activity, the following concepts were practiced:

- Understanding regression problems
- Simple Linear Regression
- Feature and target selection
- Train-test splitting
- Model training
- Regression coefficients
- Prediction
- MAE
- MSE
- RMSE
- R² score
- Actual vs predicted visualization
- Interpretation of model performance
- Understanding model limitations

---

## 👤 Author

**Student: Madhura Jagtap 
**Roll Number: AD3172  
**Course: Machine Learning  
**Activity: CIE 2  
**Repository: Public GitHub Repository

---

## 📄 License

This repository is created for academic/educational purposes as part of the Machine Learning CIE 2 activity.